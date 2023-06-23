# Comparing `tmp/funboost-23.3-py3-none-any.whl.zip` & `tmp/funboost-23.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,248 +1,222 @@
-Zip file size: 1915034 bytes, number of entries: 246
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-19 02:37 funboost/__init__.py
--rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-13 01:20 funboost/__init__old.py
--rw-rw-rw-  2.0 fat     6261 b- defN 23-Jun-20 05:54 funboost/constant.py
--rw-rw-rw-  2.0 fat     7358 b- defN 23-Jun-05 04:48 funboost/funboost_config_deafult.py
--rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-13 09:47 funboost/set_frame_config.py
--rw-rw-rw-  2.0 fat     4186 b- defN 23-Jun-19 02:19 funboost/assist/celery_helper.py
--rw-rw-rw-  2.0 fat     2089 b- defN 23-May-22 01:31 funboost/assist/dramatiq_helper.py
--rw-rw-rw-  2.0 fat     1760 b- defN 23-May-24 11:10 funboost/assist/huey_helper.py
--rw-rw-rw-  2.0 fat     1509 b- defN 23-Jun-09 03:23 funboost/assist/rq_helper.py
--rw-rw-rw-  2.0 fat     4831 b- defN 23-Jun-09 01:42 funboost/assist/rq_windows_worker.py
--rw-rw-rw-  2.0 fat     3930 b- defN 22-Sep-17 06:12 funboost/beggar_version_implementation/beggar_redis_consumer.py
--rw-rw-rw-  2.0 fat      759 b- defN 22-Dec-19 11:45 funboost/concurrent_pool/__init__.py
--rw-rw-rw-  2.0 fat     3256 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/async_helper.py
--rw-rw-rw-  2.0 fat     7227 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/async_pool_executor.py
--rw-rw-rw-  2.0 fat     4723 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
--rw-rw-rw-  2.0 fat     3011 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
--rw-rw-rw-  2.0 fat     1571 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_threadpoolexcutor.py
--rw-rw-rw-  2.0 fat     1872 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/concurrent_pool_with_multi_process.py
--rw-rw-rw-  2.0 fat     2402 b- defN 22-Sep-17 06:12 funboost/concurrent_pool/custom_evenlet_pool_executor.py
--rw-rw-rw-  2.0 fat     4421 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/custom_gevent_pool_executor.py
--rw-rw-rw-  2.0 fat    11745 b- defN 22-Dec-19 11:43 funboost/concurrent_pool/custom_threadpool_executor.py
--rw-rw-rw-  2.0 fat     9317 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/custom_threadpool_executor000.py
--rw-rw-rw-  2.0 fat      373 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/single_thread_executor.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-24 11:39 funboost/concurrent_pool/backup/__init__.py
--rw-rw-rw-  2.0 fat     9548 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor0223.py
--rw-rw-rw-  2.0 fat     9568 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_back.py
--rw-rw-rw-  2.0 fat     5728 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_janus.py
--rw-rw-rw-  2.0 fat      126 b- defN 22-Sep-17 06:12 funboost/consumers/__init__.py
--rw-rw-rw-  2.0 fat    82870 b- defN 23-Jun-19 02:19 funboost/consumers/base_consumer.py
--rw-rw-rw-  2.0 fat     7574 b- defN 23-Jun-06 01:47 funboost/consumers/celery_consumer.py
--rw-rw-rw-  2.0 fat     4574 b- defN 23-May-04 06:09 funboost/consumers/celery_consumer000.py
--rw-rw-rw-  2.0 fat     6033 b- defN 23-Jun-20 04:59 funboost/consumers/confirm_mixin.py
--rw-rw-rw-  2.0 fat     2144 b- defN 23-May-23 07:08 funboost/consumers/dramatiq_consumer.py
--rw-rw-rw-  2.0 fat     2025 b- defN 23-May-15 01:33 funboost/consumers/http_consumer.py
--rw-rw-rw-  2.0 fat     4463 b- defN 22-Sep-17 06:12 funboost/consumers/http_consumer000.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-04 12:12 funboost/consumers/httpsqs_consumer.py
--rw-rw-rw-  2.0 fat     1856 b- defN 23-May-24 11:08 funboost/consumers/huey_consumer.py
--rw-rw-rw-  2.0 fat     4217 b- defN 23-May-04 12:12 funboost/consumers/kafka_consumer.py
--rw-rw-rw-  2.0 fat     6947 b- defN 23-Jun-09 09:53 funboost/consumers/kafka_consumer_manually_commit.py
--rw-rw-rw-  2.0 fat    10186 b- defN 23-May-12 08:42 funboost/consumers/kombu_consumer.py
--rw-rw-rw-  2.0 fat     1291 b- defN 23-May-04 12:12 funboost/consumers/local_python_queue_consumer.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-May-04 12:12 funboost/consumers/mongomq_consumer.py
--rw-rw-rw-  2.0 fat     2228 b- defN 23-May-04 12:12 funboost/consumers/mqtt_consumer.py
--rw-rw-rw-  2.0 fat     2183 b- defN 23-May-04 12:12 funboost/consumers/nameko_consumer.py
--rw-rw-rw-  2.0 fat     1076 b- defN 23-May-04 12:12 funboost/consumers/nats_consumer.py
--rw-rw-rw-  2.0 fat     1461 b- defN 23-May-18 03:26 funboost/consumers/nsq_consumer.py
--rw-rw-rw-  2.0 fat     1238 b- defN 23-May-04 12:12 funboost/consumers/peewee_conusmer.py
--rw-rw-rw-  2.0 fat     1005 b- defN 23-May-04 12:12 funboost/consumers/persist_queue_consumer.py
--rw-rw-rw-  2.0 fat     2414 b- defN 23-May-04 12:12 funboost/consumers/pulsar_consumer.py
--rw-rw-rw-  2.0 fat     2048 b- defN 23-Jun-20 01:27 funboost/consumers/rabbitmq_amqpstorm_consumer.py
--rw-rw-rw-  2.0 fat     5433 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_pika_consumer.py
--rw-rw-rw-  2.0 fat     4674 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_pika_consumerv0.py
--rw-rw-rw-  2.0 fat     1260 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_rabbitpy_consumer.py
--rw-rw-rw-  2.0 fat     3031 b- defN 23-May-04 12:12 funboost/consumers/redis_brpoplpush_consumer.py
--rw-rw-rw-  2.0 fat     2829 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer.py
--rw-rw-rw-  2.0 fat     7545 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_ack_able.py
--rw-rw-rw-  2.0 fat     4282 b- defN 23-Jun-21 02:07 funboost/consumers/redis_consumer_priority.py
--rw-rw-rw-  2.0 fat      922 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_simple.py
--rw-rw-rw-  2.0 fat     7135 b- defN 22-Sep-17 06:12 funboost/consumers/redis_filter.py
--rw-rw-rw-  2.0 fat     1206 b- defN 23-May-04 12:12 funboost/consumers/redis_pubsub_consumer.py
--rw-rw-rw-  2.0 fat     6497 b- defN 23-May-25 02:22 funboost/consumers/redis_stream_consumer.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-May-04 12:12 funboost/consumers/rocketmq_consumer.py
--rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-08 11:07 funboost/consumers/rq_consumer.py
--rw-rw-rw-  2.0 fat     1309 b- defN 23-May-04 12:12 funboost/consumers/sqlachemy_consumer.py
--rw-rw-rw-  2.0 fat     2045 b- defN 23-May-04 12:12 funboost/consumers/tcp_consumer.py
--rw-rw-rw-  2.0 fat     1340 b- defN 23-May-04 12:12 funboost/consumers/txt_file_consumer.py
--rw-rw-rw-  2.0 fat     1643 b- defN 23-May-04 12:12 funboost/consumers/udp_consumer.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-May-04 12:12 funboost/consumers/zeromq_consumer.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-05 10:31 funboost/contrib/__init__.py
--rw-rw-rw-  2.0 fat     4680 b- defN 23-May-15 08:24 funboost/contrib/queue2queue.py
--rw-rw-rw-  2.0 fat     1817 b- defN 23-Mar-22 02:09 funboost/contrib/redis_consume_latest_msg_broker.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 04:48 funboost/core/__init__.py
--rw-rw-rw-  2.0 fat     4984 b- defN 23-Jun-05 04:48 funboost/core/active_cousumer_info_getter.py
--rw-rw-rw-  2.0 fat    16372 b- defN 23-Jun-08 02:26 funboost/core/booster.py
--rw-rw-rw-  2.0 fat      576 b- defN 23-Jun-13 01:20 funboost/core/exit_signal.py
--rw-rw-rw-  2.0 fat     8875 b- defN 23-Jun-05 04:48 funboost/core/fabric_deploy_helper.py
--rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-05 04:48 funboost/core/function_result_status_config.py
--rw-rw-rw-  2.0 fat     8819 b- defN 23-Jun-05 04:48 funboost/core/function_result_status_saver.py
--rw-rw-rw-  2.0 fat     1169 b- defN 23-Jun-08 03:26 funboost/core/get_booster.py
--rw-rw-rw-  2.0 fat      340 b- defN 23-Jun-08 02:52 funboost/core/global_boosters.py
--rw-rw-rw-  2.0 fat     1193 b- defN 23-Jun-12 01:35 funboost/core/helper_funs.py
--rw-rw-rw-  2.0 fat     7782 b- defN 23-Jun-05 04:48 funboost/core/msg_result_getter.py
--rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-08 03:05 funboost/core/muliti_process_enhance.py
--rw-rw-rw-  2.0 fat      178 b- defN 22-Sep-17 06:12 funboost/factories/__init__.py
--rw-rw-rw-  2.0 fat     8976 b- defN 23-Jun-20 05:54 funboost/factories/broker_kind__publsiher_consumer_type_map.py
--rw-rw-rw-  2.0 fat      946 b- defN 23-May-29 03:09 funboost/factories/consumer_factory.py
--rw-rw-rw-  2.0 fat     2281 b- defN 23-May-29 03:09 funboost/factories/publisher_factotry.py
--rw-rw-rw-  2.0 fat     4841 b- defN 22-Sep-17 06:12 funboost/function_result_web/app.py
--rw-rw-rw-  2.0 fat     7345 b- defN 23-Mar-08 10:19 funboost/function_result_web/functions.py
--rw-rw-rw-  2.0 fat     4045 b- defN 22-Feb-21 07:34 funboost/function_result_web/__pycache__/app.cpython-37.pyc
--rw-rw-rw-  2.0 fat     3921 b- defN 22-Mar-30 13:56 funboost/function_result_web/__pycache__/functions.cpython-37.pyc
--rw-rw-rw-  2.0 fat     7674 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/css/custom.css
--rw-rw-rw-  2.0 fat    42839 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/css/jquery.mCustomScrollbar.min.css
--rw-rw-rw-  2.0 fat    23610 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/img/user.jpg
--rw-rw-rw-  2.0 fat     1106 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/js/custom.js
--rw-rw-rw-  2.0 fat    45483 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/js/jquery.mCustomScrollbar.concat.min.js
--rw-rw-rw-  2.0 fat    11065 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/css/style.css
--rw-rw-rw-  2.0 fat  1153168 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/bg.jpg
--rw-rw-rw-  2.0 fat      546 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/password.png
--rw-rw-rw-  2.0 fat     2912 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/tick.png
--rw-rw-rw-  2.0 fat      622 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/user.png
--rw-rw-rw-  2.0 fat    96383 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/js/jquery-1.11.0.min.js
--rw-rw-rw-  2.0 fat    19501 b- defN 22-Feb-21 12:32 funboost/function_result_web/templates/index.html
--rw-rw-rw-  2.0 fat     2007 b- defN 21-Dec-27 01:40 funboost/function_result_web/templates/login.html
--rw-rw-rw-  2.0 fat      131 b- defN 22-Sep-17 06:12 funboost/publishers/__init__.py
--rw-rw-rw-  2.0 fat    15844 b- defN 23-Jun-20 05:06 funboost/publishers/base_publisher.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-Jun-20 04:23 funboost/publishers/celery_publisher.py
--rw-rw-rw-  2.0 fat     3897 b- defN 23-May-04 06:09 funboost/publishers/celery_publisher000.py
--rw-rw-rw-  2.0 fat     3541 b- defN 23-Mar-23 05:32 funboost/publishers/confluent_kafka_publisher.py
--rw-rw-rw-  2.0 fat     1410 b- defN 23-May-22 01:23 funboost/publishers/dramatiq_publisher.py
--rw-rw-rw-  2.0 fat      753 b- defN 23-May-04 11:53 funboost/publishers/http_publisher.py
--rw-rw-rw-  2.0 fat     2783 b- defN 22-Sep-17 06:12 funboost/publishers/httpsqs_publisher.py
--rw-rw-rw-  2.0 fat     1101 b- defN 23-May-24 11:08 funboost/publishers/huey_publisher.py
--rw-rw-rw-  2.0 fat     2160 b- defN 23-Apr-03 10:55 funboost/publishers/kafka_publisher.py
--rw-rw-rw-  2.0 fat     5321 b- defN 23-May-15 01:33 funboost/publishers/kombu_publisher.py
--rw-rw-rw-  2.0 fat     1365 b- defN 22-Sep-17 06:12 funboost/publishers/local_python_queue_publisher.py
--rw-rw-rw-  2.0 fat     1874 b- defN 23-Mar-14 02:56 funboost/publishers/mongomq_publisher.py
--rw-rw-rw-  2.0 fat     3050 b- defN 22-Sep-17 06:12 funboost/publishers/mqtt_publisher.py
--rw-rw-rw-  2.0 fat     1662 b- defN 23-Jun-19 06:54 funboost/publishers/nameko_publisher.py
--rw-rw-rw-  2.0 fat      776 b- defN 21-Dec-27 01:40 funboost/publishers/nats_publisher.py
--rw-rw-rw-  2.0 fat     1302 b- defN 22-Sep-17 06:12 funboost/publishers/nsq_publisher.py
--rw-rw-rw-  2.0 fat     1095 b- defN 22-Sep-17 06:12 funboost/publishers/peewee_publisher.py
--rw-rw-rw-  2.0 fat     2540 b- defN 22-Sep-17 06:12 funboost/publishers/persist_queue_publisher.py
--rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-13 03:56 funboost/publishers/pulsar_publisher.py
--rw-rw-rw-  2.0 fat     3137 b- defN 23-Jun-20 02:17 funboost/publishers/rabbitmq_amqpstorm_publisher.py
--rw-rw-rw-  2.0 fat     2343 b- defN 22-Sep-17 06:12 funboost/publishers/rabbitmq_pika_publisher.py
--rw-rw-rw-  2.0 fat     1953 b- defN 22-Sep-17 06:12 funboost/publishers/rabbitmq_rabbitpy_publisher.py
--rw-rw-rw-  2.0 fat     3982 b- defN 23-May-10 03:22 funboost/publishers/redis_publisher.py
--rw-rw-rw-  2.0 fat      278 b- defN 22-Sep-17 06:12 funboost/publishers/redis_publisher_lpush.py
--rw-rw-rw-  2.0 fat     2104 b- defN 23-Jun-20 05:54 funboost/publishers/redis_publisher_priority.py
--rw-rw-rw-  2.0 fat      872 b- defN 23-Apr-28 03:12 funboost/publishers/redis_publisher_simple.py
--rw-rw-rw-  2.0 fat      721 b- defN 22-Sep-17 06:12 funboost/publishers/redis_pubsub_publisher.py
--rw-rw-rw-  2.0 fat     2037 b- defN 21-Dec-27 01:40 funboost/publishers/redis_stream_publisher.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-Mar-23 05:32 funboost/publishers/rocketmq_publisher.py
--rw-rw-rw-  2.0 fat      893 b- defN 23-Jun-13 01:20 funboost/publishers/rq_publisher.py
--rw-rw-rw-  2.0 fat     1215 b- defN 22-Sep-17 06:12 funboost/publishers/sqla_queue_publisher.py
--rw-rw-rw-  2.0 fat     1335 b- defN 23-May-10 08:53 funboost/publishers/tcp_publisher.py
--rw-rw-rw-  2.0 fat     1380 b- defN 22-Sep-17 08:52 funboost/publishers/txt_file_publisher.py
--rw-rw-rw-  2.0 fat     1194 b- defN 23-May-04 11:53 funboost/publishers/udp_publisher.py
--rw-rw-rw-  2.0 fat     1002 b- defN 21-Dec-27 01:40 funboost/publishers/zeromq_publisher.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-22 02:44 funboost/queues/__init__.py
--rw-rw-rw-  2.0 fat     4944 b- defN 23-May-22 04:27 funboost/queues/peewee_queue.py
--rw-rw-rw-  2.0 fat    11024 b- defN 23-May-05 02:38 funboost/queues/sqla_queue.py
--rw-rw-rw-  2.0 fat     8267 b- defN 23-Jun-13 01:20 funboost/timing_job/__init__.py
--rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-06 06:09 funboost/timing_job/apscheduler_use_mysql_store.py
--rw-rw-rw-  2.0 fat      876 b- defN 23-May-30 09:38 funboost/timing_job/apscheduler_use_redis_store.py
--rw-rw-rw-  2.0 fat     1951 b- defN 23-Mar-09 07:27 funboost/utils/__init__.py
--rw-rw-rw-  2.0 fat     3124 b- defN 21-Dec-27 01:40 funboost/utils/apscheduler_monkey.py
--rw-rw-rw-  2.0 fat       96 b- defN 23-Jan-29 07:41 funboost/utils/block_exit.py
--rw-rw-rw-  2.0 fat     9972 b- defN 22-Apr-01 02:17 funboost/utils/bulk_operation.py
--rw-rw-rw-  2.0 fat     5923 b- defN 21-Dec-27 01:40 funboost/utils/custom_pysnooper.py
--rw-rw-rw-  2.0 fat    24296 b- defN 23-Jun-13 01:20 funboost/utils/decorators.py
--rw-rw-rw-  2.0 fat      251 b- defN 21-Dec-27 01:40 funboost/utils/develop_log.py
--rw-rw-rw-  2.0 fat     2837 b- defN 23-Jun-19 02:19 funboost/utils/kill_thread.py
--rw-rw-rw-  2.0 fat     2984 b- defN 23-Apr-07 02:11 funboost/utils/mongo_util.py
--rw-rw-rw-  2.0 fat     7367 b- defN 23-Mar-23 05:34 funboost/utils/monkey_color_log.py
--rw-rw-rw-  2.0 fat     2882 b- defN 23-Feb-23 05:04 funboost/utils/monkey_patches.py
--rw-rw-rw-  2.0 fat     3199 b- defN 21-Dec-27 01:40 funboost/utils/mqtt_util.py
--rw-rw-rw-  2.0 fat     4901 b- defN 21-Dec-27 01:40 funboost/utils/paramiko_util.py
--rw-rw-rw-  2.0 fat     2963 b- defN 22-Sep-17 06:12 funboost/utils/rabbitmq_factory.py
--rw-rw-rw-  2.0 fat     4628 b- defN 23-May-12 03:14 funboost/utils/redis_manager.py
--rw-rw-rw-  2.0 fat     5532 b- defN 22-Sep-17 06:12 funboost/utils/resource_monitoring.py
--rw-rw-rw-  2.0 fat     1418 b- defN 23-Mar-15 02:41 funboost/utils/restart_python.py
--rw-rw-rw-  2.0 fat     2985 b- defN 23-Jun-19 02:19 funboost/utils/show_funboost_flag.py
--rw-rw-rw-  2.0 fat     1204 b- defN 22-Dec-12 08:11 funboost/utils/simple_data_class.py
--rw-rw-rw-  2.0 fat     5407 b- defN 21-Dec-27 01:40 funboost/utils/time_util.py
--rw-rw-rw-  2.0 fat      408 b- defN 22-Jan-17 01:57 funboost/utils/un_strict_json_dumps.py
--rw-rw-rw-  2.0 fat        0 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/__init__.py
--rw-rw-rw-  2.0 fat      131 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/mongomq/__init__.py
--rw-rw-rw-  2.0 fat     2486 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/lock.py
--rw-rw-rw-  2.0 fat     7902 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/mongomq.py
--rw-rw-rw-  2.0 fat     7867 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/mongomq0000.py
--rw-rw-rw-  2.0 fat     4811 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/test.py
--rw-rw-rw-  2.0 fat      377 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/mongomq/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-19 06:09 funboost/utils/dependency_packages_in_pythonpath/__init__.py
--rw-rw-rw-  2.0 fat      341 b- defN 23-Mar-09 12:29 funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
--rw-rw-rw-  2.0 fat      814 b- defN 23-Jun-19 02:58 funboost/utils/dependency_packages_in_pythonpath/readme.md
--rw-rw-rw-  2.0 fat      165 b- defN 23-Jun-19 10:52 funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-  2.0 fat      475 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc
--rw-rw-rw-  2.0 fat      312 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-37.pyc
--rw-rw-rw-  2.0 fat      316 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc
--rw-rw-rw-  2.0 fat     1223 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
--rw-rw-rw-  2.0 fat   182652 b- defN 23-Mar-23 05:34 funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py
--rw-rw-rw-  2.0 fat      183 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py
--rw-rw-rw-  2.0 fat    62239 b- defN 23-Mar-23 05:34 funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py
--rw-rw-rw-  2.0 fat     1586 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py
--rw-rw-rw-  2.0 fat    11651 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py
--rw-rw-rw-  2.0 fat      427 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/py.typed
--rw-rw-rw-  2.0 fat      617 b- defN 23-Mar-07 10:20 funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md
--rw-rw-rw-  2.0 fat    12536 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py
--rw-rw-rw-  2.0 fat     1284 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py
--rw-rw-rw-  2.0 fat     1696 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-  2.0 fat     1272 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-  2.0 fat     1208 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-  2.0 fat   238822 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-311.pyc
--rw-rw-rw-  2.0 fat   158582 b- defN 23-Mar-30 09:33 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-37.pyc
--rw-rw-rw-  2.0 fat   157873 b- defN 23-Apr-07 04:20 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-39.pyc
--rw-rw-rw-  2.0 fat      439 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-311.pyc
--rw-rw-rw-  2.0 fat      338 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-37.pyc
--rw-rw-rw-  2.0 fat      342 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-39.pyc
--rw-rw-rw-  2.0 fat    79446 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-311.pyc
--rw-rw-rw-  2.0 fat    41714 b- defN 23-Mar-30 09:33 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-37.pyc
--rw-rw-rw-  2.0 fat    42233 b- defN 23-Apr-07 04:20 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-39.pyc
--rw-rw-rw-  2.0 fat     4280 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-311.pyc
--rw-rw-rw-  2.0 fat     3274 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-37.pyc
--rw-rw-rw-  2.0 fat     3135 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-39.pyc
--rw-rw-rw-  2.0 fat    14348 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-311.pyc
--rw-rw-rw-  2.0 fat    10139 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-37.pyc
--rw-rw-rw-  2.0 fat    10198 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-39.pyc
--rw-rw-rw-  2.0 fat     2926 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-  2.0 fat     1971 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-37.pyc
--rw-rw-rw-  2.0 fat     2017 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-  2.0 fat     5246 b- defN 23-Mar-23 05:32 funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py
--rw-rw-rw-  2.0 fat      587 b- defN 23-Mar-09 04:50 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py
--rw-rw-rw-  2.0 fat     9297 b- defN 23-Mar-23 05:32 funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py
--rw-rw-rw-  2.0 fat     3974 b- defN 23-Mar-09 04:14 funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py
--rw-rw-rw-  2.0 fat      169 b- defN 23-Mar-09 04:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py
--rw-rw-rw-  2.0 fat      280 b- defN 23-Mar-09 04:14 funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py
--rw-rw-rw-  2.0 fat     6480 b- defN 23-Mar-09 04:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-311.pyc
--rw-rw-rw-  2.0 fat     5063 b- defN 23-Mar-30 09:33 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-37.pyc
--rw-rw-rw-  2.0 fat     5083 b- defN 23-Apr-07 04:20 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-39.pyc
--rw-rw-rw-  2.0 fat      857 b- defN 23-Mar-09 04:50 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-  2.0 fat      763 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-  2.0 fat      767 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-  2.0 fat    11443 b- defN 23-Mar-09 07:17 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-311.pyc
--rw-rw-rw-  2.0 fat     8208 b- defN 23-Mar-30 09:33 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-37.pyc
--rw-rw-rw-  2.0 fat     8001 b- defN 23-Apr-07 04:20 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-39.pyc
--rw-rw-rw-  2.0 fat     4592 b- defN 23-Mar-09 04:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-311.pyc
--rw-rw-rw-  2.0 fat     3708 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-37.pyc
--rw-rw-rw-  2.0 fat     3732 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-39.pyc
--rw-rw-rw-  2.0 fat      357 b- defN 23-Mar-09 04:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-311.pyc
--rw-rw-rw-  2.0 fat      303 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc
--rw-rw-rw-  2.0 fat      311 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc
--rw-rw-rw-  2.0 fat      909 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/__init__.py
--rw-rw-rw-  2.0 fat     2243 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/pycompat.py
--rw-rw-rw-  2.0 fat    19131 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/tracer.py
--rw-rw-rw-  2.0 fat     2753 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/utils.py
--rw-rw-rw-  2.0 fat     3693 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/variables.py
--rw-rw-rw-  2.0 fat     2417 b- defN 23-Jun-09 01:42 funboost/utils/times/__init__.py
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-09 01:42 funboost/utils/times/version.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    26616 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    26669 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/RECORD
-246 files, 3302262 bytes uncompressed, 1870838 bytes compressed:  43.4%
+Zip file size: 1683837 bytes, number of entries: 220
+-rw-rw-rw-  2.0 fat     2402 b- defN 23-Jun-23 09:05 funboost/__init__.py
+-rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-03 06:12 funboost/__init__old.py
+-rw-rw-rw-  2.0 fat     6489 b- defN 23-Jun-21 13:54 funboost/constant.py
+-rw-rw-rw-  2.0 fat     7399 b- defN 23-Jun-23 09:05 funboost/funboost_config_deafult.py
+-rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-27 12:40 funboost/set_frame_config.py
+-rw-rw-rw-  2.0 fat     4186 b- defN 23-Jun-17 05:37 funboost/assist/celery_helper.py
+-rw-rw-rw-  2.0 fat     2089 b- defN 23-May-22 13:41 funboost/assist/dramatiq_helper.py
+-rw-rw-rw-  2.0 fat     1760 b- defN 23-May-26 03:56 funboost/assist/huey_helper.py
+-rw-rw-rw-  2.0 fat     1509 b- defN 23-Jun-09 14:04 funboost/assist/rq_helper.py
+-rw-rw-rw-  2.0 fat     4831 b- defN 23-Jun-08 14:14 funboost/assist/rq_windows_worker.py
+-rw-rw-rw-  2.0 fat     3930 b- defN 23-Apr-27 12:40 funboost/beggar_version_implementation/beggar_redis_consumer.py
+-rw-rw-rw-  2.0 fat      759 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/__init__.py
+-rw-rw-rw-  2.0 fat     3256 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/async_helper.py
+-rw-rw-rw-  2.0 fat     7227 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/async_pool_executor.py
+-rw-rw-rw-  2.0 fat     4723 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
+-rw-rw-rw-  2.0 fat     3011 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
+-rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/bounded_threadpoolexcutor.py
+-rw-rw-rw-  2.0 fat     1872 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/concurrent_pool_with_multi_process.py
+-rw-rw-rw-  2.0 fat     2402 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/custom_evenlet_pool_executor.py
+-rw-rw-rw-  2.0 fat     4421 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/custom_gevent_pool_executor.py
+-rw-rw-rw-  2.0 fat    11745 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/custom_threadpool_executor.py
+-rw-rw-rw-  2.0 fat     9317 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/custom_threadpool_executor000.py
+-rw-rw-rw-  2.0 fat      373 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/single_thread_executor.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/__init__.py
+-rw-rw-rw-  2.0 fat     9548 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor0223.py
+-rw-rw-rw-  2.0 fat     9568 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor_back.py
+-rw-rw-rw-  2.0 fat     5728 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor_janus.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Apr-27 12:40 funboost/consumers/__init__.py
+-rw-rw-rw-  2.0 fat    85359 b- defN 23-Jun-23 09:34 funboost/consumers/base_consumer.py
+-rw-rw-rw-  2.0 fat     7574 b- defN 23-Jun-05 13:53 funboost/consumers/celery_consumer.py
+-rw-rw-rw-  2.0 fat     4574 b- defN 23-Apr-27 12:40 funboost/consumers/celery_consumer000.py
+-rw-rw-rw-  2.0 fat     6033 b- defN 23-Jun-20 13:31 funboost/consumers/confirm_mixin.py
+-rw-rw-rw-  2.0 fat     2144 b- defN 23-May-26 03:56 funboost/consumers/dramatiq_consumer.py
+-rw-rw-rw-  2.0 fat     2025 b- defN 23-May-13 11:56 funboost/consumers/http_consumer.py
+-rw-rw-rw-  2.0 fat     4463 b- defN 23-Apr-27 12:40 funboost/consumers/http_consumer000.py
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-13 08:23 funboost/consumers/httpsqs_consumer.py
+-rw-rw-rw-  2.0 fat     1856 b- defN 23-May-26 03:56 funboost/consumers/huey_consumer.py
+-rw-rw-rw-  2.0 fat     4217 b- defN 23-May-13 08:23 funboost/consumers/kafka_consumer.py
+-rw-rw-rw-  2.0 fat     6947 b- defN 23-Jun-12 13:29 funboost/consumers/kafka_consumer_manually_commit.py
+-rw-rw-rw-  2.0 fat    10186 b- defN 23-May-13 08:23 funboost/consumers/kombu_consumer.py
+-rw-rw-rw-  2.0 fat     1291 b- defN 23-May-13 08:23 funboost/consumers/local_python_queue_consumer.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-May-13 08:23 funboost/consumers/mongomq_consumer.py
+-rw-rw-rw-  2.0 fat     2228 b- defN 23-May-13 08:23 funboost/consumers/mqtt_consumer.py
+-rw-rw-rw-  2.0 fat     2183 b- defN 23-May-13 08:23 funboost/consumers/nameko_consumer.py
+-rw-rw-rw-  2.0 fat     1076 b- defN 23-May-13 08:23 funboost/consumers/nats_consumer.py
+-rw-rw-rw-  2.0 fat     1461 b- defN 23-May-13 08:23 funboost/consumers/nsq_consumer.py
+-rw-rw-rw-  2.0 fat     1238 b- defN 23-May-13 08:16 funboost/consumers/peewee_conusmer.py
+-rw-rw-rw-  2.0 fat     1005 b- defN 23-May-13 08:16 funboost/consumers/persist_queue_consumer.py
+-rw-rw-rw-  2.0 fat     2414 b- defN 23-May-13 08:16 funboost/consumers/pulsar_consumer.py
+-rw-rw-rw-  2.0 fat     2048 b- defN 23-Jun-20 13:31 funboost/consumers/rabbitmq_amqpstorm_consumer.py
+-rw-rw-rw-  2.0 fat     5433 b- defN 23-May-13 08:17 funboost/consumers/rabbitmq_pika_consumer.py
+-rw-rw-rw-  2.0 fat     4674 b- defN 23-May-13 08:23 funboost/consumers/rabbitmq_pika_consumerv0.py
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-May-13 08:23 funboost/consumers/rabbitmq_rabbitpy_consumer.py
+-rw-rw-rw-  2.0 fat     3031 b- defN 23-May-13 08:23 funboost/consumers/redis_brpoplpush_consumer.py
+-rw-rw-rw-  2.0 fat     2829 b- defN 23-May-13 08:23 funboost/consumers/redis_consumer.py
+-rw-rw-rw-  2.0 fat     7545 b- defN 23-May-13 08:23 funboost/consumers/redis_consumer_ack_able.py
+-rw-rw-rw-  2.0 fat     4282 b- defN 23-Jun-21 13:54 funboost/consumers/redis_consumer_priority.py
+-rw-rw-rw-  2.0 fat      922 b- defN 23-May-13 08:23 funboost/consumers/redis_consumer_simple.py
+-rw-rw-rw-  2.0 fat     7135 b- defN 23-Apr-27 12:40 funboost/consumers/redis_filter.py
+-rw-rw-rw-  2.0 fat     1206 b- defN 23-May-13 08:23 funboost/consumers/redis_pubsub_consumer.py
+-rw-rw-rw-  2.0 fat     6497 b- defN 23-Jun-03 04:51 funboost/consumers/redis_stream_consumer.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-May-13 08:23 funboost/consumers/rocketmq_consumer.py
+-rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-08 14:00 funboost/consumers/rq_consumer.py
+-rw-rw-rw-  2.0 fat     1309 b- defN 23-May-13 08:23 funboost/consumers/sqlachemy_consumer.py
+-rw-rw-rw-  2.0 fat     2045 b- defN 23-May-13 08:23 funboost/consumers/tcp_consumer.py
+-rw-rw-rw-  2.0 fat     1340 b- defN 23-May-13 08:23 funboost/consumers/txt_file_consumer.py
+-rw-rw-rw-  2.0 fat     1643 b- defN 23-May-13 08:23 funboost/consumers/udp_consumer.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-May-13 08:23 funboost/consumers/zeromq_consumer.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 12:40 funboost/contrib/__init__.py
+-rw-rw-rw-  2.0 fat     4680 b- defN 23-May-22 13:41 funboost/contrib/queue2queue.py
+-rw-rw-rw-  2.0 fat     1817 b- defN 23-Apr-27 12:40 funboost/contrib/redis_consume_latest_msg_broker.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-03 05:40 funboost/core/__init__.py
+-rw-rw-rw-  2.0 fat     4984 b- defN 23-Jun-03 06:40 funboost/core/active_cousumer_info_getter.py
+-rw-rw-rw-  2.0 fat    16688 b- defN 23-Jun-23 09:05 funboost/core/booster.py
+-rw-rw-rw-  2.0 fat      576 b- defN 23-Jun-10 06:27 funboost/core/exit_signal.py
+-rw-rw-rw-  2.0 fat     8875 b- defN 23-Jun-04 14:54 funboost/core/fabric_deploy_helper.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-03 06:43 funboost/core/function_result_status_config.py
+-rw-rw-rw-  2.0 fat     8886 b- defN 23-Jun-23 09:05 funboost/core/function_result_status_saver.py
+-rw-rw-rw-  2.0 fat     1169 b- defN 23-Jun-08 14:00 funboost/core/get_booster.py
+-rw-rw-rw-  2.0 fat      340 b- defN 23-Jun-08 14:00 funboost/core/global_boosters.py
+-rw-rw-rw-  2.0 fat     1192 b- defN 23-Jun-23 09:05 funboost/core/helper_funs.py
+-rw-rw-rw-  2.0 fat     5388 b- defN 23-Jun-23 09:24 funboost/core/kill_remote_task.py
+-rw-rw-rw-  2.0 fat     7782 b- defN 23-Apr-27 12:40 funboost/core/msg_result_getter.py
+-rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-08 14:00 funboost/core/muliti_process_enhance.py
+-rw-rw-rw-  2.0 fat      178 b- defN 23-Apr-27 12:40 funboost/factories/__init__.py
+-rw-rw-rw-  2.0 fat     8976 b- defN 23-Jun-21 13:54 funboost/factories/broker_kind__publsiher_consumer_type_map.py
+-rw-rw-rw-  2.0 fat      946 b- defN 23-Jun-03 04:51 funboost/factories/consumer_factory.py
+-rw-rw-rw-  2.0 fat     2281 b- defN 23-Jun-03 04:51 funboost/factories/publisher_factotry.py
+-rw-rw-rw-  2.0 fat     4841 b- defN 23-Apr-27 12:40 funboost/function_result_web/app.py
+-rw-rw-rw-  2.0 fat     7345 b- defN 23-Apr-27 12:40 funboost/function_result_web/functions.py
+-rw-rw-rw-  2.0 fat     7674 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/assets/css/custom.css
+-rw-rw-rw-  2.0 fat    42839 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/assets/css/jquery.mCustomScrollbar.min.css
+-rw-rw-rw-  2.0 fat    23610 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/assets/img/user.jpg
+-rw-rw-rw-  2.0 fat     1106 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/assets/js/custom.js
+-rw-rw-rw-  2.0 fat    45483 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/assets/js/jquery.mCustomScrollbar.concat.min.js
+-rw-rw-rw-  2.0 fat    11065 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/css/style.css
+-rw-rw-rw-  2.0 fat  1153168 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/images/bg.jpg
+-rw-rw-rw-  2.0 fat      546 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/images/password.png
+-rw-rw-rw-  2.0 fat     2912 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/images/tick.png
+-rw-rw-rw-  2.0 fat      622 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/images/user.png
+-rw-rw-rw-  2.0 fat    96383 b- defN 22-Jul-15 16:25 funboost/function_result_web/static/js/jquery-1.11.0.min.js
+-rw-rw-rw-  2.0 fat    19501 b- defN 22-Jul-15 16:25 funboost/function_result_web/templates/index.html
+-rw-rw-rw-  2.0 fat     2007 b- defN 22-Jul-15 16:25 funboost/function_result_web/templates/login.html
+-rw-rw-rw-  2.0 fat      131 b- defN 23-Apr-27 12:40 funboost/publishers/__init__.py
+-rw-rw-rw-  2.0 fat    15860 b- defN 23-Jun-23 09:09 funboost/publishers/base_publisher.py
+-rw-rw-rw-  2.0 fat     3081 b- defN 23-Jun-23 09:09 funboost/publishers/celery_publisher.py
+-rw-rw-rw-  2.0 fat     3897 b- defN 23-Apr-28 13:25 funboost/publishers/celery_publisher000.py
+-rw-rw-rw-  2.0 fat     3541 b- defN 23-Apr-27 12:40 funboost/publishers/confluent_kafka_publisher.py
+-rw-rw-rw-  2.0 fat     1410 b- defN 23-May-21 15:14 funboost/publishers/dramatiq_publisher.py
+-rw-rw-rw-  2.0 fat      753 b- defN 23-May-13 08:23 funboost/publishers/http_publisher.py
+-rw-rw-rw-  2.0 fat     2783 b- defN 23-Apr-27 12:40 funboost/publishers/httpsqs_publisher.py
+-rw-rw-rw-  2.0 fat     1101 b- defN 23-May-26 03:56 funboost/publishers/huey_publisher.py
+-rw-rw-rw-  2.0 fat     2160 b- defN 23-Apr-27 12:40 funboost/publishers/kafka_publisher.py
+-rw-rw-rw-  2.0 fat     5321 b- defN 23-May-13 09:20 funboost/publishers/kombu_publisher.py
+-rw-rw-rw-  2.0 fat     1365 b- defN 23-Apr-27 12:40 funboost/publishers/local_python_queue_publisher.py
+-rw-rw-rw-  2.0 fat     1874 b- defN 23-Apr-27 12:40 funboost/publishers/mongomq_publisher.py
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-Apr-27 12:40 funboost/publishers/mqtt_publisher.py
+-rw-rw-rw-  2.0 fat     1670 b- defN 23-Jun-23 09:09 funboost/publishers/nameko_publisher.py
+-rw-rw-rw-  2.0 fat      776 b- defN 22-Jul-15 16:25 funboost/publishers/nats_publisher.py
+-rw-rw-rw-  2.0 fat     1302 b- defN 23-Apr-27 12:40 funboost/publishers/nsq_publisher.py
+-rw-rw-rw-  2.0 fat     1095 b- defN 23-Apr-27 12:40 funboost/publishers/peewee_publisher.py
+-rw-rw-rw-  2.0 fat     2540 b- defN 23-Apr-27 12:40 funboost/publishers/persist_queue_publisher.py
+-rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-27 12:40 funboost/publishers/pulsar_publisher.py
+-rw-rw-rw-  2.0 fat     3137 b- defN 23-Jun-20 13:31 funboost/publishers/rabbitmq_amqpstorm_publisher.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-27 12:40 funboost/publishers/rabbitmq_pika_publisher.py
+-rw-rw-rw-  2.0 fat     1953 b- defN 23-Apr-27 12:40 funboost/publishers/rabbitmq_rabbitpy_publisher.py
+-rw-rw-rw-  2.0 fat     3982 b- defN 23-May-13 08:23 funboost/publishers/redis_publisher.py
+-rw-rw-rw-  2.0 fat      278 b- defN 23-Apr-27 12:40 funboost/publishers/redis_publisher_lpush.py
+-rw-rw-rw-  2.0 fat     2104 b- defN 23-Jun-20 13:31 funboost/publishers/redis_publisher_priority.py
+-rw-rw-rw-  2.0 fat      872 b- defN 23-Apr-28 13:25 funboost/publishers/redis_publisher_simple.py
+-rw-rw-rw-  2.0 fat      721 b- defN 23-Apr-27 12:40 funboost/publishers/redis_pubsub_publisher.py
+-rw-rw-rw-  2.0 fat     2037 b- defN 22-Jul-15 16:25 funboost/publishers/redis_stream_publisher.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-27 12:40 funboost/publishers/rocketmq_publisher.py
+-rw-rw-rw-  2.0 fat      893 b- defN 23-Jun-10 08:06 funboost/publishers/rq_publisher.py
+-rw-rw-rw-  2.0 fat     1215 b- defN 23-Apr-27 12:40 funboost/publishers/sqla_queue_publisher.py
+-rw-rw-rw-  2.0 fat     1335 b- defN 23-May-13 08:23 funboost/publishers/tcp_publisher.py
+-rw-rw-rw-  2.0 fat     1380 b- defN 23-Apr-27 12:40 funboost/publishers/txt_file_publisher.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 23-May-13 08:23 funboost/publishers/udp_publisher.py
+-rw-rw-rw-  2.0 fat     1002 b- defN 22-Jul-15 16:25 funboost/publishers/zeromq_publisher.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-24 11:36 funboost/queues/__init__.py
+-rw-rw-rw-  2.0 fat     4944 b- defN 23-May-26 03:56 funboost/queues/peewee_queue.py
+-rw-rw-rw-  2.0 fat    11024 b- defN 23-May-13 08:23 funboost/queues/sqla_queue.py
+-rw-rw-rw-  2.0 fat     8267 b- defN 23-Jun-10 09:17 funboost/timing_job/__init__.py
+-rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-27 12:40 funboost/timing_job/apscheduler_use_mysql_store.py
+-rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-03 04:51 funboost/timing_job/apscheduler_use_redis_store.py
+-rw-rw-rw-  2.0 fat     1951 b- defN 23-Apr-27 12:40 funboost/utils/__init__.py
+-rw-rw-rw-  2.0 fat     3124 b- defN 22-Jul-15 16:25 funboost/utils/apscheduler_monkey.py
+-rw-rw-rw-  2.0 fat       96 b- defN 23-Apr-27 12:40 funboost/utils/block_exit.py
+-rw-rw-rw-  2.0 fat     9972 b- defN 22-Jul-15 16:25 funboost/utils/bulk_operation.py
+-rw-rw-rw-  2.0 fat     5923 b- defN 22-Jul-15 16:25 funboost/utils/custom_pysnooper.py
+-rw-rw-rw-  2.0 fat    24671 b- defN 23-Jun-21 13:54 funboost/utils/decorators.py
+-rw-rw-rw-  2.0 fat      251 b- defN 22-Jul-15 16:25 funboost/utils/develop_log.py
+-rw-rw-rw-  2.0 fat     4732 b- defN 23-Jun-22 12:06 funboost/utils/expire_lock.py
+-rw-rw-rw-  2.0 fat     3412 b- defN 23-Jun-23 06:28 funboost/utils/kill_thread.py
+-rw-rw-rw-  2.0 fat     2984 b- defN 23-Apr-27 12:40 funboost/utils/mongo_util.py
+-rw-rw-rw-  2.0 fat     7367 b- defN 23-Apr-27 12:40 funboost/utils/monkey_color_log.py
+-rw-rw-rw-  2.0 fat     2882 b- defN 23-Apr-27 12:40 funboost/utils/monkey_patches.py
+-rw-rw-rw-  2.0 fat     3199 b- defN 22-Jul-15 16:25 funboost/utils/mqtt_util.py
+-rw-rw-rw-  2.0 fat     4901 b- defN 22-Jul-15 16:25 funboost/utils/paramiko_util.py
+-rw-rw-rw-  2.0 fat     2963 b- defN 23-Apr-27 12:40 funboost/utils/rabbitmq_factory.py
+-rw-rw-rw-  2.0 fat     4628 b- defN 23-May-20 04:45 funboost/utils/redis_manager.py
+-rw-rw-rw-  2.0 fat     5532 b- defN 23-Apr-27 12:40 funboost/utils/resource_monitoring.py
+-rw-rw-rw-  2.0 fat     1418 b- defN 23-Apr-27 12:40 funboost/utils/restart_python.py
+-rw-rw-rw-  2.0 fat     2985 b- defN 23-Jun-17 05:42 funboost/utils/show_funboost_flag.py
+-rw-rw-rw-  2.0 fat     1204 b- defN 22-Jul-15 16:25 funboost/utils/simple_data_class.py
+-rw-rw-rw-  2.0 fat     5407 b- defN 22-Jul-15 16:25 funboost/utils/time_util.py
+-rw-rw-rw-  2.0 fat      408 b- defN 22-Jul-15 16:25 funboost/utils/un_strict_json_dumps.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/__init__.py
+-rw-rw-rw-  2.0 fat      131 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/mongomq/__init__.py
+-rw-rw-rw-  2.0 fat     2486 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/mongomq/lock.py
+-rw-rw-rw-  2.0 fat     7902 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/mongomq/mongomq.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/mongomq/mongomq0000.py
+-rw-rw-rw-  2.0 fat     4811 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/mongomq/test.py
+-rw-rw-rw-  2.0 fat      377 b- defN 22-Jul-15 16:25 funboost/utils/dependency_packages/mongomq/utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-20 13:31 funboost/utils/dependency_packages_in_pythonpath/__init__.py
+-rw-rw-rw-  2.0 fat      341 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
+-rw-rw-rw-  2.0 fat      814 b- defN 23-Jun-20 13:31 funboost/utils/dependency_packages_in_pythonpath/readme.md
+-rw-rw-rw-  2.0 fat      169 b- defN 23-Jun-20 14:51 funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc
+-rw-rw-rw-  2.0 fat     1282 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
+-rw-rw-rw-  2.0 fat   187456 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py
+-rw-rw-rw-  2.0 fat      191 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py
+-rw-rw-rw-  2.0 fat    63907 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py
+-rw-rw-rw-  2.0 fat     1682 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py
+-rw-rw-rw-  2.0 fat    11957 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py
+-rw-rw-rw-  2.0 fat      442 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/py.typed
+-rw-rw-rw-  2.0 fat      617 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md
+-rw-rw-rw-  2.0 fat    12865 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py
+-rw-rw-rw-  2.0 fat     1208 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-  2.0 fat   157873 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-39.pyc
+-rw-rw-rw-  2.0 fat      342 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-39.pyc
+-rw-rw-rw-  2.0 fat    42233 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-39.pyc
+-rw-rw-rw-  2.0 fat     3135 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-39.pyc
+-rw-rw-rw-  2.0 fat    10198 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-39.pyc
+-rw-rw-rw-  2.0 fat     2017 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-39.pyc
+-rw-rw-rw-  2.0 fat     5379 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py
+-rw-rw-rw-  2.0 fat      603 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py
+-rw-rw-rw-  2.0 fat     9531 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py
+-rw-rw-rw-  2.0 fat     4072 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py
+-rw-rw-rw-  2.0 fat      176 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py
+-rw-rw-rw-  2.0 fat      287 b- defN 23-Apr-27 12:40 funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py
+-rw-rw-rw-  2.0 fat     5083 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-39.pyc
+-rw-rw-rw-  2.0 fat      767 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-  2.0 fat     8001 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-39.pyc
+-rw-rw-rw-  2.0 fat     3732 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-39.pyc
+-rw-rw-rw-  2.0 fat      311 b- defN 23-Apr-27 13:29 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc
+-rw-rw-rw-  2.0 fat      909 b- defN 22-Jul-15 16:25 funboost/utils/pysnooper_ydf/__init__.py
+-rw-rw-rw-  2.0 fat     2243 b- defN 22-Jul-15 16:25 funboost/utils/pysnooper_ydf/pycompat.py
+-rw-rw-rw-  2.0 fat    19131 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/tracer.py
+-rw-rw-rw-  2.0 fat     2753 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/utils.py
+-rw-rw-rw-  2.0 fat     3693 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/variables.py
+-rw-rw-rw-  2.0 fat     2332 b- defN 23-Jun-08 14:07 funboost/utils/times/__init__.py
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-08 14:07 funboost/utils/times/version.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26615 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    22651 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/RECORD
+220 files, 2710526 bytes uncompressed, 1646687 bytes compressed:  39.3%
```

## zipnote {}

```diff
@@ -237,14 +237,17 @@
 
 Filename: funboost/core/global_boosters.py
 Comment: 
 
 Filename: funboost/core/helper_funs.py
 Comment: 
 
+Filename: funboost/core/kill_remote_task.py
+Comment: 
+
 Filename: funboost/core/msg_result_getter.py
 Comment: 
 
 Filename: funboost/core/muliti_process_enhance.py
 Comment: 
 
 Filename: funboost/factories/__init__.py
@@ -261,20 +264,14 @@
 
 Filename: funboost/function_result_web/app.py
 Comment: 
 
 Filename: funboost/function_result_web/functions.py
 Comment: 
 
-Filename: funboost/function_result_web/__pycache__/app.cpython-37.pyc
-Comment: 
-
-Filename: funboost/function_result_web/__pycache__/functions.cpython-37.pyc
-Comment: 
-
 Filename: funboost/function_result_web/static/assets/css/custom.css
 Comment: 
 
 Filename: funboost/function_result_web/static/assets/css/jquery.mCustomScrollbar.min.css
 Comment: 
 
 Filename: funboost/function_result_web/static/assets/img/user.jpg
@@ -453,14 +450,17 @@
 
 Filename: funboost/utils/decorators.py
 Comment: 
 
 Filename: funboost/utils/develop_log.py
 Comment: 
 
+Filename: funboost/utils/expire_lock.py
+Comment: 
+
 Filename: funboost/utils/kill_thread.py
 Comment: 
 
 Filename: funboost/utils/mongo_util.py
 Comment: 
 
 Filename: funboost/utils/monkey_color_log.py
@@ -525,21 +525,15 @@
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/readme.md
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-37.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-37.pyc
+Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
 Comment: 
@@ -570,74 +564,32 @@
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-39.pyc
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py
@@ -651,56 +603,26 @@
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-39.pyc
 Comment: 
 
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-311.pyc
-Comment: 
-
-Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc
-Comment: 
-
 Filename: funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc
 Comment: 
 
 Filename: funboost/utils/pysnooper_ydf/__init__.py
 Comment: 
 
 Filename: funboost/utils/pysnooper_ydf/pycompat.py
@@ -717,23 +639,23 @@
 
 Filename: funboost/utils/times/__init__.py
 Comment: 
 
 Filename: funboost/utils/times/version.py
 Comment: 
 
-Filename: funboost-23.3.dist-info/LICENSE
+Filename: funboost-23.4.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-23.3.dist-info/METADATA
+Filename: funboost-23.4.dist-info/METADATA
 Comment: 
 
-Filename: funboost-23.3.dist-info/WHEEL
+Filename: funboost-23.4.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-23.3.dist-info/top_level.txt
+Filename: funboost-23.4.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-23.3.dist-info/RECORD
+Filename: funboost-23.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funboost/__init__.py

```diff
@@ -27,14 +27,15 @@
 from funboost.factories.consumer_factory import get_consumer
 
 from funboost.timing_job import fsdf_background_scheduler, timing_publish_deco, funboost_aps_scheduler
 from funboost.constant import BrokerEnum, ConcurrentModeEnum
 
 from funboost.core.booster import boost, Booster
 from funboost.core.get_booster import get_booster
+from funboost.core.kill_remote_task import RemoteTaskKiller
 
 from funboost.core.exit_signal import set_interrupt_signal_handler
 from funboost.core.helper_funs import run_forever
 
 
 set_interrupt_signal_handler()
```

## funboost/constant.py

```diff
@@ -1,10 +1,10 @@
 # coding= utf-8
 class BrokerEnum:
-    RABBITMQ_AMQPSTORM = 0  # 使用 amqpstorm 包操作rabbitmq  作为 分布式消息队列，支持消费确认.推荐这个。
+    RABBITMQ_AMQPSTORM = 0  # 使用 amqpstorm 包操作rabbitmq  作为 分布式消息队列，支持消费确认.强烈推荐这个作为funboost中间件。
 
     RABBITMQ_RABBITPY = 1  # 使用 rabbitpy 包操作rabbitmq  作为 分布式消息队列，支持消费确认。
 
     REDIS = 2  # 使用 redis 的 list结构，brpop 作为分布式消息队列。随意重启和关闭会丢失大量消息，不支持消费确认。注重性能不在乎丢失消息可以选这个redis方案。
 
     LOCAL_PYTHON_QUEUE = 3  # 使用python queue.Queue实现的基于当前python进程的消息队列，不支持跨进程 跨脚本 跨机器共享任务，不支持持久化，适合一次性短期简单任务。
     MEMORY_QUEUE = LOCAL_PYTHON_QUEUE  # 别名，python本地queue就是基于python自带的语言的queue.Queue，消息存在python程序的内存中，不支持重启断点接续。
@@ -22,15 +22,15 @@
 
     """基于confluent-kafka包，包的性能比kafka-python提升10倍。同时应对反复随意重启部署消费代码的场景，此消费者实现至少消费一次，第8种BrokerEnum.KAFKA是最多消费一次。"""
     CONFLUENT_KAFKA = 16
     KAFKA_CONFLUENT = CONFLUENT_KAFKA
 
     REDIS_ACK_ABLE = 9  # 基于redis的 list + 临时unack的set队列，采用了 lua脚本操持了取任务和加到pengding为原子性，随意重启和掉线不会丢失任务。
 
-    REDIS_PRIORITY = 109 #  # 基于redis的多 list + 临时unack的set队列，blpop监听多个key，和rabbitmq的x-max-priority属性一样，支持任务优先级。
+    REDIS_PRIORITY = 109 #  # 基于redis的多 list + 临时unack的set队列，blpop监听多个key，和rabbitmq的x-max-priority属性一样，支持任务优先级。看文档4.29优先级队列说明。
 
     SQLACHEMY = 10  # 基于SQLACHEMY 的连接作为分布式消息队列中间件支持持久化和消费确认。支持mysql oracle sqlserver等5种数据库。
 
     ROCKETMQ = 11  # 基于 rocketmq 作为分布式消息队列，这个中间件必须在linux下运行，win不支持。
 
     REDIS_STREAM = 12  # 基于redis 5.0 版本以后，使用 stream 数据结构作为分布式消息队列，支持消费确认和持久化和分组消费，是redis官方推荐的消息队列形式，比list结构更适合。
 
@@ -80,10 +80,10 @@
 
 
 class ConcurrentModeEnum:
     THREADING = 1
     GEVENT = 2
     EVENTLET = 3
     ASYNC = 4  # asyncio并发，适用于async def定义的函数。
-    SINGLE_THREAD = 5
+    SINGLE_THREAD = 5  # 如果你不想并发，不想预先从消息队列中间件拉取消息到python程序的内存queue队列缓冲中，那么就适合使用此并发模式。
 
 # is_fsdf_remote_run = 0
```

## funboost/funboost_config_deafult.py

```diff
@@ -140,14 +140,15 @@
     do_task_filtering = False
     task_filtering_expire_seconds = 0
 
     function_result_status_persistance_conf = FunctionResultStatusPersistanceConfig(False, False, 7 * 24 * 3600)
     user_custom_record_process_info_func = None
 
     is_using_rpc_mode = False
+    is_support_remote_kill_task = False
 
     is_do_not_run_by_specify_time_effect = False
     do_not_run_by_specify_time = ('10:00:00', '22:00:00')
 
     schedule_tasks_on_main_thread = False
 
     broker_exclusive_config = {}
```

## funboost/consumers/base_consumer.py

```diff
@@ -32,15 +32,15 @@
 from apscheduler.executors.pool import ThreadPoolExecutor as ApschedulerThreadPoolExecutor
 
 import nb_log
 from funboost.concurrent_pool.single_thread_executor import SoloExecutor
 from funboost.core.function_result_status_saver import FunctionResultStatusPersistanceConfig, ResultPersistenceHelper, FunctionResultStatus
 
 # noinspection PyUnresolvedReferences
-from funboost.core.helper_funs import _delete_keys_and_return_new_dict, get_publish_time
+from funboost.core.helper_funs import delete_keys_and_return_new_dict, get_publish_time
 from nb_log import get_logger, LoggerLevelSetterMixin, nb_print, LoggerMixin, \
     LoggerMixinDefaultWithFileHandler, stdout_write, is_main_process, \
     nb_log_config_default
 # noinspection PyUnresolvedReferences
 from funboost.concurrent_pool.async_helper import simple_run_in_executor
 from funboost.concurrent_pool.async_pool_executor import AsyncPoolExecutor
 # noinspection PyUnresolvedReferences
@@ -59,14 +59,15 @@
 from funboost.utils import decorators, time_util, RedisMixin, un_strict_json_dumps
 # noinspection PyUnresolvedReferences
 from funboost.utils.bulk_operation import MongoBulkWriteHelper, InsertOne
 from funboost.utils.mongo_util import MongoMixin
 from funboost import funboost_config_deafult
 # noinspection PyUnresolvedReferences
 from funboost.constant import ConcurrentModeEnum, BrokerEnum
+from funboost.core import kill_remote_task
 
 
 # patch_apscheduler_run_job()
 
 
 class ExceptionForRetry(Exception):
     """为了重试的，抛出错误。只是定义了一个子类，用不用都可以，函数出任何类型错误了框架都会自动重试"""
@@ -191,20 +192,21 @@
                  log_level=10, is_print_detail_exception=True, is_show_message_get_from_broker=False,
                  qps: float = 0, is_using_distributed_frequency_control=False,
                  msg_expire_senconds=0, is_send_consumer_hearbeat_to_redis=False,
                  logger_prefix='', create_logger_file=True, do_task_filtering=False,
                  task_filtering_expire_seconds=0,
                  is_do_not_run_by_specify_time_effect=False,
                  do_not_run_by_specify_time=('10:00:00', '22:00:00'),
-                 schedule_tasks_on_main_thread=False,
                  function_result_status_persistance_conf=FunctionResultStatusPersistanceConfig(
                      False, False, 7 * 24 * 3600),
                  user_custom_record_process_info_func: typing.Callable = None,
                  is_using_rpc_mode=False,
+                 is_support_remote_kill_task=False,
                  broker_exclusive_config: dict = None,
+                 schedule_tasks_on_main_thread=False,
                  ):
 
         """
         :param queue_name:
         :param consuming_function: 处理消息的函数。
         :param consumin_function_decorator : 函数的装饰器。因为此框架做参数自动转指点，需要获取精准的入参名称，不支持在消费函数上叠加 @ *args  **kwargs的装饰器，如果想用装饰器可以这里指定。
         :param function_timeout : 超时秒数，函数运行超过这个时间，则自动杀死函数。为0是不限制。
@@ -237,14 +239,15 @@
         :param is_do_not_run_by_specify_time_effect :是否使不运行的时间段生效
         :param do_not_run_by_specify_time   :不运行的时间段
         :param schedule_tasks_on_main_thread :直接在主线程调度任务，意味着不能直接在当前主线程同时开启两个消费者。
         :param function_result_status_persistance_conf   :配置。是否保存函数的入参，运行结果和运行状态到mongodb。
                这一步用于后续的参数追溯，任务统计和web展示，需要安装mongo。
         :param user_custom_record_process_info_func  提供一个用户自定义的保存消息处理记录到某个地方例如mysql数据库的函数，函数仅仅接受一个入参，入参类型是 FunctionResultStatus，用户可以打印参数
         :param is_using_rpc_mode 是否使用rpc模式，可以在发布端获取消费端的结果回调，但消耗一定性能，使用async_result.result时候会等待阻塞住当前线程。
+        :param is_support_remote_kill_task 是否支持远程任务杀死功能，如果任务数量少，单个任务耗时长，确实需要远程发送命令来杀死正在运行的函数，才设置为true，否则不建议开启此功能。
         :param broker_exclusive_config 加上一个不同种类中间件非通用的配置,不同中间件自身独有的配置，不是所有中间件都兼容的配置，因为框架支持30种消息队列，消息队列不仅仅是一般的先进先出queue这么简单的概念，
             例如kafka支持消费者组，rabbitmq也支持各种独特概念例如各种ack机制 复杂路由机制，每一种消息队列都有独特的配置参数意义，可以通过这里传递。
 
         执行流程为
         1、 实例化消费者类，设置各种控制属性
         2、启动 start_consuming_message 启动消费
         3、start_consuming_message 中 调用 _shedual_task 从中间件循环取消息
@@ -379,15 +382,16 @@
         self._do_not_run_by_specify_time = do_not_run_by_specify_time  # 可以设置在指定的时间段不运行。
         self._schedule_tasks_on_main_thread = schedule_tasks_on_main_thread
 
         self._function_result_status_persistance_conf = function_result_status_persistance_conf
         self._result_persistence_helper: ResultPersistenceHelper
         self._user_custom_record_process_info_func = user_custom_record_process_info_func
 
-        self._is_using_rpc_mode = is_using_rpc_mode
+        self._is_using_rpc_mode = is_using_rpc_mode  # 是否使用rpc模式 需要安装和配置好redis
+        self._is_support_remote_kill_task = is_support_remote_kill_task # 是否支持远程杀死函数task，需要安装和配置好redis
 
         if broker_exclusive_config is None:
             broker_exclusive_config = {}
         self.broker_exclusive_config = copy.deepcopy(self.BROKER_EXCLUSIVE_CONFIG_DEFAULT)
         self.broker_exclusive_config.update(broker_exclusive_config)
 
         self._stop_flag = None
@@ -518,14 +522,16 @@
 
         self._distributed_consumer_statistics = DistributedConsumerStatistics(self)
         if self._is_send_consumer_hearbeat_to_redis:
             self._distributed_consumer_statistics.run()
             self.logger.warning(f'启动了分布式环境 使用 redis 的键 hearbeat:{self._queue_name} 统计活跃消费者 ，当前消费者唯一标识为 {self.consumer_identification}')
 
         self.keep_circulating(10, block=False)(self.check_heartbeat_and_message_count)()  # 间隔时间最好比self._unit_time_for_count小整数倍，不然日志不准。
+        if self._is_support_remote_kill_task:
+            kill_remote_task.RemoteTaskKiller(self.queue_name, None).start_cycle_kill_task()
         if self._do_task_filtering:
             self._redis_filter.delete_expire_filter_task_cycle()  # 这个默认是RedisFilter类，是个pass不运行。所以用别的消息中间件模式，不需要安装和配置redis。
         if self._schedule_tasks_on_main_thread:
             self.keep_circulating(1)(self._shedual_task)()
         else:
             self._concurrent_mode_dispatcher.schedulal_task_with_no_block()
         setattr(funboost_config_deafult, 'has_start_a_consumer_flag', 1)
@@ -572,15 +578,15 @@
                 break
 
         if self._judge_is_daylight():
             self._requeue(kw)
             time.sleep(self.time_interval_for_check_do_not_run_time)
             return
 
-        function_only_params = _delete_keys_and_return_new_dict(kw['body'], )
+        function_only_params = delete_keys_and_return_new_dict(kw['body'], )
         if self._get_priority_conf(kw, 'do_task_filtering') and self._redis_filter.check_value_exists(
                 function_only_params):  # 对函数的参数进行检查，过滤已经执行过并且成功的任务。
             self.logger.warning(f'redis的 [{self._redis_filter_key_name}] 键 中 过滤任务 {kw["body"]}')
             self._confirm_consume(kw)
             return
         publish_time = get_publish_time(kw['body'])
         msg_expire_senconds_priority = self._get_priority_conf(kw, 'msg_expire_senconds')
@@ -695,34 +701,39 @@
         elif self._concurrent_mode == 3:
             # noinspection PyArgumentList
             concurrent_info = f'[{eventlet.getcurrent()}  {threading.active_count()}]'
         '''
         return concurrent_info
 
     def _set_do_not_delete_extra_from_msg(self):
-        """例如从死信队列，把完整的包括extra的消息移到另一个正常队列，不要把extra中的参数去掉"""
+        """例如从死信队列，把完整的包括extra的消息移到另一个正常队列，不要把extra中的参数去掉
+        queue2queue.py 的 consume_and_push_to_another_queue 中操作了这个，普通用户无需调用这个方法。
+        """
         self._do_not_delete_extra_from_msg = True
 
+    # noinspection PyProtectedMember
     def _run(self, kw: dict, ):
         # print(kw)
         try:
             t_start_run_fun = time.time()
             max_retry_times = self._get_priority_conf(kw, 'max_retry_times')
             current_function_result_status = FunctionResultStatus(self.queue_name, self.consuming_function.__name__, kw['body'], )
             current_retry_times = 0
-            function_only_params = _delete_keys_and_return_new_dict(kw['body'])
+            function_only_params = delete_keys_and_return_new_dict(kw['body'])
             for current_retry_times in range(max_retry_times + 1):
                 current_function_result_status = self._run_consuming_function_with_confirm_and_retry(kw, current_retry_times=current_retry_times,
                                                                                                      function_result_status=FunctionResultStatus(
                                                                                                          self.queue_name, self.consuming_function.__name__,
                                                                                                          kw['body']))
                 if (current_function_result_status.success is True or current_retry_times == max_retry_times
-                        or current_function_result_status.has_requeue or current_function_result_status.has_to_dlx_queue):
+                        or current_function_result_status._has_requeue
+                        or current_function_result_status._has_to_dlx_queue
+                        or current_function_result_status._has_kill_task):
                     break
-            if not (current_function_result_status.has_requeue and self.BROKER_KIND in [BrokerEnum.RABBITMQ_AMQPSTORM, BrokerEnum.RABBITMQ_PIKA, BrokerEnum.RABBITMQ_RABBITPY]):  # 已经nack了，不能ack，否则rabbitmq delevar tag 报错
+            if not (current_function_result_status._has_requeue and self.BROKER_KIND in [BrokerEnum.RABBITMQ_AMQPSTORM, BrokerEnum.RABBITMQ_PIKA, BrokerEnum.RABBITMQ_RABBITPY]):  # 已经nack了，不能ack，否则rabbitmq delevar tag 报错
                 self._confirm_consume(kw)
 
             self._result_persistence_helper.save_function_result_to_mongo(current_function_result_status)
             if self._get_priority_conf(kw, 'do_task_filtering'):
                 self._redis_filter.add_a_value(function_only_params)  # 函数执行成功后，添加函数的参数排序后的键值对字符串到set中。
             if current_function_result_status.success is False and current_retry_times == max_retry_times:
                 log_msg = f'函数 {self.consuming_function.__name__} 达到最大重试次数 {self._get_priority_conf(kw, "max_retry_times")} 后,仍然失败， 入参是  {function_only_params} '
@@ -764,24 +775,32 @@
             if self._user_custom_record_process_info_func:
                 self._user_custom_record_process_info_func(current_function_result_status)
         except BaseException as e:
             log_msg = f' error 严重错误 {type(e)} {e} '
             self.logger.critical(msg=f'{log_msg} \n', exc_info=True)
             self.error_file_logger.critical(msg=f'{log_msg} \n', exc_info=True)
 
+    # noinspection PyProtectedMember
     def _run_consuming_function_with_confirm_and_retry(self, kw: dict, current_retry_times,
                                                        function_result_status: FunctionResultStatus, ):
-        function_only_params = _delete_keys_and_return_new_dict(kw['body']) if self._do_not_delete_extra_from_msg is False else kw['body']
+        function_only_params = delete_keys_and_return_new_dict(kw['body']) if self._do_not_delete_extra_from_msg is False else kw['body']
+        task_id = kw['body']['extra']['task_id']
         t_start = time.time()
         function_result_status.run_times = current_retry_times + 1
         try:
             function_timeout = self._get_priority_conf(kw, 'function_timeout')
             function_run0 = self.consuming_function if self._consumin_function_decorator is None else self._consumin_function_decorator(self.consuming_function)
             function_run = function_run0 if not function_timeout else self._concurrent_mode_dispatcher.timeout_deco(
                 function_timeout)(function_run0)
+            if self._is_support_remote_kill_task:
+                if kill_remote_task.RemoteTaskKiller(self.queue_name, task_id).judge_need_revoke_run():  # 如果远程指令杀死任务，如果还没开始运行函数，就取消运行
+                    function_result_status._has_kill_task = True
+                    self.logger.warning(f'取消运行 {task_id} {function_only_params}')
+                    return function_result_status
+                function_run = kill_remote_task.kill_fun_deco(task_id)(function_run)  # 用杀死装饰器包装起来在另一个线程运行函数
             function_result_status.result = function_run(**function_only_params)
             if asyncio.iscoroutine(function_result_status.result):
                 log_msg = f'''异步的协程消费函数必须使用 async 并发模式并发,请设置消费函数 {self.consuming_function.__name__} 的concurrent_mode 为 ConcurrentModeEnum.ASYNC 或 4'''
                 self.logger.critical(msg=f'{log_msg} \n')
                 self.error_file_logger.critical(msg=f'{log_msg} \n')
                 # noinspection PyProtectedMember,PyUnresolvedReferences
 
@@ -800,52 +819,58 @@
                 time.sleep(0.1)  # 防止快速无限出错入队出队，导致cpu和中间件忙
                 # 重回队列如果不修改task_id,insert插入函数消费状态结果到mongo会主键重复。要么保存函数消费状态使用replace，要么需要修改taskikd
                 # kw_new = copy.deepcopy(kw)
                 # new_task_id =f'{self._queue_name}_result:{uuid.uuid4()}'
                 # kw_new['body']['extra']['task_id'] = new_task_id
                 # self._requeue(kw_new)
                 self._requeue(kw)
-                function_result_status.has_requeue = True
+                function_result_status._has_requeue = True
             if isinstance(e, ExceptionForPushToDlxqueue):
                 log_msg = f'函数 [{self.consuming_function.__name__}] 中发生错误 {type(e)}  {e}，消息放入死信队列 {self._dlx_queue_name}'
                 self.logger.critical(msg=f'{log_msg} \n')
                 self.error_file_logger.critical(msg=f'{log_msg} \n')
                 self.publisher_of_dlx_queue.publish(kw['body'])  # 发布到死信队列，不重回当前队列
-                function_result_status.has_to_dlx_queue = True
-            if isinstance(e, (ExceptionForRequeue, ExceptionForPushToDlxqueue)):
+                function_result_status._has_to_dlx_queue = True
+            if isinstance(e, kill_remote_task.TaskHasKilledError):
+                log_msg = f'task_id 为 {task_id} , 函数 [{self.consuming_function.__name__}] 运行入参 {function_only_params}   ，已被远程指令杀死 {type(e)}  {e}'
+                self.logger.critical(msg=f'{log_msg} ')
+                self.error_file_logger.critical(msg=f'{log_msg} ')
+                function_result_status._has_kill_task = True
+            if isinstance(e, (ExceptionForRequeue, ExceptionForPushToDlxqueue,kill_remote_task.TaskHasKilledError)):
                 return function_result_status
             log_msg = f'''函数 {self.consuming_function.__name__}  第{current_retry_times + 1}次运行发生错误，
                               函数运行时间是 {round(time.time() - t_start, 4)} 秒,\n  入参是  {function_only_params}    \n 原因是 {type(e)} {e} '''
             self.logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             # traceback.print_exc()
             function_result_status.exception = f'{e.__class__.__name__}    {str(e)}'
             function_result_status.result = FunctionResultStatus.FUNC_RUN_ERROR
         return function_result_status
 
+    # noinspection PyProtectedMember
     async def _async_run(self, kw: dict, ):
         # """虽然和上面有点大面积重复相似，这个是为了asyncio模式的，asyncio模式真的和普通同步模式的代码思维和形式区别太大，
         # 框架实现兼容async的消费函数很麻烦复杂，连并发池都要单独写"""
         try:
             t_start_run_fun = time.time()
             max_retry_times = self._get_priority_conf(kw, 'max_retry_times')
             current_function_result_status = FunctionResultStatus(self.queue_name, self.consuming_function.__name__, kw['body'], )
             current_retry_times = 0
-            function_only_params = _delete_keys_and_return_new_dict(kw['body'])
+            function_only_params = delete_keys_and_return_new_dict(kw['body'])
             for current_retry_times in range(max_retry_times + 1):
                 current_function_result_status = await self._async_run_consuming_function_with_confirm_and_retry(kw, current_retry_times=current_retry_times,
                                                                                                                  function_result_status=FunctionResultStatus(
                                                                                                                      self.queue_name, self.consuming_function.__name__,
                                                                                                                      kw['body'], ),
                                                                                                                  )
-                if current_function_result_status.success is True or current_retry_times == max_retry_times or current_function_result_status.has_requeue:
+                if current_function_result_status.success is True or current_retry_times == max_retry_times or current_function_result_status._has_requeue:
                     break
 
             # self._result_persistence_helper.save_function_result_to_mongo(function_result_status)
-            if not (current_function_result_status.has_requeue and self.BROKER_KIND in [BrokerEnum.RABBITMQ_AMQPSTORM, BrokerEnum.RABBITMQ_PIKA, BrokerEnum.RABBITMQ_RABBITPY]):
+            if not (current_function_result_status._has_requeue and self.BROKER_KIND in [BrokerEnum.RABBITMQ_AMQPSTORM, BrokerEnum.RABBITMQ_PIKA, BrokerEnum.RABBITMQ_RABBITPY]):
                 await simple_run_in_executor(self._confirm_consume, kw)
             await simple_run_in_executor(self._result_persistence_helper.save_function_result_to_mongo, current_function_result_status)
             if self._get_priority_conf(kw, 'do_task_filtering'):
                 # self._redis_filter.add_a_value(function_only_params)  # 函数执行成功后，添加函数的参数排序后的键值对字符串到set中。
                 await simple_run_in_executor(self._redis_filter.add_a_value, function_only_params)
             if current_function_result_status.success is False and current_retry_times == max_retry_times:
                 log_msg = f'函数 {self.consuming_function.__name__} 达到最大重试次数 {self._get_priority_conf(kw, "max_retry_times")} 后,仍然失败， 入参是  {function_only_params} '
@@ -889,19 +914,20 @@
             if self._user_custom_record_process_info_func:
                 await self._user_custom_record_process_info_func(current_function_result_status)
         except BaseException as e:
             log_msg = f' error 严重错误 {type(e)} {e} '
             self.logger.critical(msg=f'{log_msg} \n', exc_info=True)
             self.error_file_logger.critical(msg=f'{log_msg} \n', exc_info=True)
 
+    # noinspection PyProtectedMember
     async def _async_run_consuming_function_with_confirm_and_retry(self, kw: dict, current_retry_times,
                                                                    function_result_status: FunctionResultStatus, ):
         """虽然和上面有点大面积重复相似，这个是为了asyncio模式的，asyncio模式真的和普通同步模式的代码思维和形式区别太大，
         框架实现兼容async的消费函数很麻烦复杂，连并发池都要单独写"""
-        function_only_params = _delete_keys_and_return_new_dict(kw['body']) if self._do_not_delete_extra_from_msg is False else kw['body']
+        function_only_params = delete_keys_and_return_new_dict(kw['body']) if self._do_not_delete_extra_from_msg is False else kw['body']
         function_result_status.run_times = current_retry_times + 1
         # noinspection PyBroadException
         t_start = time.time()
         try:
             corotinue_obj = self.consuming_function(**function_only_params)
             if not asyncio.iscoroutine(corotinue_obj):
                 log_msg = f'''当前设置的并发模式为 async 并发模式，但消费函数不是异步协程函数，请不要把消费函数 {self.consuming_function.__name__} 的 concurrent_mode 设置为 4'''
@@ -926,21 +952,21 @@
                 log_msg = f'函数 [{self.consuming_function.__name__}] 中发生错误 {type(e)}  {e} 。 消息重新放入当前队列 {self._queue_name}'
                 self.logger.critical(msg=f'{log_msg} \n')
                 self.error_file_logger.critical(msg=f'{log_msg} \n')
                 # time.sleep(1)  # 防止快速无限出错入队出队，导致cpu和中间件忙
                 await asyncio.sleep(0.1)
                 # return self._requeue(kw)
                 await simple_run_in_executor(self._requeue, kw)
-                function_result_status.has_requeue = True
+                function_result_status._has_requeue = True
             if isinstance(e, ExceptionForPushToDlxqueue):
                 log_msg = f'函数 [{self.consuming_function.__name__}] 中发生错误 {type(e)}  {e}，消息放入死信队列 {self._dlx_queue_name}'
                 self.logger.critical(msg=f'{log_msg} \n')
                 self.error_file_logger.critical(msg=f'{log_msg} \n')
                 await simple_run_in_executor(self.publisher_of_dlx_queue.publish, kw['body'])  # 发布到死信队列，不重回当前队列
-                function_result_status.has_to_dlx_queue = True
+                function_result_status._has_to_dlx_queue = True
             if isinstance(e, (ExceptionForRequeue, ExceptionForPushToDlxqueue)):
                 return function_result_status
             log_msg = f'''函数 {self.consuming_function.__name__}  第{current_retry_times + 1}次运行发生错误，
                               函数运行时间是 {round(time.time() - t_start, 4)} 秒,\n  入参是  {function_only_params}    \n 原因是 {type(e)} {e} '''
             self.logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             function_result_status.exception = f'{e.__class__.__name__}    {str(e)}'
@@ -958,14 +984,21 @@
             if self._msg_num_in_broker != -1:
                 self.logger.info(f'队列 [{self._queue_name}] 中还有 [{self._msg_num_in_broker}] 个任务')
             self._last_timestamp_print_msg_num = time.time()
         if self._msg_num_in_broker != 0:
             self._last_timestamp_when_has_task_in_queue = time.time()
         return self._msg_num_in_broker
 
+    @staticmethod
+    def _thread_kill_task_by_task_id():
+        task_id_tuple = RedisMixin().redis_db_frame_version3.brpop(kill_remote_task.REDIS_LIST_KEY_KILL_TASK, timeout=60)
+        if task_id_tuple:
+            task_id = task_id_tuple[1]
+            kill_remote_task.kill_task(task_id)
+
     @abc.abstractmethod
     def _requeue(self, kw):
         """重新入队"""
         raise NotImplementedError
 
     def _apscheduler_job_miss(self, event):
         """
```

## funboost/core/booster.py

```diff
@@ -46,14 +46,15 @@
                  task_filtering_expire_seconds: float = _Undefined,
                  is_do_not_run_by_specify_time_effect: bool = _Undefined,
                  do_not_run_by_specify_time: bool = _Undefined,
                  schedule_tasks_on_main_thread: bool = _Undefined,
                  function_result_status_persistance_conf: FunctionResultStatusPersistanceConfig = _Undefined,
                  user_custom_record_process_info_func: typing.Union[typing.Callable, None] = _Undefined,
                  is_using_rpc_mode: bool = _Undefined,
+                 is_support_remote_kill_task: bool = _Undefined,
                  broker_exclusive_config: dict = _Undefined,
                  broker_kind: int = _Undefined,
                  boost_decorator_default_params=BoostDecoratorDefaultParams()):
         """
            funboost.funboost_config_deafult.BoostDecoratorDefaultParams 的值会自动被你项目根目录下的funboost_config.BoostDecoratorDefaultParams的值覆盖，
            如果boost装饰器不传参，默认使用funboost_config.BoostDecoratorDefaultParams的配置
 
@@ -93,14 +94,15 @@
            :param is_do_not_run_by_specify_time_effect :是否使不运行的时间段生效
            :param do_not_run_by_specify_time   :不运行的时间段
            :param schedule_tasks_on_main_thread :直接在主线程调度任务，意味着不能直接在当前主线程同时开启两个消费者。fun.consume()就阻塞了，这之后的代码不会运行
            :param function_result_status_persistance_conf   :配置。是否保存函数的入参，运行结果和运行状态到mongodb。
                   这一步用于后续的参数追溯，任务统计和web展示，需要安装mongo。
            :param user_custom_record_process_info_func  提供一个用户自定义的保存消息处理记录到某个地方例如mysql数据库的函数，函数仅仅接受一个入参，入参类型是 FunctionResultStatus，用户可以打印参数
            :param is_using_rpc_mode 是否使用rpc模式，可以在发布端获取消费端的结果回调，但消耗一定性能，使用async_result.result时候会等待阻塞住当前线程。。
+           :param is_support_remote_kill_task 是否支持远程任务杀死功能，如果任务数量少，单个任务耗时长，确实需要远程发送命令来杀死正在运行的函数，才设置为true，否则不建议开启此功能。
            :param broker_exclusive_config 加上一个不同种类中间件非通用的配置,不同中间件自身独有的配置，不是所有中间件都兼容的配置，因为框架支持30种消息队列，消息队列不仅仅是一般的先进先出queue这么简单的概念，
                    例如kafka支持消费者组，rabbitmq也支持各种独特概念例如各种ack机制 复杂路由机制，每一种消息队列都有独特的配置参数意义，可以通过这里传递。
            :param broker_kind:中间件种类，支持30种消息队列。 入参见 BrokerEnum枚举类的属性。
            :param boost_decorator_default_params: oostDecoratorDefaultParams是
                    @boost装饰器默认的全局入参。如果boost没有亲自指定某个入参，就自动使用funboost_config.py的BoostDecoratorDefaultParams中的配置。
                            如果你嫌弃每个 boost 装饰器相同入参太多重复了，可以在 funboost_config.py 文件中设置boost装饰器的全局默认值。
                    BoostDecoratorDefaultParams() 实例化时候也可以传递这个boost装饰器任何的入参，BoostDecoratorDefaultParams是个数据类，百度python3.7dataclass的概念，类似。
```

## funboost/core/function_result_status_saver.py

```diff
@@ -10,22 +10,22 @@
 import pymongo
 import pymongo.errors
 import sys
 
 from pymongo import IndexModel, ReplaceOne
 
 from funboost.core.function_result_status_config import FunctionResultStatusPersistanceConfig
-from funboost.core.helper_funs import get_publish_time, _delete_keys_and_return_new_dict
+from funboost.core.helper_funs import get_publish_time, delete_keys_and_return_new_dict
 from funboost.utils import time_util, decorators
 from funboost.utils.mongo_util import MongoMixin
 from nb_log import LoggerMixin, LoggerLevelSetterMixin
 
 
 
-class FunctionResultStatus(LoggerMixin, LoggerLevelSetterMixin):
+class FunctionResultStatus():
     host_name = socket.gethostname()
 
     script_name_long = sys.argv[0]
     script_name = script_name_long.split('/')[-1].split('\\')[-1]
 
     FUNC_RUN_ERROR = 'FUNC_RUN_ERROR'
 
@@ -37,33 +37,36 @@
         self.msg_dict = msg_dict
         self.task_id = self.msg_dict.get('extra', {}).get('task_id', '')
         self.process_id = os.getpid()
         self.thread_id = threading.get_ident()
         self.publish_time = publish_time = get_publish_time(msg_dict)
         if publish_time:
             self.publish_time_str = time_util.DatetimeConverter(publish_time).datetime_str
-        function_params = _delete_keys_and_return_new_dict(msg_dict, )
+        function_params = delete_keys_and_return_new_dict(msg_dict, )
         self.params = function_params
         self.params_str = json.dumps(function_params, ensure_ascii=False)
         self.result = None
         self.run_times = 0
         self.exception = None
         self.time_start = time.time()
         self.time_cost = None
         self.time_end = None
         self.success = False
         self.total_thread = threading.active_count()
-        self.has_requeue = False
-        self.has_to_dlx_queue = False
-        self.set_log_level(20)
+        self._has_requeue = False
+        self._has_to_dlx_queue = False
+        self._has_kill_task = False
 
     def get_status_dict(self, without_datetime_obj=False):
         self.time_end = time.time()
         self.time_cost = round(self.time_end - self.time_start, 3)
-        item = self.__dict__
+        item ={}
+        for k,v in self.__dict__.items():
+            if not k.startswith('_'):
+                item[k] =v
         item['host_name'] = self.host_name
         item['host_process'] = self.host_process
         item['script_name'] = self.script_name
         item['script_name_long'] = self.script_name_long
         # item.pop('time_start')
         datetime_str = time_util.DatetimeConverter().datetime_str
         try:
@@ -74,15 +77,15 @@
                      'insert_minutes': datetime_str[:-3],
                      })
         if not without_datetime_obj:
             item.update({'insert_time': datetime.datetime.now(),
                          'utime': datetime.datetime.utcnow(),
                          })
         else:
-            item = _delete_keys_and_return_new_dict(item, ['insert_time', 'utime'])
+            item = delete_keys_and_return_new_dict(item, ['insert_time', 'utime'])
         # kw['body']['extra']['task_id']
         # item['_id'] = self.task_id.split(':')[-1] or str(uuid.uuid4())
         item['_id'] = self.task_id or str(uuid.uuid4())
         # self.logger.warning(item['_id'])
         # self.logger.warning(item)
         return item
```

## funboost/core/helper_funs.py

```diff
@@ -6,15 +6,15 @@
     """
     :param paramsx:
     :return:
     """
     return paramsx.get('extra', {}).get('publish_time', None)
 
 
-def _delete_keys_and_return_new_dict(dictx: dict, keys: list = None):
+def delete_keys_and_return_new_dict(dictx: dict, keys: list = None):
     dict_new = copy.copy(dictx)  # 主要是去掉一级键 publish_time，浅拷贝即可。新的消息已经不是这样了。
     keys = ['publish_time', 'publish_time_format', 'extra'] if keys is None else keys
     for dict_key in keys:
         try:
             dict_new.pop(dict_key)
         except KeyError:
             pass
```

## funboost/factories/broker_kind__publsiher_consumer_type_map.py

 * *Ordering differences only*

```diff
@@ -1,14 +1,9 @@
 import typing
 
-from funboost.consumers.redis_consumer_priority import RedisPriorityConsumer
-from funboost.publishers.base_publisher import AbstractPublisher
-from funboost.consumers.base_consumer import AbstractConsumer
-
-from funboost.constant import BrokerEnum
 
 from funboost.publishers.http_publisher import HTTPPublisher
 from funboost.publishers.nats_publisher import NatsPublisher
 from funboost.publishers.peewee_publisher import PeeweePublisher
 from funboost.publishers.redis_publisher_lpush import RedisPublisherLpush
 from funboost.publishers.redis_publisher_priority import RedisPriorityPublisher
 from funboost.publishers.redis_pubsub_publisher import RedisPubSubPublisher
@@ -26,14 +21,15 @@
 from funboost.publishers.rabbitmq_rabbitpy_publisher import RabbitmqPublisherUsingRabbitpy
 from funboost.publishers.redis_publisher import RedisPublisher
 from funboost.publishers.rocketmq_publisher import RocketmqPublisher
 from funboost.publishers.redis_stream_publisher import RedisStreamPublisher
 from funboost.publishers.mqtt_publisher import MqttPublisher
 from funboost.publishers.httpsqs_publisher import HttpsqsPublisher
 
+from funboost.consumers.redis_consumer_priority import RedisPriorityConsumer
 from funboost.consumers.redis_pubsub_consumer import RedisPbSubConsumer
 from funboost.consumers.http_consumer import HTTPConsumer
 from funboost.consumers.kafka_consumer import KafkaConsumer
 from funboost.consumers.local_python_queue_consumer import LocalPythonQueueConsumer
 from funboost.consumers.mongomq_consumer import MongoMqConsumer
 from funboost.consumers.nats_consumer import NatsConsumer
 from funboost.consumers.nsq_consumer import NsqConsumer
@@ -50,14 +46,18 @@
 from funboost.consumers.tcp_consumer import TCPConsumer
 from funboost.consumers.txt_file_consumer import TxtFileConsumer
 from funboost.consumers.udp_consumer import UDPConsumer
 from funboost.consumers.zeromq_consumer import ZeroMqConsumer
 from funboost.consumers.mqtt_consumer import MqttConsumer
 from funboost.consumers.httpsqs_consumer import HttpsqsConsumer
 
+from funboost.publishers.base_publisher import AbstractPublisher
+from funboost.consumers.base_consumer import AbstractConsumer
+from funboost.constant import BrokerEnum
+
 broker_kind__publsiher_consumer_type_map = {
     BrokerEnum.RABBITMQ_AMQPSTORM: (RabbitmqPublisherUsingAmqpStorm, RabbitmqConsumerAmqpStorm),
     BrokerEnum.RABBITMQ_RABBITPY: (RabbitmqPublisherUsingRabbitpy, RabbitmqConsumerRabbitpy),
     BrokerEnum.REDIS: (RedisPublisher, RedisConsumer),
     BrokerEnum.MEMORY_QUEUE: (LocalPythonQueuePublisher, LocalPythonQueueConsumer),
     BrokerEnum.RABBITMQ_PIKA: (RabbitmqPublisher, RabbitmqConsumer),
     BrokerEnum.MONGOMQ: (MongoMqPublisher, MongoMqConsumer),
```

## funboost/publishers/base_publisher.py

```diff
@@ -211,26 +211,26 @@
         task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
         extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
                         'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
         if priority_control_config:
             extra_params.update(priority_control_config.to_dict())
         extra_params.update(raw_extra)
         msg['extra'] = extra_params
-        return msg, msg_function_kw, extra_params
+        return msg, msg_function_kw, extra_params,task_id
 
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None):
         """
 
         :param msg:函数的入参字典或者字典转json。,例如消费函数是 def add(x,y)，你就发布 {"x":1,"y":2}
         :param task_id:可以指定task_id,也可以不指定就随机生产uuid
         :param priority_control_config:优先级配置，消息可以携带优先级配置，覆盖boost的配置。
         :return:
         """
-        msg, msg_function_kw, extra_params = self._convert_msg(msg, task_id, priority_control_config)
+        msg, msg_function_kw, extra_params,task_id = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         decorators.handle_exception(retry_times=10, is_throw_error=True, time_sleep=0.1)(
             self.concrete_realization_of_publish)(json.dumps(msg, ensure_ascii=False))
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
```

## funboost/publishers/celery_publisher.py

```diff
@@ -37,15 +37,15 @@
         # self._celery_app = celery_app
         # self._celery_fun = f
 
         celery_app.conf.task_routes.update({self.queue_name: {"queue": self.queue_name}})
 
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None) -> celery.result.AsyncResult:
-        msg, msg_function_kw, extra_params = self._convert_msg(msg, task_id, priority_control_config)
+        msg, msg_function_kw, extra_params,task_id = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         celery_result = celery_app.send_task(name=self.queue_name, kwargs=msg_function_kw, task_id=extra_params['task_id'])  # type: celery.result.AsyncResult
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
             if time.time() - self._current_time > 10:
```

## funboost/publishers/nameko_publisher.py

```diff
@@ -21,15 +21,15 @@
     """
 
     def custom_init(self):
         self._rpc = ClusterRpcProxy(NAMEKO_CONFIG)
 
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None):
-        msg, msg_function_kw, extra_params = self._convert_msg(msg, task_id, priority_control_config)
+        msg, msg_function_kw, extra_params,task_id = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         with self._rpc as rpc:
             res = getattr(rpc, self.queue_name).call(**msg_function_kw)
         self.logger.debug(f'调用nameko的 {self.queue_name} service 的 call方法 耗时{round(time.time() - t_start, 4)}秒，入参  {msg_function_kw}')  # 显示msg太长了。
         return res
 
     def concrete_realization_of_publish(self, msg):
```

## funboost/utils/decorators.py

```diff
@@ -243,44 +243,57 @@
             self.logger.debug(f'对下面代码片段进行计时:  \n执行"{self._file_name}:{self._line}" 用时 {round(self.t_spend, 2)} 秒')
 
 
 class RedisDistributedLockContextManager(LoggerMixin, LoggerLevelSetterMixin):
     """
     分布式redis锁上下文管理.
     """
+    '''
+    redis 官方推荐的 redlock-py
+    https://github.com/SPSCommerce/redlock-py/blob/master/redlock/__init__.py
+    '''
+    unlock_script = """
+       if redis.call("get",KEYS[1]) == ARGV[1] then
+           return redis.call("del",KEYS[1])
+       else
+           return 0
+       end"""
 
     def __init__(self, redis_client, redis_lock_key, expire_seconds=30, ):
         self.redis_client = redis_client
         self.redis_lock_key = redis_lock_key
         self._expire_seconds = expire_seconds
         self.identifier = str(uuid.uuid4())
         self.has_aquire_lock = False
 
     def __enter__(self):
         self._line = sys._getframe().f_back.f_lineno  # 调用此方法的代码的函数
         self._file_name = sys._getframe(1).f_code.co_filename  # 哪个文件调了用此方法
-        self.redis_client.set(self.redis_lock_key, value=self.identifier, ex=self._expire_seconds, nx=True)
-        identifier_in_redis = self.redis_client.get(self.redis_lock_key)
-        if identifier_in_redis and identifier_in_redis.decode() == self.identifier:
-            self.has_aquire_lock = True
+        ret = self.redis_client.set(self.redis_lock_key, value=self.identifier, ex=self._expire_seconds, nx=True)
+
+        self.has_aquire_lock = False if ret is None else True
+        if self.has_aquire_lock:
+            log_msg = f'\n"{self._file_name}:{self._line}" 这行代码获得了redis锁 {self.redis_lock_key}'
+        else:
+            log_msg = f'\n"{self._file_name}:{self._line}" 这行代码此次没有获得redis锁 {self.redis_lock_key}'
+        # print(self.logger.level,log_msg)
+        self.logger.debug(log_msg)
         return self
 
     def __bool__(self):
         return self.has_aquire_lock
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        if self.has_aquire_lock:
-            self.redis_client.delete(self.redis_lock_key)
-        if self.has_aquire_lock:
-            log_msg = f'\n"{self._file_name}:{self._line}" 这行代码获得了redis锁 {self.redis_lock_key}'
-            self.logger.debug(log_msg)
+        # self.redis_client.delete(self.redis_lock_key)
+        unlock = self.redis_client.register_script(self.unlock_script)
+        result = unlock(keys=[self.redis_lock_key], args=[self.identifier])
+        if result:
+            return True
         else:
-            log_msg = f'\n"{self._file_name}:{self._line}" 这行代码此次没有获得redis锁 {self.redis_lock_key}'
-            self.logger.debug(log_msg)
-
+            return False
 
 """
 @contextmanager
         def some_generator(<arguments>):
             <setup>
             try:
                 yield <value>
```

## funboost/utils/kill_thread.py

```diff
@@ -1,11 +1,11 @@
 import ctypes
 import threading
 import time
-
+from funboost.utils.time_util import DatetimeConverter
 import requests
 
 
 class ThreadKillAble(threading.Thread):
     task_id = None
     killed = False
     event_kill = threading.Event()
@@ -15,30 +15,20 @@
     ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(thread_id), ctypes.py_object(SystemExit))
 
 
 class ThreadHasKilled(Exception):
     pass
 
 
-def kill_thread_by_task_id(task_id):
-    for t in threading.enumerate():
-        if isinstance(t, ThreadKillAble):
-            thread_task_id = getattr(t, 'task_id', None)
-            if thread_task_id == task_id:
-                t.killed = True
-                t.event_kill.set()
-                kill_thread(t.ident)
-
-
 def kill_fun_deco(task_id):
     def _inner(f):
         def __inner(*args, **kwargs):
             def _new_func(oldfunc, result, oldfunc_args, oldfunc_kwargs):
                 result.append(oldfunc(*oldfunc_args, **oldfunc_kwargs))
-                threading.current_thread().event_kill.set()   # noqa
+                threading.current_thread().event_kill.set()  # noqa
 
             result = []
             new_kwargs = {
                 'oldfunc': f,
                 'result': result,
                 'oldfunc_args': args,
                 'oldfunc_kwargs': kwargs
@@ -46,58 +36,78 @@
 
             thd = ThreadKillAble(target=_new_func, args=(), kwargs=new_kwargs)
             thd.task_id = task_id
             thd.event_kill = threading.Event()
             thd.start()
             thd.event_kill.wait()
             if not result and thd.killed is True:
-                raise ThreadHasKilled(f'线程已被杀死 {thd.task_id}')
+                raise ThreadHasKilled(f'{DatetimeConverter()} 线程已被杀死 {thd.task_id}')
             return result[0]
 
         return __inner
 
     return _inner
 
 
+def kill_thread_by_task_id(task_id):
+    for t in threading.enumerate():
+        if isinstance(t, ThreadKillAble):
+            thread_task_id = getattr(t, 'task_id', None)
+            if thread_task_id == task_id:
+                t.killed = True
+                t.event_kill.set()
+                kill_thread(t.ident)
+
+
 if __name__ == '__main__':
     import nb_log
+
     test_lock = threading.Lock()
-    @kill_fun_deco(task_id='task1234')
-    def my_fun(x):
-        test_lock.acquire()
-        print(f'start {x}')
-        resp = requests.get('http://127.0.0.1:5000') # flask接口里面sleep30秒，
-        print(resp.text)
-        # for i in range(10):
-        #     time.sleep(2)
-        test_lock.release()
-        print(f'over {x}')
-        return 666
 
 
-    @kill_fun_deco(task_id='task5678')
-    def my_fun2(x):
+    def my_fun(x):
+        """
+        使用lock.acquire(),强行杀死会一直无法释放锁
+        """
         test_lock.acquire()
         print(f'start {x}')
-        resp = requests.get('http://127.0.0.1:5000')
-        print(resp.text)
-        # for i in range(10):
-        #     time.sleep(2)
+        # resp = requests.get('http://127.0.0.1:5000')  # flask接口里面sleep30秒，
+        # print(resp.text)
+        for i in range(10):
+            time.sleep(2)
         test_lock.release()
         print(f'over {x}')
         return 666
 
 
-    def kill_thread_by_task(task_id):
-        time.sleep(5)
-        kill_thread_by_task_id(task_id)
-
-
-    threading.Thread(target=kill_thread_by_task,args=('task1234',)).start()
-    threading.Thread(target=my_fun, args=(777,)).start()
-    threading.Thread(target=my_fun2, args=(888,)).start()
+    def my_fun2(x):
+        """
+        使用with lock,强行杀死会不会出现一直无法释放锁
+        """
+        with test_lock:
+            print(f'start {x}')
+            # resp = requests.get('http://127.0.0.1:5000')  # flask接口里面sleep30秒，
+            # print(resp.text)
+            for i in range(10):
+                time.sleep(2)
+            print(f'over {x}')
+            return 666
+
+
+    threading.Thread(target=kill_fun_deco(task_id='task1234')(my_fun2), args=(777,)).start()
+    threading.Thread(target=kill_fun_deco(task_id='task5678')(my_fun2), args=(888,)).start()
+    time.sleep(5)
+    kill_thread_by_task_id('task1234')
 
     """
-    强行杀死线程，会导致锁一直不能释放
+    第一种代码：
+    test_lock.acquire()
+    执行io耗时代码
+    test_lock.release()
+    如果使用lock.acquire()获得锁以后，执行耗时代码时候，还没有执行lock.release() 强行杀死线程，会导致锁一直不能释放
+    
+    第二种代码
+    with test_lock:
+        执行io耗时代码
+    使用with lock 获得锁以后，执行耗时代码时候，强行杀死线程，则不会导致锁一直不能释放
+    
     """
-
-
```

## funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar  9 12:29:11 2023 UTC, .py size: 341 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,20 +1,20 @@
-00000000: 610d 0d0a 0000 0000 17d1 0964 5501 0000  a..........dU...
+00000000: 610d 0d0a 0000 0000 506d 4a64 5501 0000  a.......PmJdU...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6503 6502 6504 8301 6a05 8301 5a06  ..e.e.e...j...Z.
 00000050: 6500 6a07 a008 6403 6506 a102 0100 6401  e.j...d.e.....d.
 00000060: 5300 2904 e900 0000 004e 2901 da04 5061  S.)......N)...Pa
 00000070: 7468 e904 0000 0029 09da 0373 7973 da07  th.....)...sys..
 00000080: 7061 7468 6c69 6272 0200 0000 da03 7374  pathlibr......st
 00000090: 72da 085f 5f66 696c 655f 5fda 0670 6172  r..__file__..par
-000000a0: 656e 745a 0b63 7572 7265 6e74 5f64 6972  entZ.current_dir
+000000a0: 656e 74da 0b63 7572 7265 6e74 5f64 6972  ent..current_dir
 000000b0: da04 7061 7468 da06 696e 7365 7274 a900  ..path..insert..
-000000c0: 720b 0000 0072 0b00 0000 fa57 443a 5c63  r....r.....WD:\c
+000000c0: 720c 0000 0072 0c00 0000 fa57 443a 5c63  r....r.....WD:\c
 000000d0: 6f64 6573 5c66 756e 626f 6f73 745c 6675  odes\funboost\fu
 000000e0: 6e62 6f6f 7374 5c75 7469 6c73 5c64 6570  nboost\utils\dep
 000000f0: 656e 6465 6e63 795f 7061 636b 6167 6573  endency_packages
 00000100: 5f69 6e5f 7079 7468 6f6e 7061 7468 5c61  _in_pythonpath\a
 00000110: 6464 5f74 6f5f 7079 7468 6f6e 7061 7468  dd_to_pythonpath
 00000120: 2e70 79da 083c 6d6f 6475 6c65 3e01 0000  .py..<module>...
 00000130: 0073 0600 0000 0801 0c02 0e02            .s..........
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py

 * *Ordering differences only*

```diff
@@ -1,59 +1,59 @@
-from aioredis.client import Redis, StrictRedis
-from aioredis.connection import (
-    BlockingConnectionPool,
-    Connection,
-    ConnectionPool,
-    SSLConnection,
-    UnixDomainSocketConnection,
-)
-from aioredis.exceptions import (
-    AuthenticationError,
-    AuthenticationWrongNumberOfArgsError,
-    BusyLoadingError,
-    ChildDeadlockedError,
-    ConnectionError,
-    DataError,
-    InvalidResponse,
-    PubSubError,
-    ReadOnlyError,
-    RedisError,
-    ResponseError,
-    TimeoutError,
-    WatchError,
-)
-from aioredis.utils import from_url
-
-
-def int_or_str(value):
-    try:
-        return int(value)
-    except ValueError:
-        return value
-
-
-__version__ = "2.0.1"
-VERSION = tuple(map(int_or_str, __version__.split(".")))
-
-__all__ = [
-    "AuthenticationError",
-    "AuthenticationWrongNumberOfArgsError",
-    "BlockingConnectionPool",
-    "BusyLoadingError",
-    "ChildDeadlockedError",
-    "Connection",
-    "ConnectionError",
-    "ConnectionPool",
-    "DataError",
-    "from_url",
-    "InvalidResponse",
-    "PubSubError",
-    "ReadOnlyError",
-    "Redis",
-    "RedisError",
-    "ResponseError",
-    "SSLConnection",
-    "StrictRedis",
-    "TimeoutError",
-    "UnixDomainSocketConnection",
-    "WatchError",
-]
+from aioredis.client import Redis, StrictRedis
+from aioredis.connection import (
+    BlockingConnectionPool,
+    Connection,
+    ConnectionPool,
+    SSLConnection,
+    UnixDomainSocketConnection,
+)
+from aioredis.exceptions import (
+    AuthenticationError,
+    AuthenticationWrongNumberOfArgsError,
+    BusyLoadingError,
+    ChildDeadlockedError,
+    ConnectionError,
+    DataError,
+    InvalidResponse,
+    PubSubError,
+    ReadOnlyError,
+    RedisError,
+    ResponseError,
+    TimeoutError,
+    WatchError,
+)
+from aioredis.utils import from_url
+
+
+def int_or_str(value):
+    try:
+        return int(value)
+    except ValueError:
+        return value
+
+
+__version__ = "2.0.1"
+VERSION = tuple(map(int_or_str, __version__.split(".")))
+
+__all__ = [
+    "AuthenticationError",
+    "AuthenticationWrongNumberOfArgsError",
+    "BlockingConnectionPool",
+    "BusyLoadingError",
+    "ChildDeadlockedError",
+    "Connection",
+    "ConnectionError",
+    "ConnectionPool",
+    "DataError",
+    "from_url",
+    "InvalidResponse",
+    "PubSubError",
+    "ReadOnlyError",
+    "Redis",
+    "RedisError",
+    "ResponseError",
+    "SSLConnection",
+    "StrictRedis",
+    "TimeoutError",
+    "UnixDomainSocketConnection",
+    "WatchError",
+]
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py

 * *Ordering differences only*

```diff
@@ -1,4804 +1,4804 @@
-import asyncio
-import datetime
-import hashlib
-import inspect
-import re
-import time as mod_time
-import warnings
-from typing import (
-    AbstractSet,
-    Any,
-    AsyncIterator,
-    Awaitable,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    MutableMapping,
-    NoReturn,
-    Optional,
-    Sequence,
-    Set,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    ValuesView,
-    cast,
-)
-
-from aioredis.compat import Protocol, TypedDict
-from aioredis.connection import (
-    Connection,
-    ConnectionPool,
-    EncodableT,
-    SSLConnection,
-    UnixDomainSocketConnection,
-)
-from aioredis.exceptions import (
-    ConnectionError,
-    DataError,
-    ExecAbortError,
-    ModuleError,
-    NoScriptError,
-    PubSubError,
-    RedisError,
-    ResponseError,
-    TimeoutError,
-    WatchError,
-)
-from aioredis.lock import Lock
-from aioredis.utils import safe_str, str_if_bytes
-
-AbsExpiryT = Union[int, datetime.datetime]
-ExpiryT = Union[int, datetime.timedelta]
-ZScoreBoundT = Union[float, str]  # str allows for the [ or ( prefix
-BitfieldOffsetT = Union[int, str]  # str allows for #x syntax
-_StringLikeT = Union[bytes, str, memoryview]
-KeyT = _StringLikeT  # Main redis key space
-PatternT = _StringLikeT  # Patterns matched against keys, fields etc
-FieldT = EncodableT  # Fields within hash tables, streams and geo commands
-KeysT = Union[KeyT, Sequence[KeyT]]
-ChannelT = _StringLikeT
-GroupT = _StringLikeT  # Consumer group
-ConsumerT = _StringLikeT  # Consumer name
-StreamIdT = Union[int, _StringLikeT]
-ScriptTextT = _StringLikeT
-TimeoutSecT = Union[int, float, _StringLikeT]
-# Mapping is not covariant in the key type, which prevents
-# Mapping[_StringLikeT, X from accepting arguments of type Dict[str, X]. Using
-# a TypeVar instead of a Union allows mappings with any of the permitted types
-# to be passed. Care is needed if there is more than one such mapping in a
-# type signature because they will all be required to be the same key type.
-AnyKeyT = TypeVar("AnyKeyT", bytes, str, memoryview)
-AnyFieldT = TypeVar("AnyFieldT", bytes, str, memoryview)
-AnyChannelT = ChannelT
-PubSubHandler = Callable[[Dict[str, str]], None]
-
-SYM_EMPTY = b""
-EMPTY_RESPONSE = "EMPTY_RESPONSE"
-
-_KeyT = TypeVar("_KeyT", bound=KeyT)
-_ArgT = TypeVar("_ArgT", KeyT, EncodableT)
-_RedisT = TypeVar("_RedisT", bound="Redis")
-_NormalizeKeysT = TypeVar("_NormalizeKeysT", bound=Mapping[ChannelT, object])
-
-
-def list_or_args(
-    keys: Union[_KeyT, Iterable[_KeyT]], args: Optional[Iterable[_ArgT]]
-) -> List[Union[_KeyT, _ArgT]]:
-    # returns a single new list combining keys and args
-    key_list: List[Union[_KeyT, _ArgT]]
-    try:
-        iter(keys)  # type: ignore[arg-type]
-        keys = cast(Iterable[_KeyT], keys)
-        # a string or bytes instance can be iterated, but indicates
-        # keys wasn't passed as a list
-        if isinstance(keys, (bytes, str)):
-            key_list = [keys]
-        else:
-            key_list = list(keys)
-    except TypeError:
-        key_list = [cast(memoryview, keys)]
-    if args:
-        key_list.extend(args)
-    return key_list
-
-
-def timestamp_to_datetime(response):
-    """Converts a unix timestamp to a Python datetime object"""
-    if not response:
-        return None
-    try:
-        response = int(response)
-    except ValueError:
-        return None
-    return datetime.datetime.fromtimestamp(response)
-
-
-def string_keys_to_dict(key_string, callback):
-    return dict.fromkeys(key_string.split(), callback)
-
-
-class CaseInsensitiveDict(dict):
-    """Case insensitive dict implementation. Assumes string keys only."""
-
-    def __init__(self, data):
-        for k, v in data.items():
-            self[k.upper()] = v
-
-    def __contains__(self, k):
-        return super().__contains__(k.upper())
-
-    def __delitem__(self, k):
-        super().__delitem__(k.upper())
-
-    def __getitem__(self, k):
-        return super().__getitem__(k.upper())
-
-    def get(self, k, default=None):
-        return super().get(k.upper(), default)
-
-    def __setitem__(self, k, v):
-        super().__setitem__(k.upper(), v)
-
-    def update(self, data):
-        data = CaseInsensitiveDict(data)
-        super().update(data)
-
-
-def parse_debug_object(response):
-    """Parse the results of Redis's DEBUG OBJECT command into a Python dict"""
-    # The 'type' of the object is the first item in the response, but isn't
-    # prefixed with a name
-    response = str_if_bytes(response)
-    response = "type:" + response
-    response = dict(kv.split(":") for kv in response.split())
-
-    # parse some expected int values from the string response
-    # note: this cmd isn't spec'd so these may not appear in all redis versions
-    int_fields = ("refcount", "serializedlength", "lru", "lru_seconds_idle")
-    for field in int_fields:
-        if field in response:
-            response[field] = int(response[field])
-
-    return response
-
-
-def parse_object(response, infotype):
-    """Parse the results of an OBJECT command"""
-    if infotype in ("idletime", "refcount"):
-        return int_or_none(response)
-    return response
-
-
-def parse_info(response):
-    """Parse the result of Redis's INFO command into a Python dict"""
-    info: Dict[str, Any] = {}
-    response = str_if_bytes(response)
-
-    def get_value(value):
-        if "," not in value or "=" not in value:
-            try:
-                if "." in value:
-                    return float(value)
-                else:
-                    return int(value)
-            except ValueError:
-                return value
-        else:
-            sub_dict = {}
-            for item in value.split(","):
-                k, v = item.rsplit("=", 1)
-                sub_dict[k] = get_value(v)
-            return sub_dict
-
-    for line in response.splitlines():
-        if line and not line.startswith("#"):
-            if line.find(":") != -1:
-                # Split, the info fields keys and values.
-                # Note that the value may contain ':'. but the 'host:'
-                # pseudo-command is the only case where the key contains ':'
-                key, value = line.split(":", 1)
-                if key == "cmdstat_host":
-                    key, value = line.rsplit(":", 1)
-
-                if key == "module":
-                    # Hardcode a list for key 'modules' since there could be
-                    # multiple lines that started with 'module'
-                    info.setdefault("modules", []).append(get_value(value))
-                else:
-                    info[key] = get_value(value)
-            else:
-                # if the line isn't splittable, append it to the "__raw__" key
-                info.setdefault("__raw__", []).append(line)
-
-    return info
-
-
-def parse_memory_stats(response, **kwargs):
-    """Parse the results of MEMORY STATS"""
-    stats = pairs_to_dict(response, decode_keys=True, decode_string_values=True)
-    for key, value in stats.items():
-        if key.startswith("db."):
-            stats[key] = pairs_to_dict(
-                value, decode_keys=True, decode_string_values=True
-            )
-    return stats
-
-
-SENTINEL_STATE_TYPES = {
-    "can-failover-its-master": int,
-    "config-epoch": int,
-    "down-after-milliseconds": int,
-    "failover-timeout": int,
-    "info-refresh": int,
-    "last-hello-message": int,
-    "last-ok-ping-reply": int,
-    "last-ping-reply": int,
-    "last-ping-sent": int,
-    "master-link-down-time": int,
-    "master-port": int,
-    "num-other-sentinels": int,
-    "num-slaves": int,
-    "o-down-time": int,
-    "pending-commands": int,
-    "parallel-syncs": int,
-    "port": int,
-    "quorum": int,
-    "role-reported-time": int,
-    "s-down-time": int,
-    "slave-priority": int,
-    "slave-repl-offset": int,
-    "voted-leader-epoch": int,
-}
-
-
-def parse_sentinel_state(item):
-    result = pairs_to_dict_typed(item, SENTINEL_STATE_TYPES)
-    flags = set(result["flags"].split(","))
-    for name, flag in (
-        ("is_master", "master"),
-        ("is_slave", "slave"),
-        ("is_sdown", "s_down"),
-        ("is_odown", "o_down"),
-        ("is_sentinel", "sentinel"),
-        ("is_disconnected", "disconnected"),
-        ("is_master_down", "master_down"),
-    ):
-        result[name] = flag in flags
-    return result
-
-
-def parse_sentinel_master(response):
-    return parse_sentinel_state(map(str_if_bytes, response))
-
-
-def parse_sentinel_masters(response):
-    result = {}
-    for item in response:
-        state = parse_sentinel_state(map(str_if_bytes, item))
-        result[state["name"]] = state
-    return result
-
-
-def parse_sentinel_slaves_and_sentinels(response):
-    return [parse_sentinel_state(map(str_if_bytes, item)) for item in response]
-
-
-def parse_sentinel_get_master(response):
-    return response and (response[0], int(response[1])) or None
-
-
-def pairs_to_dict(response, decode_keys=False, decode_string_values=False):
-    """Create a dict given a list of key/value pairs"""
-    if response is None:
-        return {}
-    if decode_keys or decode_string_values:
-        # the iter form is faster, but I don't know how to make that work
-        # with a str_if_bytes() map
-        keys = response[::2]
-        if decode_keys:
-            keys = map(str_if_bytes, keys)
-        values = response[1::2]
-        if decode_string_values:
-            values = map(str_if_bytes, values)
-        return dict(zip(keys, values))
-    else:
-        it = iter(response)
-        return dict(zip(it, it))
-
-
-def pairs_to_dict_typed(response, type_info):
-    it = iter(response)
-    result = {}
-    for key, value in zip(it, it):
-        if key in type_info:
-            try:
-                value = type_info[key](value)
-            except BaseException :
-                # if for some reason the value can't be coerced, just use
-                # the string value
-                pass
-        result[key] = value
-    return result
-
-
-def zset_score_pairs(response, **options):
-    """
-    If ``withscores`` is specified in the options, return the response as
-    a list of (value, score) pairs
-    """
-    if not response or not options.get("withscores"):
-        return response
-    score_cast_func = options.get("score_cast_func", float)
-    it = iter(response)
-    return list(zip(it, map(score_cast_func, it)))
-
-
-def sort_return_tuples(response, **options):
-    """
-    If ``groups`` is specified, return the response as a list of
-    n-element tuples with n being the value found in options['groups']
-    """
-    if not response or not options.get("groups"):
-        return response
-    n = options["groups"]
-    return list(zip(*(response[i::n] for i in range(n))))
-
-
-def int_or_none(response):
-    if response is None:
-        return None
-    return int(response)
-
-
-def parse_stream_list(response):
-    if response is None:
-        return None
-    data = []
-    for r in response:
-        if r is not None:
-            data.append((r[0], pairs_to_dict(r[1])))
-        else:
-            data.append((None, None))
-    return data
-
-
-def pairs_to_dict_with_str_keys(response):
-    return pairs_to_dict(response, decode_keys=True)
-
-
-def parse_list_of_dicts(response):
-    return list(map(pairs_to_dict_with_str_keys, response))
-
-
-def parse_xclaim(response, **options):
-    if options.get("parse_justid", False):
-        return response
-    return parse_stream_list(response)
-
-
-def parse_xinfo_stream(response):
-    data = pairs_to_dict(response, decode_keys=True)
-    first = data["first-entry"]
-    if first is not None:
-        data["first-entry"] = (first[0], pairs_to_dict(first[1]))
-    last = data["last-entry"]
-    if last is not None:
-        data["last-entry"] = (last[0], pairs_to_dict(last[1]))
-    return data
-
-
-def parse_xread(response):
-    if response is None:
-        return []
-    return [[r[0], parse_stream_list(r[1])] for r in response]
-
-
-def parse_xpending(response, **options):
-    if options.get("parse_detail", False):
-        return parse_xpending_range(response)
-    consumers = [{"name": n, "pending": int(p)} for n, p in response[3] or []]
-    return {
-        "pending": response[0],
-        "min": response[1],
-        "max": response[2],
-        "consumers": consumers,
-    }
-
-
-def parse_xpending_range(response):
-    k = ("message_id", "consumer", "time_since_delivered", "times_delivered")
-    return [dict(zip(k, r)) for r in response]
-
-
-def float_or_none(response):
-    if response is None:
-        return None
-    return float(response)
-
-
-def bool_ok(response):
-    return str_if_bytes(response) == "OK"
-
-
-def parse_zadd(response, **options):
-    if response is None:
-        return None
-    if options.get("as_score"):
-        return float(response)
-    return int(response)
-
-
-def parse_client_list(response, **options):
-    clients = []
-    for c in str_if_bytes(response).splitlines():
-        # Values might contain '='
-        clients.append(dict(pair.split("=", 1) for pair in c.split(" ")))
-    return clients
-
-
-def parse_config_get(response, **options):
-    response = [str_if_bytes(i) if i is not None else None for i in response]
-    return response and pairs_to_dict(response) or {}
-
-
-def parse_scan(response, **options):
-    cursor, r = response
-    return int(cursor), r
-
-
-def parse_hscan(response, **options):
-    cursor, r = response
-    return int(cursor), r and pairs_to_dict(r) or {}
-
-
-def parse_zscan(response, **options):
-    score_cast_func = options.get("score_cast_func", float)
-    cursor, r = response
-    it = iter(r)
-    return int(cursor), list(zip(it, map(score_cast_func, it)))
-
-
-def parse_slowlog_get(response, **options):
-    space: Union[str, bytes] = " " if options.get("decode_responses", False) else b" "
-    return [
-        {
-            "id": item[0],
-            "start_time": int(item[1]),
-            "duration": int(item[2]),
-            # Redis Enterprise injects another entry at index [3], which has
-            # the complexity info (i.e. the value N in case the command has
-            # an O(N) complexity) instead of the command.
-            "command": (
-                space.join(item[3])
-                if isinstance(item[3], list)
-                else space.join(item[4])
-            ),
-        }
-        for item in response
-    ]
-
-
-def parse_cluster_info(response, **options):
-    response = str_if_bytes(response)
-    return dict(line.split(":") for line in response.splitlines() if line)
-
-
-def _parse_node_line(line):
-    line_items = line.split(" ")
-    node_id, addr, flags, master_id, ping, pong, epoch, connected = line.split(" ")[:8]
-    slots = [sl.split("-") for sl in line_items[8:]]
-    node_dict = {
-        "node_id": node_id,
-        "flags": flags,
-        "master_id": master_id,
-        "last_ping_sent": ping,
-        "last_pong_rcvd": pong,
-        "epoch": epoch,
-        "slots": slots,
-        "connected": True if connected == "connected" else False,
-    }
-    return addr, node_dict
-
-
-def parse_cluster_nodes(response, **options):
-    raw_lines = str_if_bytes(response).splitlines()
-    return dict(_parse_node_line(line) for line in raw_lines)
-
-
-def parse_georadius_generic(response, **options):
-    if options["store"] or options["store_dist"]:
-        # `store` and `store_diff` cant be combined
-        # with other command arguments.
-        return response
-
-    if type(response) != list:
-        response_list = [response]
-    else:
-        response_list = response
-
-    if not options["withdist"] and not options["withcoord"] and not options["withhash"]:
-        # just a bunch of places
-        return response_list
-
-    cast: Dict[str, Callable] = {
-        "withdist": float,
-        "withcoord": lambda ll: (float(ll[0]), float(ll[1])),
-        "withhash": int,
-    }
-
-    # zip all output results with each casting functino to get
-    # the properly native Python value.
-    f = [lambda x: x]
-    f += [cast[o] for o in ["withdist", "withhash", "withcoord"] if options[o]]
-    return [list(map(lambda fv: fv[0](fv[1]), zip(f, r))) for r in response_list]
-
-
-def parse_pubsub_numsub(response, **options):
-    return list(zip(response[0::2], response[1::2]))
-
-
-def parse_client_kill(response, **options):
-    if isinstance(response, int):
-        return response
-    return str_if_bytes(response) == "OK"
-
-
-def parse_acl_getuser(response, **options):
-    if response is None:
-        return None
-    data = pairs_to_dict(response, decode_keys=True)
-
-    # convert everything but user-defined data in 'keys' to native strings
-    data["flags"] = list(map(str_if_bytes, data["flags"]))
-    data["passwords"] = list(map(str_if_bytes, data["passwords"]))
-    data["commands"] = str_if_bytes(data["commands"])
-
-    # split 'commands' into separate 'categories' and 'commands' lists
-    commands, categories = [], []
-    for command in data["commands"].split(" "):
-        if "@" in command:
-            categories.append(command)
-        else:
-            commands.append(command)
-
-    data["commands"] = commands
-    data["categories"] = categories
-    data["enabled"] = "on" in data["flags"]
-    return data
-
-
-def parse_acl_log(response, **options):
-    if response is None:
-        return None
-    if isinstance(response, list):
-        data = []
-        for log in response:
-            log_data = pairs_to_dict(log, True, True)
-            client_info = log_data.get("client-info", "")
-            log_data["client-info"] = parse_client_info(client_info)
-
-            # float() is lossy comparing to the "double" in C
-            log_data["age-seconds"] = float(log_data["age-seconds"])
-            data.append(log_data)
-    else:
-        data = bool_ok(response)
-    return data
-
-
-def parse_client_info(value):
-    """
-    Parsing client-info in ACL Log in following format.
-    "key1=value1 key2=value2 key3=value3"
-    """
-    client_info = {}
-    infos = value.split(" ")
-    for info in infos:
-        key, value = info.split("=")
-        client_info[key] = value
-
-    # Those fields are definded as int in networking.c
-    for int_key in {
-        "id",
-        "age",
-        "idle",
-        "db",
-        "sub",
-        "psub",
-        "multi",
-        "qbuf",
-        "qbuf-free",
-        "obl",
-        "oll",
-        "omem",
-    }:
-        client_info[int_key] = int(client_info[int_key])
-    return client_info
-
-
-def parse_module_result(response):
-    if isinstance(response, ModuleError):
-        raise response
-    return True
-
-
-class ResponseCallbackProtocol(Protocol):
-    def __call__(self, response: Any, **kwargs):
-        ...
-
-
-class AsyncResponseCallbackProtocol(Protocol):
-    async def __call__(self, response: Any, **kwargs):
-        ...
-
-
-ResponseCallbackT = Union[ResponseCallbackProtocol, AsyncResponseCallbackProtocol]
-
-
-_R = TypeVar("_R")
-
-
-class Redis:
-    """
-    Implementation of the Redis protocol.
-
-    This abstract class provides a Python interface to all Redis commands
-    and an implementation of the Redis protocol.
-
-    Connection and Pipeline derive from this, implementing how
-    the commands are sent and received to the Redis server
-    """
-
-    RESPONSE_CALLBACKS = {
-        **string_keys_to_dict(
-            "AUTH EXPIRE EXPIREAT HEXISTS HMSET MOVE MSETNX PERSIST "
-            "PSETEX RENAMENX SISMEMBER SMOVE SETEX SETNX",
-            bool,
-        ),
-        **string_keys_to_dict(
-            "BITCOUNT BITPOS DECRBY DEL EXISTS GEOADD GETBIT HDEL HLEN "
-            "HSTRLEN INCRBY LINSERT LLEN LPUSHX PFADD PFCOUNT RPUSHX SADD "
-            "SCARD SDIFFSTORE SETBIT SETRANGE SINTERSTORE SREM STRLEN "
-            "SUNIONSTORE UNLINK XACK XDEL XLEN XTRIM ZCARD ZLEXCOUNT ZREM "
-            "ZREMRANGEBYLEX ZREMRANGEBYRANK ZREMRANGEBYSCORE",
-            int,
-        ),
-        **string_keys_to_dict("INCRBYFLOAT HINCRBYFLOAT", float),
-        **string_keys_to_dict(
-            # these return OK, or int if redis-server is >=1.3.4
-            "LPUSH RPUSH",
-            lambda r: isinstance(r, int) and r or str_if_bytes(r) == "OK",
-        ),
-        **string_keys_to_dict("SORT", sort_return_tuples),
-        **string_keys_to_dict("ZSCORE ZINCRBY GEODIST", float_or_none),
-        **string_keys_to_dict(
-            "FLUSHALL FLUSHDB LSET LTRIM MSET PFMERGE READONLY READWRITE "
-            "RENAME SAVE SELECT SHUTDOWN SLAVEOF SWAPDB WATCH UNWATCH ",
-            bool_ok,
-        ),
-        **string_keys_to_dict("BLPOP BRPOP", lambda r: r and tuple(r) or None),
-        **string_keys_to_dict(
-            "SDIFF SINTER SMEMBERS SUNION", lambda r: r and set(r) or set()
-        ),
-        **string_keys_to_dict(
-            "ZPOPMAX ZPOPMIN ZRANGE ZRANGEBYSCORE ZREVRANGE ZREVRANGEBYSCORE",
-            zset_score_pairs,
-        ),
-        **string_keys_to_dict(
-            "BZPOPMIN BZPOPMAX", lambda r: r and (r[0], r[1], float(r[2])) or None
-        ),
-        **string_keys_to_dict("ZRANK ZREVRANK", int_or_none),
-        **string_keys_to_dict("XREVRANGE XRANGE", parse_stream_list),
-        **string_keys_to_dict("XREAD XREADGROUP", parse_xread),
-        **string_keys_to_dict("BGREWRITEAOF BGSAVE", lambda r: True),
-        "ACL CAT": lambda r: list(map(str_if_bytes, r)),
-        "ACL DELUSER": int,
-        "ACL GENPASS": str_if_bytes,
-        "ACL GETUSER": parse_acl_getuser,
-        "ACL LIST": lambda r: list(map(str_if_bytes, r)),
-        "ACL LOAD": bool_ok,
-        "ACL LOG": parse_acl_log,
-        "ACL SAVE": bool_ok,
-        "ACL SETUSER": bool_ok,
-        "ACL USERS": lambda r: list(map(str_if_bytes, r)),
-        "ACL WHOAMI": str_if_bytes,
-        "CLIENT GETNAME": str_if_bytes,
-        "CLIENT ID": int,
-        "CLIENT KILL": parse_client_kill,
-        "CLIENT LIST": parse_client_list,
-        "CLIENT SETNAME": bool_ok,
-        "CLIENT UNBLOCK": lambda r: r and int(r) == 1 or False,
-        "CLIENT PAUSE": bool_ok,
-        "CLUSTER ADDSLOTS": bool_ok,
-        "CLUSTER COUNT-FAILURE-REPORTS": lambda x: int(x),
-        "CLUSTER COUNTKEYSINSLOT": lambda x: int(x),
-        "CLUSTER DELSLOTS": bool_ok,
-        "CLUSTER FAILOVER": bool_ok,
-        "CLUSTER FORGET": bool_ok,
-        "CLUSTER INFO": parse_cluster_info,
-        "CLUSTER KEYSLOT": lambda x: int(x),
-        "CLUSTER MEET": bool_ok,
-        "CLUSTER NODES": parse_cluster_nodes,
-        "CLUSTER REPLICATE": bool_ok,
-        "CLUSTER RESET": bool_ok,
-        "CLUSTER SAVECONFIG": bool_ok,
-        "CLUSTER SET-CONFIG-EPOCH": bool_ok,
-        "CLUSTER SETSLOT": bool_ok,
-        "CLUSTER SLAVES": parse_cluster_nodes,
-        "CONFIG GET": parse_config_get,
-        "CONFIG RESETSTAT": bool_ok,
-        "CONFIG SET": bool_ok,
-        "DEBUG OBJECT": parse_debug_object,
-        "GEOHASH": lambda r: list(map(str_if_bytes, r)),
-        "GEOPOS": lambda r: list(
-            map(lambda ll: (float(ll[0]), float(ll[1])) if ll is not None else None, r)
-        ),
-        "GEORADIUS": parse_georadius_generic,
-        "GEORADIUSBYMEMBER": parse_georadius_generic,
-        "HGETALL": lambda r: r and pairs_to_dict(r) or {},
-        "HSCAN": parse_hscan,
-        "INFO": parse_info,
-        "LASTSAVE": timestamp_to_datetime,
-        "MEMORY PURGE": bool_ok,
-        "MEMORY STATS": parse_memory_stats,
-        "MEMORY USAGE": int_or_none,
-        "MODULE LOAD": parse_module_result,
-        "MODULE UNLOAD": parse_module_result,
-        "MODULE LIST": lambda r: [pairs_to_dict(m) for m in r],
-        "OBJECT": parse_object,
-        "PING": lambda r: str_if_bytes(r) == "PONG",
-        "PUBSUB NUMSUB": parse_pubsub_numsub,
-        "RANDOMKEY": lambda r: r and r or None,
-        "SCAN": parse_scan,
-        "SCRIPT EXISTS": lambda r: list(map(bool, r)),
-        "SCRIPT FLUSH": bool_ok,
-        "SCRIPT KILL": bool_ok,
-        "SCRIPT LOAD": str_if_bytes,
-        "SENTINEL GET-MASTER-ADDR-BY-NAME": parse_sentinel_get_master,
-        "SENTINEL MASTER": parse_sentinel_master,
-        "SENTINEL MASTERS": parse_sentinel_masters,
-        "SENTINEL MONITOR": bool_ok,
-        "SENTINEL REMOVE": bool_ok,
-        "SENTINEL SENTINELS": parse_sentinel_slaves_and_sentinels,
-        "SENTINEL SET": bool_ok,
-        "SENTINEL SLAVES": parse_sentinel_slaves_and_sentinels,
-        "SET": lambda r: r and str_if_bytes(r) == "OK",
-        "SLOWLOG GET": parse_slowlog_get,
-        "SLOWLOG LEN": int,
-        "SLOWLOG RESET": bool_ok,
-        "SSCAN": parse_scan,
-        "TIME": lambda x: (int(x[0]), int(x[1])),
-        "XCLAIM": parse_xclaim,
-        "XGROUP CREATE": bool_ok,
-        "XGROUP DELCONSUMER": int,
-        "XGROUP DESTROY": bool,
-        "XGROUP SETID": bool_ok,
-        "XINFO CONSUMERS": parse_list_of_dicts,
-        "XINFO GROUPS": parse_list_of_dicts,
-        "XINFO STREAM": parse_xinfo_stream,
-        "XPENDING": parse_xpending,
-        "ZADD": parse_zadd,
-        "ZSCAN": parse_zscan,
-    }
-
-    response_callbacks: MutableMapping[Union[str, bytes], ResponseCallbackT]
-
-    @classmethod
-    def from_url(cls, url: str, **kwargs):
-        """
-        Return a Redis client object configured from the given URL
-
-        For example::
-
-            redis://[[username]:[password]]@localhost:6379/0
-            rediss://[[username]:[password]]@localhost:6379/0
-            unix://[[username]:[password]]@/path/to/socket.sock?db=0
-
-        Three URL schemes are supported:
-
-        - `redis://` creates a TCP socket connection. See more at:
-          <https://www.iana.org/assignments/uri-schemes/prov/redis>
-        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
-          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
-        - ``unix://``: creates a Unix Domain Socket connection.
-
-        The username, password, hostname, path and all querystring values
-        are passed through urllib.parse.unquote in order to replace any
-        percent-encoded values with their corresponding characters.
-
-        There are several ways to specify a database number. The first value
-        found will be used:
-            1. A ``db`` querystring option, e.g. redis://localhost?db=0
-            2. If using the redis:// or rediss:// schemes, the path argument
-               of the url, e.g. redis://localhost/0
-            3. A ``db`` keyword argument to this function.
-
-        If none of these options are specified, the default db=0 is used.
-
-        All querystring options are cast to their appropriate Python types.
-        Boolean arguments can be specified with string values "True"/"False"
-        or "Yes"/"No". Values that cannot be properly cast cause a
-        ``ValueError`` to be raised. Once parsed, the querystring arguments
-        and keyword arguments are passed to the ``ConnectionPool``'s
-        class initializer. In the case of conflicting arguments, querystring
-        arguments always win.
-
-        """
-        connection_pool = ConnectionPool.from_url(url, **kwargs)
-        return cls(connection_pool=connection_pool)
-
-    def __init__(
-        self,
-        *,
-        host: str = "localhost",
-        port: int = 6379,
-        db: Union[str, int] = 0,
-        password: Optional[str] = None,
-        socket_timeout: Optional[float] = None,
-        socket_connect_timeout: Optional[float] = None,
-        socket_keepalive: Optional[bool] = None,
-        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
-        connection_pool: Optional[ConnectionPool] = None,
-        unix_socket_path: Optional[str] = None,
-        encoding: str = "utf-8",
-        encoding_errors: str = "strict",
-        decode_responses: bool = False,
-        retry_on_timeout: bool = False,
-        ssl: bool = False,
-        ssl_keyfile: Optional[str] = None,
-        ssl_certfile: Optional[str] = None,
-        ssl_cert_reqs: str = "required",
-        ssl_ca_certs: Optional[str] = None,
-        ssl_check_hostname: bool = False,
-        max_connections: Optional[int] = None,
-        single_connection_client: bool = False,
-        health_check_interval: int = 0,
-        client_name: Optional[str] = None,
-        username: Optional[str] = None,
-    ):
-        kwargs: Dict[str, Any]
-        if not connection_pool:
-            kwargs = {
-                "db": db,
-                "username": username,
-                "password": password,
-                "socket_timeout": socket_timeout,
-                "encoding": encoding,
-                "encoding_errors": encoding_errors,
-                "decode_responses": decode_responses,
-                "retry_on_timeout": retry_on_timeout,
-                "max_connections": max_connections,
-                "health_check_interval": health_check_interval,
-                "client_name": client_name,
-            }
-            # based on input, setup appropriate connection args
-            if unix_socket_path is not None:
-                kwargs.update(
-                    {
-                        "path": unix_socket_path,
-                        "connection_class": UnixDomainSocketConnection,
-                    }
-                )
-            else:
-                # TCP specific options
-                kwargs.update(
-                    {
-                        "host": host,
-                        "port": port,
-                        "socket_connect_timeout": socket_connect_timeout,
-                        "socket_keepalive": socket_keepalive,
-                        "socket_keepalive_options": socket_keepalive_options,
-                    }
-                )
-
-                if ssl:
-                    kwargs.update(
-                        {
-                            "connection_class": SSLConnection,
-                            "ssl_keyfile": ssl_keyfile,
-                            "ssl_certfile": ssl_certfile,
-                            "ssl_cert_reqs": ssl_cert_reqs,
-                            "ssl_ca_certs": ssl_ca_certs,
-                            "ssl_check_hostname": ssl_check_hostname,
-                        }
-                    )
-            connection_pool = ConnectionPool(**kwargs)
-        self.connection_pool = connection_pool
-        self.single_connection_client = single_connection_client
-        self.connection: Optional[Connection] = None
-
-        self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}<{self.connection_pool!r}>"
-
-    def __await__(self):
-        return self.initialize().__await__()
-
-    async def initialize(self: _RedisT) -> _RedisT:
-        if self.single_connection_client and self.connection is None:
-            self.connection = await self.connection_pool.get_connection("_")
-        return self
-
-    def set_response_callback(self, command: str, callback: ResponseCallbackT):
-        """Set a custom Response Callback"""
-        self.response_callbacks[command] = callback
-
-    def pipeline(
-        self, transaction: bool = True, shard_hint: Optional[str] = None
-    ) -> "Pipeline":
-        """
-        Return a new pipeline object that can queue multiple commands for
-        later execution. ``transaction`` indicates whether all commands
-        should be executed atomically. Apart from making a group of operations
-        atomic, pipelines are useful for reducing the back-and-forth overhead
-        between the client and server.
-        """
-        return Pipeline(
-            self.connection_pool, self.response_callbacks, transaction, shard_hint
-        )
-
-    async def transaction(
-        self,
-        func: Callable[["Pipeline"], Union[Any, Awaitable[Any]]],
-        *watches: KeyT,
-        shard_hint: Optional[str] = None,
-        value_from_callable: bool = False,
-        watch_delay: Optional[float] = None,
-    ):
-        """
-        Convenience method for executing the callable `func` as a transaction
-        while watching all keys specified in `watches`. The 'func' callable
-        should expect a single argument which is a Pipeline object.
-        """
-        pipe: Pipeline
-        async with self.pipeline(True, shard_hint) as pipe:
-            while True:
-                try:
-                    if watches:
-                        await pipe.watch(*watches)
-                    func_value = func(pipe)
-                    if inspect.isawaitable(func_value):
-                        func_value = await func_value
-                    exec_value = await pipe.execute()
-                    return func_value if value_from_callable else exec_value
-                except WatchError:
-                    if watch_delay is not None and watch_delay > 0:
-                        await asyncio.sleep(watch_delay)
-                    continue
-
-    def lock(
-        self,
-        name: KeyT,
-        timeout: Optional[float] = None,
-        sleep: float = 0.1,
-        blocking_timeout: Optional[float] = None,
-        lock_class: Optional[Type[Lock]] = None,
-        thread_local=True,
-    ) -> Lock:
-        """
-        Return a new Lock object using key ``name`` that mimics
-        the behavior of threading.Lock.
-
-        If specified, ``timeout`` indicates a maximum life for the lock.
-        By default, it will remain locked until release() is called.
-
-        ``sleep`` indicates the amount of time to sleep per loop iteration
-        when the lock is in blocking mode and another client is currently
-        holding the lock.
-
-        ``blocking_timeout`` indicates the maximum amount of time in seconds to
-        spend trying to acquire the lock. A value of ``None`` indicates
-        continue trying forever. ``blocking_timeout`` can be specified as a
-        float or integer, both representing the number of seconds to wait.
-
-        ``lock_class`` forces the specified lock implementation.
-
-        ``thread_local`` indicates whether the lock token is placed in
-        thread-local storage. By default, the token is placed in thread local
-        storage so that a thread only sees its token, not a token set by
-        another thread. Consider the following timeline:
-
-            time: 0, thread-1 acquires `my-lock`, with a timeout of 5 seconds.
-                     thread-1 sets the token to "abc"
-            time: 1, thread-2 blocks trying to acquire `my-lock` using the
-                     Lock instance.
-            time: 5, thread-1 has not yet completed. redis expires the lock
-                     key.
-            time: 5, thread-2 acquired `my-lock` now that it's available.
-                     thread-2 sets the token to "xyz"
-            time: 6, thread-1 finishes its work and calls release(). if the
-                     token is *not* stored in thread local storage, then
-                     thread-1 would see the token value as "xyz" and would be
-                     able to successfully release the thread-2's lock.
-
-        In some use cases it's necessary to disable thread local storage. For
-        example, if you have code where one thread acquires a lock and passes
-        that lock instance to a worker thread to release later. If thread
-        local storage isn't disabled in this case, the worker thread won't see
-        the token set by the thread that acquired the lock. Our assumption
-        is that these cases aren't common and as such default to using
-        thread local storage."""
-        if lock_class is None:
-            lock_class = Lock
-        return lock_class(
-            self,
-            name,
-            timeout=timeout,
-            sleep=sleep,
-            blocking_timeout=blocking_timeout,
-            thread_local=thread_local,
-        )
-
-    def pubsub(self, **kwargs) -> "PubSub":
-        """
-        Return a Publish/Subscribe object. With this object, you can
-        subscribe to channels and listen for messages that get published to
-        them.
-        """
-        return PubSub(self.connection_pool, **kwargs)
-
-    def monitor(self) -> "Monitor":
-        return Monitor(self.connection_pool)
-
-    def client(self) -> "Redis":
-        return self.__class__(
-            connection_pool=self.connection_pool, single_connection_client=True
-        )
-
-    async def __aenter__(self: _RedisT) -> _RedisT:
-        return await self.initialize()
-
-    async def __aexit__(self, exc_type, exc_value, traceback):
-        await self.close()
-
-    _DEL_MESSAGE = "Unclosed Redis client"
-
-    def __del__(self, _warnings: Any = warnings) -> None:
-        if self.connection is not None:
-            _warnings.warn(
-                f"Unclosed client session {self!r}",
-                ResourceWarning,
-                source=self,
-            )
-            context = {"client": self, "message": self._DEL_MESSAGE}
-            asyncio.get_event_loop().call_exception_handler(context)
-
-    async def close(self):
-        conn = self.connection
-        if conn:
-            self.connection = None
-            await self.connection_pool.release(conn)
-
-    # COMMAND EXECUTION AND PROTOCOL PARSING
-    async def execute_command(self, *args, **options):
-        """Execute a command and return a parsed response"""
-        await self.initialize()
-        pool = self.connection_pool
-        command_name = args[0]
-        conn = self.connection or await pool.get_connection(command_name, **options)
-        try:
-            await conn.send_command(*args)
-            return await self.parse_response(conn, command_name, **options)
-        except (ConnectionError, TimeoutError) as e:
-            await conn.disconnect()
-            if not (conn.retry_on_timeout and isinstance(e, TimeoutError)):
-                raise
-            await conn.send_command(*args)
-            return await self.parse_response(conn, command_name, **options)
-        finally:
-            if not self.connection:
-                await pool.release(conn)
-
-    async def parse_response(
-        self, connection: Connection, command_name: Union[str, bytes], **options
-    ):
-        """Parses a response from the Redis server"""
-        try:
-            response = await connection.read_response()
-        except ResponseError:
-            if EMPTY_RESPONSE in options:
-                return options[EMPTY_RESPONSE]
-            raise
-        if command_name in self.response_callbacks:
-            # Mypy bug: https://github.com/python/mypy/issues/10977
-            command_name = cast(str, command_name)
-            retval = self.response_callbacks[command_name](response, **options)
-            return await retval if inspect.isawaitable(retval) else retval
-        return response
-
-    # SERVER INFORMATION
-
-    # ACL methods
-    def acl_cat(self, category: Optional[str] = None) -> Awaitable:
-        """
-        Returns a list of categories or commands within a category.
-
-        If ``category`` is not supplied, returns a list of all categories.
-        If ``category`` is supplied, returns a list of all commands within
-        that category.
-        """
-        pieces: List[EncodableT] = [category] if category else []
-        return self.execute_command("ACL CAT", *pieces)
-
-    def acl_deluser(self, username: str) -> Awaitable:
-        """Delete the ACL for the specified ``username``"""
-        return self.execute_command("ACL DELUSER", username)
-
-    def acl_genpass(self) -> Awaitable:
-        """Generate a random password value"""
-        return self.execute_command("ACL GENPASS")
-
-    def acl_getuser(self, username: str) -> Awaitable:
-        """
-        Get the ACL details for the specified ``username``.
-
-        If ``username`` does not exist, return None
-        """
-        return self.execute_command("ACL GETUSER", username)
-
-    def acl_list(self) -> Awaitable:
-        """Return a list of all ACLs on the server"""
-        return self.execute_command("ACL LIST")
-
-    def acl_log(self, count: Optional[int] = None) -> Awaitable:
-        """
-        Get ACL logs as a list.
-        :param int count: Get logs[0:count].
-        :rtype: List.
-        """
-        args = []
-        if count is not None:
-            if not isinstance(count, int):
-                raise DataError("ACL LOG count must be an integer")
-            args.append(count)
-
-        return self.execute_command("ACL LOG", *args)
-
-    def acl_log_reset(self) -> Awaitable:
-        """
-        Reset ACL logs.
-        :rtype: Boolean.
-        """
-        args = [b"RESET"]
-        return self.execute_command("ACL LOG", *args)
-
-    def acl_load(self) -> Awaitable:
-        """
-        Load ACL rules from the configured ``aclfile``.
-
-        Note that the server must be configured with the ``aclfile``
-        directive to be able to load ACL rules from an aclfile.
-        """
-        return self.execute_command("ACL LOAD")
-
-    def acl_save(self) -> Awaitable:
-        """
-        Save ACL rules to the configured ``aclfile``.
-
-        Note that the server must be configured with the ``aclfile``
-        directive to be able to save ACL rules to an aclfile.
-        """
-        return self.execute_command("ACL SAVE")
-
-    def acl_setuser(  # noqa: C901
-        self,
-        username: str,
-        enabled: bool = False,
-        nopass: bool = False,
-        passwords: Optional[Union[str, Iterable[str]]] = None,
-        hashed_passwords: Optional[Union[str, Iterable[str]]] = None,
-        categories: Optional[Iterable[str]] = None,
-        commands: Optional[Iterable[str]] = None,
-        keys: Optional[Iterable[KeyT]] = None,
-        reset: bool = False,
-        reset_keys: bool = False,
-        reset_passwords: bool = False,
-    ) -> Awaitable:
-        """
-        Create or update an ACL user.
-
-        Create or update the ACL for ``username``. If the user already exists,
-        the existing ACL is completely overwritten and replaced with the
-        specified values.
-
-        ``enabled`` is a boolean indicating whether the user should be allowed
-        to authenticate or not. Defaults to ``False``.
-
-        ``nopass`` is a boolean indicating whether the can authenticate without
-        a password. This cannot be True if ``passwords`` are also specified.
-
-        ``passwords`` if specified is a list of plain text passwords
-        to add to or remove from the user. Each password must be prefixed with
-        a '+' to add or a '-' to remove. For convenience, the value of
-        ``passwords`` can be a simple prefixed string when adding or
-        removing a single password.
-
-        ``hashed_passwords`` if specified is a list of SHA-256 hashed passwords
-        to add to or remove from the user. Each hashed password must be
-        prefixed with a '+' to add or a '-' to remove. For convenience,
-        the value of ``hashed_passwords`` can be a simple prefixed string when
-        adding or removing a single password.
-
-        ``categories`` if specified is a list of strings representing category
-        permissions. Each string must be prefixed with either a '+' to add the
-        category permission or a '-' to remove the category permission.
-
-        ``commands`` if specified is a list of strings representing command
-        permissions. Each string must be prefixed with either a '+' to add the
-        command permission or a '-' to remove the command permission.
-
-        ``keys`` if specified is a list of key patterns to grant the user
-        access to. Keys patterns allow '*' to support wildcard matching. For
-        example, '*' grants access to all keys while 'cache:*' grants access
-        to all keys that are prefixed with 'cache:'. ``keys`` should not be
-        prefixed with a '~'.
-
-        ``reset`` is a boolean indicating whether the user should be fully
-        reset prior to applying the new ACL. Setting this to True will
-        remove all existing passwords, flags and privileges from the user and
-        then apply the specified rules. If this is False, the user's existing
-        passwords, flags and privileges will be kept and any new specified
-        rules will be applied on top.
-
-        ``reset_keys`` is a boolean indicating whether the user's key
-        permissions should be reset prior to applying any new key permissions
-        specified in ``keys``. If this is False, the user's existing
-        key permissions will be kept and any new specified key permissions
-        will be applied on top.
-
-        ``reset_passwords`` is a boolean indicating whether to remove all
-        existing passwords and the 'nopass' flag from the user prior to
-        applying any new passwords specified in 'passwords' or
-        'hashed_passwords'. If this is False, the user's existing passwords
-        and 'nopass' status will be kept and any new specified passwords
-        or hashed_passwords will be applied on top.
-        """
-        encoder = self.connection_pool.get_encoder()
-        pieces: List[Union[str, bytes]] = [username]
-
-        if reset:
-            pieces.append(b"reset")
-
-        if reset_keys:
-            pieces.append(b"resetkeys")
-
-        if reset_passwords:
-            pieces.append(b"resetpass")
-
-        if enabled:
-            pieces.append(b"on")
-        else:
-            pieces.append(b"off")
-
-        if (passwords or hashed_passwords) and nopass:
-            raise DataError(
-                "Cannot set 'nopass' and supply " "'passwords' or 'hashed_passwords'"
-            )
-
-        if passwords:
-            # as most users will have only one password, allow remove_passwords
-            # to be specified as a simple string or a list
-            converted_passwords = list_or_args(passwords, [])
-            for i, raw_password in enumerate(converted_passwords):
-                password = encoder.encode(raw_password)
-                if password.startswith(b"+"):
-                    pieces.append(b">%s" % password[1:])
-                elif password.startswith(b"-"):
-                    pieces.append(b"<%s" % password[1:])
-                else:
-                    raise DataError(
-                        "Password %d must be prefixeed with a "
-                        '"+" to add or a "-" to remove' % i
-                    )
-
-        if hashed_passwords:
-            # as most users will have only one password, allow remove_passwords
-            # to be specified as a simple string or a list
-            parsed_hashed_passwords = list_or_args(hashed_passwords, [])
-            for i, raw_hashed_password in enumerate(parsed_hashed_passwords):
-                hashed_password = encoder.encode(raw_hashed_password)
-                if hashed_password.startswith(b"+"):
-                    pieces.append(b"#%s" % hashed_password[1:])
-                elif hashed_password.startswith(b"-"):
-                    pieces.append(b"!%s" % hashed_password[1:])
-                else:
-                    raise DataError(
-                        "Hashed %d password must be prefixeed "
-                        'with a "+" to add or a "-" to remove' % i
-                    )
-
-        if nopass:
-            pieces.append(b"nopass")
-
-        if categories:
-            for raw_category in categories:
-                category = encoder.encode(raw_category)
-                # categories can be prefixed with one of (+@, +, -@, -)
-                if category.startswith(b"+@"):
-                    pieces.append(category)
-                elif category.startswith(b"+"):
-                    pieces.append(b"+@%s" % category[1:])
-                elif category.startswith(b"-@"):
-                    pieces.append(category)
-                elif category.startswith(b"-"):
-                    pieces.append(b"-@%s" % category[1:])
-                else:
-                    raise DataError(
-                        f'Category "{encoder.decode(category, force=True)}" must be '
-                        'prefixed with "+" or "-"'
-                    )
-        if commands:
-            for raw_cmd in commands:
-                cmd = encoder.encode(raw_cmd)
-                if not cmd.startswith(b"+") and not cmd.startswith(b"-"):
-                    raise DataError(
-                        f'Command "{encoder.decode(cmd, force=True)}" must be '
-                        'prefixed with "+" or "-"'
-                    )
-                pieces.append(cmd)
-
-        if keys:
-            for raw_key in keys:
-                key = encoder.encode(raw_key)
-                pieces.append(b"~%s" % key)
-
-        return self.execute_command("ACL SETUSER", *pieces)
-
-    def acl_users(self) -> Awaitable:
-        """Returns a list of all registered users on the server."""
-        return self.execute_command("ACL USERS")
-
-    def acl_whoami(self) -> Awaitable:
-        """Get the username for the current connection"""
-        return self.execute_command("ACL WHOAMI")
-
-    def bgrewriteaof(self) -> Awaitable:
-        """Tell the Redis server to rewrite the AOF file from data in memory."""
-        return self.execute_command("BGREWRITEAOF")
-
-    def bgsave(self) -> Awaitable:
-        """
-        Tell the Redis server to save its data to disk.  Unlike save(),
-        this method is asynchronous and returns immediately.
-        """
-        return self.execute_command("BGSAVE")
-
-    def client_kill(self, address: str) -> Awaitable:
-        """Disconnects the client at ``address`` (ip:port)"""
-        return self.execute_command("CLIENT KILL", address)
-
-    def client_kill_filter(
-        self,
-        _id: Optional[str] = None,
-        _type: Optional[str] = None,
-        addr: Optional[str] = None,
-        skipme: Optional[bool] = None,
-    ) -> Awaitable:
-        """
-        Disconnects client(s) using a variety of filter options
-        :param _id: Kills a client by its unique ID field
-        :param _type: Kills a client by type where type is one of 'normal',
-        'master', 'slave' or 'pubsub'
-        :param addr: Kills a client by its 'address:port'
-        :param skipme: If True, then the client calling the command
-        will not get killed even if it is identified by one of the filter
-        options. If skipme is not provided, the server defaults to skipme=True
-        """
-        args: List[Union[bytes, str]] = []
-        if _type is not None:
-            client_types = ("normal", "master", "slave", "pubsub")
-            if str(_type).lower() not in client_types:
-                raise DataError(f"CLIENT KILL type must be one of {client_types!r}")
-            args.extend((b"TYPE", _type))
-        if skipme is not None:
-            if not isinstance(skipme, bool):
-                raise DataError("CLIENT KILL skipme must be a bool")
-            if skipme:
-                args.extend((b"SKIPME", b"YES"))
-            else:
-                args.extend((b"SKIPME", b"NO"))
-        if _id is not None:
-            args.extend((b"ID", _id))
-        if addr is not None:
-            args.extend((b"ADDR", addr))
-        if not args:
-            raise DataError(
-                "CLIENT KILL <filter> <value> ... ... <filter> "
-                "<value> must specify at least one filter"
-            )
-        return self.execute_command("CLIENT KILL", *args)
-
-    def client_list(self, _type: Optional[str] = None) -> Awaitable:
-        """
-        Returns a list of currently connected clients.
-        If type of client specified, only that type will be returned.
-        :param _type: optional. one of the client types (normal, master,
-         replica, pubsub)
-        """
-        "Returns a list of currently connected clients"
-        if _type is not None:
-            client_types = ("normal", "master", "replica", "pubsub")
-            if str(_type).lower() not in client_types:
-                raise DataError(f"CLIENT LIST _type must be one of {client_types!r}")
-            return self.execute_command("CLIENT LIST", b"TYPE", _type)
-        return self.execute_command("CLIENT LIST")
-
-    def client_getname(self) -> Awaitable:
-        """Returns the current connection name"""
-        return self.execute_command("CLIENT GETNAME")
-
-    def client_id(self) -> Awaitable:
-        """Returns the current connection id"""
-        return self.execute_command("CLIENT ID")
-
-    def client_setname(self, name: str) -> Awaitable:
-        """Sets the current connection name"""
-        return self.execute_command("CLIENT SETNAME", name)
-
-    def client_unblock(self, client_id: int, error: bool = False) -> Awaitable:
-        """
-        Unblocks a connection by its client id.
-        If ``error`` is True, unblocks the client with a special error message.
-        If ``error`` is False (default), the client is unblocked using the
-        regular timeout mechanism.
-        """
-        args = ["CLIENT UNBLOCK", int(client_id)]
-        if error:
-            args.append(b"ERROR")
-        return self.execute_command(*args)
-
-    def client_pause(self, timeout: int) -> Awaitable:
-        """
-        Suspend all the Redis clients for the specified amount of time
-        :param timeout: milliseconds to pause clients
-        """
-        if not isinstance(timeout, int):
-            raise DataError("CLIENT PAUSE timeout must be an integer")
-        return self.execute_command("CLIENT PAUSE", str(timeout))
-
-    def readwrite(self) -> Awaitable:
-        """Disables read queries for a connection to a Redis Cluster slave node"""
-        return self.execute_command("READWRITE")
-
-    def readonly(self) -> Awaitable:
-        """Enables read queries for a connection to a Redis Cluster replica node"""
-        return self.execute_command("READONLY")
-
-    def config_get(self, pattern: str = "*") -> Awaitable:
-        """Return a dictionary of configuration based on the ``pattern``"""
-        return self.execute_command("CONFIG GET", pattern)
-
-    def config_set(self, name: str, value: EncodableT) -> Awaitable:
-        """Set config item ``name`` with ``value``"""
-        return self.execute_command("CONFIG SET", name, value)
-
-    def config_resetstat(self) -> Awaitable:
-        """Reset runtime statistics"""
-        return self.execute_command("CONFIG RESETSTAT")
-
-    def config_rewrite(self) -> Awaitable:
-        """Rewrite config file with the minimal change to reflect running config"""
-        return self.execute_command("CONFIG REWRITE")
-
-    def dbsize(self) -> Awaitable:
-        """Returns the number of keys in the current database"""
-        return self.execute_command("DBSIZE")
-
-    def debug_object(self, key: KeyT) -> Awaitable:
-        """Returns version specific meta information about a given key"""
-        return self.execute_command("DEBUG OBJECT", key)
-
-    def echo(self, value: EncodableT) -> Awaitable:
-        """Echo the string back from the server"""
-        return self.execute_command("ECHO", value)
-
-    def flushall(self, asynchronous: bool = False) -> Awaitable:
-        """
-        Delete all keys in all databases on the current host.
-
-        ``asynchronous`` indicates whether the operation is
-        executed asynchronously by the server.
-        """
-        args = []
-        if asynchronous:
-            args.append(b"ASYNC")
-        return self.execute_command("FLUSHALL", *args)
-
-    def flushdb(self, asynchronous: bool = False) -> Awaitable:
-        """
-        Delete all keys in the current database.
-
-        ``asynchronous`` indicates whether the operation is
-        executed asynchronously by the server.
-        """
-        args = []
-        if asynchronous:
-            args.append(b"ASYNC")
-        return self.execute_command("FLUSHDB", *args)
-
-    def swapdb(self, first: int, second: int) -> Awaitable:
-        """Swap two databases"""
-        return self.execute_command("SWAPDB", first, second)
-
-    def info(self, section: Optional[str] = None) -> Awaitable:
-        """
-        Returns a dictionary containing information about the Redis server
-
-        The ``section`` option can be used to select a specific section
-        of information
-
-        The section option is not supported by older versions of Redis Server,
-        and will generate ResponseError
-        """
-        if section is None:
-            return self.execute_command("INFO")
-        else:
-            return self.execute_command("INFO", section)
-
-    def lastsave(self) -> Awaitable:
-        """
-        Return a Python datetime object representing the last time the
-        Redis database was saved to disk
-        """
-        return self.execute_command("LASTSAVE")
-
-    def migrate(
-        self,
-        host: str,
-        port: int,
-        keys: KeysT,
-        destination_db: int,
-        timeout: int,
-        copy: bool = False,
-        replace: bool = False,
-        auth: Optional[str] = None,
-    ) -> Awaitable:
-        """
-        Migrate 1 or more keys from the current Redis server to a different
-        server specified by the ``host``, ``port`` and ``destination_db``.
-
-        The ``timeout``, specified in milliseconds, indicates the maximum
-        time the connection between the two servers can be idle before the
-        command is interrupted.
-
-        If ``copy`` is True, the specified ``keys`` are NOT deleted from
-        the source server.
-
-        If ``replace`` is True, this operation will overwrite the keys
-        on the destination server if they exist.
-
-        If ``auth`` is specified, authenticate to the destination server with
-        the password provided.
-        """
-        keys = list_or_args(keys, [])
-        if not keys:
-            raise DataError("MIGRATE requires at least one key")
-        pieces: List[EncodableT] = []
-        if copy:
-            pieces.append(b"COPY")
-        if replace:
-            pieces.append(b"REPLACE")
-        if auth:
-            pieces.append(b"AUTH")
-            pieces.append(auth)
-        pieces.append(b"KEYS")
-        pieces.extend(keys)
-        return self.execute_command(
-            "MIGRATE", host, port, "", destination_db, timeout, *pieces
-        )
-
-    def object(self, infotype: str, key: KeyT) -> Awaitable:
-        """Return the encoding, idletime, or refcount about the key"""
-        return self.execute_command("OBJECT", infotype, key, infotype=infotype)
-
-    def memory_stats(self) -> Awaitable:
-        """Return a dictionary of memory stats"""
-        return self.execute_command("MEMORY STATS")
-
-    def memory_usage(self, key: KeyT, samples: Optional[int] = None) -> Awaitable:
-        """
-        Return the total memory usage for key, its value and associated
-        administrative overheads.
-
-        For nested data structures, ``samples`` is the number of elements to
-        sample. If left unspecified, the server's default is 5. Use 0 to sample
-        all elements.
-        """
-        args = []
-        if isinstance(samples, int):
-            args.extend([b"SAMPLES", samples])
-        return self.execute_command("MEMORY USAGE", key, *args)
-
-    def memory_purge(self) -> Awaitable:
-        """Attempts to purge dirty pages for reclamation by allocator"""
-        return self.execute_command("MEMORY PURGE")
-
-    def ping(self) -> Awaitable:
-        """Ping the Redis server"""
-        return self.execute_command("PING")
-
-    def save(self) -> Awaitable:
-        """
-        Tell the Redis server to save its data to disk,
-        blocking until the save is complete
-        """
-        return self.execute_command("SAVE")
-
-    def sentinel_get_master_addr_by_name(self, service_name: str) -> Awaitable:
-        """Returns a (host, port) pair for the given ``service_name``"""
-        return self.execute_command("SENTINEL GET-MASTER-ADDR-BY-NAME", service_name)
-
-    def sentinel_master(self, service_name: str) -> Awaitable:
-        """Returns a dictionary containing the specified masters state."""
-        return self.execute_command("SENTINEL MASTER", service_name)
-
-    def sentinel_masters(self) -> Awaitable:
-        """Returns a list of dictionaries containing each master's state."""
-        return self.execute_command("SENTINEL MASTERS")
-
-    def sentinel_monitor(self, name: str, ip: str, port: int, quorum: int) -> Awaitable:
-        """Add a new master to Sentinel to be monitored"""
-        return self.execute_command("SENTINEL MONITOR", name, ip, port, quorum)
-
-    def sentinel_remove(self, name: str) -> Awaitable:
-        """Remove a master from Sentinel's monitoring"""
-        return self.execute_command("SENTINEL REMOVE", name)
-
-    def sentinel_sentinels(self, service_name: str) -> Awaitable:
-        """Returns a list of sentinels for ``service_name``"""
-        return self.execute_command("SENTINEL SENTINELS", service_name)
-
-    def sentinel_set(self, name: str, option: str, value: EncodableT) -> Awaitable:
-        """Set Sentinel monitoring parameters for a given master"""
-        return self.execute_command("SENTINEL SET", name, option, value)
-
-    def sentinel_slaves(self, service_name: str) -> Awaitable:
-        """Returns a list of slaves for ``service_name``"""
-        return self.execute_command("SENTINEL SLAVES", service_name)
-
-    def shutdown(self, save: bool = False, nosave: bool = False) -> None:
-        """Shutdown the Redis server.  If Redis has persistence configured,
-        data will be flushed before shutdown.  If the "save" option is set,
-        a data flush will be attempted even if there is no persistence
-        configured.  If the "nosave" option is set, no data flush will be
-        attempted.  The "save" and "nosave" options cannot both be set.
-        """
-        if save and nosave:
-            raise DataError("SHUTDOWN save and nosave cannot both be set")
-        args = ["SHUTDOWN"]
-        if save:
-            args.append("SAVE")
-        if nosave:
-            args.append("NOSAVE")
-        try:
-            self.execute_command(*args)
-        except ConnectionError:
-            # a ConnectionError here is expected
-            return
-        raise RedisError("SHUTDOWN seems to have failed.")
-
-    def slaveof(
-        self, host: Optional[str] = None, port: Optional[int] = None
-    ) -> Awaitable:
-        """
-        Set the server to be a replicated slave of the instance identified
-        by the ``host`` and ``port``. If called without arguments, the
-        instance is promoted to a master instead.
-        """
-        if host is None and port is None:
-            return self.execute_command("SLAVEOF", b"NO", b"ONE")
-        return self.execute_command("SLAVEOF", host, port)
-
-    def slowlog_get(self, num: Optional[int] = None) -> Awaitable:
-        """
-        Get the entries from the slowlog. If ``num`` is specified, get the
-        most recent ``num`` items.
-        """
-        args: List[EncodableT] = ["SLOWLOG GET"]
-        if num is not None:
-            args.append(num)
-        decode_responses = self.connection_pool.connection_kwargs.get(
-            "decode_responses", False
-        )
-        return self.execute_command(*args, decode_responses=decode_responses)
-
-    def slowlog_len(self) -> Awaitable:
-        """Get the number of items in the slowlog"""
-        return self.execute_command("SLOWLOG LEN")
-
-    def slowlog_reset(self) -> Awaitable:
-        """Remove all items in the slowlog"""
-        return self.execute_command("SLOWLOG RESET")
-
-    def time(self) -> Awaitable:
-        """
-        Returns the server time as a 2-item tuple of ints:
-        (seconds since epoch, microseconds into this second).
-        """
-        return self.execute_command("TIME")
-
-    def wait(self, num_replicas: int, timeout: int) -> Awaitable:
-        """
-        Redis synchronous replication
-        That returns the number of replicas that processed the query when
-        we finally have at least ``num_replicas``, or when the ``timeout`` was
-        reached.
-        """
-        return self.execute_command("WAIT", num_replicas, timeout)
-
-    # BASIC KEY COMMANDS
-    def append(self, key: KeyT, value: EncodableT) -> Awaitable:
-        """
-        Appends the string ``value`` to the value at ``key``. If ``key``
-        doesn't already exist, create it with a value of ``value``.
-        Returns the new length of the value at ``key``.
-        """
-        return self.execute_command("APPEND", key, value)
-
-    def bitcount(
-        self, key: KeyT, start: Optional[int] = None, end: Optional[int] = None
-    ) -> Awaitable:
-        """
-        Returns the count of set bits in the value of ``key``.  Optional
-        ``start`` and ``end`` paramaters indicate which bytes to consider
-        """
-        params: List[EncodableT] = [key]
-        if start is not None and end is not None:
-            params.append(start)
-            params.append(end)
-        elif (start is not None and end is None) or (end is not None and start is None):
-            raise DataError("Both start and end must be specified")
-        return self.execute_command("BITCOUNT", *params)
-
-    def bitfield(
-        self, key: KeyT, default_overflow: Optional[str] = None
-    ) -> "BitFieldOperation":
-        """
-        Return a BitFieldOperation instance to conveniently construct one or
-        more bitfield operations on ``key``.
-        """
-        return BitFieldOperation(self, key, default_overflow=default_overflow)
-
-    def bitop(self, operation: str, dest: KeyT, *keys: KeyT) -> Awaitable:
-        """
-        Perform a bitwise operation using ``operation`` between ``keys`` and
-        store the result in ``dest``.
-        """
-        return self.execute_command("BITOP", operation, dest, *keys)
-
-    def bitpos(
-        self,
-        key: KeyT,
-        bit: int,
-        start: Optional[int] = None,
-        end: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Return the position of the first bit set to 1 or 0 in a string.
-        ``start`` and ``end`` difines search range. The range is interpreted
-        as a range of bytes and not a range of bits, so start=0 and end=2
-        means to look at the first three bytes.
-        """
-        if bit not in (0, 1):
-            raise DataError("bit must be 0 or 1")
-        params = [key, bit]
-
-        if start is not None:
-            params.append(start)
-            if end is not None:
-                params.append(end)
-        elif end is not None:
-            raise DataError("start argument is not set, when end is specified")
-        return self.execute_command("BITPOS", *params)
-
-    def decr(self, name: KeyT, amount: int = 1) -> Awaitable:
-        """
-        Decrements the value of ``key`` by ``amount``.  If no key exists,
-        the value will be initialized as 0 - ``amount``
-        """
-        # An alias for ``decr()``, because it is already implemented
-        # as DECRBY redis command.
-        return self.decrby(name, amount)
-
-    def decrby(self, name: KeyT, amount: int = 1) -> Awaitable:
-        """
-        Decrements the value of ``key`` by ``amount``.  If no key exists,
-        the value will be initialized as 0 - ``amount``
-        """
-        return self.execute_command("DECRBY", name, amount)
-
-    def delete(self, *names: KeyT) -> Awaitable:
-        """Delete one or more keys specified by ``names``"""
-        return self.execute_command("DEL", *names)
-
-    def dump(self, name: KeyT) -> Awaitable:
-        """
-        Return a serialized version of the value stored at the specified key.
-        If key does not exist a nil bulk reply is returned.
-        """
-        return self.execute_command("DUMP", name)
-
-    def exists(self, *names: KeyT) -> Awaitable:
-        """Returns the number of ``names`` that exist"""
-        return self.execute_command("EXISTS", *names)
-
-    def expire(self, name: KeyT, time: ExpiryT) -> Awaitable:
-        """
-        Set an expire flag on key ``name`` for ``time`` seconds. ``time``
-        can be represented by an integer or a Python timedelta object.
-        """
-        if isinstance(time, datetime.timedelta):
-            time = int(time.total_seconds())
-        return self.execute_command("EXPIRE", name, time)
-
-    def expireat(self, name: KeyT, when: AbsExpiryT) -> Awaitable:
-        """
-        Set an expire flag on key ``name``. ``when`` can be represented
-        as an integer indicating unix time or a Python datetime object.
-        """
-        if isinstance(when, datetime.datetime):
-            when = int(mod_time.mktime(when.timetuple()))
-        return self.execute_command("EXPIREAT", name, when)
-
-    def get(self, name: KeyT) -> Awaitable:
-        """
-        Return the value at key ``name``, or None if the key doesn't exist
-        """
-        return self.execute_command("GET", name)
-
-    def getbit(self, name: KeyT, offset: int) -> Awaitable:
-        """Returns a boolean indicating the value of ``offset`` in ``name``"""
-        return self.execute_command("GETBIT", name, offset)
-
-    def getrange(self, key: KeyT, start: int, end: int) -> Awaitable:
-        """
-        Returns the substring of the string value stored at ``key``,
-        determined by the offsets ``start`` and ``end`` (both are inclusive)
-        """
-        return self.execute_command("GETRANGE", key, start, end)
-
-    def getset(self, name: KeyT, value: EncodableT) -> Awaitable:
-        """
-        Sets the value at key ``name`` to ``value``
-        and returns the old value at key ``name`` atomically.
-        """
-        return self.execute_command("GETSET", name, value)
-
-    def incr(self, name: KeyT, amount: int = 1) -> Awaitable:
-        """
-        Increments the value of ``key`` by ``amount``.  If no key exists,
-        the value will be initialized as ``amount``
-        """
-        return self.incrby(name, amount)
-
-    def incrby(self, name: KeyT, amount: int = 1) -> Awaitable:
-        """
-        Increments the value of ``key`` by ``amount``.  If no key exists,
-        the value will be initialized as ``amount``
-        """
-        # An alias for ``incr()``, because it is already implemented
-        # as INCRBY redis command.
-        return self.execute_command("INCRBY", name, amount)
-
-    def incrbyfloat(self, name: KeyT, amount: float = 1.0) -> Awaitable:
-        """
-        Increments the value at key ``name`` by floating ``amount``.
-        If no key exists, the value will be initialized as ``amount``
-        """
-        return self.execute_command("INCRBYFLOAT", name, amount)
-
-    def keys(self, pattern: PatternT = "*") -> Awaitable:
-        """Returns a list of keys matching ``pattern``"""
-        return self.execute_command("KEYS", pattern)
-
-    def mget(self, keys: KeysT, *args: EncodableT) -> Awaitable:
-        """
-        Returns a list of values ordered identically to ``keys``
-        """
-        encoded_args = list_or_args(keys, args)
-        options: Dict[str, Union[EncodableT, Iterable[EncodableT]]] = {}
-        if not encoded_args:
-            options[EMPTY_RESPONSE] = []
-        return self.execute_command("MGET", *encoded_args, **options)
-
-    def mset(self, mapping: Mapping[AnyKeyT, EncodableT]) -> Awaitable:
-        """
-        Sets key/values based on a mapping. Mapping is a dictionary of
-        key/value pairs. Both keys and values should be strings or types that
-        can be cast to a string via str().
-        """
-        items: List[EncodableT] = []
-        for pair in mapping.items():
-            items.extend(pair)
-        return self.execute_command("MSET", *items)
-
-    def msetnx(self, mapping: Mapping[AnyKeyT, EncodableT]) -> Awaitable:
-        """
-        Sets key/values based on a mapping if none of the keys are already set.
-        Mapping is a dictionary of key/value pairs. Both keys and values
-        should be strings or types that can be cast to a string via str().
-        Returns a boolean indicating if the operation was successful.
-        """
-        items: List[EncodableT] = []
-        for pair in mapping.items():
-            items.extend(pair)
-        return self.execute_command("MSETNX", *items)
-
-    def move(self, name: KeyT, db: int) -> Awaitable:
-        """Moves the key ``name`` to a different Redis database ``db``"""
-        return self.execute_command("MOVE", name, db)
-
-    def persist(self, name: KeyT) -> Awaitable:
-        """Removes an expiration on ``name``"""
-        return self.execute_command("PERSIST", name)
-
-    def pexpire(self, name: KeyT, time: ExpiryT) -> Awaitable:
-        """
-        Set an expire flag on key ``name`` for ``time`` milliseconds.
-        ``time`` can be represented by an integer or a Python timedelta
-        object.
-        """
-        if isinstance(time, datetime.timedelta):
-            time = int(time.total_seconds() * 1000)
-        return self.execute_command("PEXPIRE", name, time)
-
-    def pexpireat(self, name: KeyT, when: AbsExpiryT) -> Awaitable:
-        """
-        Set an expire flag on key ``name``. ``when`` can be represented
-        as an integer representing unix time in milliseconds (unix time * 1000)
-        or a Python datetime object.
-        """
-        if isinstance(when, datetime.datetime):
-            ms = int(when.microsecond / 1000)
-            when = int(mod_time.mktime(when.timetuple())) * 1000 + ms
-        return self.execute_command("PEXPIREAT", name, when)
-
-    def psetex(self, name: KeyT, time_ms: ExpiryT, value: EncodableT) -> Awaitable:
-        """
-        Set the value of key ``name`` to ``value`` that expires in ``time_ms``
-        milliseconds. ``time_ms`` can be represented by an integer or a Python
-        timedelta object
-        """
-        if isinstance(time_ms, datetime.timedelta):
-            time_ms = int(time_ms.total_seconds() * 1000)
-        return self.execute_command("PSETEX", name, time_ms, value)
-
-    def pttl(self, name: KeyT) -> Awaitable:
-        """Returns the number of milliseconds until the key ``name`` will expire"""
-        return self.execute_command("PTTL", name)
-
-    def randomkey(self) -> Awaitable:
-        """Returns the name of a random key"""
-        return self.execute_command("RANDOMKEY")
-
-    def rename(self, src: KeyT, dst: KeyT) -> Awaitable:
-        """
-        Rename key ``src`` to ``dst``
-        """
-        return self.execute_command("RENAME", src, dst)
-
-    def renamenx(self, src: KeyT, dst: KeyT) -> Awaitable:
-        """Rename key ``src`` to ``dst`` if ``dst`` doesn't already exist"""
-        return self.execute_command("RENAMENX", src, dst)
-
-    def restore(
-        self,
-        name: KeyT,
-        ttl: float,
-        value: EncodableT,
-        replace: bool = False,
-        absttl: bool = False,
-    ) -> Awaitable:
-        """
-        Create a key using the provided serialized value, previously obtained
-        using DUMP.
-
-        ``replace`` allows an existing key on ``name`` to be overridden. If
-        it's not specified an error is raised on collision.
-
-        ``absttl`` if True, specified ``ttl`` should represent an absolute Unix
-        timestamp in milliseconds in which the key will expire. (Redis 5.0 or
-        greater).
-        """
-        params = [name, ttl, value]
-        if replace:
-            params.append("REPLACE")
-        if absttl:
-            params.append("ABSTTL")
-        return self.execute_command("RESTORE", *params)
-
-    def set(
-        self,
-        name: KeyT,
-        value: EncodableT,
-        ex: Optional[ExpiryT] = None,
-        px: Optional[ExpiryT] = None,
-        nx: bool = False,
-        xx: bool = False,
-        keepttl: bool = False,
-    ) -> Awaitable:
-        """
-        Set the value at key ``name`` to ``value``
-
-        ``ex`` sets an expire flag on key ``name`` for ``ex`` seconds.
-
-        ``px`` sets an expire flag on key ``name`` for ``px`` milliseconds.
-
-        ``nx`` if set to True, set the value at key ``name`` to ``value`` only
-            if it does not exist.
-
-        ``xx`` if set to True, set the value at key ``name`` to ``value`` only
-            if it already exists.
-
-        ``keepttl`` if True, retain the time to live associated with the key.
-            (Available since Redis 6.0)
-        """
-        pieces: List[EncodableT] = [name, value]
-        if ex is not None:
-            pieces.append("EX")
-            if isinstance(ex, datetime.timedelta):
-                ex = int(ex.total_seconds())
-            pieces.append(ex)
-        if px is not None:
-            pieces.append("PX")
-            if isinstance(px, datetime.timedelta):
-                px = int(px.total_seconds() * 1000)
-            pieces.append(px)
-
-        if nx:
-            pieces.append("NX")
-        if xx:
-            pieces.append("XX")
-
-        if keepttl:
-            pieces.append("KEEPTTL")
-
-        return self.execute_command("SET", *pieces)
-
-    def setbit(self, name: KeyT, offset: int, value: int) -> Awaitable:
-        """
-        Flag the ``offset`` in ``name`` as ``value``. Returns a boolean
-        indicating the previous value of ``offset``.
-        """
-        value = value and 1 or 0
-        return self.execute_command("SETBIT", name, offset, value)
-
-    def setex(
-        self, name: KeyT, time: Union[int, datetime.timedelta], value: EncodableT
-    ) -> Awaitable:
-        """
-        Set the value of key ``name`` to ``value`` that expires in ``time``
-        seconds. ``time`` can be represented by an integer or a Python
-        timedelta object.
-        """
-        if isinstance(time, datetime.timedelta):
-            time = int(time.total_seconds())
-        return self.execute_command("SETEX", name, time, value)
-
-    def setnx(self, name: KeyT, value: EncodableT) -> Awaitable:
-        """Set the value of key ``name`` to ``value`` if key doesn't exist"""
-        return self.execute_command("SETNX", name, value)
-
-    def setrange(self, name: KeyT, offset: int, value: EncodableT) -> Awaitable:
-        """
-        Overwrite bytes in the value of ``name`` starting at ``offset`` with
-        ``value``. If ``offset`` plus the length of ``value`` exceeds the
-        length of the original value, the new value will be larger than before.
-        If ``offset`` exceeds the length of the original value, null bytes
-        will be used to pad between the end of the previous value and the start
-        of what's being injected.
-
-        Returns the length of the new string.
-        """
-        return self.execute_command("SETRANGE", name, offset, value)
-
-    def strlen(self, name: KeyT) -> Awaitable:
-        """Return the number of bytes stored in the value of ``name``"""
-        return self.execute_command("STRLEN", name)
-
-    def substr(self, name: KeyT, start: int, end: int = -1) -> Awaitable:
-        """
-        Return a substring of the string at key ``name``. ``start`` and ``end``
-        are 0-based integers specifying the portion of the string to return.
-        """
-        return self.execute_command("SUBSTR", name, start, end)
-
-    def touch(self, *args: KeyT) -> Awaitable:
-        """
-        Alters the last access time of a key(s) ``*args``. A key is ignored
-        if it does not exist.
-        """
-        return self.execute_command("TOUCH", *args)
-
-    def ttl(self, name: KeyT) -> Awaitable:
-        """Returns the number of seconds until the key ``name`` will expire"""
-        return self.execute_command("TTL", name)
-
-    def type(self, name: KeyT) -> Awaitable:
-        """Returns the type of key ``name``"""
-        return self.execute_command("TYPE", name)
-
-    def unlink(self, *names: KeyT) -> Awaitable:
-        """Unlink one or more keys specified by ``names``"""
-        return self.execute_command("UNLINK", *names)
-
-    # LIST COMMANDS
-    def blpop(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
-        """
-        LPOP a value off of the first non-empty list
-        named in the ``keys`` list.
-
-        If none of the lists in ``keys`` has a value to LPOP, then block
-        for ``timeout`` seconds, or until a value gets pushed on to one
-        of the lists.
-
-        If timeout is 0, then block indefinitely.
-        """
-        return self.execute_command("BLPOP", *list_or_args(keys, (timeout,)))
-
-    def brpop(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
-        """
-        RPOP a value off of the first non-empty list
-        named in the ``keys`` list.
-
-        If none of the lists in ``keys`` has a value to RPOP, then block
-        for ``timeout`` seconds, or until a value gets pushed on to one
-        of the lists.
-
-        If timeout is 0, then block indefinitely.
-        """
-        return self.execute_command("BRPOP", *list_or_args(keys, (timeout,)))
-
-    def brpoplpush(self, src: KeyT, dst: KeyT, timeout: TimeoutSecT = 0) -> Awaitable:
-        """
-        Pop a value off the tail of ``src``, push it on the head of ``dst``
-        and then return it.
-
-        This command blocks until a value is in ``src`` or until ``timeout``
-        seconds elapse, whichever is first. A ``timeout`` value of 0 blocks
-        forever.
-        """
-        return self.execute_command("BRPOPLPUSH", src, dst, timeout)
-
-    def lindex(self, name: KeyT, index: int) -> Awaitable:
-        """
-        Return the item from list ``name`` at position ``index``
-
-        Negative indexes are supported and will return an item at the
-        end of the list
-        """
-        return self.execute_command("LINDEX", name, index)
-
-    def linsert(
-        self, name: KeyT, where: str, refvalue: EncodableT, value: EncodableT
-    ) -> Awaitable:
-        """
-        Insert ``value`` in list ``name`` either immediately before or after
-        [``where``] ``refvalue``
-
-        Returns the new length of the list on success or -1 if ``refvalue``
-        is not in the list.
-        """
-        return self.execute_command("LINSERT", name, where, refvalue, value)
-
-    def llen(self, name: KeyT) -> Awaitable:
-        """Return the length of the list ``name``"""
-        return self.execute_command("LLEN", name)
-
-    def lpop(self, name: KeyT) -> Awaitable:
-        """Remove and return the first item of the list ``name``"""
-        return self.execute_command("LPOP", name)
-
-    def lpush(self, name: KeyT, *values: EncodableT) -> Awaitable:
-        """Push ``values`` onto the head of the list ``name``"""
-        return self.execute_command("LPUSH", name, *values)
-
-    def lpushx(self, name: KeyT, value: EncodableT) -> Awaitable:
-        """Push ``value`` onto the head of the list ``name`` if ``name`` exists"""
-        return self.execute_command("LPUSHX", name, value)
-
-    def lrange(self, name: KeyT, start: int, end: int) -> Awaitable:
-        """
-        Return a slice of the list ``name`` between
-        position ``start`` and ``end``
-
-        ``start`` and ``end`` can be negative numbers just like
-        Python slicing notation
-        """
-        return self.execute_command("LRANGE", name, start, end)
-
-    def lrem(self, name: KeyT, count: int, value: EncodableT) -> Awaitable:
-        """
-        Remove the first ``count`` occurrences of elements equal to ``value``
-        from the list stored at ``name``.
-
-        The count argument influences the operation in the following ways:
-            count > 0: Remove elements equal to value moving from head to tail.
-            count < 0: Remove elements equal to value moving from tail to head.
-            count = 0: Remove all elements equal to value.
-        """
-        return self.execute_command("LREM", name, count, value)
-
-    def lset(self, name: KeyT, index: int, value: EncodableT) -> Awaitable:
-        """Set ``position`` of list ``name`` to ``value``"""
-        return self.execute_command("LSET", name, index, value)
-
-    def ltrim(self, name: KeyT, start: int, end: int) -> Awaitable:
-        """
-        Trim the list ``name``, removing all values not within the slice
-        between ``start`` and ``end``
-
-        ``start`` and ``end`` can be negative numbers just like
-        Python slicing notation
-        """
-        return self.execute_command("LTRIM", name, start, end)
-
-    def rpop(self, name: KeyT) -> Awaitable:
-        """Remove and return the last item of the list ``name``"""
-        return self.execute_command("RPOP", name)
-
-    def rpoplpush(self, src: KeyT, dst: KeyT) -> Awaitable:
-        """
-        RPOP a value off of the ``src`` list and atomically LPUSH it
-        on to the ``dst`` list.  Returns the value.
-        """
-        return self.execute_command("RPOPLPUSH", src, dst)
-
-    def rpush(self, name: KeyT, *values: EncodableT) -> Awaitable:
-        """Push ``values`` onto the tail of the list ``name``"""
-        return self.execute_command("RPUSH", name, *values)
-
-    def rpushx(self, name: KeyT, value: EncodableT) -> Awaitable:
-        """Push ``value`` onto the tail of the list ``name`` if ``name`` exists"""
-        return self.execute_command("RPUSHX", name, value)
-
-    def lpos(
-        self,
-        name: KeyT,
-        value: EncodableT,
-        rank: Optional[int] = None,
-        count: Optional[int] = None,
-        maxlen: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Get position of ``value`` within the list ``name``
-
-         If specified, ``rank`` indicates the "rank" of the first element to
-         return in case there are multiple copies of ``value`` in the list.
-         By default, LPOS returns the position of the first occurrence of
-         ``value`` in the list. When ``rank`` 2, LPOS returns the position of
-         the second ``value`` in the list. If ``rank`` is negative, LPOS
-         searches the list in reverse. For example, -1 would return the
-         position of the last occurrence of ``value`` and -2 would return the
-         position of the next to last occurrence of ``value``.
-
-         If specified, ``count`` indicates that LPOS should return a list of
-         up to ``count`` positions. A ``count`` of 2 would return a list of
-         up to 2 positions. A ``count`` of 0 returns a list of all positions
-         matching ``value``. When ``count`` is specified and but ``value``
-         does not exist in the list, an empty list is returned.
-
-         If specified, ``maxlen`` indicates the maximum number of list
-         elements to scan. A ``maxlen`` of 1000 will only return the
-         position(s) of items within the first 1000 entries in the list.
-         A ``maxlen`` of 0 (the default) will scan the entire list.
-        """
-        pieces: List[EncodableT] = [name, value]
-        if rank is not None:
-            pieces.extend(["RANK", rank])
-
-        if count is not None:
-            pieces.extend(["COUNT", count])
-
-        if maxlen is not None:
-            pieces.extend(["MAXLEN", maxlen])
-
-        return self.execute_command("LPOS", *pieces)
-
-    def sort(
-        self,
-        name: KeyT,
-        start: Optional[int] = None,
-        num: Optional[int] = None,
-        by: Optional[KeyT] = None,
-        get: Optional[KeysT] = None,
-        desc: bool = False,
-        alpha: bool = False,
-        store: Optional[KeyT] = None,
-        groups: bool = False,
-    ) -> Awaitable:
-        """
-        Sort and return the list, set or sorted set at ``name``.
-
-        ``start`` and ``num`` allow for paging through the sorted data
-
-        ``by`` allows using an external key to weight and sort the items.
-            Use an "*" to indicate where in the key the item value is located
-
-        ``get`` allows for returning items from external keys rather than the
-            sorted data itself.  Use an "*" to indicate where in the key
-            the item value is located
-
-        ``desc`` allows for reversing the sort
-
-        ``alpha`` allows for sorting lexicographically rather than numerically
-
-        ``store`` allows for storing the result of the sort into
-            the key ``store``
-
-        ``groups`` if set to True and if ``get`` contains at least two
-            elements, sort will return a list of tuples, each containing the
-            values fetched from the arguments to ``get``.
-
-        """
-        if (start is not None and num is None) or (num is not None and start is None):
-            raise DataError("``start`` and ``num`` must both be specified")
-
-        pieces: List[EncodableT] = [name]
-        if by is not None:
-            pieces.append(b"BY")
-            pieces.append(by)
-        if start is not None and num is not None:
-            pieces.append(b"LIMIT")
-            pieces.append(start)
-            pieces.append(num)
-        if get is not None:
-            # If get is a string assume we want to get a single value.
-            # Otherwise assume it's an interable and we want to get multiple
-            # values. We can't just iterate blindly because strings are
-            # iterable.
-            if isinstance(get, (bytes, str)):
-                pieces.append(b"GET")
-                pieces.append(get)
-            else:
-                for g in get:
-                    pieces.append(b"GET")
-                    pieces.append(g)
-        if desc:
-            pieces.append(b"DESC")
-        if alpha:
-            pieces.append(b"ALPHA")
-        if store is not None:
-            pieces.append(b"STORE")
-            pieces.append(store)
-
-        if groups:
-            if not get or isinstance(get, (bytes, str)) or len(get) < 2:
-                raise DataError(
-                    'when using "groups" the "get" argument '
-                    "must be specified and contain at least "
-                    "two keys"
-                )
-            options: Dict[str, Optional[int]] = {"groups": len(get)}
-        else:
-            options = {"groups": None}
-
-        return self.execute_command("SORT", *pieces, **options)
-
-    # SCAN COMMANDS
-    def scan(
-        self,
-        cursor: int = 0,
-        match: Optional[PatternT] = None,
-        count: Optional[int] = None,
-        _type: Optional[str] = None,
-    ) -> Awaitable:
-        """
-        Incrementally return lists of key names. Also return a cursor
-        indicating the scan position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` provides a hint to Redis about the number of keys to
-            return per batch.
-
-        ``_type`` filters the returned values by a particular Redis type.
-            Stock Redis instances allow for the following types:
-            HASH, LIST, SET, STREAM, STRING, ZSET
-            Additionally, Redis modules can expose other types as well.
-        """
-        pieces: List[EncodableT] = [cursor]
-        if match is not None:
-            pieces.extend([b"MATCH", match])
-        if count is not None:
-            pieces.extend([b"COUNT", count])
-        if _type is not None:
-            pieces.extend([b"TYPE", _type])
-        return self.execute_command("SCAN", *pieces)
-
-    async def scan_iter(
-        self,
-        match: Optional[PatternT] = None,
-        count: Optional[int] = None,
-        _type: Optional[str] = None,
-    ) -> AsyncIterator:
-        """
-        Make an iterator using the SCAN command so that the client doesn't
-        need to remember the cursor position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` provides a hint to Redis about the number of keys to
-            return per batch.
-
-        ``_type`` filters the returned values by a particular Redis type.
-            Stock Redis instances allow for the following types:
-            HASH, LIST, SET, STREAM, STRING, ZSET
-            Additionally, Redis modules can expose other types as well.
-        """
-        cursor = None
-        while cursor != 0:
-            cursor, data = await self.scan(
-                cursor=cursor or 0, match=match, count=count, _type=_type
-            )
-            for d in data:
-                yield d
-
-    def sscan(
-        self,
-        name: KeyT,
-        cursor: int = 0,
-        match: Optional[PatternT] = None,
-        count: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Incrementally return lists of elements in a set. Also return a cursor
-        indicating the scan position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` allows for hint the minimum number of returns
-        """
-        pieces: List[EncodableT] = [name, cursor]
-        if match is not None:
-            pieces.extend([b"MATCH", match])
-        if count is not None:
-            pieces.extend([b"COUNT", count])
-        return self.execute_command("SSCAN", *pieces)
-
-    async def sscan_iter(
-        self, name: KeyT, match: Optional[PatternT] = None, count: Optional[int] = None
-    ) -> AsyncIterator:
-        """
-        Make an iterator using the SSCAN command so that the client doesn't
-        need to remember the cursor position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` allows for hint the minimum number of returns
-        """
-        cursor = None
-        while cursor != 0:
-            cursor, data = await self.sscan(
-                name, cursor=cursor or 0, match=match, count=count
-            )
-            for d in data:
-                yield d
-
-    def hscan(
-        self,
-        name: KeyT,
-        cursor: int = 0,
-        match: Optional[PatternT] = None,
-        count: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Incrementally return key/value slices in a hash. Also return a cursor
-        indicating the scan position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` allows for hint the minimum number of returns
-        """
-        pieces: List[EncodableT] = [name, cursor]
-        if match is not None:
-            pieces.extend([b"MATCH", match])
-        if count is not None:
-            pieces.extend([b"COUNT", count])
-        return self.execute_command("HSCAN", *pieces)
-
-    async def hscan_iter(
-        self, name: str, match: Optional[PatternT] = None, count: Optional[int] = None
-    ) -> AsyncIterator:
-        """
-        Make an iterator using the HSCAN command so that the client doesn't
-        need to remember the cursor position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` allows for hint the minimum number of returns
-        """
-        cursor = None
-        while cursor != 0:
-            cursor, data = await self.hscan(
-                name, cursor=cursor or 0, match=match, count=count
-            )
-            for it in data.items():
-                yield it
-
-    def zscan(
-        self,
-        name: KeyT,
-        cursor: int = 0,
-        match: Optional[PatternT] = None,
-        count: Optional[int] = None,
-        score_cast_func: Union[Type, Callable] = float,
-    ) -> Awaitable:
-        """
-        Incrementally return lists of elements in a sorted set. Also return a
-        cursor indicating the scan position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` allows for hint the minimum number of returns
-
-        ``score_cast_func`` a callable used to cast the score return value
-        """
-        pieces: List[EncodableT] = [name, cursor]
-        if match is not None:
-            pieces.extend([b"MATCH", match])
-        if count is not None:
-            pieces.extend([b"COUNT", count])
-        options = {"score_cast_func": score_cast_func}
-        return self.execute_command("ZSCAN", *pieces, **options)
-
-    async def zscan_iter(
-        self,
-        name: KeyT,
-        match: Optional[PatternT] = None,
-        count: Optional[int] = None,
-        score_cast_func: Union[Type, Callable] = float,
-    ) -> AsyncIterator:
-        """
-        Make an iterator using the ZSCAN command so that the client doesn't
-        need to remember the cursor position.
-
-        ``match`` allows for filtering the keys by pattern
-
-        ``count`` allows for hint the minimum number of returns
-
-        ``score_cast_func`` a callable used to cast the score return value
-        """
-        cursor = None
-        while cursor != 0:
-            cursor, data = await self.zscan(
-                name,
-                cursor=cursor or 0,
-                match=match,
-                count=count,
-                score_cast_func=score_cast_func,
-            )
-            for d in data:
-                yield d
-
-    # SET COMMANDS
-    def sadd(self, name: KeyT, *values: EncodableT) -> Awaitable:
-        """Add ``value(s)`` to set ``name``"""
-        return self.execute_command("SADD", name, *values)
-
-    def scard(self, name: KeyT) -> Awaitable:
-        """Return the number of elements in set ``name``"""
-        return self.execute_command("SCARD", name)
-
-    def sdiff(self, keys: KeysT, *args: EncodableT) -> Awaitable:
-        """Return the difference of sets specified by ``keys``"""
-        parsed_args = list_or_args(keys, args)
-        return self.execute_command("SDIFF", *parsed_args)
-
-    def sdiffstore(self, dest: KeyT, keys: KeysT, *args: EncodableT) -> Awaitable:
-        """
-        Store the difference of sets specified by ``keys`` into a new
-        set named ``dest``.  Returns the number of keys in the new set.
-        """
-        parsed_args = list_or_args(keys, args)
-        return self.execute_command("SDIFFSTORE", dest, *parsed_args)
-
-    def sinter(self, keys: KeysT, *args: EncodableT) -> Awaitable:
-        """Return the intersection of sets specified by ``keys``"""
-        parsed_args = list_or_args(keys, args)
-        return self.execute_command("SINTER", *parsed_args)
-
-    def sinterstore(self, dest: KeyT, keys: KeysT, *args: EncodableT) -> Awaitable:
-        """
-        Store the intersection of sets specified by ``keys`` into a new
-        set named ``dest``.  Returns the number of keys in the new set.
-        """
-        parsed_args = list_or_args(keys, args)
-        return self.execute_command("SINTERSTORE", dest, *parsed_args)
-
-    def sismember(self, name: KeyT, value: EncodableT) -> Awaitable:
-        """Return a boolean indicating if ``value`` is a member of set ``name``"""
-        return self.execute_command("SISMEMBER", name, value)
-
-    def smembers(self, name: KeyT) -> Awaitable:
-        """Return all members of the set ``name``"""
-        return self.execute_command("SMEMBERS", name)
-
-    def smove(self, src: KeyT, dst: KeyT, value: EncodableT) -> Awaitable:
-        """Move ``value`` from set ``src`` to set ``dst`` atomically"""
-        return self.execute_command("SMOVE", src, dst, value)
-
-    def spop(self, name: KeyT, count: Optional[int] = None) -> Awaitable:
-        """Remove and return a random member of set ``name``"""
-        args = (count is not None) and [count] or []
-        return self.execute_command("SPOP", name, *args)
-
-    def srandmember(self, name: KeyT, number: Optional[int] = None) -> Awaitable:
-        """
-        If ``number`` is None, returns a random member of set ``name``.
-
-        If ``number`` is supplied, returns a list of ``number`` random
-        members of set ``name``. Note this is only available when running
-        Redis 2.6+.
-        """
-        args = (number is not None) and [number] or []
-        return self.execute_command("SRANDMEMBER", name, *args)
-
-    def srem(self, name: KeyT, *values: EncodableT) -> Awaitable:
-        """Remove ``values`` from set ``name``"""
-        return self.execute_command("SREM", name, *values)
-
-    def sunion(self, keys: KeysT, *args: EncodableT) -> Awaitable:
-        """Return the union of sets specified by ``keys``"""
-        parsed_args = list_or_args(keys, args)
-        return self.execute_command("SUNION", *parsed_args)
-
-    def sunionstore(self, dest: KeyT, keys: KeysT, *args: EncodableT) -> Awaitable:
-        """
-        Store the union of sets specified by ``keys`` into a new
-        set named ``dest``.  Returns the number of keys in the new set.
-        """
-        parsed_args = list_or_args(keys, args)
-        return self.execute_command("SUNIONSTORE", dest, *parsed_args)
-
-    # STREAMS COMMANDS
-    def xack(self, name: KeyT, groupname: GroupT, *ids: StreamIdT) -> Awaitable:
-        """
-        Acknowledges the successful processing of one or more messages.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        *ids: message ids to acknowlege.
-        """
-        return self.execute_command("XACK", name, groupname, *ids)
-
-    def xadd(
-        self,
-        name: KeyT,
-        fields: Dict[FieldT, EncodableT],
-        id: StreamIdT = "*",
-        maxlen: Optional[int] = None,
-        approximate: bool = True,
-    ) -> Awaitable:
-        """
-        Add to a stream.
-        name: name of the stream
-        fields: dict of field/value pairs to insert into the stream
-        id: Location to insert this record. By default it is appended.
-        maxlen: truncate old stream members beyond this size
-        approximate: actual stream length may be slightly more than maxlen
-
-        """
-        pieces: List[EncodableT] = []
-        if maxlen is not None:
-            if not isinstance(maxlen, int) or maxlen < 1:
-                raise DataError("XADD maxlen must be a positive integer")
-            pieces.append(b"MAXLEN")
-            if approximate:
-                pieces.append(b"~")
-            pieces.append(str(maxlen))
-        pieces.append(id)
-        if not isinstance(fields, dict) or len(fields) == 0:
-            raise DataError("XADD fields must be a non-empty dict")
-        for pair in fields.items():
-            pieces.extend(pair)
-        return self.execute_command("XADD", name, *pieces)
-
-    def xclaim(
-        self,
-        name: KeyT,
-        groupname: GroupT,
-        consumername: ConsumerT,
-        min_idle_time: int,
-        message_ids: Union[List[StreamIdT], Tuple[StreamIdT]],
-        idle: Optional[int] = None,
-        time: Optional[int] = None,
-        retrycount: Optional[int] = None,
-        force: bool = False,
-        justid: bool = False,
-    ) -> Awaitable:
-        """
-        Changes the ownership of a pending message.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        consumername: name of a consumer that claims the message.
-        min_idle_time: filter messages that were idle less than this amount of
-        milliseconds
-        message_ids: non-empty list or tuple of message IDs to claim
-        idle: optional. Set the idle time (last time it was delivered) of the
-         message in ms
-        time: optional integer. This is the same as idle but instead of a
-         relative amount of milliseconds, it sets the idle time to a specific
-         Unix time (in milliseconds).
-        retrycount: optional integer. set the retry counter to the specified
-         value. This counter is incremented every time a message is delivered
-         again.
-        force: optional boolean, false by default. Creates the pending message
-         entry in the PEL even if certain specified IDs are not already in the
-         PEL assigned to a different client.
-        justid: optional boolean, false by default. Return just an array of IDs
-         of messages successfully claimed, without returning the actual message
-        """
-        if not isinstance(min_idle_time, int) or min_idle_time < 0:
-            raise DataError("XCLAIM min_idle_time must be a non negative " "integer")
-        if not isinstance(message_ids, (list, tuple)) or not message_ids:
-            raise DataError(
-                "XCLAIM message_ids must be a non empty list or "
-                "tuple of message IDs to claim"
-            )
-
-        kwargs = {}
-        pieces: List[EncodableT] = [name, groupname, consumername, str(min_idle_time)]
-        pieces.extend(list(message_ids))
-
-        if idle is not None:
-            if not isinstance(idle, int):
-                raise DataError("XCLAIM idle must be an integer")
-            pieces.extend((b"IDLE", str(idle)))
-        if time is not None:
-            if not isinstance(time, int):
-                raise DataError("XCLAIM time must be an integer")
-            pieces.extend((b"TIME", str(time)))
-        if retrycount is not None:
-            if not isinstance(retrycount, int):
-                raise DataError("XCLAIM retrycount must be an integer")
-            pieces.extend((b"RETRYCOUNT", str(retrycount)))
-
-        if force:
-            if not isinstance(force, bool):
-                raise DataError("XCLAIM force must be a boolean")
-            pieces.append(b"FORCE")
-        if justid:
-            if not isinstance(justid, bool):
-                raise DataError("XCLAIM justid must be a boolean")
-            pieces.append(b"JUSTID")
-            kwargs["parse_justid"] = True
-        return self.execute_command("XCLAIM", *pieces, **kwargs)
-
-    def xdel(self, name: KeyT, *ids: StreamIdT) -> Awaitable:
-        """
-        Deletes one or more messages from a stream.
-        name: name of the stream.
-        *ids: message ids to delete.
-        """
-        return self.execute_command("XDEL", name, *ids)
-
-    def xgroup_create(
-        self, name: KeyT, groupname: GroupT, id: StreamIdT = "$", mkstream: bool = False
-    ) -> Awaitable:
-        """
-        Create a new consumer group associated with a stream.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        id: ID of the last item in the stream to consider already delivered.
-        """
-        pieces: List[EncodableT] = ["XGROUP CREATE", name, groupname, id]
-        if mkstream:
-            pieces.append(b"MKSTREAM")
-        return self.execute_command(*pieces)
-
-    def xgroup_delconsumer(
-        self, name: KeyT, groupname: GroupT, consumername: ConsumerT
-    ) -> Awaitable:
-        """
-        Remove a specific consumer from a consumer group.
-        Returns the number of pending messages that the consumer had before it
-        was deleted.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        consumername: name of consumer to delete
-        """
-        return self.execute_command("XGROUP DELCONSUMER", name, groupname, consumername)
-
-    def xgroup_destroy(self, name: KeyT, groupname: GroupT) -> Awaitable:
-        """
-        Destroy a consumer group.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        """
-        return self.execute_command("XGROUP DESTROY", name, groupname)
-
-    def xgroup_setid(self, name: KeyT, groupname: GroupT, id: StreamIdT) -> Awaitable:
-        """
-        Set the consumer group last delivered ID to something else.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        id: ID of the last item in the stream to consider already delivered.
-        """
-        return self.execute_command("XGROUP SETID", name, groupname, id)
-
-    def xinfo_consumers(self, name: KeyT, groupname: GroupT) -> Awaitable:
-        """
-        Returns general information about the consumers in the group.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        """
-        return self.execute_command("XINFO CONSUMERS", name, groupname)
-
-    def xinfo_groups(self, name: KeyT) -> Awaitable:
-        """
-        Returns general information about the consumer groups of the stream.
-        name: name of the stream.
-        """
-        return self.execute_command("XINFO GROUPS", name)
-
-    def xinfo_stream(self, name: KeyT) -> Awaitable:
-        """
-        Returns general information about the stream.
-        name: name of the stream.
-        """
-        return self.execute_command("XINFO STREAM", name)
-
-    def xlen(self, name: KeyT) -> Awaitable:
-        """
-        Returns the number of elements in a given stream.
-        """
-        return self.execute_command("XLEN", name)
-
-    def xpending(self, name: KeyT, groupname: GroupT) -> Awaitable:
-        """
-        Returns information about pending messages of a group.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        """
-        return self.execute_command("XPENDING", name, groupname)
-
-    def xpending_range(
-        self,
-        name: KeyT,
-        groupname: GroupT,
-        min: Optional[StreamIdT],
-        max: Optional[StreamIdT],
-        count: Optional[int],
-        consumername: Optional[ConsumerT] = None,
-    ) -> Awaitable:
-        """
-        Returns information about pending messages, in a range.
-        name: name of the stream.
-        groupname: name of the consumer group.
-        min: minimum stream ID.
-        max: maximum stream ID.
-        count: number of messages to return
-        consumername: name of a consumer to filter by (optional).
-        """
-        pieces: List[EncodableT] = [name, groupname]
-        if min is not None or max is not None or count is not None:
-            if min is None or max is None or count is None:
-                raise DataError(
-                    "XPENDING must be provided with min, max "
-                    "and count parameters, or none of them. "
-                )
-            if not isinstance(count, int) or count < -1:
-                raise DataError("XPENDING count must be a integer >= -1")
-            pieces.extend((min, max, str(count)))
-        if consumername is not None:
-            if min is None or max is None or count is None:
-                raise DataError(
-                    "if XPENDING is provided with consumername,"
-                    " it must be provided with min, max and"
-                    " count parameters"
-                )
-            pieces.append(consumername)
-        return self.execute_command("XPENDING", *pieces, parse_detail=True)
-
-    def xrange(
-        self,
-        name: KeyT,
-        min: StreamIdT = "-",
-        max: StreamIdT = "+",
-        count: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Read stream values within an interval.
-        name: name of the stream.
-        start: first stream ID. defaults to '-',
-               meaning the earliest available.
-        finish: last stream ID. defaults to '+',
-                meaning the latest available.
-        count: if set, only return this many items, beginning with the
-               earliest available.
-        """
-        pieces: List[EncodableT] = [min, max]
-        if count is not None:
-            if not isinstance(count, int) or count < 1:
-                raise DataError("XRANGE count must be a positive integer")
-            pieces.append(b"COUNT")
-            pieces.append(str(count))
-
-        return self.execute_command("XRANGE", name, *pieces)
-
-    def xread(
-        self,
-        streams: Dict[KeyT, StreamIdT],
-        count: Optional[int] = None,
-        block: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Block and monitor multiple streams for new data.
-        streams: a dict of stream names to stream IDs, where
-                   IDs indicate the last ID already seen.
-        count: if set, only return this many items, beginning with the
-               earliest available.
-        block: number of milliseconds to wait, if nothing already present.
-        """
-        pieces: List[EncodableT] = []
-        if block is not None:
-            if not isinstance(block, int) or block < 0:
-                raise DataError("XREAD block must be a non-negative integer")
-            pieces.append(b"BLOCK")
-            pieces.append(str(block))
-        if count is not None:
-            if not isinstance(count, int) or count < 1:
-                raise DataError("XREAD count must be a positive integer")
-            pieces.append(b"COUNT")
-            pieces.append(str(count))
-        if not isinstance(streams, dict) or len(streams) == 0:
-            raise DataError("XREAD streams must be a non empty dict")
-        pieces.append(b"STREAMS")
-        keys, values = zip(*streams.items())
-        pieces.extend(keys)
-        pieces.extend(values)
-        return self.execute_command("XREAD", *pieces)
-
-    def xreadgroup(
-        self,
-        groupname: str,
-        consumername: str,
-        streams: Dict[KeyT, StreamIdT],
-        count: Optional[int] = None,
-        block: Optional[int] = None,
-        noack: bool = False,
-    ) -> Awaitable:
-        """
-        Read from a stream via a consumer group.
-        groupname: name of the consumer group.
-        consumername: name of the requesting consumer.
-        streams: a dict of stream names to stream IDs, where
-               IDs indicate the last ID already seen.
-        count: if set, only return this many items, beginning with the
-               earliest available.
-        block: number of milliseconds to wait, if nothing already present.
-        noack: do not add messages to the PEL
-        """
-        pieces: List[EncodableT] = [b"GROUP", groupname, consumername]
-        if count is not None:
-            if not isinstance(count, int) or count < 1:
-                raise DataError("XREADGROUP count must be a positive integer")
-            pieces.append(b"COUNT")
-            pieces.append(str(count))
-        if block is not None:
-            if not isinstance(block, int) or block < 0:
-                raise DataError("XREADGROUP block must be a non-negative " "integer")
-            pieces.append(b"BLOCK")
-            pieces.append(str(block))
-        if noack:
-            pieces.append(b"NOACK")
-        if not isinstance(streams, dict) or len(streams) == 0:
-            raise DataError("XREADGROUP streams must be a non empty dict")
-        pieces.append(b"STREAMS")
-        pieces.extend(streams.keys())
-        pieces.extend(streams.values())
-        return self.execute_command("XREADGROUP", *pieces)
-
-    def xrevrange(
-        self,
-        name: KeyT,
-        max: StreamIdT = "+",
-        min: StreamIdT = "-",
-        count: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Read stream values within an interval, in reverse order.
-        name: name of the stream
-        start: first stream ID. defaults to '+',
-               meaning the latest available.
-        finish: last stream ID. defaults to '-',
-                meaning the earliest available.
-        count: if set, only return this many items, beginning with the
-               latest available.
-        """
-        pieces: List[EncodableT] = [max, min]
-        if count is not None:
-            if not isinstance(count, int) or count < 1:
-                raise DataError("XREVRANGE count must be a positive integer")
-            pieces.append(b"COUNT")
-            pieces.append(str(count))
-
-        return self.execute_command("XREVRANGE", name, *pieces)
-
-    def xtrim(self, name: KeyT, maxlen: int, approximate: bool = True) -> Awaitable:
-        """
-        Trims old messages from a stream.
-        name: name of the stream.
-        maxlen: truncate old stream messages beyond this size
-        approximate: actual stream length may be slightly more than maxlen
-        """
-        pieces: List[EncodableT] = [b"MAXLEN"]
-        if approximate:
-            pieces.append(b"~")
-        pieces.append(maxlen)
-        return self.execute_command("XTRIM", name, *pieces)
-
-    # SORTED SET COMMANDS
-    def zadd(
-        self,
-        name: KeyT,
-        mapping: Mapping[AnyKeyT, EncodableT],
-        nx: bool = False,
-        xx: bool = False,
-        ch: bool = False,
-        incr: bool = False,
-    ) -> Awaitable:
-        """
-        Set any number of element-name, score pairs to the key ``name``. Pairs
-        are specified as a dict of element-names keys to score values.
-
-        ``nx`` forces ZADD to only create new elements and not to update
-        scores for elements that already exist.
-
-        ``xx`` forces ZADD to only update scores of elements that already
-        exist. New elements will not be added.
-
-        ``ch`` modifies the return value to be the numbers of elements changed.
-        Changed elements include new elements that were added and elements
-        whose scores changed.
-
-        ``incr`` modifies ZADD to behave like ZINCRBY. In this mode only a
-        single element/score pair can be specified and the score is the amount
-        the existing score will be incremented by. When using this mode the
-        return value of ZADD will be the new score of the element.
-
-        The return value of ZADD varies based on the mode specified. With no
-        options, ZADD returns the number of new elements added to the sorted
-        set.
-        """
-        if not mapping:
-            raise DataError("ZADD requires at least one element/score pair")
-        if nx and xx:
-            raise DataError("ZADD allows either 'nx' or 'xx', not both")
-        if incr and len(mapping) != 1:
-            raise DataError(
-                "ZADD option 'incr' only works when passing a "
-                "single element/score pair"
-            )
-        pieces: List[EncodableT] = []
-        options = {}
-        if nx:
-            pieces.append(b"NX")
-        if xx:
-            pieces.append(b"XX")
-        if ch:
-            pieces.append(b"CH")
-        if incr:
-            pieces.append(b"INCR")
-            options["as_score"] = True
-        for pair in mapping.items():
-            pieces.append(pair[1])
-            pieces.append(pair[0])
-        return self.execute_command("ZADD", name, *pieces, **options)
-
-    def zcard(self, name: KeyT) -> Awaitable:
-        """Return the number of elements in the sorted set ``name``"""
-        return self.execute_command("ZCARD", name)
-
-    def zcount(self, name: KeyT, min: ZScoreBoundT, max: ZScoreBoundT) -> Awaitable:
-        """
-        Returns the number of elements in the sorted set at key ``name`` with
-        a score between ``min`` and ``max``.
-        """
-        return self.execute_command("ZCOUNT", name, min, max)
-
-    def zincrby(self, name: KeyT, amount: float, value: EncodableT) -> Awaitable:
-        """Increment the score of ``value`` in sorted set ``name`` by ``amount``"""
-        return self.execute_command("ZINCRBY", name, amount, value)
-
-    def zinterstore(
-        self,
-        dest: KeyT,
-        keys: Union[Sequence[KeyT], Mapping[AnyKeyT, float]],
-        aggregate: Optional[str] = None,
-    ) -> Awaitable:
-        """
-        Intersect multiple sorted sets specified by ``keys`` into
-        a new sorted set, ``dest``. Scores in the destination will be
-        aggregated based on the ``aggregate``, or SUM if none is provided.
-        """
-        return self._zaggregate("ZINTERSTORE", dest, keys, aggregate)
-
-    def zlexcount(self, name: KeyT, min: EncodableT, max: EncodableT) -> Awaitable:
-        """
-        Return the number of items in the sorted set ``name`` between the
-        lexicographical range ``min`` and ``max``.
-        """
-        return self.execute_command("ZLEXCOUNT", name, min, max)
-
-    def zpopmax(self, name: KeyT, count: Optional[int] = None) -> Awaitable:
-        """
-        Remove and return up to ``count`` members with the highest scores
-        from the sorted set ``name``.
-        """
-        args = (count is not None) and [count] or []
-        options = {"withscores": True}
-        return self.execute_command("ZPOPMAX", name, *args, **options)
-
-    def zpopmin(self, name: KeyT, count: Optional[int] = None) -> Awaitable:
-        """
-        Remove and return up to ``count`` members with the lowest scores
-        from the sorted set ``name``.
-        """
-        args = (count is not None) and [count] or []
-        options = {"withscores": True}
-        return self.execute_command("ZPOPMIN", name, *args, **options)
-
-    def bzpopmax(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
-        """
-        ZPOPMAX a value off of the first non-empty sorted set
-        named in the ``keys`` list.
-
-        If none of the sorted sets in ``keys`` has a value to ZPOPMAX,
-        then block for ``timeout`` seconds, or until a member gets added
-        to one of the sorted sets.
-
-        If timeout is 0, then block indefinitely.
-        """
-        parsed_keys = list_or_args(keys, (timeout,))
-        return self.execute_command("BZPOPMAX", *parsed_keys)
-
-    def bzpopmin(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
-        """
-        ZPOPMIN a value off of the first non-empty sorted set
-        named in the ``keys`` list.
-
-        If none of the sorted sets in ``keys`` has a value to ZPOPMIN,
-        then block for ``timeout`` seconds, or until a member gets added
-        to one of the sorted sets.
-
-        If timeout is 0, then block indefinitely.
-        """
-        klist: List[EncodableT] = list_or_args(keys, None)
-        klist.append(timeout)
-        return self.execute_command("BZPOPMIN", *klist)
-
-    def zrange(
-        self,
-        name: KeyT,
-        start: int,
-        end: int,
-        desc: bool = False,
-        withscores: bool = False,
-        score_cast_func: Union[Type, Callable] = float,
-    ) -> Awaitable:
-        """
-        Return a range of values from sorted set ``name`` between
-        ``start`` and ``end`` sorted in ascending order.
-
-        ``start`` and ``end`` can be negative, indicating the end of the range.
-
-        ``desc`` a boolean indicating whether to sort the results descendingly
-
-        ``withscores`` indicates to return the scores along with the values.
-        The return type is a list of (value, score) pairs
-
-        ``score_cast_func`` a callable used to cast the score return value
-        """
-        if desc:
-            return self.zrevrange(name, start, end, withscores, score_cast_func)
-        pieces: List[EncodableT] = ["ZRANGE", name, start, end]
-        if withscores:
-            pieces.append(b"WITHSCORES")
-        options = {"withscores": withscores, "score_cast_func": score_cast_func}
-        return self.execute_command(*pieces, **options)
-
-    def zrangebylex(
-        self,
-        name: KeyT,
-        min: EncodableT,
-        max: EncodableT,
-        start: Optional[int] = None,
-        num: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Return the lexicographical range of values from sorted set ``name``
-        between ``min`` and ``max``.
-
-        If ``start`` and ``num`` are specified, then return a slice of the
-        range.
-        """
-        if (start is not None and num is None) or (num is not None and start is None):
-            raise DataError("``start`` and ``num`` must both be specified")
-        pieces: List[EncodableT] = ["ZRANGEBYLEX", name, min, max]
-        if start is not None and num is not None:
-            pieces.extend([b"LIMIT", start, num])
-        return self.execute_command(*pieces)
-
-    def zrevrangebylex(
-        self,
-        name: KeyT,
-        max: EncodableT,
-        min: EncodableT,
-        start: Optional[int] = None,
-        num: Optional[int] = None,
-    ) -> Awaitable:
-        """
-        Return the reversed lexicographical range of values from sorted set
-        ``name`` between ``max`` and ``min``.
-
-        If ``start`` and ``num`` are specified, then return a slice of the
-        range.
-        """
-        if (start is not None and num is None) or (num is not None and start is None):
-            raise DataError("``start`` and ``num`` must both be specified")
-        pieces: List[EncodableT] = ["ZREVRANGEBYLEX", name, max, min]
-        if start is not None and num is not None:
-            pieces.extend([b"LIMIT", start, num])
-        return self.execute_command(*pieces)
-
-    def zrangebyscore(
-        self,
-        name: KeyT,
-        min: ZScoreBoundT,
-        max: ZScoreBoundT,
-        start: Optional[int] = None,
-        num: Optional[int] = None,
-        withscores: bool = False,
-        score_cast_func: Union[Type, Callable] = float,
-    ) -> Awaitable:
-        """
-        Return a range of values from the sorted set ``name`` with scores
-        between ``min`` and ``max``.
-
-        If ``start`` and ``num`` are specified, then return a slice
-        of the range.
-
-        ``withscores`` indicates to return the scores along with the values.
-        The return type is a list of (value, score) pairs
-
-        `score_cast_func`` a callable used to cast the score return value
-        """
-        if (start is not None and num is None) or (num is not None and start is None):
-            raise DataError("``start`` and ``num`` must both be specified")
-        pieces: List[EncodableT] = ["ZRANGEBYSCORE", name, min, max]
-        if start is not None and num is not None:
-            pieces.extend([b"LIMIT", start, num])
-        if withscores:
-            pieces.append(b"WITHSCORES")
-        options = {"withscores": withscores, "score_cast_func": score_cast_func}
-        return self.execute_command(*pieces, **options)
-
-    def zrank(self, name: KeyT, value: EncodableT) -> Awaitable:
-        """
-        Returns a 0-based value indicating the rank of ``value`` in sorted set
-        ``name``
-        """
-        return self.execute_command("ZRANK", name, value)
-
-    def zrem(self, name: KeyT, *values: EncodableT) -> Awaitable:
-        """Remove member ``values`` from sorted set ``name``"""
-        return self.execute_command("ZREM", name, *values)
-
-    def zremrangebylex(self, name: KeyT, min: EncodableT, max: EncodableT) -> Awaitable:
-        """
-        Remove all elements in the sorted set ``name`` between the
-        lexicographical range specified by ``min`` and ``max``.
-
-        Returns the number of elements removed.
-        """
-        return self.execute_command("ZREMRANGEBYLEX", name, min, max)
-
-    def zremrangebyrank(self, name: KeyT, min: int, max: int) -> Awaitable:
-        """
-        Remove all elements in the sorted set ``name`` with ranks between
-        ``min`` and ``max``. Values are 0-based, ordered from smallest score
-        to largest. Values can be negative indicating the highest scores.
-        Returns the number of elements removed
-        """
-        return self.execute_command("ZREMRANGEBYRANK", name, min, max)
-
-    def zremrangebyscore(
-        self, name: KeyT, min: ZScoreBoundT, max: ZScoreBoundT
-    ) -> Awaitable:
-        """
-        Remove all elements in the sorted set ``name`` with scores
-        between ``min`` and ``max``. Returns the number of elements removed.
-        """
-        return self.execute_command("ZREMRANGEBYSCORE", name, min, max)
-
-    def zrevrange(
-        self,
-        name: KeyT,
-        start: int,
-        end: int,
-        withscores: bool = False,
-        score_cast_func: Union[Type, Callable] = float,
-    ) -> Awaitable:
-        """
-        Return a range of values from sorted set ``name`` between
-        ``start`` and ``end`` sorted in descending order.
-
-        ``start`` and ``end`` can be negative, indicating the end of the range.
-
-        ``withscores`` indicates to return the scores along with the values
-        The return type is a list of (value, score) pairs
-
-        ``score_cast_func`` a callable used to cast the score return value
-        """
-        pieces: List[EncodableT] = ["ZREVRANGE", name, start, end]
-        if withscores:
-            pieces.append(b"WITHSCORES")
-        options = {"withscores": withscores, "score_cast_func": score_cast_func}
-        return self.execute_command(*pieces, **options)
-
-    def zrevrangebyscore(
-        self,
-        name: KeyT,
-        min: ZScoreBoundT,
-        max: ZScoreBoundT,
-        start: Optional[int] = None,
-        num: Optional[int] = None,
-        withscores: bool = False,
-        score_cast_func: Union[Type, Callable] = float,
-    ) -> Awaitable:
-        """
-        Return a range of values from the sorted set ``name`` with scores
-        between ``min`` and ``max`` in descending order.
-
-        If ``start`` and ``num`` are specified, then return a slice
-        of the range.
-
-        ``withscores`` indicates to return the scores along with the values.
-        The return type is a list of (value, score) pairs
-
-        ``score_cast_func`` a callable used to cast the score return value
-        """
-        if (start is not None and num is None) or (num is not None and start is None):
-            raise DataError("``start`` and ``num`` must both be specified")
-        pieces: List[EncodableT] = ["ZREVRANGEBYSCORE", name, min, max]
-        if start is not None and num is not None:
-            pieces.extend([b"LIMIT", start, num])
-        if withscores:
-            pieces.append(b"WITHSCORES")
-        options = {"withscores": withscores, "score_cast_func": score_cast_func}
-        return self.execute_command(*pieces, **options)
-
-    def zrevrank(self, name: KeyT, value: EncodableT) -> Awaitable:
-        """
-        Returns a 0-based value indicating the descending rank of
-        ``value`` in sorted set ``name``
-        """
-        return self.execute_command("ZREVRANK", name, value)
-
-    def zscore(self, name: str, value: EncodableT) -> Awaitable:
-        """Return the score of element ``value`` in sorted set ``name``"""
-        return self.execute_command("ZSCORE", name, value)
-
-    def zunionstore(
-        self,
-        dest: KeyT,
-        keys: Union[Sequence[KeyT], Mapping[AnyKeyT, float]],
-        aggregate: Optional[str] = None,
-    ) -> Awaitable:
-        """
-        Union multiple sorted sets specified by ``keys`` into
-        a new sorted set, ``dest``. Scores in the destination will be
-        aggregated based on the ``aggregate``, or SUM if none is provided.
-        """
-        return self._zaggregate("ZUNIONSTORE", dest, keys, aggregate)
-
-    def _zaggregate(
-        self,
-        command: str,
-        dest: KeyT,
-        keys: Union[Sequence[KeyT], Mapping[AnyKeyT, float]],
-        aggregate: Optional[str] = None,
-    ) -> Awaitable:
-        pieces: List[EncodableT] = [command, dest, len(keys)]
-        key_names: Union[Sequence[KeyT], AbstractSet[AnyKeyT]]
-        weights: Optional[ValuesView[float]]
-        if isinstance(keys, Mapping):
-            key_names, weights = keys.keys(), keys.values()
-        else:
-            key_names = keys
-            weights = None
-        pieces.extend(key_names)
-        if weights:
-            pieces.append(b"WEIGHTS")
-            pieces.extend(weights)
-        if aggregate:
-            pieces.append(b"AGGREGATE")
-            pieces.append(aggregate)
-        return self.execute_command(*pieces)
-
-    # HYPERLOGLOG COMMANDS
-    def pfadd(self, name: KeyT, *values: EncodableT) -> Awaitable:
-        """Adds the specified elements to the specified HyperLogLog."""
-        return self.execute_command("PFADD", name, *values)
-
-    def pfcount(self, *sources: KeyT) -> Awaitable:
-        """
-        Return the approximated cardinality of
-        the set observed by the HyperLogLog at key(s).
-        """
-        return self.execute_command("PFCOUNT", *sources)
-
-    def pfmerge(self, dest: KeyT, *sources: KeyT) -> Awaitable:
-        """Merge N different HyperLogLogs into a single one."""
-        return self.execute_command("PFMERGE", dest, *sources)
-
-    # HASH COMMANDS
-    def hdel(self, name: KeyT, *keys: FieldT) -> Awaitable:
-        """Delete ``keys`` from hash ``name``"""
-        return self.execute_command("HDEL", name, *keys)
-
-    def hexists(self, name: KeyT, key: FieldT) -> Awaitable:
-        """Returns a boolean indicating if ``key`` exists within hash ``name``"""
-        return self.execute_command("HEXISTS", name, key)
-
-    def hget(self, name: KeyT, key: FieldT) -> Awaitable:
-        """Return the value of ``key`` within the hash ``name``"""
-        return self.execute_command("HGET", name, key)
-
-    def hgetall(self, name: KeyT) -> Awaitable:
-        """Return a Python dict of the hash's name/value pairs"""
-        return self.execute_command("HGETALL", name)
-
-    def hincrby(self, name: KeyT, key: FieldT, amount: int = 1) -> Awaitable:
-        """Increment the value of ``key`` in hash ``name`` by ``amount``"""
-        return self.execute_command("HINCRBY", name, key, amount)
-
-    def hincrbyfloat(self, name: KeyT, key: FieldT, amount: float = 1.0) -> Awaitable:
-        """
-        Increment the value of ``key`` in hash ``name`` by floating ``amount``
-        """
-        return self.execute_command("HINCRBYFLOAT", name, key, amount)
-
-    def hkeys(self, name: KeyT) -> Awaitable:
-        """Return the list of keys within hash ``name``"""
-        return self.execute_command("HKEYS", name)
-
-    def hlen(self, name: KeyT) -> Awaitable:
-        """Return the number of elements in hash ``name``"""
-        return self.execute_command("HLEN", name)
-
-    def hset(
-        self,
-        name: KeyT,
-        key: Optional[FieldT] = None,
-        value: Optional[EncodableT] = None,
-        mapping: Optional[Mapping[AnyFieldT, EncodableT]] = None,
-    ) -> Awaitable:
-        """
-        Set ``key`` to ``value`` within hash ``name``,
-        ``mapping`` accepts a dict of key/value pairs that that will be
-        added to hash ``name``.
-        Returns the number of fields that were added.
-        """
-        if key is None and not mapping:
-            raise DataError("'hset' with no key value pairs")
-        items: List[Union[FieldT, Optional[EncodableT]]] = []
-        if key is not None:
-            items.extend((key, value))
-        if mapping:
-            for pair in mapping.items():
-                items.extend(pair)
-
-        return self.execute_command("HSET", name, *items)
-
-    def hsetnx(self, name: KeyT, key: FieldT, value: EncodableT) -> Awaitable:
-        """
-        Set ``key`` to ``value`` within hash ``name`` if ``key`` does not
-        exist.  Returns 1 if HSETNX created a field, otherwise 0.
-        """
-        return self.execute_command("HSETNX", name, key, value)
-
-    def hmset(self, name: KeyT, mapping: Mapping[AnyFieldT, EncodableT]) -> Awaitable:
-        """
-        Set key to value within hash ``name`` for each corresponding
-        key and value from the ``mapping`` dict.
-        """
-        warnings.warn(
-            f"{self.__class__.__name__}.hmset() is deprecated. "
-            f"Use {self.__class__.__name__}.hset() instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        if not mapping:
-            raise DataError("'hmset' with 'mapping' of length 0")
-        items: List[Union[AnyFieldT, EncodableT]] = []
-        for pair in mapping.items():
-            items.extend(pair)
-        return self.execute_command("HMSET", name, *items)
-
-    def hmget(self, name: KeyT, keys: Sequence[KeyT], *args: FieldT) -> Awaitable:
-        """Returns a list of values ordered identically to ``keys``"""
-        parsed_args = list_or_args(keys, args)
-        return self.execute_command("HMGET", name, *parsed_args)
-
-    def hvals(self, name: KeyT) -> Awaitable:
-        """Return the list of values within hash ``name``"""
-        return self.execute_command("HVALS", name)
-
-    def hstrlen(self, name: KeyT, key: FieldT) -> Awaitable:
-        """
-        Return the number of bytes stored in the value of ``key``
-        within hash ``name``
-        """
-        return self.execute_command("HSTRLEN", name, key)
-
-    def publish(self, channel: ChannelT, message: EncodableT) -> Awaitable:
-        """
-        Publish ``message`` on ``channel``.
-        Returns the number of subscribers the message was delivered to.
-        """
-        return self.execute_command("PUBLISH", channel, message)
-
-    def pubsub_channels(self, pattern: PatternT = "*") -> Awaitable:
-        """
-        Return a list of channels that have at least one subscriber
-        """
-        return self.execute_command("PUBSUB CHANNELS", pattern)
-
-    def pubsub_numpat(self) -> Awaitable:
-        """
-        Returns the number of subscriptions to patterns
-        """
-        return self.execute_command("PUBSUB NUMPAT")
-
-    def pubsub_numsub(self, *args: ChannelT) -> Awaitable:
-        """
-        Return a list of (channel, number of subscribers) tuples
-        for each channel given in ``*args``
-        """
-        return self.execute_command("PUBSUB NUMSUB", *args)
-
-    def cluster(self, cluster_arg: str, *args: str) -> Awaitable:
-        return self.execute_command(f"CLUSTER {cluster_arg.upper()}", *args)
-
-    def eval(
-        self, script: ScriptTextT, numkeys: int, *keys_and_args: EncodableT
-    ) -> Awaitable:
-        """
-        Execute the Lua ``script``, specifying the ``numkeys`` the script
-        will touch and the key names and argument values in ``keys_and_args``.
-        Returns the result of the script.
-
-        In practice, use the object returned by ``register_script``. This
-        function exists purely for Redis API completion.
-        """
-        return self.execute_command("EVAL", script, numkeys, *keys_and_args)
-
-    def evalsha(self, sha: str, numkeys: int, *keys_and_args: EncodableT) -> Awaitable:
-        """
-        Use the ``sha`` to execute a Lua script already registered via EVAL
-        or SCRIPT LOAD. Specify the ``numkeys`` the script will touch and the
-        key names and argument values in ``keys_and_args``. Returns the result
-        of the script.
-
-        In practice, use the object returned by ``register_script``. This
-        function exists purely for Redis API completion.
-        """
-        return self.execute_command("EVALSHA", sha, numkeys, *keys_and_args)
-
-    def script_exists(self, *args: str) -> Awaitable:
-        """
-        Check if a script exists in the script cache by specifying the SHAs of
-        each script as ``args``. Returns a list of boolean values indicating if
-        if each already script exists in the cache.
-        """
-        return self.execute_command("SCRIPT EXISTS", *args)
-
-    def script_flush(self) -> Awaitable:
-        """Flush all scripts from the script cache"""
-        return self.execute_command("SCRIPT FLUSH")
-
-    def script_kill(self) -> Awaitable:
-        """Kill the currently executing Lua script"""
-        return self.execute_command("SCRIPT KILL")
-
-    def script_load(self, script: ScriptTextT) -> Awaitable:
-        """Load a Lua ``script`` into the script cache. Returns the SHA."""
-        return self.execute_command("SCRIPT LOAD", script)
-
-    def register_script(self, script: ScriptTextT) -> "Script":
-        """
-        Register a Lua ``script`` specifying the ``keys`` it will touch.
-        Returns a Script object that is callable and hides the complexity of
-        deal with scripts, keys, and shas. This is the preferred way to work
-        with Lua scripts.
-        """
-        return Script(self, script)
-
-    # GEO COMMANDS
-    def geoadd(self, name: KeyT, *values: EncodableT) -> Awaitable:
-        """
-        Add the specified geospatial items to the specified key identified
-        by the ``name`` argument. The Geospatial items are given as ordered
-        members of the ``values`` argument, each item or place is formed by
-        the triad longitude, latitude and name.
-        """
-        if len(values) % 3 != 0:
-            raise DataError("GEOADD requires places with lon, lat and name values")
-        return self.execute_command("GEOADD", name, *values)
-
-    def geodist(
-        self, name: KeyT, place1: FieldT, place2: FieldT, unit: Optional[str] = None
-    ) -> Awaitable:
-        """
-        Return the distance between ``place1`` and ``place2`` members of the
-        ``name`` key.
-        The units must be one of the following : m, km mi, ft. By default
-        meters are used.
-        """
-        pieces: List[EncodableT] = [name, place1, place2]
-        if unit and unit not in ("m", "km", "mi", "ft"):
-            raise DataError("GEODIST invalid unit")
-        elif unit:
-            pieces.append(unit)
-        return self.execute_command("GEODIST", *pieces)
-
-    def geohash(self, name: KeyT, *values: FieldT) -> Awaitable:
-        """
-        Return the geo hash string for each item of ``values`` members of
-        the specified key identified by the ``name`` argument.
-        """
-        return self.execute_command("GEOHASH", name, *values)
-
-    def geopos(self, name: KeyT, *values: FieldT) -> Awaitable:
-        """
-        Return the positions of each item of ``values`` as members of
-        the specified key identified by the ``name`` argument. Each position
-        is represented by the pairs lon and lat.
-        """
-        return self.execute_command("GEOPOS", name, *values)
-
-    def georadius(
-        self,
-        name: KeyT,
-        longitude: float,
-        latitude: float,
-        radius: float,
-        unit: Optional[str] = None,
-        withdist: bool = False,
-        withcoord: bool = False,
-        withhash: bool = False,
-        count: Optional[int] = None,
-        sort: Optional[str] = None,
-        store: Optional[KeyT] = None,
-        store_dist: Optional[KeyT] = None,
-    ) -> Awaitable:
-        """
-        Return the members of the specified key identified by the
-        ``name`` argument which are within the borders of the area specified
-        with the ``latitude`` and ``longitude`` location and the maximum
-        distance from the center specified by the ``radius`` value.
-
-        The units must be one of the following : m, km mi, ft. By default
-
-        ``withdist`` indicates to return the distances of each place.
-
-        ``withcoord`` indicates to return the latitude and longitude of
-        each place.
-
-        ``withhash`` indicates to return the geohash string of each place.
-
-        ``count`` indicates to return the number of elements up to N.
-
-        ``sort`` indicates to return the places in a sorted way, ASC for
-        nearest to fairest and DESC for fairest to nearest.
-
-        ``store`` indicates to save the places names in a sorted set named
-        with a specific key, each element of the destination sorted set is
-        populated with the score got from the original geo sorted set.
-
-        ``store_dist`` indicates to save the places names in a sorted set
-        named with a specific key, instead of ``store`` the sorted set
-        destination score is set with the distance.
-        """
-        return self._georadiusgeneric(
-            "GEORADIUS",
-            name,
-            longitude,
-            latitude,
-            radius,
-            unit=unit,
-            withdist=withdist,
-            withcoord=withcoord,
-            withhash=withhash,
-            count=count,
-            sort=sort,
-            store=store,
-            store_dist=store_dist,
-        )
-
-    def georadiusbymember(
-        self,
-        name: KeyT,
-        member: FieldT,
-        radius: float,
-        unit: Optional[str] = None,
-        withdist: bool = False,
-        withcoord: bool = False,
-        withhash: bool = False,
-        count: Optional[int] = None,
-        sort: Optional[str] = None,
-        store: Optional[KeyT] = None,
-        store_dist: Optional[KeyT] = None,
-    ) -> Awaitable:
-        """
-        This command is exactly like ``georadius`` with the sole difference
-        that instead of taking, as the center of the area to query, a longitude
-        and latitude value, it takes the name of a member already existing
-        inside the geospatial index represented by the sorted set.
-        """
-        return self._georadiusgeneric(
-            "GEORADIUSBYMEMBER",
-            name,
-            member,
-            radius,
-            unit=unit,
-            withdist=withdist,
-            withcoord=withcoord,
-            withhash=withhash,
-            count=count,
-            sort=sort,
-            store=store,
-            store_dist=store_dist,
-        )
-
-    def _georadiusgeneric(
-        self, command: str, *args: EncodableT, **kwargs: Optional[EncodableT]
-    ) -> Awaitable:
-        pieces: List[Optional[EncodableT]] = list(args)
-        if kwargs["unit"] and kwargs["unit"] not in ("m", "km", "mi", "ft"):
-            raise DataError("GEORADIUS invalid unit")
-        elif kwargs["unit"]:
-            pieces.append(kwargs["unit"])
-        else:
-            pieces.append(
-                "m",
-            )
-
-        for arg_name, byte_repr in (
-            ("withdist", b"WITHDIST"),
-            ("withcoord", b"WITHCOORD"),
-            ("withhash", b"WITHHASH"),
-        ):
-            if kwargs[arg_name]:
-                pieces.append(byte_repr)
-
-        if kwargs["count"]:
-            pieces.extend([b"COUNT", kwargs["count"]])
-
-        if kwargs["sort"]:
-            if kwargs["sort"] == "ASC":
-                pieces.append(b"ASC")
-            elif kwargs["sort"] == "DESC":
-                pieces.append(b"DESC")
-            else:
-                raise DataError("GEORADIUS invalid sort")
-
-        if kwargs["store"] and kwargs["store_dist"]:
-            raise DataError("GEORADIUS store and store_dist cant be set" " together")
-
-        if kwargs["store"]:
-            pieces.extend([b"STORE", kwargs["store"]])
-
-        if kwargs["store_dist"]:
-            pieces.extend([b"STOREDIST", kwargs["store_dist"]])
-
-        return self.execute_command(command, *pieces, **kwargs)
-
-    # MODULE COMMANDS
-    def module_load(self, path: str) -> Awaitable:
-        """
-        Loads the module from ``path``.
-        Raises ``ModuleError`` if a module is not found at ``path``.
-        """
-        return self.execute_command("MODULE LOAD", path)
-
-    def module_unload(self, name: str) -> Awaitable:
-        """
-        Unloads the module ``name``.
-        Raises ``ModuleError`` if ``name`` is not in loaded modules.
-        """
-        return self.execute_command("MODULE UNLOAD", name)
-
-    def module_list(self) -> Awaitable:
-        """
-        Returns a list of dictionaries containing the name and version of
-        all loaded modules.
-        """
-        return self.execute_command("MODULE LIST")
-
-
-StrictRedis = Redis
-
-
-class MonitorCommandInfo(TypedDict):
-    time: float
-    db: int
-    client_address: str
-    client_port: str
-    client_type: str
-    command: str
-
-
-class Monitor:
-    """
-    Monitor is useful for handling the MONITOR command to the redis server.
-    next_command() method returns one command from monitor
-    listen() method yields commands from monitor.
-    """
-
-    monitor_re = re.compile(r"\[(\d+) (.*)\] (.*)")
-    command_re = re.compile(r'"(.*?)(?<!\\)"')
-
-    def __init__(self, connection_pool: ConnectionPool):
-        self.connection_pool = connection_pool
-        self.connection: Optional[Connection] = None
-
-    async def connect(self):
-        if self.connection is None:
-            self.connection = await self.connection_pool.get_connection("MONITOR")
-
-    async def __aenter__(self):
-        await self.connect()
-        self.connection = cast(Connection, self.connection)  # Connected above.
-        await self.connection.send_command("MONITOR")
-        # check that monitor returns 'OK', but don't return it to user
-        response = await self.connection.read_response()
-        if not bool_ok(response):
-            raise RedisError(f"MONITOR failed: {response}")
-        return self
-
-    async def __aexit__(self, *args):
-        assert self.connection is not None
-        await self.connection.disconnect()
-        await self.connection_pool.release(self.connection)
-
-    async def next_command(self) -> MonitorCommandInfo:
-        """Parse the response from a monitor command"""
-        if self.connection is None:
-            raise RedisError("Connection already closed.")
-        await self.connect()
-        response = await self.connection.read_response()
-        if isinstance(response, bytes):
-            response = self.connection.encoder.decode(response, force=True)
-        command_time, command_data = response.split(" ", 1)
-        m = self.monitor_re.match(command_data)
-        if m is None:
-            raise RedisError("Invalid command received.")
-        db_id, client_info, command = m.groups()
-        command = " ".join(self.command_re.findall(command))
-        # Redis escapes double quotes because each piece of the command
-        # string is surrounded by double quotes. We don't have that
-        # requirement so remove the escaping and leave the quote.
-        command = command.replace('\\"', '"')
-
-        if client_info == "lua":
-            client_address = "lua"
-            client_port = ""
-            client_type = "lua"
-        elif client_info.startswith("unix"):
-            client_address = "unix"
-            client_port = client_info[5:]
-            client_type = "unix"
-        else:
-            # use rsplit as ipv6 addresses contain colons
-            client_address, client_port = client_info.rsplit(":", 1)
-            client_type = "tcp"
-        return {
-            "time": float(command_time),
-            "db": int(db_id),
-            "client_address": client_address,
-            "client_port": client_port,
-            "client_type": client_type,
-            "command": command,
-        }
-
-    async def listen(self) -> AsyncIterator[MonitorCommandInfo]:
-        """Listen for commands coming to the server."""
-        while True:
-            yield await self.next_command()
-
-
-class PubSub:
-    """
-    PubSub provides publish, subscribe and listen support to Redis channels.
-
-    After subscribing to one or more channels, the listen() method will block
-    until a message arrives on one of the subscribed channels. That message
-    will be returned and it's safe to start listening again.
-    """
-
-    PUBLISH_MESSAGE_TYPES = ("message", "pmessage")
-    UNSUBSCRIBE_MESSAGE_TYPES = ("unsubscribe", "punsubscribe")
-    HEALTH_CHECK_MESSAGE = "aioredis-py-health-check"
-
-    def __init__(
-        self,
-        connection_pool: ConnectionPool,
-        shard_hint: Optional[str] = None,
-        ignore_subscribe_messages: bool = False,
-    ):
-        self.connection_pool = connection_pool
-        self.shard_hint = shard_hint
-        self.ignore_subscribe_messages = ignore_subscribe_messages
-        self.connection: Optional[Connection] = None
-        # we need to know the encoding options for this connection in order
-        # to lookup channel and pattern names for callback handlers.
-        self.encoder = self.connection_pool.get_encoder()
-        if self.encoder.decode_responses:
-            self.health_check_response: Iterable[Union[str, bytes]] = [
-                "pong",
-                self.HEALTH_CHECK_MESSAGE,
-            ]
-        else:
-            self.health_check_response = [
-                b"pong",
-                self.encoder.encode(self.HEALTH_CHECK_MESSAGE),
-            ]
-        self.channels: Dict[ChannelT, PubSubHandler] = {}
-        self.pending_unsubscribe_channels: Set[ChannelT] = set()
-        self.patterns: Dict[ChannelT, PubSubHandler] = {}
-        self.pending_unsubscribe_patterns: Set[ChannelT] = set()
-        self._lock = asyncio.Lock()
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, exc_type, exc_value, traceback):
-        await self.reset()
-
-    def __del__(self):
-        if self.connection:
-            self.connection.clear_connect_callbacks()
-
-    async def reset(self):
-        async with self._lock:
-            if self.connection:
-                await self.connection.disconnect()
-                self.connection.clear_connect_callbacks()
-                await self.connection_pool.release(self.connection)
-                self.connection = None
-            self.channels = {}
-            self.pending_unsubscribe_channels = set()
-            self.patterns = {}
-            self.pending_unsubscribe_patterns = set()
-
-    def close(self) -> Awaitable[NoReturn]:
-        return self.reset()
-
-    async def on_connect(self, connection: Connection):
-        """Re-subscribe to any channels and patterns previously subscribed to"""
-        # NOTE: for python3, we can't pass bytestrings as keyword arguments
-        # so we need to decode channel/pattern names back to unicode strings
-        # before passing them to [p]subscribe.
-        self.pending_unsubscribe_channels.clear()
-        self.pending_unsubscribe_patterns.clear()
-        if self.channels:
-            channels = {}
-            for k, v in self.channels.items():
-                channels[self.encoder.decode(k, force=True)] = v
-            await self.subscribe(**channels)
-        if self.patterns:
-            patterns = {}
-            for k, v in self.patterns.items():
-                patterns[self.encoder.decode(k, force=True)] = v
-            await self.psubscribe(**patterns)
-
-    @property
-    def subscribed(self):
-        """Indicates if there are subscriptions to any channels or patterns"""
-        return bool(self.channels or self.patterns)
-
-    async def execute_command(self, *args: EncodableT):
-        """Execute a publish/subscribe command"""
-
-        # NOTE: don't parse the response in this function -- it could pull a
-        # legitimate message off the stack if the connection is already
-        # subscribed to one or more channels
-
-        if self.connection is None:
-            self.connection = await self.connection_pool.get_connection(
-                "pubsub", self.shard_hint
-            )
-            # register a callback that re-subscribes to any channels we
-            # were listening to when we were disconnected
-            self.connection.register_connect_callback(self.on_connect)
-        connection = self.connection
-        kwargs = {"check_health": not self.subscribed}
-        await self._execute(connection, connection.send_command, *args, **kwargs)
-
-    async def _execute(self, connection, command, *args, **kwargs):
-        try:
-            return await command(*args, **kwargs)
-        except (ConnectionError, TimeoutError) as e:
-            await connection.disconnect()
-            if not (connection.retry_on_timeout and isinstance(e, TimeoutError)):
-                raise
-            # Connect manually here. If the Redis server is down, this will
-            # fail and raise a ConnectionError as desired.
-            await connection.connect()
-            # the ``on_connect`` callback should haven been called by the
-            # connection to resubscribe us to any channels and patterns we were
-            # previously listening to
-            return await command(*args, **kwargs)
-
-    async def parse_response(self, block: bool = True, timeout: float = 0):
-        """Parse the response from a publish/subscribe command"""
-        conn = self.connection
-        if conn is None:
-            raise RuntimeError(
-                "pubsub connection not set: "
-                "did you forget to call subscribe() or psubscribe()?"
-            )
-
-        await self.check_health()
-
-        if not block and not await conn.can_read(timeout=timeout):
-            return None
-        response = await self._execute(conn, conn.read_response)
-
-        if conn.health_check_interval and response == self.health_check_response:
-            # ignore the health check message as user might not expect it
-            return None
-        return response
-
-    async def check_health(self):
-        conn = self.connection
-        if conn is None:
-            raise RuntimeError(
-                "pubsub connection not set: "
-                "did you forget to call subscribe() or psubscribe()?"
-            )
-
-        if (
-            conn.health_check_interval
-            and asyncio.get_event_loop().time() > conn.next_health_check
-        ):
-            await conn.send_command(
-                "PING", self.HEALTH_CHECK_MESSAGE, check_health=False
-            )
-
-    def _normalize_keys(self, data: _NormalizeKeysT) -> _NormalizeKeysT:
-        """
-        normalize channel/pattern names to be either bytes or strings
-        based on whether responses are automatically decoded. this saves us
-        from coercing the value for each message coming in.
-        """
-        encode = self.encoder.encode
-        decode = self.encoder.decode
-        return {decode(encode(k)): v for k, v in data.items()}  # type: ignore[return-value]
-
-    async def psubscribe(self, *args: ChannelT, **kwargs: PubSubHandler):
-        """
-        Subscribe to channel patterns. Patterns supplied as keyword arguments
-        expect a pattern name as the key and a callable as the value. A
-        pattern's callable will be invoked automatically when a message is
-        received on that pattern rather than producing a message via
-        ``listen()``.
-        """
-        parsed_args = list_or_args((args[0],), args[1:]) if args else args
-        new_patterns: Dict[ChannelT, PubSubHandler] = dict.fromkeys(parsed_args)
-        # Mypy bug: https://github.com/python/mypy/issues/10970
-        new_patterns.update(kwargs)  # type: ignore[arg-type]
-        ret_val = await self.execute_command("PSUBSCRIBE", *new_patterns.keys())
-        # update the patterns dict AFTER we send the command. we don't want to
-        # subscribe twice to these patterns, once for the command and again
-        # for the reconnection.
-        new_patterns = self._normalize_keys(new_patterns)
-        self.patterns.update(new_patterns)
-        self.pending_unsubscribe_patterns.difference_update(new_patterns)
-        return ret_val
-
-    def punsubscribe(self, *args: ChannelT) -> Awaitable:
-        """
-        Unsubscribe from the supplied patterns. If empty, unsubscribe from
-        all patterns.
-        """
-        patterns: Iterable[ChannelT]
-        if args:
-            parsed_args = list_or_args((args[0],), args[1:])
-            patterns = self._normalize_keys(dict.fromkeys(parsed_args)).keys()
-        else:
-            parsed_args = []
-            patterns = self.patterns
-        self.pending_unsubscribe_patterns.update(patterns)
-        return self.execute_command("PUNSUBSCRIBE", *parsed_args)
-
-    async def subscribe(self, *args: ChannelT, **kwargs: Callable):
-        """
-        Subscribe to channels. Channels supplied as keyword arguments expect
-        a channel name as the key and a callable as the value. A channel's
-        callable will be invoked automatically when a message is received on
-        that channel rather than producing a message via ``listen()`` or
-        ``get_message()``.
-        """
-        parsed_args = list_or_args((args[0],), args[1:]) if args else ()
-        new_channels = dict.fromkeys(parsed_args)
-        # Mypy bug: https://github.com/python/mypy/issues/10970
-        new_channels.update(kwargs)  # type: ignore[arg-type]
-        ret_val = await self.execute_command("SUBSCRIBE", *new_channels.keys())
-        # update the channels dict AFTER we send the command. we don't want to
-        # subscribe twice to these channels, once for the command and again
-        # for the reconnection.
-        new_channels = self._normalize_keys(new_channels)
-        self.channels.update(new_channels)
-        self.pending_unsubscribe_channels.difference_update(new_channels)
-        return ret_val
-
-    def unsubscribe(self, *args) -> Awaitable:
-        """
-        Unsubscribe from the supplied channels. If empty, unsubscribe from
-        all channels
-        """
-        if args:
-            parsed_args = list_or_args(args[0], args[1:])
-            channels = self._normalize_keys(dict.fromkeys(parsed_args))
-        else:
-            parsed_args = []
-            channels = self.channels
-        self.pending_unsubscribe_channels.update(channels)
-        return self.execute_command("UNSUBSCRIBE", *parsed_args)
-
-    async def listen(self) -> AsyncIterator:
-        """Listen for messages on channels this client has been subscribed to"""
-        while self.subscribed:
-            response = self.handle_message(await self.parse_response(block=True))
-            if response is not None:
-                yield response
-
-    async def get_message(
-        self, ignore_subscribe_messages: bool = False, timeout: float = 0.0
-    ):
-        """
-        Get the next message if one is available, otherwise None.
-
-        If timeout is specified, the system will wait for `timeout` seconds
-        before returning. Timeout should be specified as a floating point
-        number.
-        """
-        response = await self.parse_response(block=False, timeout=timeout)
-        if response:
-            return self.handle_message(response, ignore_subscribe_messages)
-        return None
-
-    def ping(self, message=None) -> Awaitable:
-        """
-        Ping the Redis server
-        """
-        message = "" if message is None else message
-        return self.execute_command("PING", message)
-
-    def handle_message(self, response, ignore_subscribe_messages=False):
-        """
-        Parses a pub/sub message. If the channel or pattern was subscribed to
-        with a message handler, the handler is invoked instead of a parsed
-        message being returned.
-        """
-        message_type = str_if_bytes(response[0])
-        if message_type == "pmessage":
-            message = {
-                "type": message_type,
-                "pattern": response[1],
-                "channel": response[2],
-                "data": response[3],
-            }
-        elif message_type == "pong":
-            message = {
-                "type": message_type,
-                "pattern": None,
-                "channel": None,
-                "data": response[1],
-            }
-        else:
-            message = {
-                "type": message_type,
-                "pattern": None,
-                "channel": response[1],
-                "data": response[2],
-            }
-
-        # if this is an unsubscribe message, remove it from memory
-        if message_type in self.UNSUBSCRIBE_MESSAGE_TYPES:
-            if message_type == "punsubscribe":
-                pattern = response[1]
-                if pattern in self.pending_unsubscribe_patterns:
-                    self.pending_unsubscribe_patterns.remove(pattern)
-                    self.patterns.pop(pattern, None)
-            else:
-                channel = response[1]
-                if channel in self.pending_unsubscribe_channels:
-                    self.pending_unsubscribe_channels.remove(channel)
-                    self.channels.pop(channel, None)
-
-        if message_type in self.PUBLISH_MESSAGE_TYPES:
-            # if there's a message handler, invoke it
-            if message_type == "pmessage":
-                handler = self.patterns.get(message["pattern"], None)
-            else:
-                handler = self.channels.get(message["channel"], None)
-            if handler:
-                handler(message)
-                return None
-        elif message_type != "pong":
-            # this is a subscribe/unsubscribe message. ignore if we don't
-            # want them
-            if ignore_subscribe_messages or self.ignore_subscribe_messages:
-                return None
-
-        return message
-
-    async def run(
-        self,
-        *,
-        exception_handler: Optional["PSWorkerThreadExcHandlerT"] = None,
-        poll_timeout: float = 1.0,
-    ) -> None:
-        """Process pub/sub messages using registered callbacks.
-
-        This is the equivalent of :py:meth:`redis.PubSub.run_in_thread` in
-        redis-py, but it is a coroutine. To launch it as a separate task, use
-        ``asyncio.create_task``:
-
-            >>> task = asyncio.create_task(pubsub.run())
-
-        To shut it down, use asyncio cancellation:
-
-            >>> task.cancel()
-            >>> await task
-        """
-        for channel, handler in self.channels.items():
-            if handler is None:
-                raise PubSubError(f"Channel: '{channel}' has no handler registered")
-        for pattern, handler in self.patterns.items():
-            if handler is None:
-                raise PubSubError(f"Pattern: '{pattern}' has no handler registered")
-
-        while True:
-            try:
-                await self.get_message(
-                    ignore_subscribe_messages=True, timeout=poll_timeout
-                )
-            except asyncio.CancelledError:
-                raise
-            except BaseException as e:
-                if exception_handler is None:
-                    raise
-                res = exception_handler(e, self)
-                if inspect.isawaitable(res):
-                    await res
-            # Ensure that other tasks on the event loop get a chance to run
-            # if we didn't have to block for I/O anywhere.
-            await asyncio.sleep(0)
-
-
-class PubsubWorkerExceptionHandler(Protocol):
-    def __call__(self, e: BaseException, pubsub: PubSub):
-        ...
-
-
-class AsyncPubsubWorkerExceptionHandler(Protocol):
-    async def __call__(self, e: BaseException, pubsub: PubSub):
-        ...
-
-
-PSWorkerThreadExcHandlerT = Union[
-    PubsubWorkerExceptionHandler, AsyncPubsubWorkerExceptionHandler
-]
-
-
-CommandT = Tuple[Tuple[Union[str, bytes], ...], Mapping[str, Any]]
-CommandStackT = List[CommandT]
-
-
-class Pipeline(Redis):  # lgtm [py/init-calls-subclass]
-    """
-    Pipelines provide a way to transmit multiple commands to the Redis server
-    in one transmission.  This is convenient for batch processing, such as
-    saving all the values in a list to Redis.
-
-    All commands executed within a pipeline are wrapped with MULTI and EXEC
-    calls. This guarantees all commands executed in the pipeline will be
-    executed atomically.
-
-    Any command raising an exception does *not* halt the execution of
-    subsequent commands in the pipeline. Instead, the exception is caught
-    and its instance is placed into the response list returned by execute().
-    Code iterating over the response list should be able to deal with an
-    instance of an exception as a potential value. In general, these will be
-    ResponseError exceptions, such as those raised when issuing a command
-    on a key of a different datatype.
-    """
-
-    UNWATCH_COMMANDS = {"DISCARD", "EXEC", "UNWATCH"}
-
-    def __init__(
-        self,
-        connection_pool: ConnectionPool,
-        response_callbacks: MutableMapping[Union[str, bytes], ResponseCallbackT],
-        transaction: bool,
-        shard_hint: Optional[str],
-    ):
-        self.connection_pool = connection_pool
-        self.connection = None
-        self.response_callbacks = response_callbacks
-        self.is_transaction = transaction
-        self.shard_hint = shard_hint
-        self.watching = False
-        self.command_stack: CommandStackT = []
-        self.scripts: Set[Script] = set()
-        self.explicit_transaction = False
-
-    async def __aenter__(self: _RedisT) -> _RedisT:
-        return self
-
-    async def __aexit__(self, exc_type, exc_value, traceback):
-        await self.reset()
-
-    def __await__(self):
-        return self._async_self().__await__()
-
-    _DEL_MESSAGE = "Unclosed Pipeline client"
-
-    def __len__(self):
-        return len(self.command_stack)
-
-    def __bool__(self):
-        """Pipeline instances should always evaluate to True"""
-        return True
-
-    async def _async_self(self):
-        return self
-
-    async def reset(self):
-        self.command_stack = []
-        self.scripts = set()
-        # make sure to reset the connection state in the event that we were
-        # watching something
-        if self.watching and self.connection:
-            try:
-                # call this manually since our unwatch or
-                # immediate_execute_command methods can call reset()
-                await self.connection.send_command("UNWATCH")
-                await self.connection.read_response()
-            except ConnectionError:
-                # disconnect will also remove any previous WATCHes
-                if self.connection:
-                    await self.connection.disconnect()
-        # clean up the other instance attributes
-        self.watching = False
-        self.explicit_transaction = False
-        # we can safely return the connection to the pool here since we're
-        # sure we're no longer WATCHing anything
-        if self.connection:
-            await self.connection_pool.release(self.connection)
-            self.connection = None
-
-    def multi(self):
-        """
-        Start a transactional block of the pipeline after WATCH commands
-        are issued. End the transactional block with `execute`.
-        """
-        if self.explicit_transaction:
-            raise RedisError("Cannot issue nested calls to MULTI")
-        if self.command_stack:
-            raise RedisError(
-                "Commands without an initial WATCH have already " "been issued"
-            )
-        self.explicit_transaction = True
-
-    def execute_command(
-        self, *args, **kwargs
-    ) -> Union["Pipeline", Awaitable["Pipeline"]]:
-        if (self.watching or args[0] == "WATCH") and not self.explicit_transaction:
-            return self.immediate_execute_command(*args, **kwargs)
-        return self.pipeline_execute_command(*args, **kwargs)
-
-    async def immediate_execute_command(self, *args, **options):
-        """
-        Execute a command immediately, but don't auto-retry on a
-        ConnectionError if we're already WATCHing a variable. Used when
-        issuing WATCH or subsequent commands retrieving their values but before
-        MULTI is called.
-        """
-        command_name = args[0]
-        conn = self.connection
-        # if this is the first call, we need a connection
-        if not conn:
-            conn = await self.connection_pool.get_connection(
-                command_name, self.shard_hint
-            )
-            self.connection = conn
-        conn = cast(Connection, conn)
-        try:
-            await conn.send_command(*args)
-            return await self.parse_response(conn, command_name, **options)
-        except (ConnectionError, TimeoutError) as e:
-            await conn.disconnect()
-            # if we were already watching a variable, the watch is no longer
-            # valid since this connection has died. raise a WatchError, which
-            # indicates the user should retry this transaction.
-            if self.watching:
-                await self.reset()
-                raise WatchError(
-                    "A ConnectionError occurred on while watching one or more keys"
-                ) from e
-            # if retry_on_timeout is not set, or the error is not
-            # a TimeoutError, raise it
-            if not (conn.retry_on_timeout and isinstance(e, TimeoutError)):
-                await self.reset()
-                raise
-
-            # retry_on_timeout is set, this is a TimeoutError and we are not
-            # already WATCHing any variables. retry the command.
-            try:
-                await conn.send_command(*args)
-                return self.parse_response(conn, command_name, **options)
-            except (ConnectionError, TimeoutError):
-                # a subsequent failure should simply be raised
-                await self.reset()
-                raise
-        except asyncio.CancelledError:
-            await conn.disconnect()
-            raise
-
-    def pipeline_execute_command(self, *args, **options):
-        """
-        Stage a command to be executed when execute() is next called
-
-        Returns the current Pipeline object back so commands can be
-        chained together, such as:
-
-        pipe = pipe.set('foo', 'bar').incr('baz').decr('bang')
-
-        At some other point, you can then run: pipe.execute(),
-        which will execute all commands queued in the pipe.
-        """
-        self.command_stack.append((args, options))
-        return self
-
-    async def _execute_transaction(  # noqa: C901
-        self, connection: Connection, commands: CommandStackT, raise_on_error
-    ):
-        pre: CommandT = (("MULTI",), {})
-        post: CommandT = (("EXEC",), {})
-        cmds = (pre, *commands, post)
-        all_cmds = connection.pack_commands(
-            args for args, options in cmds if EMPTY_RESPONSE not in options
-        )
-        await connection.send_packed_command(all_cmds)
-        errors = []
-
-        # parse off the response for MULTI
-        # NOTE: we need to handle ResponseErrors here and continue
-        # so that we read all the additional command messages from
-        # the socket
-        try:
-            await self.parse_response(connection, "_")
-        except ResponseError as err:
-            errors.append((0, err))
-
-        # and all the other commands
-        for i, command in enumerate(commands):
-            if EMPTY_RESPONSE in command[1]:
-                errors.append((i, command[1][EMPTY_RESPONSE]))
-            else:
-                try:
-                    await self.parse_response(connection, "_")
-                except ResponseError as err:
-                    self.annotate_exception(err, i + 1, command[0])
-                    errors.append((i, err))
-
-        # parse the EXEC.
-        try:
-            response = await self.parse_response(connection, "_")
-        except ExecAbortError as err:
-            if errors:
-                raise errors[0][1] from err
-            raise
-
-        # EXEC clears any watched keys
-        self.watching = False
-
-        if response is None:
-            raise WatchError("Watched variable changed.") from None
-
-        # put any parse errors into the response
-        for i, e in errors:
-            response.insert(i, e)
-
-        if len(response) != len(commands):
-            if self.connection:
-                await self.connection.disconnect()
-            raise ResponseError(
-                "Wrong number of response items from pipeline execution"
-            ) from None
-
-        # find any errors in the response and raise if necessary
-        if raise_on_error:
-            self.raise_first_error(commands, response)
-
-        # We have to run response callbacks manually
-        data = []
-        for r, cmd in zip(response, commands):
-            if not isinstance(r, Exception):
-                args, options = cmd
-                command_name = args[0]
-                if command_name in self.response_callbacks:
-                    r = self.response_callbacks[command_name](r, **options)
-                    if inspect.isawaitable(r):
-                        r = await r
-            data.append(r)
-        return data
-
-    async def _execute_pipeline(
-        self, connection: Connection, commands: CommandStackT, raise_on_error: bool
-    ):
-        # build up all commands into a single request to increase network perf
-        all_cmds = connection.pack_commands([args for args, _ in commands])
-        await connection.send_packed_command(all_cmds)
-
-        response = []
-        for args, options in commands:
-            try:
-                response.append(
-                    await self.parse_response(connection, args[0], **options)
-                )
-            except ResponseError as e:
-                response.append(e)
-
-        if raise_on_error:
-            self.raise_first_error(commands, response)
-        return response
-
-    def raise_first_error(self, commands: CommandStackT, response: Iterable[Any]):
-        for i, r in enumerate(response):
-            if isinstance(r, ResponseError):
-                self.annotate_exception(r, i + 1, commands[i][0])
-                raise r
-
-    def annotate_exception(
-        self, exception: Exception, number: int, command: Iterable[object]
-    ) -> None:
-        cmd = " ".join(map(safe_str, command))
-        msg = f"Command # {number} ({cmd}) of pipeline caused error: {exception.args}"
-        exception.args = (msg,) + exception.args[1:]
-
-    def parse_response(
-        self, connection: Connection, command_name: Union[str, bytes], **options
-    ):
-        result = super().parse_response(connection, command_name, **options)
-        if command_name in self.UNWATCH_COMMANDS:
-            self.watching = False
-        elif command_name == "WATCH":
-            self.watching = True
-        return result
-
-    async def load_scripts(self):
-        # make sure all scripts that are about to be run on this pipeline exist
-        scripts = list(self.scripts)
-        immediate = self.immediate_execute_command
-        shas = [s.sha for s in scripts]
-        # we can't use the normal script_* methods because they would just
-        # get buffered in the pipeline.
-        exists = await immediate("SCRIPT EXISTS", *shas)
-        if not all(exists):
-            for s, exist in zip(scripts, exists):
-                if not exist:
-                    s.sha = await immediate("SCRIPT LOAD", s.script)
-
-    async def execute(self, raise_on_error: bool = True):
-        """Execute all the commands in the current pipeline"""
-        stack = self.command_stack
-        if not stack and not self.watching:
-            return []
-        if self.scripts:
-            await self.load_scripts()
-        if self.is_transaction or self.explicit_transaction:
-            execute = self._execute_transaction
-        else:
-            execute = self._execute_pipeline
-
-        conn = self.connection
-        if not conn:
-            conn = await self.connection_pool.get_connection("MULTI", self.shard_hint)
-            # assign to self.connection so reset() releases the connection
-            # back to the pool after we're done
-            self.connection = conn
-        conn = cast(Connection, conn)
-
-        try:
-            return await execute(conn, stack, raise_on_error)
-        except (ConnectionError, TimeoutError) as e:
-            await conn.disconnect()
-            # if we were watching a variable, the watch is no longer valid
-            # since this connection has died. raise a WatchError, which
-            # indicates the user should retry this transaction.
-            if self.watching:
-                raise WatchError(
-                    "A ConnectionError occurred on while " "watching one or more keys"
-                ) from e
-            # if retry_on_timeout is not set, or the error is not
-            # a TimeoutError, raise it
-            if not (conn.retry_on_timeout and isinstance(e, TimeoutError)):
-                raise
-            # retry a TimeoutError when retry_on_timeout is set
-            return await execute(conn, stack, raise_on_error)
-        finally:
-            await self.reset()
-
-    async def watch(self, *names: KeyT):
-        """Watches the values at keys ``names``"""
-        if self.explicit_transaction:
-            raise RedisError("Cannot issue a WATCH after a MULTI")
-        return await self.execute_command("WATCH", *names)
-
-    async def unwatch(self):
-        """Unwatches all previously specified keys"""
-        return self.watching and await self.execute_command("UNWATCH") or True
-
-
-class Script:
-    """An executable Lua script object returned by ``register_script``"""
-
-    def __init__(self, registered_client: Redis, script: ScriptTextT):
-        self.registered_client = registered_client
-        self.script = script
-        # Precalculate and store the SHA1 hex digest of the script.
-
-        if isinstance(script, str):
-            # We need the encoding from the client in order to generate an
-            # accurate byte representation of the script
-            encoder = registered_client.connection_pool.get_encoder()
-            script_bytes = encoder.encode(script)
-        else:
-            script_bytes = script
-        self.sha = hashlib.sha1(script_bytes).hexdigest()
-
-    async def __call__(
-        self,
-        keys: Optional[Sequence[KeyT]] = None,
-        args: Optional[Iterable[EncodableT]] = None,
-        client: Optional[Redis] = None,
-    ):
-        """Execute the script, passing any required ``args``"""
-        keys = keys or []
-        args = args or []
-        if client is None:
-            client = self.registered_client
-        args = tuple(keys) + tuple(args)
-        # make sure the Redis server knows about the script
-        if isinstance(client, Pipeline):
-            # Make sure the pipeline can register the script before executing.
-            client.scripts.add(self)
-            return client.evalsha(self.sha, len(keys), *args)
-        try:
-            return await client.evalsha(self.sha, len(keys), *args)
-        except NoScriptError:
-            # Maybe the client is pointed to a differnet server than the client
-            # that created this instance?
-            # Overwrite the sha just in case there was a discrepancy.
-            self.sha = await client.script_load(self.script)
-            return await client.evalsha(self.sha, len(keys), *args)
-
-
-class BitFieldOperation:
-    """
-    Command builder for BITFIELD commands.
-    """
-
-    def __init__(
-        self, client: Redis, key: KeyT, default_overflow: Optional[str] = None
-    ):
-        self.client = client
-        self.key = key
-        self._default_overflow = default_overflow
-        self.operations: List[Tuple[EncodableT, ...]] = []
-        self._last_overflow = "WRAP"
-        self.reset()
-
-    def reset(self):
-        """
-        Reset the state of the instance to when it was constructed
-        """
-        self.operations = []
-        self._last_overflow = "WRAP"
-        self.overflow(self._default_overflow or self._last_overflow)
-
-    def overflow(self, overflow: str):
-        """
-        Update the overflow algorithm of successive INCRBY operations
-        :param overflow: Overflow algorithm, one of WRAP, SAT, FAIL. See the
-            Redis docs for descriptions of these algorithmsself.
-        :returns: a :py:class:`BitFieldOperation` instance.
-        """
-        overflow = overflow.upper()
-        if overflow != self._last_overflow:
-            self._last_overflow = overflow
-            self.operations.append(("OVERFLOW", overflow))
-        return self
-
-    def incrby(
-        self,
-        fmt: str,
-        offset: BitfieldOffsetT,
-        increment: int,
-        overflow: Optional[str] = None,
-    ):
-        """
-        Increment a bitfield by a given amount.
-        :param fmt: format-string for the bitfield being updated, e.g. 'u8'
-            for an unsigned 8-bit integer.
-        :param offset: offset (in number of bits). If prefixed with a
-            '#', this is an offset multiplier, e.g. given the arguments
-            fmt='u8', offset='#2', the offset will be 16.
-        :param int increment: value to increment the bitfield by.
-        :param str overflow: overflow algorithm. Defaults to WRAP, but other
-            acceptable values are SAT and FAIL. See the Redis docs for
-            descriptions of these algorithms.
-        :returns: a :py:class:`BitFieldOperation` instance.
-        """
-        if overflow is not None:
-            self.overflow(overflow)
-
-        self.operations.append(("INCRBY", fmt, offset, increment))
-        return self
-
-    def get(self, fmt: str, offset: BitfieldOffsetT):
-        """
-        Get the value of a given bitfield.
-        :param fmt: format-string for the bitfield being read, e.g. 'u8' for
-            an unsigned 8-bit integer.
-        :param offset: offset (in number of bits). If prefixed with a
-            '#', this is an offset multiplier, e.g. given the arguments
-            fmt='u8', offset='#2', the offset will be 16.
-        :returns: a :py:class:`BitFieldOperation` instance.
-        """
-        self.operations.append(("GET", fmt, offset))
-        return self
-
-    def set(self, fmt: str, offset: BitfieldOffsetT, value: int):
-        """
-        Set the value of a given bitfield.
-        :param fmt: format-string for the bitfield being read, e.g. 'u8' for
-            an unsigned 8-bit integer.
-        :param offset: offset (in number of bits). If prefixed with a
-            '#', this is an offset multiplier, e.g. given the arguments
-            fmt='u8', offset='#2', the offset will be 16.
-        :param int value: value to set at the given position.
-        :returns: a :py:class:`BitFieldOperation` instance.
-        """
-        self.operations.append(("SET", fmt, offset, value))
-        return self
-
-    @property
-    def command(self):
-        cmd: List[EncodableT] = ["BITFIELD", self.key]
-        for ops in self.operations:
-            cmd.extend(ops)
-        return cmd
-
-    def execute(self):
-        """
-        Execute the operation(s) in a single BITFIELD command. The return value
-        is a list of values corresponding to each operation. If the client
-        used to create this instance was a pipeline, the list of values
-        will be present within the pipeline's execute.
-        """
-        command = self.command
-        self.reset()
-        return self.client.execute_command(*command)
+import asyncio
+import datetime
+import hashlib
+import inspect
+import re
+import time as mod_time
+import warnings
+from typing import (
+    AbstractSet,
+    Any,
+    AsyncIterator,
+    Awaitable,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Mapping,
+    MutableMapping,
+    NoReturn,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    ValuesView,
+    cast,
+)
+
+from aioredis.compat import Protocol, TypedDict
+from aioredis.connection import (
+    Connection,
+    ConnectionPool,
+    EncodableT,
+    SSLConnection,
+    UnixDomainSocketConnection,
+)
+from aioredis.exceptions import (
+    ConnectionError,
+    DataError,
+    ExecAbortError,
+    ModuleError,
+    NoScriptError,
+    PubSubError,
+    RedisError,
+    ResponseError,
+    TimeoutError,
+    WatchError,
+)
+from aioredis.lock import Lock
+from aioredis.utils import safe_str, str_if_bytes
+
+AbsExpiryT = Union[int, datetime.datetime]
+ExpiryT = Union[int, datetime.timedelta]
+ZScoreBoundT = Union[float, str]  # str allows for the [ or ( prefix
+BitfieldOffsetT = Union[int, str]  # str allows for #x syntax
+_StringLikeT = Union[bytes, str, memoryview]
+KeyT = _StringLikeT  # Main redis key space
+PatternT = _StringLikeT  # Patterns matched against keys, fields etc
+FieldT = EncodableT  # Fields within hash tables, streams and geo commands
+KeysT = Union[KeyT, Sequence[KeyT]]
+ChannelT = _StringLikeT
+GroupT = _StringLikeT  # Consumer group
+ConsumerT = _StringLikeT  # Consumer name
+StreamIdT = Union[int, _StringLikeT]
+ScriptTextT = _StringLikeT
+TimeoutSecT = Union[int, float, _StringLikeT]
+# Mapping is not covariant in the key type, which prevents
+# Mapping[_StringLikeT, X from accepting arguments of type Dict[str, X]. Using
+# a TypeVar instead of a Union allows mappings with any of the permitted types
+# to be passed. Care is needed if there is more than one such mapping in a
+# type signature because they will all be required to be the same key type.
+AnyKeyT = TypeVar("AnyKeyT", bytes, str, memoryview)
+AnyFieldT = TypeVar("AnyFieldT", bytes, str, memoryview)
+AnyChannelT = ChannelT
+PubSubHandler = Callable[[Dict[str, str]], None]
+
+SYM_EMPTY = b""
+EMPTY_RESPONSE = "EMPTY_RESPONSE"
+
+_KeyT = TypeVar("_KeyT", bound=KeyT)
+_ArgT = TypeVar("_ArgT", KeyT, EncodableT)
+_RedisT = TypeVar("_RedisT", bound="Redis")
+_NormalizeKeysT = TypeVar("_NormalizeKeysT", bound=Mapping[ChannelT, object])
+
+
+def list_or_args(
+    keys: Union[_KeyT, Iterable[_KeyT]], args: Optional[Iterable[_ArgT]]
+) -> List[Union[_KeyT, _ArgT]]:
+    # returns a single new list combining keys and args
+    key_list: List[Union[_KeyT, _ArgT]]
+    try:
+        iter(keys)  # type: ignore[arg-type]
+        keys = cast(Iterable[_KeyT], keys)
+        # a string or bytes instance can be iterated, but indicates
+        # keys wasn't passed as a list
+        if isinstance(keys, (bytes, str)):
+            key_list = [keys]
+        else:
+            key_list = list(keys)
+    except TypeError:
+        key_list = [cast(memoryview, keys)]
+    if args:
+        key_list.extend(args)
+    return key_list
+
+
+def timestamp_to_datetime(response):
+    """Converts a unix timestamp to a Python datetime object"""
+    if not response:
+        return None
+    try:
+        response = int(response)
+    except ValueError:
+        return None
+    return datetime.datetime.fromtimestamp(response)
+
+
+def string_keys_to_dict(key_string, callback):
+    return dict.fromkeys(key_string.split(), callback)
+
+
+class CaseInsensitiveDict(dict):
+    """Case insensitive dict implementation. Assumes string keys only."""
+
+    def __init__(self, data):
+        for k, v in data.items():
+            self[k.upper()] = v
+
+    def __contains__(self, k):
+        return super().__contains__(k.upper())
+
+    def __delitem__(self, k):
+        super().__delitem__(k.upper())
+
+    def __getitem__(self, k):
+        return super().__getitem__(k.upper())
+
+    def get(self, k, default=None):
+        return super().get(k.upper(), default)
+
+    def __setitem__(self, k, v):
+        super().__setitem__(k.upper(), v)
+
+    def update(self, data):
+        data = CaseInsensitiveDict(data)
+        super().update(data)
+
+
+def parse_debug_object(response):
+    """Parse the results of Redis's DEBUG OBJECT command into a Python dict"""
+    # The 'type' of the object is the first item in the response, but isn't
+    # prefixed with a name
+    response = str_if_bytes(response)
+    response = "type:" + response
+    response = dict(kv.split(":") for kv in response.split())
+
+    # parse some expected int values from the string response
+    # note: this cmd isn't spec'd so these may not appear in all redis versions
+    int_fields = ("refcount", "serializedlength", "lru", "lru_seconds_idle")
+    for field in int_fields:
+        if field in response:
+            response[field] = int(response[field])
+
+    return response
+
+
+def parse_object(response, infotype):
+    """Parse the results of an OBJECT command"""
+    if infotype in ("idletime", "refcount"):
+        return int_or_none(response)
+    return response
+
+
+def parse_info(response):
+    """Parse the result of Redis's INFO command into a Python dict"""
+    info: Dict[str, Any] = {}
+    response = str_if_bytes(response)
+
+    def get_value(value):
+        if "," not in value or "=" not in value:
+            try:
+                if "." in value:
+                    return float(value)
+                else:
+                    return int(value)
+            except ValueError:
+                return value
+        else:
+            sub_dict = {}
+            for item in value.split(","):
+                k, v = item.rsplit("=", 1)
+                sub_dict[k] = get_value(v)
+            return sub_dict
+
+    for line in response.splitlines():
+        if line and not line.startswith("#"):
+            if line.find(":") != -1:
+                # Split, the info fields keys and values.
+                # Note that the value may contain ':'. but the 'host:'
+                # pseudo-command is the only case where the key contains ':'
+                key, value = line.split(":", 1)
+                if key == "cmdstat_host":
+                    key, value = line.rsplit(":", 1)
+
+                if key == "module":
+                    # Hardcode a list for key 'modules' since there could be
+                    # multiple lines that started with 'module'
+                    info.setdefault("modules", []).append(get_value(value))
+                else:
+                    info[key] = get_value(value)
+            else:
+                # if the line isn't splittable, append it to the "__raw__" key
+                info.setdefault("__raw__", []).append(line)
+
+    return info
+
+
+def parse_memory_stats(response, **kwargs):
+    """Parse the results of MEMORY STATS"""
+    stats = pairs_to_dict(response, decode_keys=True, decode_string_values=True)
+    for key, value in stats.items():
+        if key.startswith("db."):
+            stats[key] = pairs_to_dict(
+                value, decode_keys=True, decode_string_values=True
+            )
+    return stats
+
+
+SENTINEL_STATE_TYPES = {
+    "can-failover-its-master": int,
+    "config-epoch": int,
+    "down-after-milliseconds": int,
+    "failover-timeout": int,
+    "info-refresh": int,
+    "last-hello-message": int,
+    "last-ok-ping-reply": int,
+    "last-ping-reply": int,
+    "last-ping-sent": int,
+    "master-link-down-time": int,
+    "master-port": int,
+    "num-other-sentinels": int,
+    "num-slaves": int,
+    "o-down-time": int,
+    "pending-commands": int,
+    "parallel-syncs": int,
+    "port": int,
+    "quorum": int,
+    "role-reported-time": int,
+    "s-down-time": int,
+    "slave-priority": int,
+    "slave-repl-offset": int,
+    "voted-leader-epoch": int,
+}
+
+
+def parse_sentinel_state(item):
+    result = pairs_to_dict_typed(item, SENTINEL_STATE_TYPES)
+    flags = set(result["flags"].split(","))
+    for name, flag in (
+        ("is_master", "master"),
+        ("is_slave", "slave"),
+        ("is_sdown", "s_down"),
+        ("is_odown", "o_down"),
+        ("is_sentinel", "sentinel"),
+        ("is_disconnected", "disconnected"),
+        ("is_master_down", "master_down"),
+    ):
+        result[name] = flag in flags
+    return result
+
+
+def parse_sentinel_master(response):
+    return parse_sentinel_state(map(str_if_bytes, response))
+
+
+def parse_sentinel_masters(response):
+    result = {}
+    for item in response:
+        state = parse_sentinel_state(map(str_if_bytes, item))
+        result[state["name"]] = state
+    return result
+
+
+def parse_sentinel_slaves_and_sentinels(response):
+    return [parse_sentinel_state(map(str_if_bytes, item)) for item in response]
+
+
+def parse_sentinel_get_master(response):
+    return response and (response[0], int(response[1])) or None
+
+
+def pairs_to_dict(response, decode_keys=False, decode_string_values=False):
+    """Create a dict given a list of key/value pairs"""
+    if response is None:
+        return {}
+    if decode_keys or decode_string_values:
+        # the iter form is faster, but I don't know how to make that work
+        # with a str_if_bytes() map
+        keys = response[::2]
+        if decode_keys:
+            keys = map(str_if_bytes, keys)
+        values = response[1::2]
+        if decode_string_values:
+            values = map(str_if_bytes, values)
+        return dict(zip(keys, values))
+    else:
+        it = iter(response)
+        return dict(zip(it, it))
+
+
+def pairs_to_dict_typed(response, type_info):
+    it = iter(response)
+    result = {}
+    for key, value in zip(it, it):
+        if key in type_info:
+            try:
+                value = type_info[key](value)
+            except BaseException :
+                # if for some reason the value can't be coerced, just use
+                # the string value
+                pass
+        result[key] = value
+    return result
+
+
+def zset_score_pairs(response, **options):
+    """
+    If ``withscores`` is specified in the options, return the response as
+    a list of (value, score) pairs
+    """
+    if not response or not options.get("withscores"):
+        return response
+    score_cast_func = options.get("score_cast_func", float)
+    it = iter(response)
+    return list(zip(it, map(score_cast_func, it)))
+
+
+def sort_return_tuples(response, **options):
+    """
+    If ``groups`` is specified, return the response as a list of
+    n-element tuples with n being the value found in options['groups']
+    """
+    if not response or not options.get("groups"):
+        return response
+    n = options["groups"]
+    return list(zip(*(response[i::n] for i in range(n))))
+
+
+def int_or_none(response):
+    if response is None:
+        return None
+    return int(response)
+
+
+def parse_stream_list(response):
+    if response is None:
+        return None
+    data = []
+    for r in response:
+        if r is not None:
+            data.append((r[0], pairs_to_dict(r[1])))
+        else:
+            data.append((None, None))
+    return data
+
+
+def pairs_to_dict_with_str_keys(response):
+    return pairs_to_dict(response, decode_keys=True)
+
+
+def parse_list_of_dicts(response):
+    return list(map(pairs_to_dict_with_str_keys, response))
+
+
+def parse_xclaim(response, **options):
+    if options.get("parse_justid", False):
+        return response
+    return parse_stream_list(response)
+
+
+def parse_xinfo_stream(response):
+    data = pairs_to_dict(response, decode_keys=True)
+    first = data["first-entry"]
+    if first is not None:
+        data["first-entry"] = (first[0], pairs_to_dict(first[1]))
+    last = data["last-entry"]
+    if last is not None:
+        data["last-entry"] = (last[0], pairs_to_dict(last[1]))
+    return data
+
+
+def parse_xread(response):
+    if response is None:
+        return []
+    return [[r[0], parse_stream_list(r[1])] for r in response]
+
+
+def parse_xpending(response, **options):
+    if options.get("parse_detail", False):
+        return parse_xpending_range(response)
+    consumers = [{"name": n, "pending": int(p)} for n, p in response[3] or []]
+    return {
+        "pending": response[0],
+        "min": response[1],
+        "max": response[2],
+        "consumers": consumers,
+    }
+
+
+def parse_xpending_range(response):
+    k = ("message_id", "consumer", "time_since_delivered", "times_delivered")
+    return [dict(zip(k, r)) for r in response]
+
+
+def float_or_none(response):
+    if response is None:
+        return None
+    return float(response)
+
+
+def bool_ok(response):
+    return str_if_bytes(response) == "OK"
+
+
+def parse_zadd(response, **options):
+    if response is None:
+        return None
+    if options.get("as_score"):
+        return float(response)
+    return int(response)
+
+
+def parse_client_list(response, **options):
+    clients = []
+    for c in str_if_bytes(response).splitlines():
+        # Values might contain '='
+        clients.append(dict(pair.split("=", 1) for pair in c.split(" ")))
+    return clients
+
+
+def parse_config_get(response, **options):
+    response = [str_if_bytes(i) if i is not None else None for i in response]
+    return response and pairs_to_dict(response) or {}
+
+
+def parse_scan(response, **options):
+    cursor, r = response
+    return int(cursor), r
+
+
+def parse_hscan(response, **options):
+    cursor, r = response
+    return int(cursor), r and pairs_to_dict(r) or {}
+
+
+def parse_zscan(response, **options):
+    score_cast_func = options.get("score_cast_func", float)
+    cursor, r = response
+    it = iter(r)
+    return int(cursor), list(zip(it, map(score_cast_func, it)))
+
+
+def parse_slowlog_get(response, **options):
+    space: Union[str, bytes] = " " if options.get("decode_responses", False) else b" "
+    return [
+        {
+            "id": item[0],
+            "start_time": int(item[1]),
+            "duration": int(item[2]),
+            # Redis Enterprise injects another entry at index [3], which has
+            # the complexity info (i.e. the value N in case the command has
+            # an O(N) complexity) instead of the command.
+            "command": (
+                space.join(item[3])
+                if isinstance(item[3], list)
+                else space.join(item[4])
+            ),
+        }
+        for item in response
+    ]
+
+
+def parse_cluster_info(response, **options):
+    response = str_if_bytes(response)
+    return dict(line.split(":") for line in response.splitlines() if line)
+
+
+def _parse_node_line(line):
+    line_items = line.split(" ")
+    node_id, addr, flags, master_id, ping, pong, epoch, connected = line.split(" ")[:8]
+    slots = [sl.split("-") for sl in line_items[8:]]
+    node_dict = {
+        "node_id": node_id,
+        "flags": flags,
+        "master_id": master_id,
+        "last_ping_sent": ping,
+        "last_pong_rcvd": pong,
+        "epoch": epoch,
+        "slots": slots,
+        "connected": True if connected == "connected" else False,
+    }
+    return addr, node_dict
+
+
+def parse_cluster_nodes(response, **options):
+    raw_lines = str_if_bytes(response).splitlines()
+    return dict(_parse_node_line(line) for line in raw_lines)
+
+
+def parse_georadius_generic(response, **options):
+    if options["store"] or options["store_dist"]:
+        # `store` and `store_diff` cant be combined
+        # with other command arguments.
+        return response
+
+    if type(response) != list:
+        response_list = [response]
+    else:
+        response_list = response
+
+    if not options["withdist"] and not options["withcoord"] and not options["withhash"]:
+        # just a bunch of places
+        return response_list
+
+    cast: Dict[str, Callable] = {
+        "withdist": float,
+        "withcoord": lambda ll: (float(ll[0]), float(ll[1])),
+        "withhash": int,
+    }
+
+    # zip all output results with each casting functino to get
+    # the properly native Python value.
+    f = [lambda x: x]
+    f += [cast[o] for o in ["withdist", "withhash", "withcoord"] if options[o]]
+    return [list(map(lambda fv: fv[0](fv[1]), zip(f, r))) for r in response_list]
+
+
+def parse_pubsub_numsub(response, **options):
+    return list(zip(response[0::2], response[1::2]))
+
+
+def parse_client_kill(response, **options):
+    if isinstance(response, int):
+        return response
+    return str_if_bytes(response) == "OK"
+
+
+def parse_acl_getuser(response, **options):
+    if response is None:
+        return None
+    data = pairs_to_dict(response, decode_keys=True)
+
+    # convert everything but user-defined data in 'keys' to native strings
+    data["flags"] = list(map(str_if_bytes, data["flags"]))
+    data["passwords"] = list(map(str_if_bytes, data["passwords"]))
+    data["commands"] = str_if_bytes(data["commands"])
+
+    # split 'commands' into separate 'categories' and 'commands' lists
+    commands, categories = [], []
+    for command in data["commands"].split(" "):
+        if "@" in command:
+            categories.append(command)
+        else:
+            commands.append(command)
+
+    data["commands"] = commands
+    data["categories"] = categories
+    data["enabled"] = "on" in data["flags"]
+    return data
+
+
+def parse_acl_log(response, **options):
+    if response is None:
+        return None
+    if isinstance(response, list):
+        data = []
+        for log in response:
+            log_data = pairs_to_dict(log, True, True)
+            client_info = log_data.get("client-info", "")
+            log_data["client-info"] = parse_client_info(client_info)
+
+            # float() is lossy comparing to the "double" in C
+            log_data["age-seconds"] = float(log_data["age-seconds"])
+            data.append(log_data)
+    else:
+        data = bool_ok(response)
+    return data
+
+
+def parse_client_info(value):
+    """
+    Parsing client-info in ACL Log in following format.
+    "key1=value1 key2=value2 key3=value3"
+    """
+    client_info = {}
+    infos = value.split(" ")
+    for info in infos:
+        key, value = info.split("=")
+        client_info[key] = value
+
+    # Those fields are definded as int in networking.c
+    for int_key in {
+        "id",
+        "age",
+        "idle",
+        "db",
+        "sub",
+        "psub",
+        "multi",
+        "qbuf",
+        "qbuf-free",
+        "obl",
+        "oll",
+        "omem",
+    }:
+        client_info[int_key] = int(client_info[int_key])
+    return client_info
+
+
+def parse_module_result(response):
+    if isinstance(response, ModuleError):
+        raise response
+    return True
+
+
+class ResponseCallbackProtocol(Protocol):
+    def __call__(self, response: Any, **kwargs):
+        ...
+
+
+class AsyncResponseCallbackProtocol(Protocol):
+    async def __call__(self, response: Any, **kwargs):
+        ...
+
+
+ResponseCallbackT = Union[ResponseCallbackProtocol, AsyncResponseCallbackProtocol]
+
+
+_R = TypeVar("_R")
+
+
+class Redis:
+    """
+    Implementation of the Redis protocol.
+
+    This abstract class provides a Python interface to all Redis commands
+    and an implementation of the Redis protocol.
+
+    Connection and Pipeline derive from this, implementing how
+    the commands are sent and received to the Redis server
+    """
+
+    RESPONSE_CALLBACKS = {
+        **string_keys_to_dict(
+            "AUTH EXPIRE EXPIREAT HEXISTS HMSET MOVE MSETNX PERSIST "
+            "PSETEX RENAMENX SISMEMBER SMOVE SETEX SETNX",
+            bool,
+        ),
+        **string_keys_to_dict(
+            "BITCOUNT BITPOS DECRBY DEL EXISTS GEOADD GETBIT HDEL HLEN "
+            "HSTRLEN INCRBY LINSERT LLEN LPUSHX PFADD PFCOUNT RPUSHX SADD "
+            "SCARD SDIFFSTORE SETBIT SETRANGE SINTERSTORE SREM STRLEN "
+            "SUNIONSTORE UNLINK XACK XDEL XLEN XTRIM ZCARD ZLEXCOUNT ZREM "
+            "ZREMRANGEBYLEX ZREMRANGEBYRANK ZREMRANGEBYSCORE",
+            int,
+        ),
+        **string_keys_to_dict("INCRBYFLOAT HINCRBYFLOAT", float),
+        **string_keys_to_dict(
+            # these return OK, or int if redis-server is >=1.3.4
+            "LPUSH RPUSH",
+            lambda r: isinstance(r, int) and r or str_if_bytes(r) == "OK",
+        ),
+        **string_keys_to_dict("SORT", sort_return_tuples),
+        **string_keys_to_dict("ZSCORE ZINCRBY GEODIST", float_or_none),
+        **string_keys_to_dict(
+            "FLUSHALL FLUSHDB LSET LTRIM MSET PFMERGE READONLY READWRITE "
+            "RENAME SAVE SELECT SHUTDOWN SLAVEOF SWAPDB WATCH UNWATCH ",
+            bool_ok,
+        ),
+        **string_keys_to_dict("BLPOP BRPOP", lambda r: r and tuple(r) or None),
+        **string_keys_to_dict(
+            "SDIFF SINTER SMEMBERS SUNION", lambda r: r and set(r) or set()
+        ),
+        **string_keys_to_dict(
+            "ZPOPMAX ZPOPMIN ZRANGE ZRANGEBYSCORE ZREVRANGE ZREVRANGEBYSCORE",
+            zset_score_pairs,
+        ),
+        **string_keys_to_dict(
+            "BZPOPMIN BZPOPMAX", lambda r: r and (r[0], r[1], float(r[2])) or None
+        ),
+        **string_keys_to_dict("ZRANK ZREVRANK", int_or_none),
+        **string_keys_to_dict("XREVRANGE XRANGE", parse_stream_list),
+        **string_keys_to_dict("XREAD XREADGROUP", parse_xread),
+        **string_keys_to_dict("BGREWRITEAOF BGSAVE", lambda r: True),
+        "ACL CAT": lambda r: list(map(str_if_bytes, r)),
+        "ACL DELUSER": int,
+        "ACL GENPASS": str_if_bytes,
+        "ACL GETUSER": parse_acl_getuser,
+        "ACL LIST": lambda r: list(map(str_if_bytes, r)),
+        "ACL LOAD": bool_ok,
+        "ACL LOG": parse_acl_log,
+        "ACL SAVE": bool_ok,
+        "ACL SETUSER": bool_ok,
+        "ACL USERS": lambda r: list(map(str_if_bytes, r)),
+        "ACL WHOAMI": str_if_bytes,
+        "CLIENT GETNAME": str_if_bytes,
+        "CLIENT ID": int,
+        "CLIENT KILL": parse_client_kill,
+        "CLIENT LIST": parse_client_list,
+        "CLIENT SETNAME": bool_ok,
+        "CLIENT UNBLOCK": lambda r: r and int(r) == 1 or False,
+        "CLIENT PAUSE": bool_ok,
+        "CLUSTER ADDSLOTS": bool_ok,
+        "CLUSTER COUNT-FAILURE-REPORTS": lambda x: int(x),
+        "CLUSTER COUNTKEYSINSLOT": lambda x: int(x),
+        "CLUSTER DELSLOTS": bool_ok,
+        "CLUSTER FAILOVER": bool_ok,
+        "CLUSTER FORGET": bool_ok,
+        "CLUSTER INFO": parse_cluster_info,
+        "CLUSTER KEYSLOT": lambda x: int(x),
+        "CLUSTER MEET": bool_ok,
+        "CLUSTER NODES": parse_cluster_nodes,
+        "CLUSTER REPLICATE": bool_ok,
+        "CLUSTER RESET": bool_ok,
+        "CLUSTER SAVECONFIG": bool_ok,
+        "CLUSTER SET-CONFIG-EPOCH": bool_ok,
+        "CLUSTER SETSLOT": bool_ok,
+        "CLUSTER SLAVES": parse_cluster_nodes,
+        "CONFIG GET": parse_config_get,
+        "CONFIG RESETSTAT": bool_ok,
+        "CONFIG SET": bool_ok,
+        "DEBUG OBJECT": parse_debug_object,
+        "GEOHASH": lambda r: list(map(str_if_bytes, r)),
+        "GEOPOS": lambda r: list(
+            map(lambda ll: (float(ll[0]), float(ll[1])) if ll is not None else None, r)
+        ),
+        "GEORADIUS": parse_georadius_generic,
+        "GEORADIUSBYMEMBER": parse_georadius_generic,
+        "HGETALL": lambda r: r and pairs_to_dict(r) or {},
+        "HSCAN": parse_hscan,
+        "INFO": parse_info,
+        "LASTSAVE": timestamp_to_datetime,
+        "MEMORY PURGE": bool_ok,
+        "MEMORY STATS": parse_memory_stats,
+        "MEMORY USAGE": int_or_none,
+        "MODULE LOAD": parse_module_result,
+        "MODULE UNLOAD": parse_module_result,
+        "MODULE LIST": lambda r: [pairs_to_dict(m) for m in r],
+        "OBJECT": parse_object,
+        "PING": lambda r: str_if_bytes(r) == "PONG",
+        "PUBSUB NUMSUB": parse_pubsub_numsub,
+        "RANDOMKEY": lambda r: r and r or None,
+        "SCAN": parse_scan,
+        "SCRIPT EXISTS": lambda r: list(map(bool, r)),
+        "SCRIPT FLUSH": bool_ok,
+        "SCRIPT KILL": bool_ok,
+        "SCRIPT LOAD": str_if_bytes,
+        "SENTINEL GET-MASTER-ADDR-BY-NAME": parse_sentinel_get_master,
+        "SENTINEL MASTER": parse_sentinel_master,
+        "SENTINEL MASTERS": parse_sentinel_masters,
+        "SENTINEL MONITOR": bool_ok,
+        "SENTINEL REMOVE": bool_ok,
+        "SENTINEL SENTINELS": parse_sentinel_slaves_and_sentinels,
+        "SENTINEL SET": bool_ok,
+        "SENTINEL SLAVES": parse_sentinel_slaves_and_sentinels,
+        "SET": lambda r: r and str_if_bytes(r) == "OK",
+        "SLOWLOG GET": parse_slowlog_get,
+        "SLOWLOG LEN": int,
+        "SLOWLOG RESET": bool_ok,
+        "SSCAN": parse_scan,
+        "TIME": lambda x: (int(x[0]), int(x[1])),
+        "XCLAIM": parse_xclaim,
+        "XGROUP CREATE": bool_ok,
+        "XGROUP DELCONSUMER": int,
+        "XGROUP DESTROY": bool,
+        "XGROUP SETID": bool_ok,
+        "XINFO CONSUMERS": parse_list_of_dicts,
+        "XINFO GROUPS": parse_list_of_dicts,
+        "XINFO STREAM": parse_xinfo_stream,
+        "XPENDING": parse_xpending,
+        "ZADD": parse_zadd,
+        "ZSCAN": parse_zscan,
+    }
+
+    response_callbacks: MutableMapping[Union[str, bytes], ResponseCallbackT]
+
+    @classmethod
+    def from_url(cls, url: str, **kwargs):
+        """
+        Return a Redis client object configured from the given URL
+
+        For example::
+
+            redis://[[username]:[password]]@localhost:6379/0
+            rediss://[[username]:[password]]@localhost:6379/0
+            unix://[[username]:[password]]@/path/to/socket.sock?db=0
+
+        Three URL schemes are supported:
+
+        - `redis://` creates a TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/redis>
+        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
+        - ``unix://``: creates a Unix Domain Socket connection.
+
+        The username, password, hostname, path and all querystring values
+        are passed through urllib.parse.unquote in order to replace any
+        percent-encoded values with their corresponding characters.
+
+        There are several ways to specify a database number. The first value
+        found will be used:
+            1. A ``db`` querystring option, e.g. redis://localhost?db=0
+            2. If using the redis:// or rediss:// schemes, the path argument
+               of the url, e.g. redis://localhost/0
+            3. A ``db`` keyword argument to this function.
+
+        If none of these options are specified, the default db=0 is used.
+
+        All querystring options are cast to their appropriate Python types.
+        Boolean arguments can be specified with string values "True"/"False"
+        or "Yes"/"No". Values that cannot be properly cast cause a
+        ``ValueError`` to be raised. Once parsed, the querystring arguments
+        and keyword arguments are passed to the ``ConnectionPool``'s
+        class initializer. In the case of conflicting arguments, querystring
+        arguments always win.
+
+        """
+        connection_pool = ConnectionPool.from_url(url, **kwargs)
+        return cls(connection_pool=connection_pool)
+
+    def __init__(
+        self,
+        *,
+        host: str = "localhost",
+        port: int = 6379,
+        db: Union[str, int] = 0,
+        password: Optional[str] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        socket_keepalive: Optional[bool] = None,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        connection_pool: Optional[ConnectionPool] = None,
+        unix_socket_path: Optional[str] = None,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        retry_on_timeout: bool = False,
+        ssl: bool = False,
+        ssl_keyfile: Optional[str] = None,
+        ssl_certfile: Optional[str] = None,
+        ssl_cert_reqs: str = "required",
+        ssl_ca_certs: Optional[str] = None,
+        ssl_check_hostname: bool = False,
+        max_connections: Optional[int] = None,
+        single_connection_client: bool = False,
+        health_check_interval: int = 0,
+        client_name: Optional[str] = None,
+        username: Optional[str] = None,
+    ):
+        kwargs: Dict[str, Any]
+        if not connection_pool:
+            kwargs = {
+                "db": db,
+                "username": username,
+                "password": password,
+                "socket_timeout": socket_timeout,
+                "encoding": encoding,
+                "encoding_errors": encoding_errors,
+                "decode_responses": decode_responses,
+                "retry_on_timeout": retry_on_timeout,
+                "max_connections": max_connections,
+                "health_check_interval": health_check_interval,
+                "client_name": client_name,
+            }
+            # based on input, setup appropriate connection args
+            if unix_socket_path is not None:
+                kwargs.update(
+                    {
+                        "path": unix_socket_path,
+                        "connection_class": UnixDomainSocketConnection,
+                    }
+                )
+            else:
+                # TCP specific options
+                kwargs.update(
+                    {
+                        "host": host,
+                        "port": port,
+                        "socket_connect_timeout": socket_connect_timeout,
+                        "socket_keepalive": socket_keepalive,
+                        "socket_keepalive_options": socket_keepalive_options,
+                    }
+                )
+
+                if ssl:
+                    kwargs.update(
+                        {
+                            "connection_class": SSLConnection,
+                            "ssl_keyfile": ssl_keyfile,
+                            "ssl_certfile": ssl_certfile,
+                            "ssl_cert_reqs": ssl_cert_reqs,
+                            "ssl_ca_certs": ssl_ca_certs,
+                            "ssl_check_hostname": ssl_check_hostname,
+                        }
+                    )
+            connection_pool = ConnectionPool(**kwargs)
+        self.connection_pool = connection_pool
+        self.single_connection_client = single_connection_client
+        self.connection: Optional[Connection] = None
+
+        self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}<{self.connection_pool!r}>"
+
+    def __await__(self):
+        return self.initialize().__await__()
+
+    async def initialize(self: _RedisT) -> _RedisT:
+        if self.single_connection_client and self.connection is None:
+            self.connection = await self.connection_pool.get_connection("_")
+        return self
+
+    def set_response_callback(self, command: str, callback: ResponseCallbackT):
+        """Set a custom Response Callback"""
+        self.response_callbacks[command] = callback
+
+    def pipeline(
+        self, transaction: bool = True, shard_hint: Optional[str] = None
+    ) -> "Pipeline":
+        """
+        Return a new pipeline object that can queue multiple commands for
+        later execution. ``transaction`` indicates whether all commands
+        should be executed atomically. Apart from making a group of operations
+        atomic, pipelines are useful for reducing the back-and-forth overhead
+        between the client and server.
+        """
+        return Pipeline(
+            self.connection_pool, self.response_callbacks, transaction, shard_hint
+        )
+
+    async def transaction(
+        self,
+        func: Callable[["Pipeline"], Union[Any, Awaitable[Any]]],
+        *watches: KeyT,
+        shard_hint: Optional[str] = None,
+        value_from_callable: bool = False,
+        watch_delay: Optional[float] = None,
+    ):
+        """
+        Convenience method for executing the callable `func` as a transaction
+        while watching all keys specified in `watches`. The 'func' callable
+        should expect a single argument which is a Pipeline object.
+        """
+        pipe: Pipeline
+        async with self.pipeline(True, shard_hint) as pipe:
+            while True:
+                try:
+                    if watches:
+                        await pipe.watch(*watches)
+                    func_value = func(pipe)
+                    if inspect.isawaitable(func_value):
+                        func_value = await func_value
+                    exec_value = await pipe.execute()
+                    return func_value if value_from_callable else exec_value
+                except WatchError:
+                    if watch_delay is not None and watch_delay > 0:
+                        await asyncio.sleep(watch_delay)
+                    continue
+
+    def lock(
+        self,
+        name: KeyT,
+        timeout: Optional[float] = None,
+        sleep: float = 0.1,
+        blocking_timeout: Optional[float] = None,
+        lock_class: Optional[Type[Lock]] = None,
+        thread_local=True,
+    ) -> Lock:
+        """
+        Return a new Lock object using key ``name`` that mimics
+        the behavior of threading.Lock.
+
+        If specified, ``timeout`` indicates a maximum life for the lock.
+        By default, it will remain locked until release() is called.
+
+        ``sleep`` indicates the amount of time to sleep per loop iteration
+        when the lock is in blocking mode and another client is currently
+        holding the lock.
+
+        ``blocking_timeout`` indicates the maximum amount of time in seconds to
+        spend trying to acquire the lock. A value of ``None`` indicates
+        continue trying forever. ``blocking_timeout`` can be specified as a
+        float or integer, both representing the number of seconds to wait.
+
+        ``lock_class`` forces the specified lock implementation.
+
+        ``thread_local`` indicates whether the lock token is placed in
+        thread-local storage. By default, the token is placed in thread local
+        storage so that a thread only sees its token, not a token set by
+        another thread. Consider the following timeline:
+
+            time: 0, thread-1 acquires `my-lock`, with a timeout of 5 seconds.
+                     thread-1 sets the token to "abc"
+            time: 1, thread-2 blocks trying to acquire `my-lock` using the
+                     Lock instance.
+            time: 5, thread-1 has not yet completed. redis expires the lock
+                     key.
+            time: 5, thread-2 acquired `my-lock` now that it's available.
+                     thread-2 sets the token to "xyz"
+            time: 6, thread-1 finishes its work and calls release(). if the
+                     token is *not* stored in thread local storage, then
+                     thread-1 would see the token value as "xyz" and would be
+                     able to successfully release the thread-2's lock.
+
+        In some use cases it's necessary to disable thread local storage. For
+        example, if you have code where one thread acquires a lock and passes
+        that lock instance to a worker thread to release later. If thread
+        local storage isn't disabled in this case, the worker thread won't see
+        the token set by the thread that acquired the lock. Our assumption
+        is that these cases aren't common and as such default to using
+        thread local storage."""
+        if lock_class is None:
+            lock_class = Lock
+        return lock_class(
+            self,
+            name,
+            timeout=timeout,
+            sleep=sleep,
+            blocking_timeout=blocking_timeout,
+            thread_local=thread_local,
+        )
+
+    def pubsub(self, **kwargs) -> "PubSub":
+        """
+        Return a Publish/Subscribe object. With this object, you can
+        subscribe to channels and listen for messages that get published to
+        them.
+        """
+        return PubSub(self.connection_pool, **kwargs)
+
+    def monitor(self) -> "Monitor":
+        return Monitor(self.connection_pool)
+
+    def client(self) -> "Redis":
+        return self.__class__(
+            connection_pool=self.connection_pool, single_connection_client=True
+        )
+
+    async def __aenter__(self: _RedisT) -> _RedisT:
+        return await self.initialize()
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.close()
+
+    _DEL_MESSAGE = "Unclosed Redis client"
+
+    def __del__(self, _warnings: Any = warnings) -> None:
+        if self.connection is not None:
+            _warnings.warn(
+                f"Unclosed client session {self!r}",
+                ResourceWarning,
+                source=self,
+            )
+            context = {"client": self, "message": self._DEL_MESSAGE}
+            asyncio.get_event_loop().call_exception_handler(context)
+
+    async def close(self):
+        conn = self.connection
+        if conn:
+            self.connection = None
+            await self.connection_pool.release(conn)
+
+    # COMMAND EXECUTION AND PROTOCOL PARSING
+    async def execute_command(self, *args, **options):
+        """Execute a command and return a parsed response"""
+        await self.initialize()
+        pool = self.connection_pool
+        command_name = args[0]
+        conn = self.connection or await pool.get_connection(command_name, **options)
+        try:
+            await conn.send_command(*args)
+            return await self.parse_response(conn, command_name, **options)
+        except (ConnectionError, TimeoutError) as e:
+            await conn.disconnect()
+            if not (conn.retry_on_timeout and isinstance(e, TimeoutError)):
+                raise
+            await conn.send_command(*args)
+            return await self.parse_response(conn, command_name, **options)
+        finally:
+            if not self.connection:
+                await pool.release(conn)
+
+    async def parse_response(
+        self, connection: Connection, command_name: Union[str, bytes], **options
+    ):
+        """Parses a response from the Redis server"""
+        try:
+            response = await connection.read_response()
+        except ResponseError:
+            if EMPTY_RESPONSE in options:
+                return options[EMPTY_RESPONSE]
+            raise
+        if command_name in self.response_callbacks:
+            # Mypy bug: https://github.com/python/mypy/issues/10977
+            command_name = cast(str, command_name)
+            retval = self.response_callbacks[command_name](response, **options)
+            return await retval if inspect.isawaitable(retval) else retval
+        return response
+
+    # SERVER INFORMATION
+
+    # ACL methods
+    def acl_cat(self, category: Optional[str] = None) -> Awaitable:
+        """
+        Returns a list of categories or commands within a category.
+
+        If ``category`` is not supplied, returns a list of all categories.
+        If ``category`` is supplied, returns a list of all commands within
+        that category.
+        """
+        pieces: List[EncodableT] = [category] if category else []
+        return self.execute_command("ACL CAT", *pieces)
+
+    def acl_deluser(self, username: str) -> Awaitable:
+        """Delete the ACL for the specified ``username``"""
+        return self.execute_command("ACL DELUSER", username)
+
+    def acl_genpass(self) -> Awaitable:
+        """Generate a random password value"""
+        return self.execute_command("ACL GENPASS")
+
+    def acl_getuser(self, username: str) -> Awaitable:
+        """
+        Get the ACL details for the specified ``username``.
+
+        If ``username`` does not exist, return None
+        """
+        return self.execute_command("ACL GETUSER", username)
+
+    def acl_list(self) -> Awaitable:
+        """Return a list of all ACLs on the server"""
+        return self.execute_command("ACL LIST")
+
+    def acl_log(self, count: Optional[int] = None) -> Awaitable:
+        """
+        Get ACL logs as a list.
+        :param int count: Get logs[0:count].
+        :rtype: List.
+        """
+        args = []
+        if count is not None:
+            if not isinstance(count, int):
+                raise DataError("ACL LOG count must be an integer")
+            args.append(count)
+
+        return self.execute_command("ACL LOG", *args)
+
+    def acl_log_reset(self) -> Awaitable:
+        """
+        Reset ACL logs.
+        :rtype: Boolean.
+        """
+        args = [b"RESET"]
+        return self.execute_command("ACL LOG", *args)
+
+    def acl_load(self) -> Awaitable:
+        """
+        Load ACL rules from the configured ``aclfile``.
+
+        Note that the server must be configured with the ``aclfile``
+        directive to be able to load ACL rules from an aclfile.
+        """
+        return self.execute_command("ACL LOAD")
+
+    def acl_save(self) -> Awaitable:
+        """
+        Save ACL rules to the configured ``aclfile``.
+
+        Note that the server must be configured with the ``aclfile``
+        directive to be able to save ACL rules to an aclfile.
+        """
+        return self.execute_command("ACL SAVE")
+
+    def acl_setuser(  # noqa: C901
+        self,
+        username: str,
+        enabled: bool = False,
+        nopass: bool = False,
+        passwords: Optional[Union[str, Iterable[str]]] = None,
+        hashed_passwords: Optional[Union[str, Iterable[str]]] = None,
+        categories: Optional[Iterable[str]] = None,
+        commands: Optional[Iterable[str]] = None,
+        keys: Optional[Iterable[KeyT]] = None,
+        reset: bool = False,
+        reset_keys: bool = False,
+        reset_passwords: bool = False,
+    ) -> Awaitable:
+        """
+        Create or update an ACL user.
+
+        Create or update the ACL for ``username``. If the user already exists,
+        the existing ACL is completely overwritten and replaced with the
+        specified values.
+
+        ``enabled`` is a boolean indicating whether the user should be allowed
+        to authenticate or not. Defaults to ``False``.
+
+        ``nopass`` is a boolean indicating whether the can authenticate without
+        a password. This cannot be True if ``passwords`` are also specified.
+
+        ``passwords`` if specified is a list of plain text passwords
+        to add to or remove from the user. Each password must be prefixed with
+        a '+' to add or a '-' to remove. For convenience, the value of
+        ``passwords`` can be a simple prefixed string when adding or
+        removing a single password.
+
+        ``hashed_passwords`` if specified is a list of SHA-256 hashed passwords
+        to add to or remove from the user. Each hashed password must be
+        prefixed with a '+' to add or a '-' to remove. For convenience,
+        the value of ``hashed_passwords`` can be a simple prefixed string when
+        adding or removing a single password.
+
+        ``categories`` if specified is a list of strings representing category
+        permissions. Each string must be prefixed with either a '+' to add the
+        category permission or a '-' to remove the category permission.
+
+        ``commands`` if specified is a list of strings representing command
+        permissions. Each string must be prefixed with either a '+' to add the
+        command permission or a '-' to remove the command permission.
+
+        ``keys`` if specified is a list of key patterns to grant the user
+        access to. Keys patterns allow '*' to support wildcard matching. For
+        example, '*' grants access to all keys while 'cache:*' grants access
+        to all keys that are prefixed with 'cache:'. ``keys`` should not be
+        prefixed with a '~'.
+
+        ``reset`` is a boolean indicating whether the user should be fully
+        reset prior to applying the new ACL. Setting this to True will
+        remove all existing passwords, flags and privileges from the user and
+        then apply the specified rules. If this is False, the user's existing
+        passwords, flags and privileges will be kept and any new specified
+        rules will be applied on top.
+
+        ``reset_keys`` is a boolean indicating whether the user's key
+        permissions should be reset prior to applying any new key permissions
+        specified in ``keys``. If this is False, the user's existing
+        key permissions will be kept and any new specified key permissions
+        will be applied on top.
+
+        ``reset_passwords`` is a boolean indicating whether to remove all
+        existing passwords and the 'nopass' flag from the user prior to
+        applying any new passwords specified in 'passwords' or
+        'hashed_passwords'. If this is False, the user's existing passwords
+        and 'nopass' status will be kept and any new specified passwords
+        or hashed_passwords will be applied on top.
+        """
+        encoder = self.connection_pool.get_encoder()
+        pieces: List[Union[str, bytes]] = [username]
+
+        if reset:
+            pieces.append(b"reset")
+
+        if reset_keys:
+            pieces.append(b"resetkeys")
+
+        if reset_passwords:
+            pieces.append(b"resetpass")
+
+        if enabled:
+            pieces.append(b"on")
+        else:
+            pieces.append(b"off")
+
+        if (passwords or hashed_passwords) and nopass:
+            raise DataError(
+                "Cannot set 'nopass' and supply " "'passwords' or 'hashed_passwords'"
+            )
+
+        if passwords:
+            # as most users will have only one password, allow remove_passwords
+            # to be specified as a simple string or a list
+            converted_passwords = list_or_args(passwords, [])
+            for i, raw_password in enumerate(converted_passwords):
+                password = encoder.encode(raw_password)
+                if password.startswith(b"+"):
+                    pieces.append(b">%s" % password[1:])
+                elif password.startswith(b"-"):
+                    pieces.append(b"<%s" % password[1:])
+                else:
+                    raise DataError(
+                        "Password %d must be prefixeed with a "
+                        '"+" to add or a "-" to remove' % i
+                    )
+
+        if hashed_passwords:
+            # as most users will have only one password, allow remove_passwords
+            # to be specified as a simple string or a list
+            parsed_hashed_passwords = list_or_args(hashed_passwords, [])
+            for i, raw_hashed_password in enumerate(parsed_hashed_passwords):
+                hashed_password = encoder.encode(raw_hashed_password)
+                if hashed_password.startswith(b"+"):
+                    pieces.append(b"#%s" % hashed_password[1:])
+                elif hashed_password.startswith(b"-"):
+                    pieces.append(b"!%s" % hashed_password[1:])
+                else:
+                    raise DataError(
+                        "Hashed %d password must be prefixeed "
+                        'with a "+" to add or a "-" to remove' % i
+                    )
+
+        if nopass:
+            pieces.append(b"nopass")
+
+        if categories:
+            for raw_category in categories:
+                category = encoder.encode(raw_category)
+                # categories can be prefixed with one of (+@, +, -@, -)
+                if category.startswith(b"+@"):
+                    pieces.append(category)
+                elif category.startswith(b"+"):
+                    pieces.append(b"+@%s" % category[1:])
+                elif category.startswith(b"-@"):
+                    pieces.append(category)
+                elif category.startswith(b"-"):
+                    pieces.append(b"-@%s" % category[1:])
+                else:
+                    raise DataError(
+                        f'Category "{encoder.decode(category, force=True)}" must be '
+                        'prefixed with "+" or "-"'
+                    )
+        if commands:
+            for raw_cmd in commands:
+                cmd = encoder.encode(raw_cmd)
+                if not cmd.startswith(b"+") and not cmd.startswith(b"-"):
+                    raise DataError(
+                        f'Command "{encoder.decode(cmd, force=True)}" must be '
+                        'prefixed with "+" or "-"'
+                    )
+                pieces.append(cmd)
+
+        if keys:
+            for raw_key in keys:
+                key = encoder.encode(raw_key)
+                pieces.append(b"~%s" % key)
+
+        return self.execute_command("ACL SETUSER", *pieces)
+
+    def acl_users(self) -> Awaitable:
+        """Returns a list of all registered users on the server."""
+        return self.execute_command("ACL USERS")
+
+    def acl_whoami(self) -> Awaitable:
+        """Get the username for the current connection"""
+        return self.execute_command("ACL WHOAMI")
+
+    def bgrewriteaof(self) -> Awaitable:
+        """Tell the Redis server to rewrite the AOF file from data in memory."""
+        return self.execute_command("BGREWRITEAOF")
+
+    def bgsave(self) -> Awaitable:
+        """
+        Tell the Redis server to save its data to disk.  Unlike save(),
+        this method is asynchronous and returns immediately.
+        """
+        return self.execute_command("BGSAVE")
+
+    def client_kill(self, address: str) -> Awaitable:
+        """Disconnects the client at ``address`` (ip:port)"""
+        return self.execute_command("CLIENT KILL", address)
+
+    def client_kill_filter(
+        self,
+        _id: Optional[str] = None,
+        _type: Optional[str] = None,
+        addr: Optional[str] = None,
+        skipme: Optional[bool] = None,
+    ) -> Awaitable:
+        """
+        Disconnects client(s) using a variety of filter options
+        :param _id: Kills a client by its unique ID field
+        :param _type: Kills a client by type where type is one of 'normal',
+        'master', 'slave' or 'pubsub'
+        :param addr: Kills a client by its 'address:port'
+        :param skipme: If True, then the client calling the command
+        will not get killed even if it is identified by one of the filter
+        options. If skipme is not provided, the server defaults to skipme=True
+        """
+        args: List[Union[bytes, str]] = []
+        if _type is not None:
+            client_types = ("normal", "master", "slave", "pubsub")
+            if str(_type).lower() not in client_types:
+                raise DataError(f"CLIENT KILL type must be one of {client_types!r}")
+            args.extend((b"TYPE", _type))
+        if skipme is not None:
+            if not isinstance(skipme, bool):
+                raise DataError("CLIENT KILL skipme must be a bool")
+            if skipme:
+                args.extend((b"SKIPME", b"YES"))
+            else:
+                args.extend((b"SKIPME", b"NO"))
+        if _id is not None:
+            args.extend((b"ID", _id))
+        if addr is not None:
+            args.extend((b"ADDR", addr))
+        if not args:
+            raise DataError(
+                "CLIENT KILL <filter> <value> ... ... <filter> "
+                "<value> must specify at least one filter"
+            )
+        return self.execute_command("CLIENT KILL", *args)
+
+    def client_list(self, _type: Optional[str] = None) -> Awaitable:
+        """
+        Returns a list of currently connected clients.
+        If type of client specified, only that type will be returned.
+        :param _type: optional. one of the client types (normal, master,
+         replica, pubsub)
+        """
+        "Returns a list of currently connected clients"
+        if _type is not None:
+            client_types = ("normal", "master", "replica", "pubsub")
+            if str(_type).lower() not in client_types:
+                raise DataError(f"CLIENT LIST _type must be one of {client_types!r}")
+            return self.execute_command("CLIENT LIST", b"TYPE", _type)
+        return self.execute_command("CLIENT LIST")
+
+    def client_getname(self) -> Awaitable:
+        """Returns the current connection name"""
+        return self.execute_command("CLIENT GETNAME")
+
+    def client_id(self) -> Awaitable:
+        """Returns the current connection id"""
+        return self.execute_command("CLIENT ID")
+
+    def client_setname(self, name: str) -> Awaitable:
+        """Sets the current connection name"""
+        return self.execute_command("CLIENT SETNAME", name)
+
+    def client_unblock(self, client_id: int, error: bool = False) -> Awaitable:
+        """
+        Unblocks a connection by its client id.
+        If ``error`` is True, unblocks the client with a special error message.
+        If ``error`` is False (default), the client is unblocked using the
+        regular timeout mechanism.
+        """
+        args = ["CLIENT UNBLOCK", int(client_id)]
+        if error:
+            args.append(b"ERROR")
+        return self.execute_command(*args)
+
+    def client_pause(self, timeout: int) -> Awaitable:
+        """
+        Suspend all the Redis clients for the specified amount of time
+        :param timeout: milliseconds to pause clients
+        """
+        if not isinstance(timeout, int):
+            raise DataError("CLIENT PAUSE timeout must be an integer")
+        return self.execute_command("CLIENT PAUSE", str(timeout))
+
+    def readwrite(self) -> Awaitable:
+        """Disables read queries for a connection to a Redis Cluster slave node"""
+        return self.execute_command("READWRITE")
+
+    def readonly(self) -> Awaitable:
+        """Enables read queries for a connection to a Redis Cluster replica node"""
+        return self.execute_command("READONLY")
+
+    def config_get(self, pattern: str = "*") -> Awaitable:
+        """Return a dictionary of configuration based on the ``pattern``"""
+        return self.execute_command("CONFIG GET", pattern)
+
+    def config_set(self, name: str, value: EncodableT) -> Awaitable:
+        """Set config item ``name`` with ``value``"""
+        return self.execute_command("CONFIG SET", name, value)
+
+    def config_resetstat(self) -> Awaitable:
+        """Reset runtime statistics"""
+        return self.execute_command("CONFIG RESETSTAT")
+
+    def config_rewrite(self) -> Awaitable:
+        """Rewrite config file with the minimal change to reflect running config"""
+        return self.execute_command("CONFIG REWRITE")
+
+    def dbsize(self) -> Awaitable:
+        """Returns the number of keys in the current database"""
+        return self.execute_command("DBSIZE")
+
+    def debug_object(self, key: KeyT) -> Awaitable:
+        """Returns version specific meta information about a given key"""
+        return self.execute_command("DEBUG OBJECT", key)
+
+    def echo(self, value: EncodableT) -> Awaitable:
+        """Echo the string back from the server"""
+        return self.execute_command("ECHO", value)
+
+    def flushall(self, asynchronous: bool = False) -> Awaitable:
+        """
+        Delete all keys in all databases on the current host.
+
+        ``asynchronous`` indicates whether the operation is
+        executed asynchronously by the server.
+        """
+        args = []
+        if asynchronous:
+            args.append(b"ASYNC")
+        return self.execute_command("FLUSHALL", *args)
+
+    def flushdb(self, asynchronous: bool = False) -> Awaitable:
+        """
+        Delete all keys in the current database.
+
+        ``asynchronous`` indicates whether the operation is
+        executed asynchronously by the server.
+        """
+        args = []
+        if asynchronous:
+            args.append(b"ASYNC")
+        return self.execute_command("FLUSHDB", *args)
+
+    def swapdb(self, first: int, second: int) -> Awaitable:
+        """Swap two databases"""
+        return self.execute_command("SWAPDB", first, second)
+
+    def info(self, section: Optional[str] = None) -> Awaitable:
+        """
+        Returns a dictionary containing information about the Redis server
+
+        The ``section`` option can be used to select a specific section
+        of information
+
+        The section option is not supported by older versions of Redis Server,
+        and will generate ResponseError
+        """
+        if section is None:
+            return self.execute_command("INFO")
+        else:
+            return self.execute_command("INFO", section)
+
+    def lastsave(self) -> Awaitable:
+        """
+        Return a Python datetime object representing the last time the
+        Redis database was saved to disk
+        """
+        return self.execute_command("LASTSAVE")
+
+    def migrate(
+        self,
+        host: str,
+        port: int,
+        keys: KeysT,
+        destination_db: int,
+        timeout: int,
+        copy: bool = False,
+        replace: bool = False,
+        auth: Optional[str] = None,
+    ) -> Awaitable:
+        """
+        Migrate 1 or more keys from the current Redis server to a different
+        server specified by the ``host``, ``port`` and ``destination_db``.
+
+        The ``timeout``, specified in milliseconds, indicates the maximum
+        time the connection between the two servers can be idle before the
+        command is interrupted.
+
+        If ``copy`` is True, the specified ``keys`` are NOT deleted from
+        the source server.
+
+        If ``replace`` is True, this operation will overwrite the keys
+        on the destination server if they exist.
+
+        If ``auth`` is specified, authenticate to the destination server with
+        the password provided.
+        """
+        keys = list_or_args(keys, [])
+        if not keys:
+            raise DataError("MIGRATE requires at least one key")
+        pieces: List[EncodableT] = []
+        if copy:
+            pieces.append(b"COPY")
+        if replace:
+            pieces.append(b"REPLACE")
+        if auth:
+            pieces.append(b"AUTH")
+            pieces.append(auth)
+        pieces.append(b"KEYS")
+        pieces.extend(keys)
+        return self.execute_command(
+            "MIGRATE", host, port, "", destination_db, timeout, *pieces
+        )
+
+    def object(self, infotype: str, key: KeyT) -> Awaitable:
+        """Return the encoding, idletime, or refcount about the key"""
+        return self.execute_command("OBJECT", infotype, key, infotype=infotype)
+
+    def memory_stats(self) -> Awaitable:
+        """Return a dictionary of memory stats"""
+        return self.execute_command("MEMORY STATS")
+
+    def memory_usage(self, key: KeyT, samples: Optional[int] = None) -> Awaitable:
+        """
+        Return the total memory usage for key, its value and associated
+        administrative overheads.
+
+        For nested data structures, ``samples`` is the number of elements to
+        sample. If left unspecified, the server's default is 5. Use 0 to sample
+        all elements.
+        """
+        args = []
+        if isinstance(samples, int):
+            args.extend([b"SAMPLES", samples])
+        return self.execute_command("MEMORY USAGE", key, *args)
+
+    def memory_purge(self) -> Awaitable:
+        """Attempts to purge dirty pages for reclamation by allocator"""
+        return self.execute_command("MEMORY PURGE")
+
+    def ping(self) -> Awaitable:
+        """Ping the Redis server"""
+        return self.execute_command("PING")
+
+    def save(self) -> Awaitable:
+        """
+        Tell the Redis server to save its data to disk,
+        blocking until the save is complete
+        """
+        return self.execute_command("SAVE")
+
+    def sentinel_get_master_addr_by_name(self, service_name: str) -> Awaitable:
+        """Returns a (host, port) pair for the given ``service_name``"""
+        return self.execute_command("SENTINEL GET-MASTER-ADDR-BY-NAME", service_name)
+
+    def sentinel_master(self, service_name: str) -> Awaitable:
+        """Returns a dictionary containing the specified masters state."""
+        return self.execute_command("SENTINEL MASTER", service_name)
+
+    def sentinel_masters(self) -> Awaitable:
+        """Returns a list of dictionaries containing each master's state."""
+        return self.execute_command("SENTINEL MASTERS")
+
+    def sentinel_monitor(self, name: str, ip: str, port: int, quorum: int) -> Awaitable:
+        """Add a new master to Sentinel to be monitored"""
+        return self.execute_command("SENTINEL MONITOR", name, ip, port, quorum)
+
+    def sentinel_remove(self, name: str) -> Awaitable:
+        """Remove a master from Sentinel's monitoring"""
+        return self.execute_command("SENTINEL REMOVE", name)
+
+    def sentinel_sentinels(self, service_name: str) -> Awaitable:
+        """Returns a list of sentinels for ``service_name``"""
+        return self.execute_command("SENTINEL SENTINELS", service_name)
+
+    def sentinel_set(self, name: str, option: str, value: EncodableT) -> Awaitable:
+        """Set Sentinel monitoring parameters for a given master"""
+        return self.execute_command("SENTINEL SET", name, option, value)
+
+    def sentinel_slaves(self, service_name: str) -> Awaitable:
+        """Returns a list of slaves for ``service_name``"""
+        return self.execute_command("SENTINEL SLAVES", service_name)
+
+    def shutdown(self, save: bool = False, nosave: bool = False) -> None:
+        """Shutdown the Redis server.  If Redis has persistence configured,
+        data will be flushed before shutdown.  If the "save" option is set,
+        a data flush will be attempted even if there is no persistence
+        configured.  If the "nosave" option is set, no data flush will be
+        attempted.  The "save" and "nosave" options cannot both be set.
+        """
+        if save and nosave:
+            raise DataError("SHUTDOWN save and nosave cannot both be set")
+        args = ["SHUTDOWN"]
+        if save:
+            args.append("SAVE")
+        if nosave:
+            args.append("NOSAVE")
+        try:
+            self.execute_command(*args)
+        except ConnectionError:
+            # a ConnectionError here is expected
+            return
+        raise RedisError("SHUTDOWN seems to have failed.")
+
+    def slaveof(
+        self, host: Optional[str] = None, port: Optional[int] = None
+    ) -> Awaitable:
+        """
+        Set the server to be a replicated slave of the instance identified
+        by the ``host`` and ``port``. If called without arguments, the
+        instance is promoted to a master instead.
+        """
+        if host is None and port is None:
+            return self.execute_command("SLAVEOF", b"NO", b"ONE")
+        return self.execute_command("SLAVEOF", host, port)
+
+    def slowlog_get(self, num: Optional[int] = None) -> Awaitable:
+        """
+        Get the entries from the slowlog. If ``num`` is specified, get the
+        most recent ``num`` items.
+        """
+        args: List[EncodableT] = ["SLOWLOG GET"]
+        if num is not None:
+            args.append(num)
+        decode_responses = self.connection_pool.connection_kwargs.get(
+            "decode_responses", False
+        )
+        return self.execute_command(*args, decode_responses=decode_responses)
+
+    def slowlog_len(self) -> Awaitable:
+        """Get the number of items in the slowlog"""
+        return self.execute_command("SLOWLOG LEN")
+
+    def slowlog_reset(self) -> Awaitable:
+        """Remove all items in the slowlog"""
+        return self.execute_command("SLOWLOG RESET")
+
+    def time(self) -> Awaitable:
+        """
+        Returns the server time as a 2-item tuple of ints:
+        (seconds since epoch, microseconds into this second).
+        """
+        return self.execute_command("TIME")
+
+    def wait(self, num_replicas: int, timeout: int) -> Awaitable:
+        """
+        Redis synchronous replication
+        That returns the number of replicas that processed the query when
+        we finally have at least ``num_replicas``, or when the ``timeout`` was
+        reached.
+        """
+        return self.execute_command("WAIT", num_replicas, timeout)
+
+    # BASIC KEY COMMANDS
+    def append(self, key: KeyT, value: EncodableT) -> Awaitable:
+        """
+        Appends the string ``value`` to the value at ``key``. If ``key``
+        doesn't already exist, create it with a value of ``value``.
+        Returns the new length of the value at ``key``.
+        """
+        return self.execute_command("APPEND", key, value)
+
+    def bitcount(
+        self, key: KeyT, start: Optional[int] = None, end: Optional[int] = None
+    ) -> Awaitable:
+        """
+        Returns the count of set bits in the value of ``key``.  Optional
+        ``start`` and ``end`` paramaters indicate which bytes to consider
+        """
+        params: List[EncodableT] = [key]
+        if start is not None and end is not None:
+            params.append(start)
+            params.append(end)
+        elif (start is not None and end is None) or (end is not None and start is None):
+            raise DataError("Both start and end must be specified")
+        return self.execute_command("BITCOUNT", *params)
+
+    def bitfield(
+        self, key: KeyT, default_overflow: Optional[str] = None
+    ) -> "BitFieldOperation":
+        """
+        Return a BitFieldOperation instance to conveniently construct one or
+        more bitfield operations on ``key``.
+        """
+        return BitFieldOperation(self, key, default_overflow=default_overflow)
+
+    def bitop(self, operation: str, dest: KeyT, *keys: KeyT) -> Awaitable:
+        """
+        Perform a bitwise operation using ``operation`` between ``keys`` and
+        store the result in ``dest``.
+        """
+        return self.execute_command("BITOP", operation, dest, *keys)
+
+    def bitpos(
+        self,
+        key: KeyT,
+        bit: int,
+        start: Optional[int] = None,
+        end: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Return the position of the first bit set to 1 or 0 in a string.
+        ``start`` and ``end`` difines search range. The range is interpreted
+        as a range of bytes and not a range of bits, so start=0 and end=2
+        means to look at the first three bytes.
+        """
+        if bit not in (0, 1):
+            raise DataError("bit must be 0 or 1")
+        params = [key, bit]
+
+        if start is not None:
+            params.append(start)
+            if end is not None:
+                params.append(end)
+        elif end is not None:
+            raise DataError("start argument is not set, when end is specified")
+        return self.execute_command("BITPOS", *params)
+
+    def decr(self, name: KeyT, amount: int = 1) -> Awaitable:
+        """
+        Decrements the value of ``key`` by ``amount``.  If no key exists,
+        the value will be initialized as 0 - ``amount``
+        """
+        # An alias for ``decr()``, because it is already implemented
+        # as DECRBY redis command.
+        return self.decrby(name, amount)
+
+    def decrby(self, name: KeyT, amount: int = 1) -> Awaitable:
+        """
+        Decrements the value of ``key`` by ``amount``.  If no key exists,
+        the value will be initialized as 0 - ``amount``
+        """
+        return self.execute_command("DECRBY", name, amount)
+
+    def delete(self, *names: KeyT) -> Awaitable:
+        """Delete one or more keys specified by ``names``"""
+        return self.execute_command("DEL", *names)
+
+    def dump(self, name: KeyT) -> Awaitable:
+        """
+        Return a serialized version of the value stored at the specified key.
+        If key does not exist a nil bulk reply is returned.
+        """
+        return self.execute_command("DUMP", name)
+
+    def exists(self, *names: KeyT) -> Awaitable:
+        """Returns the number of ``names`` that exist"""
+        return self.execute_command("EXISTS", *names)
+
+    def expire(self, name: KeyT, time: ExpiryT) -> Awaitable:
+        """
+        Set an expire flag on key ``name`` for ``time`` seconds. ``time``
+        can be represented by an integer or a Python timedelta object.
+        """
+        if isinstance(time, datetime.timedelta):
+            time = int(time.total_seconds())
+        return self.execute_command("EXPIRE", name, time)
+
+    def expireat(self, name: KeyT, when: AbsExpiryT) -> Awaitable:
+        """
+        Set an expire flag on key ``name``. ``when`` can be represented
+        as an integer indicating unix time or a Python datetime object.
+        """
+        if isinstance(when, datetime.datetime):
+            when = int(mod_time.mktime(when.timetuple()))
+        return self.execute_command("EXPIREAT", name, when)
+
+    def get(self, name: KeyT) -> Awaitable:
+        """
+        Return the value at key ``name``, or None if the key doesn't exist
+        """
+        return self.execute_command("GET", name)
+
+    def getbit(self, name: KeyT, offset: int) -> Awaitable:
+        """Returns a boolean indicating the value of ``offset`` in ``name``"""
+        return self.execute_command("GETBIT", name, offset)
+
+    def getrange(self, key: KeyT, start: int, end: int) -> Awaitable:
+        """
+        Returns the substring of the string value stored at ``key``,
+        determined by the offsets ``start`` and ``end`` (both are inclusive)
+        """
+        return self.execute_command("GETRANGE", key, start, end)
+
+    def getset(self, name: KeyT, value: EncodableT) -> Awaitable:
+        """
+        Sets the value at key ``name`` to ``value``
+        and returns the old value at key ``name`` atomically.
+        """
+        return self.execute_command("GETSET", name, value)
+
+    def incr(self, name: KeyT, amount: int = 1) -> Awaitable:
+        """
+        Increments the value of ``key`` by ``amount``.  If no key exists,
+        the value will be initialized as ``amount``
+        """
+        return self.incrby(name, amount)
+
+    def incrby(self, name: KeyT, amount: int = 1) -> Awaitable:
+        """
+        Increments the value of ``key`` by ``amount``.  If no key exists,
+        the value will be initialized as ``amount``
+        """
+        # An alias for ``incr()``, because it is already implemented
+        # as INCRBY redis command.
+        return self.execute_command("INCRBY", name, amount)
+
+    def incrbyfloat(self, name: KeyT, amount: float = 1.0) -> Awaitable:
+        """
+        Increments the value at key ``name`` by floating ``amount``.
+        If no key exists, the value will be initialized as ``amount``
+        """
+        return self.execute_command("INCRBYFLOAT", name, amount)
+
+    def keys(self, pattern: PatternT = "*") -> Awaitable:
+        """Returns a list of keys matching ``pattern``"""
+        return self.execute_command("KEYS", pattern)
+
+    def mget(self, keys: KeysT, *args: EncodableT) -> Awaitable:
+        """
+        Returns a list of values ordered identically to ``keys``
+        """
+        encoded_args = list_or_args(keys, args)
+        options: Dict[str, Union[EncodableT, Iterable[EncodableT]]] = {}
+        if not encoded_args:
+            options[EMPTY_RESPONSE] = []
+        return self.execute_command("MGET", *encoded_args, **options)
+
+    def mset(self, mapping: Mapping[AnyKeyT, EncodableT]) -> Awaitable:
+        """
+        Sets key/values based on a mapping. Mapping is a dictionary of
+        key/value pairs. Both keys and values should be strings or types that
+        can be cast to a string via str().
+        """
+        items: List[EncodableT] = []
+        for pair in mapping.items():
+            items.extend(pair)
+        return self.execute_command("MSET", *items)
+
+    def msetnx(self, mapping: Mapping[AnyKeyT, EncodableT]) -> Awaitable:
+        """
+        Sets key/values based on a mapping if none of the keys are already set.
+        Mapping is a dictionary of key/value pairs. Both keys and values
+        should be strings or types that can be cast to a string via str().
+        Returns a boolean indicating if the operation was successful.
+        """
+        items: List[EncodableT] = []
+        for pair in mapping.items():
+            items.extend(pair)
+        return self.execute_command("MSETNX", *items)
+
+    def move(self, name: KeyT, db: int) -> Awaitable:
+        """Moves the key ``name`` to a different Redis database ``db``"""
+        return self.execute_command("MOVE", name, db)
+
+    def persist(self, name: KeyT) -> Awaitable:
+        """Removes an expiration on ``name``"""
+        return self.execute_command("PERSIST", name)
+
+    def pexpire(self, name: KeyT, time: ExpiryT) -> Awaitable:
+        """
+        Set an expire flag on key ``name`` for ``time`` milliseconds.
+        ``time`` can be represented by an integer or a Python timedelta
+        object.
+        """
+        if isinstance(time, datetime.timedelta):
+            time = int(time.total_seconds() * 1000)
+        return self.execute_command("PEXPIRE", name, time)
+
+    def pexpireat(self, name: KeyT, when: AbsExpiryT) -> Awaitable:
+        """
+        Set an expire flag on key ``name``. ``when`` can be represented
+        as an integer representing unix time in milliseconds (unix time * 1000)
+        or a Python datetime object.
+        """
+        if isinstance(when, datetime.datetime):
+            ms = int(when.microsecond / 1000)
+            when = int(mod_time.mktime(when.timetuple())) * 1000 + ms
+        return self.execute_command("PEXPIREAT", name, when)
+
+    def psetex(self, name: KeyT, time_ms: ExpiryT, value: EncodableT) -> Awaitable:
+        """
+        Set the value of key ``name`` to ``value`` that expires in ``time_ms``
+        milliseconds. ``time_ms`` can be represented by an integer or a Python
+        timedelta object
+        """
+        if isinstance(time_ms, datetime.timedelta):
+            time_ms = int(time_ms.total_seconds() * 1000)
+        return self.execute_command("PSETEX", name, time_ms, value)
+
+    def pttl(self, name: KeyT) -> Awaitable:
+        """Returns the number of milliseconds until the key ``name`` will expire"""
+        return self.execute_command("PTTL", name)
+
+    def randomkey(self) -> Awaitable:
+        """Returns the name of a random key"""
+        return self.execute_command("RANDOMKEY")
+
+    def rename(self, src: KeyT, dst: KeyT) -> Awaitable:
+        """
+        Rename key ``src`` to ``dst``
+        """
+        return self.execute_command("RENAME", src, dst)
+
+    def renamenx(self, src: KeyT, dst: KeyT) -> Awaitable:
+        """Rename key ``src`` to ``dst`` if ``dst`` doesn't already exist"""
+        return self.execute_command("RENAMENX", src, dst)
+
+    def restore(
+        self,
+        name: KeyT,
+        ttl: float,
+        value: EncodableT,
+        replace: bool = False,
+        absttl: bool = False,
+    ) -> Awaitable:
+        """
+        Create a key using the provided serialized value, previously obtained
+        using DUMP.
+
+        ``replace`` allows an existing key on ``name`` to be overridden. If
+        it's not specified an error is raised on collision.
+
+        ``absttl`` if True, specified ``ttl`` should represent an absolute Unix
+        timestamp in milliseconds in which the key will expire. (Redis 5.0 or
+        greater).
+        """
+        params = [name, ttl, value]
+        if replace:
+            params.append("REPLACE")
+        if absttl:
+            params.append("ABSTTL")
+        return self.execute_command("RESTORE", *params)
+
+    def set(
+        self,
+        name: KeyT,
+        value: EncodableT,
+        ex: Optional[ExpiryT] = None,
+        px: Optional[ExpiryT] = None,
+        nx: bool = False,
+        xx: bool = False,
+        keepttl: bool = False,
+    ) -> Awaitable:
+        """
+        Set the value at key ``name`` to ``value``
+
+        ``ex`` sets an expire flag on key ``name`` for ``ex`` seconds.
+
+        ``px`` sets an expire flag on key ``name`` for ``px`` milliseconds.
+
+        ``nx`` if set to True, set the value at key ``name`` to ``value`` only
+            if it does not exist.
+
+        ``xx`` if set to True, set the value at key ``name`` to ``value`` only
+            if it already exists.
+
+        ``keepttl`` if True, retain the time to live associated with the key.
+            (Available since Redis 6.0)
+        """
+        pieces: List[EncodableT] = [name, value]
+        if ex is not None:
+            pieces.append("EX")
+            if isinstance(ex, datetime.timedelta):
+                ex = int(ex.total_seconds())
+            pieces.append(ex)
+        if px is not None:
+            pieces.append("PX")
+            if isinstance(px, datetime.timedelta):
+                px = int(px.total_seconds() * 1000)
+            pieces.append(px)
+
+        if nx:
+            pieces.append("NX")
+        if xx:
+            pieces.append("XX")
+
+        if keepttl:
+            pieces.append("KEEPTTL")
+
+        return self.execute_command("SET", *pieces)
+
+    def setbit(self, name: KeyT, offset: int, value: int) -> Awaitable:
+        """
+        Flag the ``offset`` in ``name`` as ``value``. Returns a boolean
+        indicating the previous value of ``offset``.
+        """
+        value = value and 1 or 0
+        return self.execute_command("SETBIT", name, offset, value)
+
+    def setex(
+        self, name: KeyT, time: Union[int, datetime.timedelta], value: EncodableT
+    ) -> Awaitable:
+        """
+        Set the value of key ``name`` to ``value`` that expires in ``time``
+        seconds. ``time`` can be represented by an integer or a Python
+        timedelta object.
+        """
+        if isinstance(time, datetime.timedelta):
+            time = int(time.total_seconds())
+        return self.execute_command("SETEX", name, time, value)
+
+    def setnx(self, name: KeyT, value: EncodableT) -> Awaitable:
+        """Set the value of key ``name`` to ``value`` if key doesn't exist"""
+        return self.execute_command("SETNX", name, value)
+
+    def setrange(self, name: KeyT, offset: int, value: EncodableT) -> Awaitable:
+        """
+        Overwrite bytes in the value of ``name`` starting at ``offset`` with
+        ``value``. If ``offset`` plus the length of ``value`` exceeds the
+        length of the original value, the new value will be larger than before.
+        If ``offset`` exceeds the length of the original value, null bytes
+        will be used to pad between the end of the previous value and the start
+        of what's being injected.
+
+        Returns the length of the new string.
+        """
+        return self.execute_command("SETRANGE", name, offset, value)
+
+    def strlen(self, name: KeyT) -> Awaitable:
+        """Return the number of bytes stored in the value of ``name``"""
+        return self.execute_command("STRLEN", name)
+
+    def substr(self, name: KeyT, start: int, end: int = -1) -> Awaitable:
+        """
+        Return a substring of the string at key ``name``. ``start`` and ``end``
+        are 0-based integers specifying the portion of the string to return.
+        """
+        return self.execute_command("SUBSTR", name, start, end)
+
+    def touch(self, *args: KeyT) -> Awaitable:
+        """
+        Alters the last access time of a key(s) ``*args``. A key is ignored
+        if it does not exist.
+        """
+        return self.execute_command("TOUCH", *args)
+
+    def ttl(self, name: KeyT) -> Awaitable:
+        """Returns the number of seconds until the key ``name`` will expire"""
+        return self.execute_command("TTL", name)
+
+    def type(self, name: KeyT) -> Awaitable:
+        """Returns the type of key ``name``"""
+        return self.execute_command("TYPE", name)
+
+    def unlink(self, *names: KeyT) -> Awaitable:
+        """Unlink one or more keys specified by ``names``"""
+        return self.execute_command("UNLINK", *names)
+
+    # LIST COMMANDS
+    def blpop(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
+        """
+        LPOP a value off of the first non-empty list
+        named in the ``keys`` list.
+
+        If none of the lists in ``keys`` has a value to LPOP, then block
+        for ``timeout`` seconds, or until a value gets pushed on to one
+        of the lists.
+
+        If timeout is 0, then block indefinitely.
+        """
+        return self.execute_command("BLPOP", *list_or_args(keys, (timeout,)))
+
+    def brpop(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
+        """
+        RPOP a value off of the first non-empty list
+        named in the ``keys`` list.
+
+        If none of the lists in ``keys`` has a value to RPOP, then block
+        for ``timeout`` seconds, or until a value gets pushed on to one
+        of the lists.
+
+        If timeout is 0, then block indefinitely.
+        """
+        return self.execute_command("BRPOP", *list_or_args(keys, (timeout,)))
+
+    def brpoplpush(self, src: KeyT, dst: KeyT, timeout: TimeoutSecT = 0) -> Awaitable:
+        """
+        Pop a value off the tail of ``src``, push it on the head of ``dst``
+        and then return it.
+
+        This command blocks until a value is in ``src`` or until ``timeout``
+        seconds elapse, whichever is first. A ``timeout`` value of 0 blocks
+        forever.
+        """
+        return self.execute_command("BRPOPLPUSH", src, dst, timeout)
+
+    def lindex(self, name: KeyT, index: int) -> Awaitable:
+        """
+        Return the item from list ``name`` at position ``index``
+
+        Negative indexes are supported and will return an item at the
+        end of the list
+        """
+        return self.execute_command("LINDEX", name, index)
+
+    def linsert(
+        self, name: KeyT, where: str, refvalue: EncodableT, value: EncodableT
+    ) -> Awaitable:
+        """
+        Insert ``value`` in list ``name`` either immediately before or after
+        [``where``] ``refvalue``
+
+        Returns the new length of the list on success or -1 if ``refvalue``
+        is not in the list.
+        """
+        return self.execute_command("LINSERT", name, where, refvalue, value)
+
+    def llen(self, name: KeyT) -> Awaitable:
+        """Return the length of the list ``name``"""
+        return self.execute_command("LLEN", name)
+
+    def lpop(self, name: KeyT) -> Awaitable:
+        """Remove and return the first item of the list ``name``"""
+        return self.execute_command("LPOP", name)
+
+    def lpush(self, name: KeyT, *values: EncodableT) -> Awaitable:
+        """Push ``values`` onto the head of the list ``name``"""
+        return self.execute_command("LPUSH", name, *values)
+
+    def lpushx(self, name: KeyT, value: EncodableT) -> Awaitable:
+        """Push ``value`` onto the head of the list ``name`` if ``name`` exists"""
+        return self.execute_command("LPUSHX", name, value)
+
+    def lrange(self, name: KeyT, start: int, end: int) -> Awaitable:
+        """
+        Return a slice of the list ``name`` between
+        position ``start`` and ``end``
+
+        ``start`` and ``end`` can be negative numbers just like
+        Python slicing notation
+        """
+        return self.execute_command("LRANGE", name, start, end)
+
+    def lrem(self, name: KeyT, count: int, value: EncodableT) -> Awaitable:
+        """
+        Remove the first ``count`` occurrences of elements equal to ``value``
+        from the list stored at ``name``.
+
+        The count argument influences the operation in the following ways:
+            count > 0: Remove elements equal to value moving from head to tail.
+            count < 0: Remove elements equal to value moving from tail to head.
+            count = 0: Remove all elements equal to value.
+        """
+        return self.execute_command("LREM", name, count, value)
+
+    def lset(self, name: KeyT, index: int, value: EncodableT) -> Awaitable:
+        """Set ``position`` of list ``name`` to ``value``"""
+        return self.execute_command("LSET", name, index, value)
+
+    def ltrim(self, name: KeyT, start: int, end: int) -> Awaitable:
+        """
+        Trim the list ``name``, removing all values not within the slice
+        between ``start`` and ``end``
+
+        ``start`` and ``end`` can be negative numbers just like
+        Python slicing notation
+        """
+        return self.execute_command("LTRIM", name, start, end)
+
+    def rpop(self, name: KeyT) -> Awaitable:
+        """Remove and return the last item of the list ``name``"""
+        return self.execute_command("RPOP", name)
+
+    def rpoplpush(self, src: KeyT, dst: KeyT) -> Awaitable:
+        """
+        RPOP a value off of the ``src`` list and atomically LPUSH it
+        on to the ``dst`` list.  Returns the value.
+        """
+        return self.execute_command("RPOPLPUSH", src, dst)
+
+    def rpush(self, name: KeyT, *values: EncodableT) -> Awaitable:
+        """Push ``values`` onto the tail of the list ``name``"""
+        return self.execute_command("RPUSH", name, *values)
+
+    def rpushx(self, name: KeyT, value: EncodableT) -> Awaitable:
+        """Push ``value`` onto the tail of the list ``name`` if ``name`` exists"""
+        return self.execute_command("RPUSHX", name, value)
+
+    def lpos(
+        self,
+        name: KeyT,
+        value: EncodableT,
+        rank: Optional[int] = None,
+        count: Optional[int] = None,
+        maxlen: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Get position of ``value`` within the list ``name``
+
+         If specified, ``rank`` indicates the "rank" of the first element to
+         return in case there are multiple copies of ``value`` in the list.
+         By default, LPOS returns the position of the first occurrence of
+         ``value`` in the list. When ``rank`` 2, LPOS returns the position of
+         the second ``value`` in the list. If ``rank`` is negative, LPOS
+         searches the list in reverse. For example, -1 would return the
+         position of the last occurrence of ``value`` and -2 would return the
+         position of the next to last occurrence of ``value``.
+
+         If specified, ``count`` indicates that LPOS should return a list of
+         up to ``count`` positions. A ``count`` of 2 would return a list of
+         up to 2 positions. A ``count`` of 0 returns a list of all positions
+         matching ``value``. When ``count`` is specified and but ``value``
+         does not exist in the list, an empty list is returned.
+
+         If specified, ``maxlen`` indicates the maximum number of list
+         elements to scan. A ``maxlen`` of 1000 will only return the
+         position(s) of items within the first 1000 entries in the list.
+         A ``maxlen`` of 0 (the default) will scan the entire list.
+        """
+        pieces: List[EncodableT] = [name, value]
+        if rank is not None:
+            pieces.extend(["RANK", rank])
+
+        if count is not None:
+            pieces.extend(["COUNT", count])
+
+        if maxlen is not None:
+            pieces.extend(["MAXLEN", maxlen])
+
+        return self.execute_command("LPOS", *pieces)
+
+    def sort(
+        self,
+        name: KeyT,
+        start: Optional[int] = None,
+        num: Optional[int] = None,
+        by: Optional[KeyT] = None,
+        get: Optional[KeysT] = None,
+        desc: bool = False,
+        alpha: bool = False,
+        store: Optional[KeyT] = None,
+        groups: bool = False,
+    ) -> Awaitable:
+        """
+        Sort and return the list, set or sorted set at ``name``.
+
+        ``start`` and ``num`` allow for paging through the sorted data
+
+        ``by`` allows using an external key to weight and sort the items.
+            Use an "*" to indicate where in the key the item value is located
+
+        ``get`` allows for returning items from external keys rather than the
+            sorted data itself.  Use an "*" to indicate where in the key
+            the item value is located
+
+        ``desc`` allows for reversing the sort
+
+        ``alpha`` allows for sorting lexicographically rather than numerically
+
+        ``store`` allows for storing the result of the sort into
+            the key ``store``
+
+        ``groups`` if set to True and if ``get`` contains at least two
+            elements, sort will return a list of tuples, each containing the
+            values fetched from the arguments to ``get``.
+
+        """
+        if (start is not None and num is None) or (num is not None and start is None):
+            raise DataError("``start`` and ``num`` must both be specified")
+
+        pieces: List[EncodableT] = [name]
+        if by is not None:
+            pieces.append(b"BY")
+            pieces.append(by)
+        if start is not None and num is not None:
+            pieces.append(b"LIMIT")
+            pieces.append(start)
+            pieces.append(num)
+        if get is not None:
+            # If get is a string assume we want to get a single value.
+            # Otherwise assume it's an interable and we want to get multiple
+            # values. We can't just iterate blindly because strings are
+            # iterable.
+            if isinstance(get, (bytes, str)):
+                pieces.append(b"GET")
+                pieces.append(get)
+            else:
+                for g in get:
+                    pieces.append(b"GET")
+                    pieces.append(g)
+        if desc:
+            pieces.append(b"DESC")
+        if alpha:
+            pieces.append(b"ALPHA")
+        if store is not None:
+            pieces.append(b"STORE")
+            pieces.append(store)
+
+        if groups:
+            if not get or isinstance(get, (bytes, str)) or len(get) < 2:
+                raise DataError(
+                    'when using "groups" the "get" argument '
+                    "must be specified and contain at least "
+                    "two keys"
+                )
+            options: Dict[str, Optional[int]] = {"groups": len(get)}
+        else:
+            options = {"groups": None}
+
+        return self.execute_command("SORT", *pieces, **options)
+
+    # SCAN COMMANDS
+    def scan(
+        self,
+        cursor: int = 0,
+        match: Optional[PatternT] = None,
+        count: Optional[int] = None,
+        _type: Optional[str] = None,
+    ) -> Awaitable:
+        """
+        Incrementally return lists of key names. Also return a cursor
+        indicating the scan position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` provides a hint to Redis about the number of keys to
+            return per batch.
+
+        ``_type`` filters the returned values by a particular Redis type.
+            Stock Redis instances allow for the following types:
+            HASH, LIST, SET, STREAM, STRING, ZSET
+            Additionally, Redis modules can expose other types as well.
+        """
+        pieces: List[EncodableT] = [cursor]
+        if match is not None:
+            pieces.extend([b"MATCH", match])
+        if count is not None:
+            pieces.extend([b"COUNT", count])
+        if _type is not None:
+            pieces.extend([b"TYPE", _type])
+        return self.execute_command("SCAN", *pieces)
+
+    async def scan_iter(
+        self,
+        match: Optional[PatternT] = None,
+        count: Optional[int] = None,
+        _type: Optional[str] = None,
+    ) -> AsyncIterator:
+        """
+        Make an iterator using the SCAN command so that the client doesn't
+        need to remember the cursor position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` provides a hint to Redis about the number of keys to
+            return per batch.
+
+        ``_type`` filters the returned values by a particular Redis type.
+            Stock Redis instances allow for the following types:
+            HASH, LIST, SET, STREAM, STRING, ZSET
+            Additionally, Redis modules can expose other types as well.
+        """
+        cursor = None
+        while cursor != 0:
+            cursor, data = await self.scan(
+                cursor=cursor or 0, match=match, count=count, _type=_type
+            )
+            for d in data:
+                yield d
+
+    def sscan(
+        self,
+        name: KeyT,
+        cursor: int = 0,
+        match: Optional[PatternT] = None,
+        count: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Incrementally return lists of elements in a set. Also return a cursor
+        indicating the scan position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` allows for hint the minimum number of returns
+        """
+        pieces: List[EncodableT] = [name, cursor]
+        if match is not None:
+            pieces.extend([b"MATCH", match])
+        if count is not None:
+            pieces.extend([b"COUNT", count])
+        return self.execute_command("SSCAN", *pieces)
+
+    async def sscan_iter(
+        self, name: KeyT, match: Optional[PatternT] = None, count: Optional[int] = None
+    ) -> AsyncIterator:
+        """
+        Make an iterator using the SSCAN command so that the client doesn't
+        need to remember the cursor position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` allows for hint the minimum number of returns
+        """
+        cursor = None
+        while cursor != 0:
+            cursor, data = await self.sscan(
+                name, cursor=cursor or 0, match=match, count=count
+            )
+            for d in data:
+                yield d
+
+    def hscan(
+        self,
+        name: KeyT,
+        cursor: int = 0,
+        match: Optional[PatternT] = None,
+        count: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Incrementally return key/value slices in a hash. Also return a cursor
+        indicating the scan position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` allows for hint the minimum number of returns
+        """
+        pieces: List[EncodableT] = [name, cursor]
+        if match is not None:
+            pieces.extend([b"MATCH", match])
+        if count is not None:
+            pieces.extend([b"COUNT", count])
+        return self.execute_command("HSCAN", *pieces)
+
+    async def hscan_iter(
+        self, name: str, match: Optional[PatternT] = None, count: Optional[int] = None
+    ) -> AsyncIterator:
+        """
+        Make an iterator using the HSCAN command so that the client doesn't
+        need to remember the cursor position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` allows for hint the minimum number of returns
+        """
+        cursor = None
+        while cursor != 0:
+            cursor, data = await self.hscan(
+                name, cursor=cursor or 0, match=match, count=count
+            )
+            for it in data.items():
+                yield it
+
+    def zscan(
+        self,
+        name: KeyT,
+        cursor: int = 0,
+        match: Optional[PatternT] = None,
+        count: Optional[int] = None,
+        score_cast_func: Union[Type, Callable] = float,
+    ) -> Awaitable:
+        """
+        Incrementally return lists of elements in a sorted set. Also return a
+        cursor indicating the scan position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` allows for hint the minimum number of returns
+
+        ``score_cast_func`` a callable used to cast the score return value
+        """
+        pieces: List[EncodableT] = [name, cursor]
+        if match is not None:
+            pieces.extend([b"MATCH", match])
+        if count is not None:
+            pieces.extend([b"COUNT", count])
+        options = {"score_cast_func": score_cast_func}
+        return self.execute_command("ZSCAN", *pieces, **options)
+
+    async def zscan_iter(
+        self,
+        name: KeyT,
+        match: Optional[PatternT] = None,
+        count: Optional[int] = None,
+        score_cast_func: Union[Type, Callable] = float,
+    ) -> AsyncIterator:
+        """
+        Make an iterator using the ZSCAN command so that the client doesn't
+        need to remember the cursor position.
+
+        ``match`` allows for filtering the keys by pattern
+
+        ``count`` allows for hint the minimum number of returns
+
+        ``score_cast_func`` a callable used to cast the score return value
+        """
+        cursor = None
+        while cursor != 0:
+            cursor, data = await self.zscan(
+                name,
+                cursor=cursor or 0,
+                match=match,
+                count=count,
+                score_cast_func=score_cast_func,
+            )
+            for d in data:
+                yield d
+
+    # SET COMMANDS
+    def sadd(self, name: KeyT, *values: EncodableT) -> Awaitable:
+        """Add ``value(s)`` to set ``name``"""
+        return self.execute_command("SADD", name, *values)
+
+    def scard(self, name: KeyT) -> Awaitable:
+        """Return the number of elements in set ``name``"""
+        return self.execute_command("SCARD", name)
+
+    def sdiff(self, keys: KeysT, *args: EncodableT) -> Awaitable:
+        """Return the difference of sets specified by ``keys``"""
+        parsed_args = list_or_args(keys, args)
+        return self.execute_command("SDIFF", *parsed_args)
+
+    def sdiffstore(self, dest: KeyT, keys: KeysT, *args: EncodableT) -> Awaitable:
+        """
+        Store the difference of sets specified by ``keys`` into a new
+        set named ``dest``.  Returns the number of keys in the new set.
+        """
+        parsed_args = list_or_args(keys, args)
+        return self.execute_command("SDIFFSTORE", dest, *parsed_args)
+
+    def sinter(self, keys: KeysT, *args: EncodableT) -> Awaitable:
+        """Return the intersection of sets specified by ``keys``"""
+        parsed_args = list_or_args(keys, args)
+        return self.execute_command("SINTER", *parsed_args)
+
+    def sinterstore(self, dest: KeyT, keys: KeysT, *args: EncodableT) -> Awaitable:
+        """
+        Store the intersection of sets specified by ``keys`` into a new
+        set named ``dest``.  Returns the number of keys in the new set.
+        """
+        parsed_args = list_or_args(keys, args)
+        return self.execute_command("SINTERSTORE", dest, *parsed_args)
+
+    def sismember(self, name: KeyT, value: EncodableT) -> Awaitable:
+        """Return a boolean indicating if ``value`` is a member of set ``name``"""
+        return self.execute_command("SISMEMBER", name, value)
+
+    def smembers(self, name: KeyT) -> Awaitable:
+        """Return all members of the set ``name``"""
+        return self.execute_command("SMEMBERS", name)
+
+    def smove(self, src: KeyT, dst: KeyT, value: EncodableT) -> Awaitable:
+        """Move ``value`` from set ``src`` to set ``dst`` atomically"""
+        return self.execute_command("SMOVE", src, dst, value)
+
+    def spop(self, name: KeyT, count: Optional[int] = None) -> Awaitable:
+        """Remove and return a random member of set ``name``"""
+        args = (count is not None) and [count] or []
+        return self.execute_command("SPOP", name, *args)
+
+    def srandmember(self, name: KeyT, number: Optional[int] = None) -> Awaitable:
+        """
+        If ``number`` is None, returns a random member of set ``name``.
+
+        If ``number`` is supplied, returns a list of ``number`` random
+        members of set ``name``. Note this is only available when running
+        Redis 2.6+.
+        """
+        args = (number is not None) and [number] or []
+        return self.execute_command("SRANDMEMBER", name, *args)
+
+    def srem(self, name: KeyT, *values: EncodableT) -> Awaitable:
+        """Remove ``values`` from set ``name``"""
+        return self.execute_command("SREM", name, *values)
+
+    def sunion(self, keys: KeysT, *args: EncodableT) -> Awaitable:
+        """Return the union of sets specified by ``keys``"""
+        parsed_args = list_or_args(keys, args)
+        return self.execute_command("SUNION", *parsed_args)
+
+    def sunionstore(self, dest: KeyT, keys: KeysT, *args: EncodableT) -> Awaitable:
+        """
+        Store the union of sets specified by ``keys`` into a new
+        set named ``dest``.  Returns the number of keys in the new set.
+        """
+        parsed_args = list_or_args(keys, args)
+        return self.execute_command("SUNIONSTORE", dest, *parsed_args)
+
+    # STREAMS COMMANDS
+    def xack(self, name: KeyT, groupname: GroupT, *ids: StreamIdT) -> Awaitable:
+        """
+        Acknowledges the successful processing of one or more messages.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        *ids: message ids to acknowlege.
+        """
+        return self.execute_command("XACK", name, groupname, *ids)
+
+    def xadd(
+        self,
+        name: KeyT,
+        fields: Dict[FieldT, EncodableT],
+        id: StreamIdT = "*",
+        maxlen: Optional[int] = None,
+        approximate: bool = True,
+    ) -> Awaitable:
+        """
+        Add to a stream.
+        name: name of the stream
+        fields: dict of field/value pairs to insert into the stream
+        id: Location to insert this record. By default it is appended.
+        maxlen: truncate old stream members beyond this size
+        approximate: actual stream length may be slightly more than maxlen
+
+        """
+        pieces: List[EncodableT] = []
+        if maxlen is not None:
+            if not isinstance(maxlen, int) or maxlen < 1:
+                raise DataError("XADD maxlen must be a positive integer")
+            pieces.append(b"MAXLEN")
+            if approximate:
+                pieces.append(b"~")
+            pieces.append(str(maxlen))
+        pieces.append(id)
+        if not isinstance(fields, dict) or len(fields) == 0:
+            raise DataError("XADD fields must be a non-empty dict")
+        for pair in fields.items():
+            pieces.extend(pair)
+        return self.execute_command("XADD", name, *pieces)
+
+    def xclaim(
+        self,
+        name: KeyT,
+        groupname: GroupT,
+        consumername: ConsumerT,
+        min_idle_time: int,
+        message_ids: Union[List[StreamIdT], Tuple[StreamIdT]],
+        idle: Optional[int] = None,
+        time: Optional[int] = None,
+        retrycount: Optional[int] = None,
+        force: bool = False,
+        justid: bool = False,
+    ) -> Awaitable:
+        """
+        Changes the ownership of a pending message.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        consumername: name of a consumer that claims the message.
+        min_idle_time: filter messages that were idle less than this amount of
+        milliseconds
+        message_ids: non-empty list or tuple of message IDs to claim
+        idle: optional. Set the idle time (last time it was delivered) of the
+         message in ms
+        time: optional integer. This is the same as idle but instead of a
+         relative amount of milliseconds, it sets the idle time to a specific
+         Unix time (in milliseconds).
+        retrycount: optional integer. set the retry counter to the specified
+         value. This counter is incremented every time a message is delivered
+         again.
+        force: optional boolean, false by default. Creates the pending message
+         entry in the PEL even if certain specified IDs are not already in the
+         PEL assigned to a different client.
+        justid: optional boolean, false by default. Return just an array of IDs
+         of messages successfully claimed, without returning the actual message
+        """
+        if not isinstance(min_idle_time, int) or min_idle_time < 0:
+            raise DataError("XCLAIM min_idle_time must be a non negative " "integer")
+        if not isinstance(message_ids, (list, tuple)) or not message_ids:
+            raise DataError(
+                "XCLAIM message_ids must be a non empty list or "
+                "tuple of message IDs to claim"
+            )
+
+        kwargs = {}
+        pieces: List[EncodableT] = [name, groupname, consumername, str(min_idle_time)]
+        pieces.extend(list(message_ids))
+
+        if idle is not None:
+            if not isinstance(idle, int):
+                raise DataError("XCLAIM idle must be an integer")
+            pieces.extend((b"IDLE", str(idle)))
+        if time is not None:
+            if not isinstance(time, int):
+                raise DataError("XCLAIM time must be an integer")
+            pieces.extend((b"TIME", str(time)))
+        if retrycount is not None:
+            if not isinstance(retrycount, int):
+                raise DataError("XCLAIM retrycount must be an integer")
+            pieces.extend((b"RETRYCOUNT", str(retrycount)))
+
+        if force:
+            if not isinstance(force, bool):
+                raise DataError("XCLAIM force must be a boolean")
+            pieces.append(b"FORCE")
+        if justid:
+            if not isinstance(justid, bool):
+                raise DataError("XCLAIM justid must be a boolean")
+            pieces.append(b"JUSTID")
+            kwargs["parse_justid"] = True
+        return self.execute_command("XCLAIM", *pieces, **kwargs)
+
+    def xdel(self, name: KeyT, *ids: StreamIdT) -> Awaitable:
+        """
+        Deletes one or more messages from a stream.
+        name: name of the stream.
+        *ids: message ids to delete.
+        """
+        return self.execute_command("XDEL", name, *ids)
+
+    def xgroup_create(
+        self, name: KeyT, groupname: GroupT, id: StreamIdT = "$", mkstream: bool = False
+    ) -> Awaitable:
+        """
+        Create a new consumer group associated with a stream.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        id: ID of the last item in the stream to consider already delivered.
+        """
+        pieces: List[EncodableT] = ["XGROUP CREATE", name, groupname, id]
+        if mkstream:
+            pieces.append(b"MKSTREAM")
+        return self.execute_command(*pieces)
+
+    def xgroup_delconsumer(
+        self, name: KeyT, groupname: GroupT, consumername: ConsumerT
+    ) -> Awaitable:
+        """
+        Remove a specific consumer from a consumer group.
+        Returns the number of pending messages that the consumer had before it
+        was deleted.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        consumername: name of consumer to delete
+        """
+        return self.execute_command("XGROUP DELCONSUMER", name, groupname, consumername)
+
+    def xgroup_destroy(self, name: KeyT, groupname: GroupT) -> Awaitable:
+        """
+        Destroy a consumer group.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        """
+        return self.execute_command("XGROUP DESTROY", name, groupname)
+
+    def xgroup_setid(self, name: KeyT, groupname: GroupT, id: StreamIdT) -> Awaitable:
+        """
+        Set the consumer group last delivered ID to something else.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        id: ID of the last item in the stream to consider already delivered.
+        """
+        return self.execute_command("XGROUP SETID", name, groupname, id)
+
+    def xinfo_consumers(self, name: KeyT, groupname: GroupT) -> Awaitable:
+        """
+        Returns general information about the consumers in the group.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        """
+        return self.execute_command("XINFO CONSUMERS", name, groupname)
+
+    def xinfo_groups(self, name: KeyT) -> Awaitable:
+        """
+        Returns general information about the consumer groups of the stream.
+        name: name of the stream.
+        """
+        return self.execute_command("XINFO GROUPS", name)
+
+    def xinfo_stream(self, name: KeyT) -> Awaitable:
+        """
+        Returns general information about the stream.
+        name: name of the stream.
+        """
+        return self.execute_command("XINFO STREAM", name)
+
+    def xlen(self, name: KeyT) -> Awaitable:
+        """
+        Returns the number of elements in a given stream.
+        """
+        return self.execute_command("XLEN", name)
+
+    def xpending(self, name: KeyT, groupname: GroupT) -> Awaitable:
+        """
+        Returns information about pending messages of a group.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        """
+        return self.execute_command("XPENDING", name, groupname)
+
+    def xpending_range(
+        self,
+        name: KeyT,
+        groupname: GroupT,
+        min: Optional[StreamIdT],
+        max: Optional[StreamIdT],
+        count: Optional[int],
+        consumername: Optional[ConsumerT] = None,
+    ) -> Awaitable:
+        """
+        Returns information about pending messages, in a range.
+        name: name of the stream.
+        groupname: name of the consumer group.
+        min: minimum stream ID.
+        max: maximum stream ID.
+        count: number of messages to return
+        consumername: name of a consumer to filter by (optional).
+        """
+        pieces: List[EncodableT] = [name, groupname]
+        if min is not None or max is not None or count is not None:
+            if min is None or max is None or count is None:
+                raise DataError(
+                    "XPENDING must be provided with min, max "
+                    "and count parameters, or none of them. "
+                )
+            if not isinstance(count, int) or count < -1:
+                raise DataError("XPENDING count must be a integer >= -1")
+            pieces.extend((min, max, str(count)))
+        if consumername is not None:
+            if min is None or max is None or count is None:
+                raise DataError(
+                    "if XPENDING is provided with consumername,"
+                    " it must be provided with min, max and"
+                    " count parameters"
+                )
+            pieces.append(consumername)
+        return self.execute_command("XPENDING", *pieces, parse_detail=True)
+
+    def xrange(
+        self,
+        name: KeyT,
+        min: StreamIdT = "-",
+        max: StreamIdT = "+",
+        count: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Read stream values within an interval.
+        name: name of the stream.
+        start: first stream ID. defaults to '-',
+               meaning the earliest available.
+        finish: last stream ID. defaults to '+',
+                meaning the latest available.
+        count: if set, only return this many items, beginning with the
+               earliest available.
+        """
+        pieces: List[EncodableT] = [min, max]
+        if count is not None:
+            if not isinstance(count, int) or count < 1:
+                raise DataError("XRANGE count must be a positive integer")
+            pieces.append(b"COUNT")
+            pieces.append(str(count))
+
+        return self.execute_command("XRANGE", name, *pieces)
+
+    def xread(
+        self,
+        streams: Dict[KeyT, StreamIdT],
+        count: Optional[int] = None,
+        block: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Block and monitor multiple streams for new data.
+        streams: a dict of stream names to stream IDs, where
+                   IDs indicate the last ID already seen.
+        count: if set, only return this many items, beginning with the
+               earliest available.
+        block: number of milliseconds to wait, if nothing already present.
+        """
+        pieces: List[EncodableT] = []
+        if block is not None:
+            if not isinstance(block, int) or block < 0:
+                raise DataError("XREAD block must be a non-negative integer")
+            pieces.append(b"BLOCK")
+            pieces.append(str(block))
+        if count is not None:
+            if not isinstance(count, int) or count < 1:
+                raise DataError("XREAD count must be a positive integer")
+            pieces.append(b"COUNT")
+            pieces.append(str(count))
+        if not isinstance(streams, dict) or len(streams) == 0:
+            raise DataError("XREAD streams must be a non empty dict")
+        pieces.append(b"STREAMS")
+        keys, values = zip(*streams.items())
+        pieces.extend(keys)
+        pieces.extend(values)
+        return self.execute_command("XREAD", *pieces)
+
+    def xreadgroup(
+        self,
+        groupname: str,
+        consumername: str,
+        streams: Dict[KeyT, StreamIdT],
+        count: Optional[int] = None,
+        block: Optional[int] = None,
+        noack: bool = False,
+    ) -> Awaitable:
+        """
+        Read from a stream via a consumer group.
+        groupname: name of the consumer group.
+        consumername: name of the requesting consumer.
+        streams: a dict of stream names to stream IDs, where
+               IDs indicate the last ID already seen.
+        count: if set, only return this many items, beginning with the
+               earliest available.
+        block: number of milliseconds to wait, if nothing already present.
+        noack: do not add messages to the PEL
+        """
+        pieces: List[EncodableT] = [b"GROUP", groupname, consumername]
+        if count is not None:
+            if not isinstance(count, int) or count < 1:
+                raise DataError("XREADGROUP count must be a positive integer")
+            pieces.append(b"COUNT")
+            pieces.append(str(count))
+        if block is not None:
+            if not isinstance(block, int) or block < 0:
+                raise DataError("XREADGROUP block must be a non-negative " "integer")
+            pieces.append(b"BLOCK")
+            pieces.append(str(block))
+        if noack:
+            pieces.append(b"NOACK")
+        if not isinstance(streams, dict) or len(streams) == 0:
+            raise DataError("XREADGROUP streams must be a non empty dict")
+        pieces.append(b"STREAMS")
+        pieces.extend(streams.keys())
+        pieces.extend(streams.values())
+        return self.execute_command("XREADGROUP", *pieces)
+
+    def xrevrange(
+        self,
+        name: KeyT,
+        max: StreamIdT = "+",
+        min: StreamIdT = "-",
+        count: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Read stream values within an interval, in reverse order.
+        name: name of the stream
+        start: first stream ID. defaults to '+',
+               meaning the latest available.
+        finish: last stream ID. defaults to '-',
+                meaning the earliest available.
+        count: if set, only return this many items, beginning with the
+               latest available.
+        """
+        pieces: List[EncodableT] = [max, min]
+        if count is not None:
+            if not isinstance(count, int) or count < 1:
+                raise DataError("XREVRANGE count must be a positive integer")
+            pieces.append(b"COUNT")
+            pieces.append(str(count))
+
+        return self.execute_command("XREVRANGE", name, *pieces)
+
+    def xtrim(self, name: KeyT, maxlen: int, approximate: bool = True) -> Awaitable:
+        """
+        Trims old messages from a stream.
+        name: name of the stream.
+        maxlen: truncate old stream messages beyond this size
+        approximate: actual stream length may be slightly more than maxlen
+        """
+        pieces: List[EncodableT] = [b"MAXLEN"]
+        if approximate:
+            pieces.append(b"~")
+        pieces.append(maxlen)
+        return self.execute_command("XTRIM", name, *pieces)
+
+    # SORTED SET COMMANDS
+    def zadd(
+        self,
+        name: KeyT,
+        mapping: Mapping[AnyKeyT, EncodableT],
+        nx: bool = False,
+        xx: bool = False,
+        ch: bool = False,
+        incr: bool = False,
+    ) -> Awaitable:
+        """
+        Set any number of element-name, score pairs to the key ``name``. Pairs
+        are specified as a dict of element-names keys to score values.
+
+        ``nx`` forces ZADD to only create new elements and not to update
+        scores for elements that already exist.
+
+        ``xx`` forces ZADD to only update scores of elements that already
+        exist. New elements will not be added.
+
+        ``ch`` modifies the return value to be the numbers of elements changed.
+        Changed elements include new elements that were added and elements
+        whose scores changed.
+
+        ``incr`` modifies ZADD to behave like ZINCRBY. In this mode only a
+        single element/score pair can be specified and the score is the amount
+        the existing score will be incremented by. When using this mode the
+        return value of ZADD will be the new score of the element.
+
+        The return value of ZADD varies based on the mode specified. With no
+        options, ZADD returns the number of new elements added to the sorted
+        set.
+        """
+        if not mapping:
+            raise DataError("ZADD requires at least one element/score pair")
+        if nx and xx:
+            raise DataError("ZADD allows either 'nx' or 'xx', not both")
+        if incr and len(mapping) != 1:
+            raise DataError(
+                "ZADD option 'incr' only works when passing a "
+                "single element/score pair"
+            )
+        pieces: List[EncodableT] = []
+        options = {}
+        if nx:
+            pieces.append(b"NX")
+        if xx:
+            pieces.append(b"XX")
+        if ch:
+            pieces.append(b"CH")
+        if incr:
+            pieces.append(b"INCR")
+            options["as_score"] = True
+        for pair in mapping.items():
+            pieces.append(pair[1])
+            pieces.append(pair[0])
+        return self.execute_command("ZADD", name, *pieces, **options)
+
+    def zcard(self, name: KeyT) -> Awaitable:
+        """Return the number of elements in the sorted set ``name``"""
+        return self.execute_command("ZCARD", name)
+
+    def zcount(self, name: KeyT, min: ZScoreBoundT, max: ZScoreBoundT) -> Awaitable:
+        """
+        Returns the number of elements in the sorted set at key ``name`` with
+        a score between ``min`` and ``max``.
+        """
+        return self.execute_command("ZCOUNT", name, min, max)
+
+    def zincrby(self, name: KeyT, amount: float, value: EncodableT) -> Awaitable:
+        """Increment the score of ``value`` in sorted set ``name`` by ``amount``"""
+        return self.execute_command("ZINCRBY", name, amount, value)
+
+    def zinterstore(
+        self,
+        dest: KeyT,
+        keys: Union[Sequence[KeyT], Mapping[AnyKeyT, float]],
+        aggregate: Optional[str] = None,
+    ) -> Awaitable:
+        """
+        Intersect multiple sorted sets specified by ``keys`` into
+        a new sorted set, ``dest``. Scores in the destination will be
+        aggregated based on the ``aggregate``, or SUM if none is provided.
+        """
+        return self._zaggregate("ZINTERSTORE", dest, keys, aggregate)
+
+    def zlexcount(self, name: KeyT, min: EncodableT, max: EncodableT) -> Awaitable:
+        """
+        Return the number of items in the sorted set ``name`` between the
+        lexicographical range ``min`` and ``max``.
+        """
+        return self.execute_command("ZLEXCOUNT", name, min, max)
+
+    def zpopmax(self, name: KeyT, count: Optional[int] = None) -> Awaitable:
+        """
+        Remove and return up to ``count`` members with the highest scores
+        from the sorted set ``name``.
+        """
+        args = (count is not None) and [count] or []
+        options = {"withscores": True}
+        return self.execute_command("ZPOPMAX", name, *args, **options)
+
+    def zpopmin(self, name: KeyT, count: Optional[int] = None) -> Awaitable:
+        """
+        Remove and return up to ``count`` members with the lowest scores
+        from the sorted set ``name``.
+        """
+        args = (count is not None) and [count] or []
+        options = {"withscores": True}
+        return self.execute_command("ZPOPMIN", name, *args, **options)
+
+    def bzpopmax(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
+        """
+        ZPOPMAX a value off of the first non-empty sorted set
+        named in the ``keys`` list.
+
+        If none of the sorted sets in ``keys`` has a value to ZPOPMAX,
+        then block for ``timeout`` seconds, or until a member gets added
+        to one of the sorted sets.
+
+        If timeout is 0, then block indefinitely.
+        """
+        parsed_keys = list_or_args(keys, (timeout,))
+        return self.execute_command("BZPOPMAX", *parsed_keys)
+
+    def bzpopmin(self, keys: KeysT, timeout: TimeoutSecT = 0) -> Awaitable:
+        """
+        ZPOPMIN a value off of the first non-empty sorted set
+        named in the ``keys`` list.
+
+        If none of the sorted sets in ``keys`` has a value to ZPOPMIN,
+        then block for ``timeout`` seconds, or until a member gets added
+        to one of the sorted sets.
+
+        If timeout is 0, then block indefinitely.
+        """
+        klist: List[EncodableT] = list_or_args(keys, None)
+        klist.append(timeout)
+        return self.execute_command("BZPOPMIN", *klist)
+
+    def zrange(
+        self,
+        name: KeyT,
+        start: int,
+        end: int,
+        desc: bool = False,
+        withscores: bool = False,
+        score_cast_func: Union[Type, Callable] = float,
+    ) -> Awaitable:
+        """
+        Return a range of values from sorted set ``name`` between
+        ``start`` and ``end`` sorted in ascending order.
+
+        ``start`` and ``end`` can be negative, indicating the end of the range.
+
+        ``desc`` a boolean indicating whether to sort the results descendingly
+
+        ``withscores`` indicates to return the scores along with the values.
+        The return type is a list of (value, score) pairs
+
+        ``score_cast_func`` a callable used to cast the score return value
+        """
+        if desc:
+            return self.zrevrange(name, start, end, withscores, score_cast_func)
+        pieces: List[EncodableT] = ["ZRANGE", name, start, end]
+        if withscores:
+            pieces.append(b"WITHSCORES")
+        options = {"withscores": withscores, "score_cast_func": score_cast_func}
+        return self.execute_command(*pieces, **options)
+
+    def zrangebylex(
+        self,
+        name: KeyT,
+        min: EncodableT,
+        max: EncodableT,
+        start: Optional[int] = None,
+        num: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Return the lexicographical range of values from sorted set ``name``
+        between ``min`` and ``max``.
+
+        If ``start`` and ``num`` are specified, then return a slice of the
+        range.
+        """
+        if (start is not None and num is None) or (num is not None and start is None):
+            raise DataError("``start`` and ``num`` must both be specified")
+        pieces: List[EncodableT] = ["ZRANGEBYLEX", name, min, max]
+        if start is not None and num is not None:
+            pieces.extend([b"LIMIT", start, num])
+        return self.execute_command(*pieces)
+
+    def zrevrangebylex(
+        self,
+        name: KeyT,
+        max: EncodableT,
+        min: EncodableT,
+        start: Optional[int] = None,
+        num: Optional[int] = None,
+    ) -> Awaitable:
+        """
+        Return the reversed lexicographical range of values from sorted set
+        ``name`` between ``max`` and ``min``.
+
+        If ``start`` and ``num`` are specified, then return a slice of the
+        range.
+        """
+        if (start is not None and num is None) or (num is not None and start is None):
+            raise DataError("``start`` and ``num`` must both be specified")
+        pieces: List[EncodableT] = ["ZREVRANGEBYLEX", name, max, min]
+        if start is not None and num is not None:
+            pieces.extend([b"LIMIT", start, num])
+        return self.execute_command(*pieces)
+
+    def zrangebyscore(
+        self,
+        name: KeyT,
+        min: ZScoreBoundT,
+        max: ZScoreBoundT,
+        start: Optional[int] = None,
+        num: Optional[int] = None,
+        withscores: bool = False,
+        score_cast_func: Union[Type, Callable] = float,
+    ) -> Awaitable:
+        """
+        Return a range of values from the sorted set ``name`` with scores
+        between ``min`` and ``max``.
+
+        If ``start`` and ``num`` are specified, then return a slice
+        of the range.
+
+        ``withscores`` indicates to return the scores along with the values.
+        The return type is a list of (value, score) pairs
+
+        `score_cast_func`` a callable used to cast the score return value
+        """
+        if (start is not None and num is None) or (num is not None and start is None):
+            raise DataError("``start`` and ``num`` must both be specified")
+        pieces: List[EncodableT] = ["ZRANGEBYSCORE", name, min, max]
+        if start is not None and num is not None:
+            pieces.extend([b"LIMIT", start, num])
+        if withscores:
+            pieces.append(b"WITHSCORES")
+        options = {"withscores": withscores, "score_cast_func": score_cast_func}
+        return self.execute_command(*pieces, **options)
+
+    def zrank(self, name: KeyT, value: EncodableT) -> Awaitable:
+        """
+        Returns a 0-based value indicating the rank of ``value`` in sorted set
+        ``name``
+        """
+        return self.execute_command("ZRANK", name, value)
+
+    def zrem(self, name: KeyT, *values: EncodableT) -> Awaitable:
+        """Remove member ``values`` from sorted set ``name``"""
+        return self.execute_command("ZREM", name, *values)
+
+    def zremrangebylex(self, name: KeyT, min: EncodableT, max: EncodableT) -> Awaitable:
+        """
+        Remove all elements in the sorted set ``name`` between the
+        lexicographical range specified by ``min`` and ``max``.
+
+        Returns the number of elements removed.
+        """
+        return self.execute_command("ZREMRANGEBYLEX", name, min, max)
+
+    def zremrangebyrank(self, name: KeyT, min: int, max: int) -> Awaitable:
+        """
+        Remove all elements in the sorted set ``name`` with ranks between
+        ``min`` and ``max``. Values are 0-based, ordered from smallest score
+        to largest. Values can be negative indicating the highest scores.
+        Returns the number of elements removed
+        """
+        return self.execute_command("ZREMRANGEBYRANK", name, min, max)
+
+    def zremrangebyscore(
+        self, name: KeyT, min: ZScoreBoundT, max: ZScoreBoundT
+    ) -> Awaitable:
+        """
+        Remove all elements in the sorted set ``name`` with scores
+        between ``min`` and ``max``. Returns the number of elements removed.
+        """
+        return self.execute_command("ZREMRANGEBYSCORE", name, min, max)
+
+    def zrevrange(
+        self,
+        name: KeyT,
+        start: int,
+        end: int,
+        withscores: bool = False,
+        score_cast_func: Union[Type, Callable] = float,
+    ) -> Awaitable:
+        """
+        Return a range of values from sorted set ``name`` between
+        ``start`` and ``end`` sorted in descending order.
+
+        ``start`` and ``end`` can be negative, indicating the end of the range.
+
+        ``withscores`` indicates to return the scores along with the values
+        The return type is a list of (value, score) pairs
+
+        ``score_cast_func`` a callable used to cast the score return value
+        """
+        pieces: List[EncodableT] = ["ZREVRANGE", name, start, end]
+        if withscores:
+            pieces.append(b"WITHSCORES")
+        options = {"withscores": withscores, "score_cast_func": score_cast_func}
+        return self.execute_command(*pieces, **options)
+
+    def zrevrangebyscore(
+        self,
+        name: KeyT,
+        min: ZScoreBoundT,
+        max: ZScoreBoundT,
+        start: Optional[int] = None,
+        num: Optional[int] = None,
+        withscores: bool = False,
+        score_cast_func: Union[Type, Callable] = float,
+    ) -> Awaitable:
+        """
+        Return a range of values from the sorted set ``name`` with scores
+        between ``min`` and ``max`` in descending order.
+
+        If ``start`` and ``num`` are specified, then return a slice
+        of the range.
+
+        ``withscores`` indicates to return the scores along with the values.
+        The return type is a list of (value, score) pairs
+
+        ``score_cast_func`` a callable used to cast the score return value
+        """
+        if (start is not None and num is None) or (num is not None and start is None):
+            raise DataError("``start`` and ``num`` must both be specified")
+        pieces: List[EncodableT] = ["ZREVRANGEBYSCORE", name, min, max]
+        if start is not None and num is not None:
+            pieces.extend([b"LIMIT", start, num])
+        if withscores:
+            pieces.append(b"WITHSCORES")
+        options = {"withscores": withscores, "score_cast_func": score_cast_func}
+        return self.execute_command(*pieces, **options)
+
+    def zrevrank(self, name: KeyT, value: EncodableT) -> Awaitable:
+        """
+        Returns a 0-based value indicating the descending rank of
+        ``value`` in sorted set ``name``
+        """
+        return self.execute_command("ZREVRANK", name, value)
+
+    def zscore(self, name: str, value: EncodableT) -> Awaitable:
+        """Return the score of element ``value`` in sorted set ``name``"""
+        return self.execute_command("ZSCORE", name, value)
+
+    def zunionstore(
+        self,
+        dest: KeyT,
+        keys: Union[Sequence[KeyT], Mapping[AnyKeyT, float]],
+        aggregate: Optional[str] = None,
+    ) -> Awaitable:
+        """
+        Union multiple sorted sets specified by ``keys`` into
+        a new sorted set, ``dest``. Scores in the destination will be
+        aggregated based on the ``aggregate``, or SUM if none is provided.
+        """
+        return self._zaggregate("ZUNIONSTORE", dest, keys, aggregate)
+
+    def _zaggregate(
+        self,
+        command: str,
+        dest: KeyT,
+        keys: Union[Sequence[KeyT], Mapping[AnyKeyT, float]],
+        aggregate: Optional[str] = None,
+    ) -> Awaitable:
+        pieces: List[EncodableT] = [command, dest, len(keys)]
+        key_names: Union[Sequence[KeyT], AbstractSet[AnyKeyT]]
+        weights: Optional[ValuesView[float]]
+        if isinstance(keys, Mapping):
+            key_names, weights = keys.keys(), keys.values()
+        else:
+            key_names = keys
+            weights = None
+        pieces.extend(key_names)
+        if weights:
+            pieces.append(b"WEIGHTS")
+            pieces.extend(weights)
+        if aggregate:
+            pieces.append(b"AGGREGATE")
+            pieces.append(aggregate)
+        return self.execute_command(*pieces)
+
+    # HYPERLOGLOG COMMANDS
+    def pfadd(self, name: KeyT, *values: EncodableT) -> Awaitable:
+        """Adds the specified elements to the specified HyperLogLog."""
+        return self.execute_command("PFADD", name, *values)
+
+    def pfcount(self, *sources: KeyT) -> Awaitable:
+        """
+        Return the approximated cardinality of
+        the set observed by the HyperLogLog at key(s).
+        """
+        return self.execute_command("PFCOUNT", *sources)
+
+    def pfmerge(self, dest: KeyT, *sources: KeyT) -> Awaitable:
+        """Merge N different HyperLogLogs into a single one."""
+        return self.execute_command("PFMERGE", dest, *sources)
+
+    # HASH COMMANDS
+    def hdel(self, name: KeyT, *keys: FieldT) -> Awaitable:
+        """Delete ``keys`` from hash ``name``"""
+        return self.execute_command("HDEL", name, *keys)
+
+    def hexists(self, name: KeyT, key: FieldT) -> Awaitable:
+        """Returns a boolean indicating if ``key`` exists within hash ``name``"""
+        return self.execute_command("HEXISTS", name, key)
+
+    def hget(self, name: KeyT, key: FieldT) -> Awaitable:
+        """Return the value of ``key`` within the hash ``name``"""
+        return self.execute_command("HGET", name, key)
+
+    def hgetall(self, name: KeyT) -> Awaitable:
+        """Return a Python dict of the hash's name/value pairs"""
+        return self.execute_command("HGETALL", name)
+
+    def hincrby(self, name: KeyT, key: FieldT, amount: int = 1) -> Awaitable:
+        """Increment the value of ``key`` in hash ``name`` by ``amount``"""
+        return self.execute_command("HINCRBY", name, key, amount)
+
+    def hincrbyfloat(self, name: KeyT, key: FieldT, amount: float = 1.0) -> Awaitable:
+        """
+        Increment the value of ``key`` in hash ``name`` by floating ``amount``
+        """
+        return self.execute_command("HINCRBYFLOAT", name, key, amount)
+
+    def hkeys(self, name: KeyT) -> Awaitable:
+        """Return the list of keys within hash ``name``"""
+        return self.execute_command("HKEYS", name)
+
+    def hlen(self, name: KeyT) -> Awaitable:
+        """Return the number of elements in hash ``name``"""
+        return self.execute_command("HLEN", name)
+
+    def hset(
+        self,
+        name: KeyT,
+        key: Optional[FieldT] = None,
+        value: Optional[EncodableT] = None,
+        mapping: Optional[Mapping[AnyFieldT, EncodableT]] = None,
+    ) -> Awaitable:
+        """
+        Set ``key`` to ``value`` within hash ``name``,
+        ``mapping`` accepts a dict of key/value pairs that that will be
+        added to hash ``name``.
+        Returns the number of fields that were added.
+        """
+        if key is None and not mapping:
+            raise DataError("'hset' with no key value pairs")
+        items: List[Union[FieldT, Optional[EncodableT]]] = []
+        if key is not None:
+            items.extend((key, value))
+        if mapping:
+            for pair in mapping.items():
+                items.extend(pair)
+
+        return self.execute_command("HSET", name, *items)
+
+    def hsetnx(self, name: KeyT, key: FieldT, value: EncodableT) -> Awaitable:
+        """
+        Set ``key`` to ``value`` within hash ``name`` if ``key`` does not
+        exist.  Returns 1 if HSETNX created a field, otherwise 0.
+        """
+        return self.execute_command("HSETNX", name, key, value)
+
+    def hmset(self, name: KeyT, mapping: Mapping[AnyFieldT, EncodableT]) -> Awaitable:
+        """
+        Set key to value within hash ``name`` for each corresponding
+        key and value from the ``mapping`` dict.
+        """
+        warnings.warn(
+            f"{self.__class__.__name__}.hmset() is deprecated. "
+            f"Use {self.__class__.__name__}.hset() instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        if not mapping:
+            raise DataError("'hmset' with 'mapping' of length 0")
+        items: List[Union[AnyFieldT, EncodableT]] = []
+        for pair in mapping.items():
+            items.extend(pair)
+        return self.execute_command("HMSET", name, *items)
+
+    def hmget(self, name: KeyT, keys: Sequence[KeyT], *args: FieldT) -> Awaitable:
+        """Returns a list of values ordered identically to ``keys``"""
+        parsed_args = list_or_args(keys, args)
+        return self.execute_command("HMGET", name, *parsed_args)
+
+    def hvals(self, name: KeyT) -> Awaitable:
+        """Return the list of values within hash ``name``"""
+        return self.execute_command("HVALS", name)
+
+    def hstrlen(self, name: KeyT, key: FieldT) -> Awaitable:
+        """
+        Return the number of bytes stored in the value of ``key``
+        within hash ``name``
+        """
+        return self.execute_command("HSTRLEN", name, key)
+
+    def publish(self, channel: ChannelT, message: EncodableT) -> Awaitable:
+        """
+        Publish ``message`` on ``channel``.
+        Returns the number of subscribers the message was delivered to.
+        """
+        return self.execute_command("PUBLISH", channel, message)
+
+    def pubsub_channels(self, pattern: PatternT = "*") -> Awaitable:
+        """
+        Return a list of channels that have at least one subscriber
+        """
+        return self.execute_command("PUBSUB CHANNELS", pattern)
+
+    def pubsub_numpat(self) -> Awaitable:
+        """
+        Returns the number of subscriptions to patterns
+        """
+        return self.execute_command("PUBSUB NUMPAT")
+
+    def pubsub_numsub(self, *args: ChannelT) -> Awaitable:
+        """
+        Return a list of (channel, number of subscribers) tuples
+        for each channel given in ``*args``
+        """
+        return self.execute_command("PUBSUB NUMSUB", *args)
+
+    def cluster(self, cluster_arg: str, *args: str) -> Awaitable:
+        return self.execute_command(f"CLUSTER {cluster_arg.upper()}", *args)
+
+    def eval(
+        self, script: ScriptTextT, numkeys: int, *keys_and_args: EncodableT
+    ) -> Awaitable:
+        """
+        Execute the Lua ``script``, specifying the ``numkeys`` the script
+        will touch and the key names and argument values in ``keys_and_args``.
+        Returns the result of the script.
+
+        In practice, use the object returned by ``register_script``. This
+        function exists purely for Redis API completion.
+        """
+        return self.execute_command("EVAL", script, numkeys, *keys_and_args)
+
+    def evalsha(self, sha: str, numkeys: int, *keys_and_args: EncodableT) -> Awaitable:
+        """
+        Use the ``sha`` to execute a Lua script already registered via EVAL
+        or SCRIPT LOAD. Specify the ``numkeys`` the script will touch and the
+        key names and argument values in ``keys_and_args``. Returns the result
+        of the script.
+
+        In practice, use the object returned by ``register_script``. This
+        function exists purely for Redis API completion.
+        """
+        return self.execute_command("EVALSHA", sha, numkeys, *keys_and_args)
+
+    def script_exists(self, *args: str) -> Awaitable:
+        """
+        Check if a script exists in the script cache by specifying the SHAs of
+        each script as ``args``. Returns a list of boolean values indicating if
+        if each already script exists in the cache.
+        """
+        return self.execute_command("SCRIPT EXISTS", *args)
+
+    def script_flush(self) -> Awaitable:
+        """Flush all scripts from the script cache"""
+        return self.execute_command("SCRIPT FLUSH")
+
+    def script_kill(self) -> Awaitable:
+        """Kill the currently executing Lua script"""
+        return self.execute_command("SCRIPT KILL")
+
+    def script_load(self, script: ScriptTextT) -> Awaitable:
+        """Load a Lua ``script`` into the script cache. Returns the SHA."""
+        return self.execute_command("SCRIPT LOAD", script)
+
+    def register_script(self, script: ScriptTextT) -> "Script":
+        """
+        Register a Lua ``script`` specifying the ``keys`` it will touch.
+        Returns a Script object that is callable and hides the complexity of
+        deal with scripts, keys, and shas. This is the preferred way to work
+        with Lua scripts.
+        """
+        return Script(self, script)
+
+    # GEO COMMANDS
+    def geoadd(self, name: KeyT, *values: EncodableT) -> Awaitable:
+        """
+        Add the specified geospatial items to the specified key identified
+        by the ``name`` argument. The Geospatial items are given as ordered
+        members of the ``values`` argument, each item or place is formed by
+        the triad longitude, latitude and name.
+        """
+        if len(values) % 3 != 0:
+            raise DataError("GEOADD requires places with lon, lat and name values")
+        return self.execute_command("GEOADD", name, *values)
+
+    def geodist(
+        self, name: KeyT, place1: FieldT, place2: FieldT, unit: Optional[str] = None
+    ) -> Awaitable:
+        """
+        Return the distance between ``place1`` and ``place2`` members of the
+        ``name`` key.
+        The units must be one of the following : m, km mi, ft. By default
+        meters are used.
+        """
+        pieces: List[EncodableT] = [name, place1, place2]
+        if unit and unit not in ("m", "km", "mi", "ft"):
+            raise DataError("GEODIST invalid unit")
+        elif unit:
+            pieces.append(unit)
+        return self.execute_command("GEODIST", *pieces)
+
+    def geohash(self, name: KeyT, *values: FieldT) -> Awaitable:
+        """
+        Return the geo hash string for each item of ``values`` members of
+        the specified key identified by the ``name`` argument.
+        """
+        return self.execute_command("GEOHASH", name, *values)
+
+    def geopos(self, name: KeyT, *values: FieldT) -> Awaitable:
+        """
+        Return the positions of each item of ``values`` as members of
+        the specified key identified by the ``name`` argument. Each position
+        is represented by the pairs lon and lat.
+        """
+        return self.execute_command("GEOPOS", name, *values)
+
+    def georadius(
+        self,
+        name: KeyT,
+        longitude: float,
+        latitude: float,
+        radius: float,
+        unit: Optional[str] = None,
+        withdist: bool = False,
+        withcoord: bool = False,
+        withhash: bool = False,
+        count: Optional[int] = None,
+        sort: Optional[str] = None,
+        store: Optional[KeyT] = None,
+        store_dist: Optional[KeyT] = None,
+    ) -> Awaitable:
+        """
+        Return the members of the specified key identified by the
+        ``name`` argument which are within the borders of the area specified
+        with the ``latitude`` and ``longitude`` location and the maximum
+        distance from the center specified by the ``radius`` value.
+
+        The units must be one of the following : m, km mi, ft. By default
+
+        ``withdist`` indicates to return the distances of each place.
+
+        ``withcoord`` indicates to return the latitude and longitude of
+        each place.
+
+        ``withhash`` indicates to return the geohash string of each place.
+
+        ``count`` indicates to return the number of elements up to N.
+
+        ``sort`` indicates to return the places in a sorted way, ASC for
+        nearest to fairest and DESC for fairest to nearest.
+
+        ``store`` indicates to save the places names in a sorted set named
+        with a specific key, each element of the destination sorted set is
+        populated with the score got from the original geo sorted set.
+
+        ``store_dist`` indicates to save the places names in a sorted set
+        named with a specific key, instead of ``store`` the sorted set
+        destination score is set with the distance.
+        """
+        return self._georadiusgeneric(
+            "GEORADIUS",
+            name,
+            longitude,
+            latitude,
+            radius,
+            unit=unit,
+            withdist=withdist,
+            withcoord=withcoord,
+            withhash=withhash,
+            count=count,
+            sort=sort,
+            store=store,
+            store_dist=store_dist,
+        )
+
+    def georadiusbymember(
+        self,
+        name: KeyT,
+        member: FieldT,
+        radius: float,
+        unit: Optional[str] = None,
+        withdist: bool = False,
+        withcoord: bool = False,
+        withhash: bool = False,
+        count: Optional[int] = None,
+        sort: Optional[str] = None,
+        store: Optional[KeyT] = None,
+        store_dist: Optional[KeyT] = None,
+    ) -> Awaitable:
+        """
+        This command is exactly like ``georadius`` with the sole difference
+        that instead of taking, as the center of the area to query, a longitude
+        and latitude value, it takes the name of a member already existing
+        inside the geospatial index represented by the sorted set.
+        """
+        return self._georadiusgeneric(
+            "GEORADIUSBYMEMBER",
+            name,
+            member,
+            radius,
+            unit=unit,
+            withdist=withdist,
+            withcoord=withcoord,
+            withhash=withhash,
+            count=count,
+            sort=sort,
+            store=store,
+            store_dist=store_dist,
+        )
+
+    def _georadiusgeneric(
+        self, command: str, *args: EncodableT, **kwargs: Optional[EncodableT]
+    ) -> Awaitable:
+        pieces: List[Optional[EncodableT]] = list(args)
+        if kwargs["unit"] and kwargs["unit"] not in ("m", "km", "mi", "ft"):
+            raise DataError("GEORADIUS invalid unit")
+        elif kwargs["unit"]:
+            pieces.append(kwargs["unit"])
+        else:
+            pieces.append(
+                "m",
+            )
+
+        for arg_name, byte_repr in (
+            ("withdist", b"WITHDIST"),
+            ("withcoord", b"WITHCOORD"),
+            ("withhash", b"WITHHASH"),
+        ):
+            if kwargs[arg_name]:
+                pieces.append(byte_repr)
+
+        if kwargs["count"]:
+            pieces.extend([b"COUNT", kwargs["count"]])
+
+        if kwargs["sort"]:
+            if kwargs["sort"] == "ASC":
+                pieces.append(b"ASC")
+            elif kwargs["sort"] == "DESC":
+                pieces.append(b"DESC")
+            else:
+                raise DataError("GEORADIUS invalid sort")
+
+        if kwargs["store"] and kwargs["store_dist"]:
+            raise DataError("GEORADIUS store and store_dist cant be set" " together")
+
+        if kwargs["store"]:
+            pieces.extend([b"STORE", kwargs["store"]])
+
+        if kwargs["store_dist"]:
+            pieces.extend([b"STOREDIST", kwargs["store_dist"]])
+
+        return self.execute_command(command, *pieces, **kwargs)
+
+    # MODULE COMMANDS
+    def module_load(self, path: str) -> Awaitable:
+        """
+        Loads the module from ``path``.
+        Raises ``ModuleError`` if a module is not found at ``path``.
+        """
+        return self.execute_command("MODULE LOAD", path)
+
+    def module_unload(self, name: str) -> Awaitable:
+        """
+        Unloads the module ``name``.
+        Raises ``ModuleError`` if ``name`` is not in loaded modules.
+        """
+        return self.execute_command("MODULE UNLOAD", name)
+
+    def module_list(self) -> Awaitable:
+        """
+        Returns a list of dictionaries containing the name and version of
+        all loaded modules.
+        """
+        return self.execute_command("MODULE LIST")
+
+
+StrictRedis = Redis
+
+
+class MonitorCommandInfo(TypedDict):
+    time: float
+    db: int
+    client_address: str
+    client_port: str
+    client_type: str
+    command: str
+
+
+class Monitor:
+    """
+    Monitor is useful for handling the MONITOR command to the redis server.
+    next_command() method returns one command from monitor
+    listen() method yields commands from monitor.
+    """
+
+    monitor_re = re.compile(r"\[(\d+) (.*)\] (.*)")
+    command_re = re.compile(r'"(.*?)(?<!\\)"')
+
+    def __init__(self, connection_pool: ConnectionPool):
+        self.connection_pool = connection_pool
+        self.connection: Optional[Connection] = None
+
+    async def connect(self):
+        if self.connection is None:
+            self.connection = await self.connection_pool.get_connection("MONITOR")
+
+    async def __aenter__(self):
+        await self.connect()
+        self.connection = cast(Connection, self.connection)  # Connected above.
+        await self.connection.send_command("MONITOR")
+        # check that monitor returns 'OK', but don't return it to user
+        response = await self.connection.read_response()
+        if not bool_ok(response):
+            raise RedisError(f"MONITOR failed: {response}")
+        return self
+
+    async def __aexit__(self, *args):
+        assert self.connection is not None
+        await self.connection.disconnect()
+        await self.connection_pool.release(self.connection)
+
+    async def next_command(self) -> MonitorCommandInfo:
+        """Parse the response from a monitor command"""
+        if self.connection is None:
+            raise RedisError("Connection already closed.")
+        await self.connect()
+        response = await self.connection.read_response()
+        if isinstance(response, bytes):
+            response = self.connection.encoder.decode(response, force=True)
+        command_time, command_data = response.split(" ", 1)
+        m = self.monitor_re.match(command_data)
+        if m is None:
+            raise RedisError("Invalid command received.")
+        db_id, client_info, command = m.groups()
+        command = " ".join(self.command_re.findall(command))
+        # Redis escapes double quotes because each piece of the command
+        # string is surrounded by double quotes. We don't have that
+        # requirement so remove the escaping and leave the quote.
+        command = command.replace('\\"', '"')
+
+        if client_info == "lua":
+            client_address = "lua"
+            client_port = ""
+            client_type = "lua"
+        elif client_info.startswith("unix"):
+            client_address = "unix"
+            client_port = client_info[5:]
+            client_type = "unix"
+        else:
+            # use rsplit as ipv6 addresses contain colons
+            client_address, client_port = client_info.rsplit(":", 1)
+            client_type = "tcp"
+        return {
+            "time": float(command_time),
+            "db": int(db_id),
+            "client_address": client_address,
+            "client_port": client_port,
+            "client_type": client_type,
+            "command": command,
+        }
+
+    async def listen(self) -> AsyncIterator[MonitorCommandInfo]:
+        """Listen for commands coming to the server."""
+        while True:
+            yield await self.next_command()
+
+
+class PubSub:
+    """
+    PubSub provides publish, subscribe and listen support to Redis channels.
+
+    After subscribing to one or more channels, the listen() method will block
+    until a message arrives on one of the subscribed channels. That message
+    will be returned and it's safe to start listening again.
+    """
+
+    PUBLISH_MESSAGE_TYPES = ("message", "pmessage")
+    UNSUBSCRIBE_MESSAGE_TYPES = ("unsubscribe", "punsubscribe")
+    HEALTH_CHECK_MESSAGE = "aioredis-py-health-check"
+
+    def __init__(
+        self,
+        connection_pool: ConnectionPool,
+        shard_hint: Optional[str] = None,
+        ignore_subscribe_messages: bool = False,
+    ):
+        self.connection_pool = connection_pool
+        self.shard_hint = shard_hint
+        self.ignore_subscribe_messages = ignore_subscribe_messages
+        self.connection: Optional[Connection] = None
+        # we need to know the encoding options for this connection in order
+        # to lookup channel and pattern names for callback handlers.
+        self.encoder = self.connection_pool.get_encoder()
+        if self.encoder.decode_responses:
+            self.health_check_response: Iterable[Union[str, bytes]] = [
+                "pong",
+                self.HEALTH_CHECK_MESSAGE,
+            ]
+        else:
+            self.health_check_response = [
+                b"pong",
+                self.encoder.encode(self.HEALTH_CHECK_MESSAGE),
+            ]
+        self.channels: Dict[ChannelT, PubSubHandler] = {}
+        self.pending_unsubscribe_channels: Set[ChannelT] = set()
+        self.patterns: Dict[ChannelT, PubSubHandler] = {}
+        self.pending_unsubscribe_patterns: Set[ChannelT] = set()
+        self._lock = asyncio.Lock()
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.reset()
+
+    def __del__(self):
+        if self.connection:
+            self.connection.clear_connect_callbacks()
+
+    async def reset(self):
+        async with self._lock:
+            if self.connection:
+                await self.connection.disconnect()
+                self.connection.clear_connect_callbacks()
+                await self.connection_pool.release(self.connection)
+                self.connection = None
+            self.channels = {}
+            self.pending_unsubscribe_channels = set()
+            self.patterns = {}
+            self.pending_unsubscribe_patterns = set()
+
+    def close(self) -> Awaitable[NoReturn]:
+        return self.reset()
+
+    async def on_connect(self, connection: Connection):
+        """Re-subscribe to any channels and patterns previously subscribed to"""
+        # NOTE: for python3, we can't pass bytestrings as keyword arguments
+        # so we need to decode channel/pattern names back to unicode strings
+        # before passing them to [p]subscribe.
+        self.pending_unsubscribe_channels.clear()
+        self.pending_unsubscribe_patterns.clear()
+        if self.channels:
+            channels = {}
+            for k, v in self.channels.items():
+                channels[self.encoder.decode(k, force=True)] = v
+            await self.subscribe(**channels)
+        if self.patterns:
+            patterns = {}
+            for k, v in self.patterns.items():
+                patterns[self.encoder.decode(k, force=True)] = v
+            await self.psubscribe(**patterns)
+
+    @property
+    def subscribed(self):
+        """Indicates if there are subscriptions to any channels or patterns"""
+        return bool(self.channels or self.patterns)
+
+    async def execute_command(self, *args: EncodableT):
+        """Execute a publish/subscribe command"""
+
+        # NOTE: don't parse the response in this function -- it could pull a
+        # legitimate message off the stack if the connection is already
+        # subscribed to one or more channels
+
+        if self.connection is None:
+            self.connection = await self.connection_pool.get_connection(
+                "pubsub", self.shard_hint
+            )
+            # register a callback that re-subscribes to any channels we
+            # were listening to when we were disconnected
+            self.connection.register_connect_callback(self.on_connect)
+        connection = self.connection
+        kwargs = {"check_health": not self.subscribed}
+        await self._execute(connection, connection.send_command, *args, **kwargs)
+
+    async def _execute(self, connection, command, *args, **kwargs):
+        try:
+            return await command(*args, **kwargs)
+        except (ConnectionError, TimeoutError) as e:
+            await connection.disconnect()
+            if not (connection.retry_on_timeout and isinstance(e, TimeoutError)):
+                raise
+            # Connect manually here. If the Redis server is down, this will
+            # fail and raise a ConnectionError as desired.
+            await connection.connect()
+            # the ``on_connect`` callback should haven been called by the
+            # connection to resubscribe us to any channels and patterns we were
+            # previously listening to
+            return await command(*args, **kwargs)
+
+    async def parse_response(self, block: bool = True, timeout: float = 0):
+        """Parse the response from a publish/subscribe command"""
+        conn = self.connection
+        if conn is None:
+            raise RuntimeError(
+                "pubsub connection not set: "
+                "did you forget to call subscribe() or psubscribe()?"
+            )
+
+        await self.check_health()
+
+        if not block and not await conn.can_read(timeout=timeout):
+            return None
+        response = await self._execute(conn, conn.read_response)
+
+        if conn.health_check_interval and response == self.health_check_response:
+            # ignore the health check message as user might not expect it
+            return None
+        return response
+
+    async def check_health(self):
+        conn = self.connection
+        if conn is None:
+            raise RuntimeError(
+                "pubsub connection not set: "
+                "did you forget to call subscribe() or psubscribe()?"
+            )
+
+        if (
+            conn.health_check_interval
+            and asyncio.get_event_loop().time() > conn.next_health_check
+        ):
+            await conn.send_command(
+                "PING", self.HEALTH_CHECK_MESSAGE, check_health=False
+            )
+
+    def _normalize_keys(self, data: _NormalizeKeysT) -> _NormalizeKeysT:
+        """
+        normalize channel/pattern names to be either bytes or strings
+        based on whether responses are automatically decoded. this saves us
+        from coercing the value for each message coming in.
+        """
+        encode = self.encoder.encode
+        decode = self.encoder.decode
+        return {decode(encode(k)): v for k, v in data.items()}  # type: ignore[return-value]
+
+    async def psubscribe(self, *args: ChannelT, **kwargs: PubSubHandler):
+        """
+        Subscribe to channel patterns. Patterns supplied as keyword arguments
+        expect a pattern name as the key and a callable as the value. A
+        pattern's callable will be invoked automatically when a message is
+        received on that pattern rather than producing a message via
+        ``listen()``.
+        """
+        parsed_args = list_or_args((args[0],), args[1:]) if args else args
+        new_patterns: Dict[ChannelT, PubSubHandler] = dict.fromkeys(parsed_args)
+        # Mypy bug: https://github.com/python/mypy/issues/10970
+        new_patterns.update(kwargs)  # type: ignore[arg-type]
+        ret_val = await self.execute_command("PSUBSCRIBE", *new_patterns.keys())
+        # update the patterns dict AFTER we send the command. we don't want to
+        # subscribe twice to these patterns, once for the command and again
+        # for the reconnection.
+        new_patterns = self._normalize_keys(new_patterns)
+        self.patterns.update(new_patterns)
+        self.pending_unsubscribe_patterns.difference_update(new_patterns)
+        return ret_val
+
+    def punsubscribe(self, *args: ChannelT) -> Awaitable:
+        """
+        Unsubscribe from the supplied patterns. If empty, unsubscribe from
+        all patterns.
+        """
+        patterns: Iterable[ChannelT]
+        if args:
+            parsed_args = list_or_args((args[0],), args[1:])
+            patterns = self._normalize_keys(dict.fromkeys(parsed_args)).keys()
+        else:
+            parsed_args = []
+            patterns = self.patterns
+        self.pending_unsubscribe_patterns.update(patterns)
+        return self.execute_command("PUNSUBSCRIBE", *parsed_args)
+
+    async def subscribe(self, *args: ChannelT, **kwargs: Callable):
+        """
+        Subscribe to channels. Channels supplied as keyword arguments expect
+        a channel name as the key and a callable as the value. A channel's
+        callable will be invoked automatically when a message is received on
+        that channel rather than producing a message via ``listen()`` or
+        ``get_message()``.
+        """
+        parsed_args = list_or_args((args[0],), args[1:]) if args else ()
+        new_channels = dict.fromkeys(parsed_args)
+        # Mypy bug: https://github.com/python/mypy/issues/10970
+        new_channels.update(kwargs)  # type: ignore[arg-type]
+        ret_val = await self.execute_command("SUBSCRIBE", *new_channels.keys())
+        # update the channels dict AFTER we send the command. we don't want to
+        # subscribe twice to these channels, once for the command and again
+        # for the reconnection.
+        new_channels = self._normalize_keys(new_channels)
+        self.channels.update(new_channels)
+        self.pending_unsubscribe_channels.difference_update(new_channels)
+        return ret_val
+
+    def unsubscribe(self, *args) -> Awaitable:
+        """
+        Unsubscribe from the supplied channels. If empty, unsubscribe from
+        all channels
+        """
+        if args:
+            parsed_args = list_or_args(args[0], args[1:])
+            channels = self._normalize_keys(dict.fromkeys(parsed_args))
+        else:
+            parsed_args = []
+            channels = self.channels
+        self.pending_unsubscribe_channels.update(channels)
+        return self.execute_command("UNSUBSCRIBE", *parsed_args)
+
+    async def listen(self) -> AsyncIterator:
+        """Listen for messages on channels this client has been subscribed to"""
+        while self.subscribed:
+            response = self.handle_message(await self.parse_response(block=True))
+            if response is not None:
+                yield response
+
+    async def get_message(
+        self, ignore_subscribe_messages: bool = False, timeout: float = 0.0
+    ):
+        """
+        Get the next message if one is available, otherwise None.
+
+        If timeout is specified, the system will wait for `timeout` seconds
+        before returning. Timeout should be specified as a floating point
+        number.
+        """
+        response = await self.parse_response(block=False, timeout=timeout)
+        if response:
+            return self.handle_message(response, ignore_subscribe_messages)
+        return None
+
+    def ping(self, message=None) -> Awaitable:
+        """
+        Ping the Redis server
+        """
+        message = "" if message is None else message
+        return self.execute_command("PING", message)
+
+    def handle_message(self, response, ignore_subscribe_messages=False):
+        """
+        Parses a pub/sub message. If the channel or pattern was subscribed to
+        with a message handler, the handler is invoked instead of a parsed
+        message being returned.
+        """
+        message_type = str_if_bytes(response[0])
+        if message_type == "pmessage":
+            message = {
+                "type": message_type,
+                "pattern": response[1],
+                "channel": response[2],
+                "data": response[3],
+            }
+        elif message_type == "pong":
+            message = {
+                "type": message_type,
+                "pattern": None,
+                "channel": None,
+                "data": response[1],
+            }
+        else:
+            message = {
+                "type": message_type,
+                "pattern": None,
+                "channel": response[1],
+                "data": response[2],
+            }
+
+        # if this is an unsubscribe message, remove it from memory
+        if message_type in self.UNSUBSCRIBE_MESSAGE_TYPES:
+            if message_type == "punsubscribe":
+                pattern = response[1]
+                if pattern in self.pending_unsubscribe_patterns:
+                    self.pending_unsubscribe_patterns.remove(pattern)
+                    self.patterns.pop(pattern, None)
+            else:
+                channel = response[1]
+                if channel in self.pending_unsubscribe_channels:
+                    self.pending_unsubscribe_channels.remove(channel)
+                    self.channels.pop(channel, None)
+
+        if message_type in self.PUBLISH_MESSAGE_TYPES:
+            # if there's a message handler, invoke it
+            if message_type == "pmessage":
+                handler = self.patterns.get(message["pattern"], None)
+            else:
+                handler = self.channels.get(message["channel"], None)
+            if handler:
+                handler(message)
+                return None
+        elif message_type != "pong":
+            # this is a subscribe/unsubscribe message. ignore if we don't
+            # want them
+            if ignore_subscribe_messages or self.ignore_subscribe_messages:
+                return None
+
+        return message
+
+    async def run(
+        self,
+        *,
+        exception_handler: Optional["PSWorkerThreadExcHandlerT"] = None,
+        poll_timeout: float = 1.0,
+    ) -> None:
+        """Process pub/sub messages using registered callbacks.
+
+        This is the equivalent of :py:meth:`redis.PubSub.run_in_thread` in
+        redis-py, but it is a coroutine. To launch it as a separate task, use
+        ``asyncio.create_task``:
+
+            >>> task = asyncio.create_task(pubsub.run())
+
+        To shut it down, use asyncio cancellation:
+
+            >>> task.cancel()
+            >>> await task
+        """
+        for channel, handler in self.channels.items():
+            if handler is None:
+                raise PubSubError(f"Channel: '{channel}' has no handler registered")
+        for pattern, handler in self.patterns.items():
+            if handler is None:
+                raise PubSubError(f"Pattern: '{pattern}' has no handler registered")
+
+        while True:
+            try:
+                await self.get_message(
+                    ignore_subscribe_messages=True, timeout=poll_timeout
+                )
+            except asyncio.CancelledError:
+                raise
+            except BaseException as e:
+                if exception_handler is None:
+                    raise
+                res = exception_handler(e, self)
+                if inspect.isawaitable(res):
+                    await res
+            # Ensure that other tasks on the event loop get a chance to run
+            # if we didn't have to block for I/O anywhere.
+            await asyncio.sleep(0)
+
+
+class PubsubWorkerExceptionHandler(Protocol):
+    def __call__(self, e: BaseException, pubsub: PubSub):
+        ...
+
+
+class AsyncPubsubWorkerExceptionHandler(Protocol):
+    async def __call__(self, e: BaseException, pubsub: PubSub):
+        ...
+
+
+PSWorkerThreadExcHandlerT = Union[
+    PubsubWorkerExceptionHandler, AsyncPubsubWorkerExceptionHandler
+]
+
+
+CommandT = Tuple[Tuple[Union[str, bytes], ...], Mapping[str, Any]]
+CommandStackT = List[CommandT]
+
+
+class Pipeline(Redis):  # lgtm [py/init-calls-subclass]
+    """
+    Pipelines provide a way to transmit multiple commands to the Redis server
+    in one transmission.  This is convenient for batch processing, such as
+    saving all the values in a list to Redis.
+
+    All commands executed within a pipeline are wrapped with MULTI and EXEC
+    calls. This guarantees all commands executed in the pipeline will be
+    executed atomically.
+
+    Any command raising an exception does *not* halt the execution of
+    subsequent commands in the pipeline. Instead, the exception is caught
+    and its instance is placed into the response list returned by execute().
+    Code iterating over the response list should be able to deal with an
+    instance of an exception as a potential value. In general, these will be
+    ResponseError exceptions, such as those raised when issuing a command
+    on a key of a different datatype.
+    """
+
+    UNWATCH_COMMANDS = {"DISCARD", "EXEC", "UNWATCH"}
+
+    def __init__(
+        self,
+        connection_pool: ConnectionPool,
+        response_callbacks: MutableMapping[Union[str, bytes], ResponseCallbackT],
+        transaction: bool,
+        shard_hint: Optional[str],
+    ):
+        self.connection_pool = connection_pool
+        self.connection = None
+        self.response_callbacks = response_callbacks
+        self.is_transaction = transaction
+        self.shard_hint = shard_hint
+        self.watching = False
+        self.command_stack: CommandStackT = []
+        self.scripts: Set[Script] = set()
+        self.explicit_transaction = False
+
+    async def __aenter__(self: _RedisT) -> _RedisT:
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.reset()
+
+    def __await__(self):
+        return self._async_self().__await__()
+
+    _DEL_MESSAGE = "Unclosed Pipeline client"
+
+    def __len__(self):
+        return len(self.command_stack)
+
+    def __bool__(self):
+        """Pipeline instances should always evaluate to True"""
+        return True
+
+    async def _async_self(self):
+        return self
+
+    async def reset(self):
+        self.command_stack = []
+        self.scripts = set()
+        # make sure to reset the connection state in the event that we were
+        # watching something
+        if self.watching and self.connection:
+            try:
+                # call this manually since our unwatch or
+                # immediate_execute_command methods can call reset()
+                await self.connection.send_command("UNWATCH")
+                await self.connection.read_response()
+            except ConnectionError:
+                # disconnect will also remove any previous WATCHes
+                if self.connection:
+                    await self.connection.disconnect()
+        # clean up the other instance attributes
+        self.watching = False
+        self.explicit_transaction = False
+        # we can safely return the connection to the pool here since we're
+        # sure we're no longer WATCHing anything
+        if self.connection:
+            await self.connection_pool.release(self.connection)
+            self.connection = None
+
+    def multi(self):
+        """
+        Start a transactional block of the pipeline after WATCH commands
+        are issued. End the transactional block with `execute`.
+        """
+        if self.explicit_transaction:
+            raise RedisError("Cannot issue nested calls to MULTI")
+        if self.command_stack:
+            raise RedisError(
+                "Commands without an initial WATCH have already " "been issued"
+            )
+        self.explicit_transaction = True
+
+    def execute_command(
+        self, *args, **kwargs
+    ) -> Union["Pipeline", Awaitable["Pipeline"]]:
+        if (self.watching or args[0] == "WATCH") and not self.explicit_transaction:
+            return self.immediate_execute_command(*args, **kwargs)
+        return self.pipeline_execute_command(*args, **kwargs)
+
+    async def immediate_execute_command(self, *args, **options):
+        """
+        Execute a command immediately, but don't auto-retry on a
+        ConnectionError if we're already WATCHing a variable. Used when
+        issuing WATCH or subsequent commands retrieving their values but before
+        MULTI is called.
+        """
+        command_name = args[0]
+        conn = self.connection
+        # if this is the first call, we need a connection
+        if not conn:
+            conn = await self.connection_pool.get_connection(
+                command_name, self.shard_hint
+            )
+            self.connection = conn
+        conn = cast(Connection, conn)
+        try:
+            await conn.send_command(*args)
+            return await self.parse_response(conn, command_name, **options)
+        except (ConnectionError, TimeoutError) as e:
+            await conn.disconnect()
+            # if we were already watching a variable, the watch is no longer
+            # valid since this connection has died. raise a WatchError, which
+            # indicates the user should retry this transaction.
+            if self.watching:
+                await self.reset()
+                raise WatchError(
+                    "A ConnectionError occurred on while watching one or more keys"
+                ) from e
+            # if retry_on_timeout is not set, or the error is not
+            # a TimeoutError, raise it
+            if not (conn.retry_on_timeout and isinstance(e, TimeoutError)):
+                await self.reset()
+                raise
+
+            # retry_on_timeout is set, this is a TimeoutError and we are not
+            # already WATCHing any variables. retry the command.
+            try:
+                await conn.send_command(*args)
+                return self.parse_response(conn, command_name, **options)
+            except (ConnectionError, TimeoutError):
+                # a subsequent failure should simply be raised
+                await self.reset()
+                raise
+        except asyncio.CancelledError:
+            await conn.disconnect()
+            raise
+
+    def pipeline_execute_command(self, *args, **options):
+        """
+        Stage a command to be executed when execute() is next called
+
+        Returns the current Pipeline object back so commands can be
+        chained together, such as:
+
+        pipe = pipe.set('foo', 'bar').incr('baz').decr('bang')
+
+        At some other point, you can then run: pipe.execute(),
+        which will execute all commands queued in the pipe.
+        """
+        self.command_stack.append((args, options))
+        return self
+
+    async def _execute_transaction(  # noqa: C901
+        self, connection: Connection, commands: CommandStackT, raise_on_error
+    ):
+        pre: CommandT = (("MULTI",), {})
+        post: CommandT = (("EXEC",), {})
+        cmds = (pre, *commands, post)
+        all_cmds = connection.pack_commands(
+            args for args, options in cmds if EMPTY_RESPONSE not in options
+        )
+        await connection.send_packed_command(all_cmds)
+        errors = []
+
+        # parse off the response for MULTI
+        # NOTE: we need to handle ResponseErrors here and continue
+        # so that we read all the additional command messages from
+        # the socket
+        try:
+            await self.parse_response(connection, "_")
+        except ResponseError as err:
+            errors.append((0, err))
+
+        # and all the other commands
+        for i, command in enumerate(commands):
+            if EMPTY_RESPONSE in command[1]:
+                errors.append((i, command[1][EMPTY_RESPONSE]))
+            else:
+                try:
+                    await self.parse_response(connection, "_")
+                except ResponseError as err:
+                    self.annotate_exception(err, i + 1, command[0])
+                    errors.append((i, err))
+
+        # parse the EXEC.
+        try:
+            response = await self.parse_response(connection, "_")
+        except ExecAbortError as err:
+            if errors:
+                raise errors[0][1] from err
+            raise
+
+        # EXEC clears any watched keys
+        self.watching = False
+
+        if response is None:
+            raise WatchError("Watched variable changed.") from None
+
+        # put any parse errors into the response
+        for i, e in errors:
+            response.insert(i, e)
+
+        if len(response) != len(commands):
+            if self.connection:
+                await self.connection.disconnect()
+            raise ResponseError(
+                "Wrong number of response items from pipeline execution"
+            ) from None
+
+        # find any errors in the response and raise if necessary
+        if raise_on_error:
+            self.raise_first_error(commands, response)
+
+        # We have to run response callbacks manually
+        data = []
+        for r, cmd in zip(response, commands):
+            if not isinstance(r, Exception):
+                args, options = cmd
+                command_name = args[0]
+                if command_name in self.response_callbacks:
+                    r = self.response_callbacks[command_name](r, **options)
+                    if inspect.isawaitable(r):
+                        r = await r
+            data.append(r)
+        return data
+
+    async def _execute_pipeline(
+        self, connection: Connection, commands: CommandStackT, raise_on_error: bool
+    ):
+        # build up all commands into a single request to increase network perf
+        all_cmds = connection.pack_commands([args for args, _ in commands])
+        await connection.send_packed_command(all_cmds)
+
+        response = []
+        for args, options in commands:
+            try:
+                response.append(
+                    await self.parse_response(connection, args[0], **options)
+                )
+            except ResponseError as e:
+                response.append(e)
+
+        if raise_on_error:
+            self.raise_first_error(commands, response)
+        return response
+
+    def raise_first_error(self, commands: CommandStackT, response: Iterable[Any]):
+        for i, r in enumerate(response):
+            if isinstance(r, ResponseError):
+                self.annotate_exception(r, i + 1, commands[i][0])
+                raise r
+
+    def annotate_exception(
+        self, exception: Exception, number: int, command: Iterable[object]
+    ) -> None:
+        cmd = " ".join(map(safe_str, command))
+        msg = f"Command # {number} ({cmd}) of pipeline caused error: {exception.args}"
+        exception.args = (msg,) + exception.args[1:]
+
+    def parse_response(
+        self, connection: Connection, command_name: Union[str, bytes], **options
+    ):
+        result = super().parse_response(connection, command_name, **options)
+        if command_name in self.UNWATCH_COMMANDS:
+            self.watching = False
+        elif command_name == "WATCH":
+            self.watching = True
+        return result
+
+    async def load_scripts(self):
+        # make sure all scripts that are about to be run on this pipeline exist
+        scripts = list(self.scripts)
+        immediate = self.immediate_execute_command
+        shas = [s.sha for s in scripts]
+        # we can't use the normal script_* methods because they would just
+        # get buffered in the pipeline.
+        exists = await immediate("SCRIPT EXISTS", *shas)
+        if not all(exists):
+            for s, exist in zip(scripts, exists):
+                if not exist:
+                    s.sha = await immediate("SCRIPT LOAD", s.script)
+
+    async def execute(self, raise_on_error: bool = True):
+        """Execute all the commands in the current pipeline"""
+        stack = self.command_stack
+        if not stack and not self.watching:
+            return []
+        if self.scripts:
+            await self.load_scripts()
+        if self.is_transaction or self.explicit_transaction:
+            execute = self._execute_transaction
+        else:
+            execute = self._execute_pipeline
+
+        conn = self.connection
+        if not conn:
+            conn = await self.connection_pool.get_connection("MULTI", self.shard_hint)
+            # assign to self.connection so reset() releases the connection
+            # back to the pool after we're done
+            self.connection = conn
+        conn = cast(Connection, conn)
+
+        try:
+            return await execute(conn, stack, raise_on_error)
+        except (ConnectionError, TimeoutError) as e:
+            await conn.disconnect()
+            # if we were watching a variable, the watch is no longer valid
+            # since this connection has died. raise a WatchError, which
+            # indicates the user should retry this transaction.
+            if self.watching:
+                raise WatchError(
+                    "A ConnectionError occurred on while " "watching one or more keys"
+                ) from e
+            # if retry_on_timeout is not set, or the error is not
+            # a TimeoutError, raise it
+            if not (conn.retry_on_timeout and isinstance(e, TimeoutError)):
+                raise
+            # retry a TimeoutError when retry_on_timeout is set
+            return await execute(conn, stack, raise_on_error)
+        finally:
+            await self.reset()
+
+    async def watch(self, *names: KeyT):
+        """Watches the values at keys ``names``"""
+        if self.explicit_transaction:
+            raise RedisError("Cannot issue a WATCH after a MULTI")
+        return await self.execute_command("WATCH", *names)
+
+    async def unwatch(self):
+        """Unwatches all previously specified keys"""
+        return self.watching and await self.execute_command("UNWATCH") or True
+
+
+class Script:
+    """An executable Lua script object returned by ``register_script``"""
+
+    def __init__(self, registered_client: Redis, script: ScriptTextT):
+        self.registered_client = registered_client
+        self.script = script
+        # Precalculate and store the SHA1 hex digest of the script.
+
+        if isinstance(script, str):
+            # We need the encoding from the client in order to generate an
+            # accurate byte representation of the script
+            encoder = registered_client.connection_pool.get_encoder()
+            script_bytes = encoder.encode(script)
+        else:
+            script_bytes = script
+        self.sha = hashlib.sha1(script_bytes).hexdigest()
+
+    async def __call__(
+        self,
+        keys: Optional[Sequence[KeyT]] = None,
+        args: Optional[Iterable[EncodableT]] = None,
+        client: Optional[Redis] = None,
+    ):
+        """Execute the script, passing any required ``args``"""
+        keys = keys or []
+        args = args or []
+        if client is None:
+            client = self.registered_client
+        args = tuple(keys) + tuple(args)
+        # make sure the Redis server knows about the script
+        if isinstance(client, Pipeline):
+            # Make sure the pipeline can register the script before executing.
+            client.scripts.add(self)
+            return client.evalsha(self.sha, len(keys), *args)
+        try:
+            return await client.evalsha(self.sha, len(keys), *args)
+        except NoScriptError:
+            # Maybe the client is pointed to a differnet server than the client
+            # that created this instance?
+            # Overwrite the sha just in case there was a discrepancy.
+            self.sha = await client.script_load(self.script)
+            return await client.evalsha(self.sha, len(keys), *args)
+
+
+class BitFieldOperation:
+    """
+    Command builder for BITFIELD commands.
+    """
+
+    def __init__(
+        self, client: Redis, key: KeyT, default_overflow: Optional[str] = None
+    ):
+        self.client = client
+        self.key = key
+        self._default_overflow = default_overflow
+        self.operations: List[Tuple[EncodableT, ...]] = []
+        self._last_overflow = "WRAP"
+        self.reset()
+
+    def reset(self):
+        """
+        Reset the state of the instance to when it was constructed
+        """
+        self.operations = []
+        self._last_overflow = "WRAP"
+        self.overflow(self._default_overflow or self._last_overflow)
+
+    def overflow(self, overflow: str):
+        """
+        Update the overflow algorithm of successive INCRBY operations
+        :param overflow: Overflow algorithm, one of WRAP, SAT, FAIL. See the
+            Redis docs for descriptions of these algorithmsself.
+        :returns: a :py:class:`BitFieldOperation` instance.
+        """
+        overflow = overflow.upper()
+        if overflow != self._last_overflow:
+            self._last_overflow = overflow
+            self.operations.append(("OVERFLOW", overflow))
+        return self
+
+    def incrby(
+        self,
+        fmt: str,
+        offset: BitfieldOffsetT,
+        increment: int,
+        overflow: Optional[str] = None,
+    ):
+        """
+        Increment a bitfield by a given amount.
+        :param fmt: format-string for the bitfield being updated, e.g. 'u8'
+            for an unsigned 8-bit integer.
+        :param offset: offset (in number of bits). If prefixed with a
+            '#', this is an offset multiplier, e.g. given the arguments
+            fmt='u8', offset='#2', the offset will be 16.
+        :param int increment: value to increment the bitfield by.
+        :param str overflow: overflow algorithm. Defaults to WRAP, but other
+            acceptable values are SAT and FAIL. See the Redis docs for
+            descriptions of these algorithms.
+        :returns: a :py:class:`BitFieldOperation` instance.
+        """
+        if overflow is not None:
+            self.overflow(overflow)
+
+        self.operations.append(("INCRBY", fmt, offset, increment))
+        return self
+
+    def get(self, fmt: str, offset: BitfieldOffsetT):
+        """
+        Get the value of a given bitfield.
+        :param fmt: format-string for the bitfield being read, e.g. 'u8' for
+            an unsigned 8-bit integer.
+        :param offset: offset (in number of bits). If prefixed with a
+            '#', this is an offset multiplier, e.g. given the arguments
+            fmt='u8', offset='#2', the offset will be 16.
+        :returns: a :py:class:`BitFieldOperation` instance.
+        """
+        self.operations.append(("GET", fmt, offset))
+        return self
+
+    def set(self, fmt: str, offset: BitfieldOffsetT, value: int):
+        """
+        Set the value of a given bitfield.
+        :param fmt: format-string for the bitfield being read, e.g. 'u8' for
+            an unsigned 8-bit integer.
+        :param offset: offset (in number of bits). If prefixed with a
+            '#', this is an offset multiplier, e.g. given the arguments
+            fmt='u8', offset='#2', the offset will be 16.
+        :param int value: value to set at the given position.
+        :returns: a :py:class:`BitFieldOperation` instance.
+        """
+        self.operations.append(("SET", fmt, offset, value))
+        return self
+
+    @property
+    def command(self):
+        cmd: List[EncodableT] = ["BITFIELD", self.key]
+        for ops in self.operations:
+            cmd.extend(ops)
+        return cmd
+
+    def execute(self):
+        """
+        Execute the operation(s) in a single BITFIELD command. The return value
+        is a list of values corresponding to each operation. If the client
+        used to create this instance was a pipeline, the list of values
+        will be present within the pipeline's execute.
+        """
+        command = self.command
+        self.reset()
+        return self.client.execute_command(*command)
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-import sys
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol, TypedDict
-else:
-    from typing_extensions import Protocol, TypedDict
-
-__all__ = ("Protocol", "TypedDict")
+import sys
+
+if sys.version_info >= (3, 8):
+    from typing import Protocol, TypedDict
+else:
+    from typing_extensions import Protocol, TypedDict
+
+__all__ = ("Protocol", "TypedDict")
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py

 * *Ordering differences only*

```diff
@@ -1,1668 +1,1668 @@
-import asyncio
-import enum
-import errno
-import inspect
-import io
-import os
-import socket
-import ssl
-import threading
-import warnings
-from distutils.version import StrictVersion
-from itertools import chain
-from types import MappingProxyType
-from typing import (
-    Any,
-    Callable,
-    Iterable,
-    List,
-    Mapping,
-    Optional,
-    Set,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-)
-from urllib.parse import ParseResult, parse_qs, unquote, urlparse
-
-import async_timeout
-
-from .compat import Protocol, TypedDict
-from .exceptions import (
-    AuthenticationError,
-    AuthenticationWrongNumberOfArgsError,
-    BusyLoadingError,
-    ChildDeadlockedError,
-    ConnectionError,
-    DataError,
-    ExecAbortError,
-    InvalidResponse,
-    ModuleError,
-    NoPermissionError,
-    NoScriptError,
-    ReadOnlyError,
-    RedisError,
-    ResponseError,
-    TimeoutError,
-)
-from .utils import str_if_bytes
-
-NONBLOCKING_EXCEPTION_ERROR_NUMBERS = {
-    BlockingIOError: errno.EWOULDBLOCK,
-    ssl.SSLWantReadError: 2,
-    ssl.SSLWantWriteError: 2,
-    ssl.SSLError: 2,
-}
-
-NONBLOCKING_EXCEPTIONS = tuple(NONBLOCKING_EXCEPTION_ERROR_NUMBERS.keys())
-
-try:
-    import hiredis
-
-except (ImportError, ModuleNotFoundError):
-    HIREDIS_AVAILABLE = False
-else:
-    HIREDIS_AVAILABLE = True
-    hiredis_version = StrictVersion(hiredis.__version__)
-    if hiredis_version < StrictVersion("1.0.0"):
-        warnings.warn(
-            "aioredis supports hiredis @ 1.0.0 or higher. "
-            f"You have hiredis @ {hiredis.__version__}. "
-            "Pure-python parser will be used instead."
-        )
-        HIREDIS_AVAILABLE = False
-
-SYM_STAR = b"*"
-SYM_DOLLAR = b"$"
-SYM_CRLF = b"\r\n"
-SYM_LF = b"\n"
-SYM_EMPTY = b""
-
-SERVER_CLOSED_CONNECTION_ERROR = "Connection closed by server."
-
-
-class _Sentinel(enum.Enum):
-    sentinel = object()
-
-
-SENTINEL = _Sentinel.sentinel
-MODULE_LOAD_ERROR = "Error loading the extension. Please check the server logs."
-NO_SUCH_MODULE_ERROR = "Error unloading module: no such module with that name"
-MODULE_UNLOAD_NOT_POSSIBLE_ERROR = "Error unloading module: operation not possible."
-MODULE_EXPORTS_DATA_TYPES_ERROR = (
-    "Error unloading module: the module "
-    "exports one or more module-side data "
-    "types, can't unload"
-)
-
-EncodedT = Union[bytes, memoryview]
-DecodedT = Union[str, int, float]
-EncodableT = Union[EncodedT, DecodedT]
-
-
-class _HiredisReaderArgs(TypedDict, total=False):
-    protocolError: Callable[[str], Exception]
-    replyError: Callable[[str], Exception]
-    encoding: Optional[str]
-    errors: Optional[str]
-
-
-class Encoder:
-    """Encode strings to bytes-like and decode bytes-like to strings"""
-
-    __slots__ = "encoding", "encoding_errors", "decode_responses"
-
-    def __init__(self, encoding: str, encoding_errors: str, decode_responses: bool):
-        self.encoding = encoding
-        self.encoding_errors = encoding_errors
-        self.decode_responses = decode_responses
-
-    def encode(self, value: EncodableT) -> EncodedT:
-        """Return a bytestring or bytes-like representation of the value"""
-        if isinstance(value, (bytes, memoryview)):
-            return value
-        if isinstance(value, bool):
-            # special case bool since it is a subclass of int
-            raise DataError(
-                "Invalid input of type: 'bool'. "
-                "Convert to a bytes, string, int or float first."
-            )
-        if isinstance(value, (int, float)):
-            return repr(value).encode()
-        if not isinstance(value, str):
-            # a value we don't know how to deal with. throw an error
-            typename = value.__class__.__name__  # type: ignore[unreachable]
-            raise DataError(
-                f"Invalid input of type: {typename!r}. "
-                "Convert to a bytes, string, int or float first."
-            )
-        return value.encode(self.encoding, self.encoding_errors)
-
-    def decode(self, value: EncodableT, force=False) -> EncodableT:
-        """Return a unicode string from the bytes-like representation"""
-        if self.decode_responses or force:
-            if isinstance(value, memoryview):
-                return value.tobytes().decode(self.encoding, self.encoding_errors)
-            if isinstance(value, bytes):
-                return value.decode(self.encoding, self.encoding_errors)
-        return value
-
-
-ExceptionMappingT = Mapping[str, Union[Type[Exception], Mapping[str, Type[Exception]]]]
-
-
-class BaseParser:
-    """Plain Python parsing class"""
-
-    __slots__ = "_stream", "_buffer", "_read_size"
-
-    EXCEPTION_CLASSES: ExceptionMappingT = {
-        "ERR": {
-            "max number of clients reached": ConnectionError,
-            "Client sent AUTH, but no password is set": AuthenticationError,
-            "invalid password": AuthenticationError,
-            # some Redis server versions report invalid command syntax
-            # in lowercase
-            "wrong number of arguments for 'auth' command": AuthenticationWrongNumberOfArgsError,
-            # some Redis server versions report invalid command syntax
-            # in uppercase
-            "wrong number of arguments for 'AUTH' command": AuthenticationWrongNumberOfArgsError,
-            MODULE_LOAD_ERROR: ModuleError,
-            MODULE_EXPORTS_DATA_TYPES_ERROR: ModuleError,
-            NO_SUCH_MODULE_ERROR: ModuleError,
-            MODULE_UNLOAD_NOT_POSSIBLE_ERROR: ModuleError,
-        },
-        "EXECABORT": ExecAbortError,
-        "LOADING": BusyLoadingError,
-        "NOSCRIPT": NoScriptError,
-        "READONLY": ReadOnlyError,
-        "NOAUTH": AuthenticationError,
-        "NOPERM": NoPermissionError,
-    }
-
-    def __init__(self, socket_read_size: int):
-        self._stream: Optional[asyncio.StreamReader] = None
-        self._buffer: Optional[SocketBuffer] = None
-        self._read_size = socket_read_size
-
-    def __del__(self):
-        try:
-            self.on_disconnect()
-        except BaseException :
-            pass
-
-    def parse_error(self, response: str) -> ResponseError:
-        """Parse an error response"""
-        error_code = response.split(" ")[0]
-        if error_code in self.EXCEPTION_CLASSES:
-            response = response[len(error_code) + 1 :]
-            exception_class_or_dict = self.EXCEPTION_CLASSES[error_code]
-            if isinstance(exception_class_or_dict, dict):
-                exception_class = exception_class_or_dict.get(response, ResponseError)
-            else:
-                exception_class = exception_class_or_dict
-            return exception_class(response)
-        return ResponseError(response)
-
-    def on_disconnect(self):
-        raise NotImplementedError()
-
-    def on_connect(self, connection: "Connection"):
-        raise NotImplementedError()
-
-    async def can_read(self, timeout: float) -> bool:
-        raise NotImplementedError()
-
-    async def read_response(
-        self,
-    ) -> Union[EncodableT, ResponseError, None, List[EncodableT]]:
-        raise NotImplementedError()
-
-
-class SocketBuffer:
-    """Async-friendly re-impl of redis-py's SocketBuffer.
-
-    TODO: We're currently passing through two buffers,
-        the asyncio.StreamReader and this. I imagine we can reduce the layers here
-        while maintaining compliance with prior art.
-    """
-
-    def __init__(
-        self,
-        stream_reader: asyncio.StreamReader,
-        socket_read_size: int,
-        socket_timeout: Optional[float],
-    ):
-        self._stream: Optional[asyncio.StreamReader] = stream_reader
-        self.socket_read_size = socket_read_size
-        self.socket_timeout = socket_timeout
-        self._buffer: Optional[io.BytesIO] = io.BytesIO()
-        # number of bytes written to the buffer from the socket
-        self.bytes_written = 0
-        # number of bytes read from the buffer
-        self.bytes_read = 0
-
-    @property
-    def length(self):
-        return self.bytes_written - self.bytes_read
-
-    async def _read_from_socket(
-        self,
-        length: Optional[int] = None,
-        timeout: Union[float, None, _Sentinel] = SENTINEL,
-        raise_on_timeout: bool = True,
-    ) -> bool:
-        buf = self._buffer
-        if buf is None or self._stream is None:
-            raise RedisError("Buffer is closed.")
-        buf.seek(self.bytes_written)
-        marker = 0
-        timeout = timeout if timeout is not SENTINEL else self.socket_timeout
-
-        try:
-            while True:
-                async with async_timeout.timeout(timeout):
-                    data = await self._stream.read(self.socket_read_size)
-                # an empty string indicates the server shutdown the socket
-                if isinstance(data, bytes) and len(data) == 0:
-                    raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
-                buf.write(data)
-                data_length = len(data)
-                self.bytes_written += data_length
-                marker += data_length
-
-                if length is not None and length > marker:
-                    continue
-                return True
-        except (socket.timeout, asyncio.TimeoutError):
-            if raise_on_timeout:
-                raise TimeoutError("Timeout reading from socket")
-            return False
-        except NONBLOCKING_EXCEPTIONS as ex:
-            # if we're in nonblocking mode and the recv raises a
-            # blocking error, simply return False indicating that
-            # there's no data to be read. otherwise raise the
-            # original exception.
-            allowed = NONBLOCKING_EXCEPTION_ERROR_NUMBERS.get(ex.__class__, -1)
-            if not raise_on_timeout and ex.errno == allowed:
-                return False
-            raise ConnectionError(f"Error while reading from socket: {ex.args}")
-
-    async def can_read(self, timeout: float) -> bool:
-        return bool(self.length) or await self._read_from_socket(
-            timeout=timeout, raise_on_timeout=False
-        )
-
-    async def read(self, length: int) -> bytes:
-        length = length + 2  # make sure to read the \r\n terminator
-        # make sure we've read enough data from the socket
-        if length > self.length:
-            await self._read_from_socket(length - self.length)
-
-        if self._buffer is None:
-            raise RedisError("Buffer is closed.")
-
-        self._buffer.seek(self.bytes_read)
-        data = self._buffer.read(length)
-        self.bytes_read += len(data)
-
-        # purge the buffer when we've consumed it all so it doesn't
-        # grow forever
-        if self.bytes_read == self.bytes_written:
-            self.purge()
-
-        return data[:-2]
-
-    async def readline(self) -> bytes:
-        buf = self._buffer
-        if buf is None:
-            raise RedisError("Buffer is closed.")
-
-        buf.seek(self.bytes_read)
-        data = buf.readline()
-        while not data.endswith(SYM_CRLF):
-            # there's more data in the socket that we need
-            await self._read_from_socket()
-            buf.seek(self.bytes_read)
-            data = buf.readline()
-
-        self.bytes_read += len(data)
-
-        # purge the buffer when we've consumed it all so it doesn't
-        # grow forever
-        if self.bytes_read == self.bytes_written:
-            self.purge()
-
-        return data[:-2]
-
-    def purge(self):
-        if self._buffer is None:
-            raise RedisError("Buffer is closed.")
-
-        self._buffer.seek(0)
-        self._buffer.truncate()
-        self.bytes_written = 0
-        self.bytes_read = 0
-
-    def close(self):
-        try:
-            self.purge()
-            self._buffer.close()  # type: ignore[union-attr]
-        except BaseException :
-            # issue #633 suggests the purge/close somehow raised a
-            # BadFileDescriptor error. Perhaps the client ran out of
-            # memory or something else? It's probably OK to ignore
-            # any error being raised from purge/close since we're
-            # removing the reference to the instance below.
-            pass
-        self._buffer = None
-        self._stream = None
-
-
-class PythonParser(BaseParser):
-    """Plain Python parsing class"""
-
-    __slots__ = BaseParser.__slots__ + ("encoder",)
-
-    def __init__(self, socket_read_size: int):
-        super().__init__(socket_read_size)
-        self.encoder: Optional[Encoder] = None
-
-    def on_connect(self, connection: "Connection"):
-        """Called when the stream connects"""
-        self._stream = connection._reader
-        if self._stream is None:
-            raise RedisError("Buffer is closed.")
-
-        self._buffer = SocketBuffer(
-            self._stream, self._read_size, connection.socket_timeout
-        )
-        self.encoder = connection.encoder
-
-    def on_disconnect(self):
-        """Called when the stream disconnects"""
-        if self._stream is not None:
-            self._stream = None
-        if self._buffer is not None:
-            self._buffer.close()
-            self._buffer = None
-        self.encoder = None
-
-    async def can_read(self, timeout: float):
-        return self._buffer and bool(await self._buffer.can_read(timeout))
-
-    async def read_response(self) -> Union[EncodableT, ResponseError, None]:
-        if not self._buffer or not self.encoder:
-            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
-        raw = await self._buffer.readline()
-        if not raw:
-            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
-        response: Any
-        byte, response = raw[:1], raw[1:]
-
-        if byte not in (b"-", b"+", b":", b"$", b"*"):
-            raise InvalidResponse(f"Protocol Error: {raw!r}")
-
-        # server returned an error
-        if byte == b"-":
-            response = response.decode("utf-8", errors="replace")
-            error = self.parse_error(response)
-            # if the error is a ConnectionError, raise immediately so the user
-            # is notified
-            if isinstance(error, ConnectionError):
-                raise error
-            # otherwise, we're dealing with a ResponseError that might belong
-            # inside a pipeline response. the connection's read_response()
-            # and/or the pipeline's execute() will raise this error if
-            # necessary, so just return the exception instance here.
-            return error
-        # single value
-        elif byte == b"+":
-            pass
-        # int value
-        elif byte == b":":
-            response = int(response)
-        # bulk response
-        elif byte == b"$":
-            length = int(response)
-            if length == -1:
-                return None
-            response = await self._buffer.read(length)
-        # multi-bulk response
-        elif byte == b"*":
-            length = int(response)
-            if length == -1:
-                return None
-            response = [(await self.read_response()) for _ in range(length)]
-        if isinstance(response, bytes):
-            response = self.encoder.decode(response)
-        return response
-
-
-class HiredisParser(BaseParser):
-    """Parser class for connections using Hiredis"""
-
-    __slots__ = BaseParser.__slots__ + ("_next_response", "_reader", "_socket_timeout")
-
-    _next_response: bool
-
-    def __init__(self, socket_read_size: int):
-        if not HIREDIS_AVAILABLE:
-            raise RedisError("Hiredis is not available.")
-        super().__init__(socket_read_size=socket_read_size)
-        self._reader: Optional[hiredis.Reader] = None
-        self._socket_timeout: Optional[float] = None
-
-    def on_connect(self, connection: "Connection"):
-        self._stream = connection._reader
-        kwargs: _HiredisReaderArgs = {
-            "protocolError": InvalidResponse,
-            "replyError": self.parse_error,
-        }
-        if connection.encoder.decode_responses:
-            kwargs["encoding"] = connection.encoder.encoding
-            kwargs["errors"] = connection.encoder.encoding_errors
-
-        self._reader = hiredis.Reader(**kwargs)
-        self._next_response = False
-        self._socket_timeout = connection.socket_timeout
-
-    def on_disconnect(self):
-        self._stream = None
-        self._reader = None
-        self._next_response = False
-
-    async def can_read(self, timeout: float):
-        if not self._reader:
-            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
-
-        if self._next_response is False:
-            self._next_response = self._reader.gets()
-        if self._next_response is False:
-            return await self.read_from_socket(timeout=timeout, raise_on_timeout=False)
-        return True
-
-    async def read_from_socket(
-        self,
-        timeout: Union[float, None, _Sentinel] = SENTINEL,
-        raise_on_timeout: bool = True,
-    ):
-        if self._stream is None or self._reader is None:
-            raise RedisError("Parser already closed.")
-
-        timeout = self._socket_timeout if timeout is SENTINEL else timeout
-        try:
-            async with async_timeout.timeout(timeout):
-                buffer = await self._stream.read(self._read_size)
-            if not isinstance(buffer, bytes) or len(buffer) == 0:
-                raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR) from None
-            self._reader.feed(buffer)
-            # data was read from the socket and added to the buffer.
-            # return True to indicate that data was read.
-            return True
-        except asyncio.CancelledError:
-            raise
-        except (socket.timeout, asyncio.TimeoutError):
-            if raise_on_timeout:
-                raise TimeoutError("Timeout reading from socket") from None
-            return False
-        except NONBLOCKING_EXCEPTIONS as ex:
-            # if we're in nonblocking mode and the recv raises a
-            # blocking error, simply return False indicating that
-            # there's no data to be read. otherwise raise the
-            # original exception.
-            allowed = NONBLOCKING_EXCEPTION_ERROR_NUMBERS.get(ex.__class__, -1)
-            if not raise_on_timeout and ex.errno == allowed:
-                return False
-            raise ConnectionError(f"Error while reading from socket: {ex.args}")
-
-    async def read_response(self) -> Union[EncodableT, List[EncodableT]]:
-        if not self._stream or not self._reader:
-            self.on_disconnect()
-            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR) from None
-
-        response: Union[
-            EncodableT, ConnectionError, List[Union[EncodableT, ConnectionError]]
-        ]
-        # _next_response might be cached from a can_read() call
-        if self._next_response is not False:
-            response = self._next_response
-            self._next_response = False
-            return response
-
-        response = self._reader.gets()
-        while response is False:
-            await self.read_from_socket()
-            response = self._reader.gets()
-
-        # if the response is a ConnectionError or the response is a list and
-        # the first item is a ConnectionError, raise it as something bad
-        # happened
-        if isinstance(response, ConnectionError):
-            raise response
-        elif (
-            isinstance(response, list)
-            and response
-            and isinstance(response[0], ConnectionError)
-        ):
-            raise response[0]
-        # cast as there won't be a ConnectionError here.
-        return cast(Union[EncodableT, List[EncodableT]], response)
-
-
-DefaultParser: Type[Union[PythonParser, HiredisParser]]
-if HIREDIS_AVAILABLE:
-    DefaultParser = HiredisParser
-else:
-    DefaultParser = PythonParser
-
-
-class ConnectCallbackProtocol(Protocol):
-    def __call__(self, connection: "Connection"):
-        ...
-
-
-class AsyncConnectCallbackProtocol(Protocol):
-    async def __call__(self, connection: "Connection"):
-        ...
-
-
-ConnectCallbackT = Union[ConnectCallbackProtocol, AsyncConnectCallbackProtocol]
-
-
-class Connection:
-    """Manages TCP communication to and from a Redis server"""
-
-    __slots__ = (
-        "pid",
-        "host",
-        "port",
-        "db",
-        "username",
-        "client_name",
-        "password",
-        "socket_timeout",
-        "socket_connect_timeout",
-        "socket_keepalive",
-        "socket_keepalive_options",
-        "socket_type",
-        "retry_on_timeout",
-        "health_check_interval",
-        "next_health_check",
-        "last_active_at",
-        "encoder",
-        "ssl_context",
-        "_reader",
-        "_writer",
-        "_parser",
-        "_connect_callbacks",
-        "_buffer_cutoff",
-        "_lock",
-        "__dict__",
-    )
-
-    def __init__(
-        self,
-        *,
-        host: str = "localhost",
-        port: Union[str, int] = 6379,
-        db: Union[str, int] = 0,
-        password: Optional[str] = None,
-        socket_timeout: Optional[float] = None,
-        socket_connect_timeout: Optional[float] = None,
-        socket_keepalive: bool = False,
-        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
-        socket_type: int = 0,
-        retry_on_timeout: bool = False,
-        encoding: str = "utf-8",
-        encoding_errors: str = "strict",
-        decode_responses: bool = False,
-        parser_class: Type[BaseParser] = DefaultParser,
-        socket_read_size: int = 65536,
-        health_check_interval: float = 0,
-        client_name: Optional[str] = None,
-        username: Optional[str] = None,
-        encoder_class: Type[Encoder] = Encoder,
-    ):
-        self.pid = os.getpid()
-        self.host = host
-        self.port = int(port)
-        self.db = db
-        self.username = username
-        self.client_name = client_name
-        self.password = password
-        self.socket_timeout = socket_timeout
-        self.socket_connect_timeout = socket_connect_timeout or socket_timeout or None
-        self.socket_keepalive = socket_keepalive
-        self.socket_keepalive_options = socket_keepalive_options or {}
-        self.socket_type = socket_type
-        self.retry_on_timeout = retry_on_timeout
-        self.health_check_interval = health_check_interval
-        self.next_health_check: float = -1
-        self.ssl_context: Optional[RedisSSLContext] = None
-        self.encoder = encoder_class(encoding, encoding_errors, decode_responses)
-        self._reader: Optional[asyncio.StreamReader] = None
-        self._writer: Optional[asyncio.StreamWriter] = None
-        self._parser = parser_class(
-            socket_read_size=socket_read_size,
-        )
-        self._connect_callbacks: List[ConnectCallbackT] = []
-        self._buffer_cutoff = 6000
-        self._lock = asyncio.Lock()
-
-    def __repr__(self):
-        repr_args = ",".join((f"{k}={v}" for k, v in self.repr_pieces()))
-        return f"{self.__class__.__name__}<{repr_args}>"
-
-    def repr_pieces(self):
-        pieces = [("host", self.host), ("port", self.port), ("db", self.db)]
-        if self.client_name:
-            pieces.append(("client_name", self.client_name))
-        return pieces
-
-    def __del__(self):
-        try:
-            if self.is_connected:
-                loop = asyncio.get_event_loop()
-                coro = self.disconnect()
-                if loop.is_running():
-                    loop.create_task(coro)
-                else:
-                    loop.run_until_complete(coro)
-        except BaseException :
-            pass
-
-    @property
-    def is_connected(self):
-        return bool(self._reader and self._writer)
-
-    def register_connect_callback(self, callback):
-        self._connect_callbacks.append(callback)
-
-    def clear_connect_callbacks(self):
-        self._connect_callbacks = []
-
-    async def connect(self):
-        """Connects to the Redis server if not already connected"""
-        if self.is_connected:
-            return
-        try:
-            await self._connect()
-        except asyncio.CancelledError:
-            raise
-        except (socket.timeout, asyncio.TimeoutError):
-            raise TimeoutError("Timeout connecting to server")
-        except OSError as e:
-            raise ConnectionError(self._error_message(e))
-        except BaseException as exc:
-            raise ConnectionError(exc) from exc
-
-        try:
-            await self.on_connect()
-        except RedisError:
-            # clean up after any error in on_connect
-            await self.disconnect()
-            raise
-
-        # run any user callbacks. right now the only internal callback
-        # is for pubsub channel/pattern resubscription
-        for callback in self._connect_callbacks:
-            task = callback(self)
-            if task and inspect.isawaitable(task):
-                await task
-
-    async def _connect(self):
-        """Create a TCP socket connection"""
-        async with async_timeout.timeout(self.socket_connect_timeout):
-            reader, writer = await asyncio.open_connection(
-                host=self.host,
-                port=self.port,
-                ssl=self.ssl_context.get() if self.ssl_context else None,
-            )
-        self._reader = reader
-        self._writer = writer
-        sock = writer.transport.get_extra_info("socket")
-        if sock is not None:
-            sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-            try:
-                # TCP_KEEPALIVE
-                if self.socket_keepalive:
-                    sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
-                    for k, v in self.socket_keepalive_options.items():
-                        sock.setsockopt(socket.SOL_TCP, k, v)
-
-            except (OSError, TypeError):
-                # `socket_keepalive_options` might contain invalid options
-                # causing an error. Do not leave the connection open.
-                writer.close()
-                raise
-
-    def _error_message(self, exception):
-        # args for socket.error can either be (errno, "message")
-        # or just "message"
-        if len(exception.args) == 1:
-            return f"Error connecting to {self.host}:{self.port}. {exception.args[0]}."
-        else:
-            return (
-                f"Error {exception.args[0]} connecting to {self.host}:{self.port}. "
-                f"{exception.args[0]}."
-            )
-
-    async def on_connect(self):
-        """Initialize the connection, authenticate and select a database"""
-        self._parser.on_connect(self)
-
-        # if username and/or password are set, authenticate
-        if self.username or self.password:
-            auth_args: Union[Tuple[str], Tuple[str, str]]
-            if self.username:
-                auth_args = (self.username, self.password or "")
-            else:
-                # Mypy bug: https://github.com/python/mypy/issues/10944
-                auth_args = (self.password or "",)
-            # avoid checking health here -- PING will fail if we try
-            # to check the health prior to the AUTH
-            await self.send_command("AUTH", *auth_args, check_health=False)
-
-            try:
-                auth_response = await self.read_response()
-            except AuthenticationWrongNumberOfArgsError:
-                # a username and password were specified but the Redis
-                # server seems to be < 6.0.0 which expects a single password
-                # arg. retry auth with just the password.
-                # https://github.com/andymccurdy/redis-py/issues/1274
-                await self.send_command("AUTH", self.password, check_health=False)
-                auth_response = await self.read_response()
-
-            if str_if_bytes(auth_response) != "OK":
-                raise AuthenticationError("Invalid Username or Password")
-
-        # if a client_name is given, set it
-        if self.client_name:
-            await self.send_command("CLIENT", "SETNAME", self.client_name)
-            if str_if_bytes(await self.read_response()) != "OK":
-                raise ConnectionError("Error setting client name")
-
-        # if a database is specified, switch to it
-        if self.db:
-            await self.send_command("SELECT", self.db)
-            if str_if_bytes(await self.read_response()) != "OK":
-                raise ConnectionError("Invalid Database")
-
-    async def disconnect(self):
-        """Disconnects from the Redis server"""
-        try:
-            async with async_timeout.timeout(self.socket_connect_timeout):
-                self._parser.on_disconnect()
-                if not self.is_connected:
-                    return
-                try:
-                    if os.getpid() == self.pid:
-                        self._writer.close()  # type: ignore[union-attr]
-                        # py3.6 doesn't have this method
-                        if hasattr(self._writer, "wait_closed"):
-                            await self._writer.wait_closed()  # type: ignore[union-attr]
-                except OSError:
-                    pass
-                self._reader = None
-                self._writer = None
-        except asyncio.TimeoutError:
-            raise TimeoutError(
-                f"Timed out closing connection after {self.socket_connect_timeout}"
-            ) from None
-
-    async def check_health(self):
-        """Check the health of the connection with a PING/PONG"""
-        if (
-            self.health_check_interval
-            and asyncio.get_event_loop().time() > self.next_health_check
-        ):
-            try:
-                await self.send_command("PING", check_health=False)
-                if str_if_bytes(await self.read_response()) != "PONG":
-                    raise ConnectionError("Bad response from PING health check")
-            except (ConnectionError, TimeoutError) as err:
-                await self.disconnect()
-                try:
-                    await self.send_command("PING", check_health=False)
-                    if str_if_bytes(await self.read_response()) != "PONG":
-                        raise ConnectionError(
-                            "Bad response from PING health check"
-                        ) from None
-                except BaseException as err2:
-                    raise err2 from err
-
-    async def _send_packed_command(self, command: Iterable[bytes]) -> None:
-        if self._writer is None:
-            raise RedisError("Connection already closed.")
-
-        self._writer.writelines(command)
-        await self._writer.drain()
-
-    async def send_packed_command(
-        self,
-        command: Union[bytes, str, Iterable[bytes]],
-        check_health: bool = True,
-    ):
-        """Send an already packed command to the Redis server"""
-        if not self._writer:
-            await self.connect()
-        # guard against health check recursion
-        if check_health:
-            await self.check_health()
-        try:
-            if isinstance(command, str):
-                command = command.encode()
-            if isinstance(command, bytes):
-                command = [command]
-            await asyncio.wait_for(
-                self._send_packed_command(command),
-                self.socket_timeout,
-            )
-        except asyncio.TimeoutError:
-            await self.disconnect()
-            raise TimeoutError("Timeout writing to socket") from None
-        except OSError as e:
-            await self.disconnect()
-            if len(e.args) == 1:
-                err_no, errmsg = "UNKNOWN", e.args[0]
-            else:
-                err_no = e.args[0]
-                errmsg = e.args[1]
-            raise ConnectionError(
-                f"Error {err_no} while writing to socket. {errmsg}."
-            ) from e
-        except BaseException:
-            await self.disconnect()
-            raise
-
-    async def send_command(self, *args, **kwargs):
-        """Pack and send a command to the Redis server"""
-        if not self.is_connected:
-            await self.connect()
-        await self.send_packed_command(
-            self.pack_command(*args), check_health=kwargs.get("check_health", True)
-        )
-
-    async def can_read(self, timeout: float = 0):
-        """Poll the socket to see if there's data that can be read."""
-        if not self.is_connected:
-            await self.connect()
-        return await self._parser.can_read(timeout)
-
-    async def read_response(self):
-        """Read the response from a previously sent command"""
-        try:
-            async with self._lock:
-                async with async_timeout.timeout(self.socket_timeout):
-                    response = await self._parser.read_response()
-        except asyncio.TimeoutError:
-            await self.disconnect()
-            raise TimeoutError(f"Timeout reading from {self.host}:{self.port}")
-        except OSError as e:
-            await self.disconnect()
-            raise ConnectionError(
-                f"Error while reading from {self.host}:{self.port} : {e.args}"
-            )
-        except BaseException:
-            await self.disconnect()
-            raise
-
-        if self.health_check_interval:
-            self.next_health_check = (
-                asyncio.get_event_loop().time() + self.health_check_interval
-            )
-
-        if isinstance(response, ResponseError):
-            raise response from None
-        return response
-
-    def pack_command(self, *args: EncodableT) -> List[bytes]:
-        """Pack a series of arguments into the Redis protocol"""
-        output = []
-        # the client might have included 1 or more literal arguments in
-        # the command name, e.g., 'CONFIG GET'. The Redis server expects these
-        # arguments to be sent separately, so split the first argument
-        # manually. These arguments should be bytestrings so that they are
-        # not encoded.
-        assert not isinstance(args[0], float)
-        if isinstance(args[0], str):
-            args = tuple(args[0].encode().split()) + args[1:]
-        elif b" " in args[0]:
-            args = tuple(args[0].split()) + args[1:]
-
-        buff = SYM_EMPTY.join((SYM_STAR, str(len(args)).encode(), SYM_CRLF))
-
-        buffer_cutoff = self._buffer_cutoff
-        for arg in map(self.encoder.encode, args):
-            # to avoid large string mallocs, chunk the command into the
-            # output list if we're sending large values or memoryviews
-            arg_length = len(arg)
-            if (
-                len(buff) > buffer_cutoff
-                or arg_length > buffer_cutoff
-                or isinstance(arg, memoryview)
-            ):
-                buff = SYM_EMPTY.join(
-                    (buff, SYM_DOLLAR, str(arg_length).encode(), SYM_CRLF)
-                )
-                output.append(buff)
-                output.append(arg)
-                buff = SYM_CRLF
-            else:
-                buff = SYM_EMPTY.join(
-                    (
-                        buff,
-                        SYM_DOLLAR,
-                        str(arg_length).encode(),
-                        SYM_CRLF,
-                        arg,
-                        SYM_CRLF,
-                    )
-                )
-        output.append(buff)
-        return output
-
-    def pack_commands(self, commands: Iterable[Iterable[EncodableT]]) -> List[bytes]:
-        """Pack multiple commands into the Redis protocol"""
-        output: List[bytes] = []
-        pieces: List[bytes] = []
-        buffer_length = 0
-        buffer_cutoff = self._buffer_cutoff
-
-        for cmd in commands:
-            for chunk in self.pack_command(*cmd):
-                chunklen = len(chunk)
-                if (
-                    buffer_length > buffer_cutoff
-                    or chunklen > buffer_cutoff
-                    or isinstance(chunk, memoryview)
-                ):
-                    output.append(SYM_EMPTY.join(pieces))
-                    buffer_length = 0
-                    pieces = []
-
-                if chunklen > buffer_cutoff or isinstance(chunk, memoryview):
-                    output.append(chunk)
-                else:
-                    pieces.append(chunk)
-                    buffer_length += chunklen
-
-        if pieces:
-            output.append(SYM_EMPTY.join(pieces))
-        return output
-
-
-class SSLConnection(Connection):
-    def __init__(
-        self,
-        ssl_keyfile: Optional[str] = None,
-        ssl_certfile: Optional[str] = None,
-        ssl_cert_reqs: str = "required",
-        ssl_ca_certs: Optional[str] = None,
-        ssl_check_hostname: bool = False,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.ssl_context: RedisSSLContext = RedisSSLContext(
-            keyfile=ssl_keyfile,
-            certfile=ssl_certfile,
-            cert_reqs=ssl_cert_reqs,
-            ca_certs=ssl_ca_certs,
-            check_hostname=ssl_check_hostname,
-        )
-
-    @property
-    def keyfile(self):
-        return self.ssl_context.keyfile
-
-    @property
-    def certfile(self):
-        return self.ssl_context.certfile
-
-    @property
-    def cert_reqs(self):
-        return self.ssl_context.cert_reqs
-
-    @property
-    def ca_certs(self):
-        return self.ssl_context.ca_certs
-
-    @property
-    def check_hostname(self):
-        return self.ssl_context.check_hostname
-
-
-class RedisSSLContext:
-    __slots__ = (
-        "keyfile",
-        "certfile",
-        "cert_reqs",
-        "ca_certs",
-        "context",
-        "check_hostname",
-    )
-
-    def __init__(
-        self,
-        keyfile: Optional[str] = None,
-        certfile: Optional[str] = None,
-        cert_reqs: Optional[str] = None,
-        ca_certs: Optional[str] = None,
-        check_hostname: bool = False,
-    ):
-        self.keyfile = keyfile
-        self.certfile = certfile
-        if cert_reqs is None:
-            self.cert_reqs = ssl.CERT_NONE
-        elif isinstance(cert_reqs, str):
-            CERT_REQS = {
-                "none": ssl.CERT_NONE,
-                "optional": ssl.CERT_OPTIONAL,
-                "required": ssl.CERT_REQUIRED,
-            }
-            if cert_reqs not in CERT_REQS:
-                raise RedisError(
-                    f"Invalid SSL Certificate Requirements Flag: {cert_reqs}"
-                )
-            self.cert_reqs = CERT_REQS[cert_reqs]
-        self.ca_certs = ca_certs
-        self.check_hostname = check_hostname
-        self.context: Optional[ssl.SSLContext] = None
-
-    def get(self) -> ssl.SSLContext:
-        if not self.context:
-            context = ssl.create_default_context()
-            context.check_hostname = self.check_hostname
-            context.verify_mode = self.cert_reqs
-            if self.certfile and self.keyfile:
-                context.load_cert_chain(certfile=self.certfile, keyfile=self.keyfile)
-            if self.ca_certs:
-                context.load_verify_locations(self.ca_certs)
-            self.context = context
-        return self.context
-
-
-class UnixDomainSocketConnection(Connection):  # lgtm [py/missing-call-to-init]
-    def __init__(
-        self,
-        *,
-        path: str = "",
-        db: Union[str, int] = 0,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-        socket_timeout: Optional[float] = None,
-        socket_connect_timeout: Optional[float] = None,
-        encoding: str = "utf-8",
-        encoding_errors: str = "strict",
-        decode_responses: bool = False,
-        retry_on_timeout: bool = False,
-        parser_class: Type[BaseParser] = DefaultParser,
-        socket_read_size: int = 65536,
-        health_check_interval: float = 0.0,
-        client_name=None,
-    ):
-        self.pid = os.getpid()
-        self.path = path
-        self.db = db
-        self.username = username
-        self.client_name = client_name
-        self.password = password
-        self.socket_timeout = socket_timeout
-        self.socket_connect_timeout = socket_connect_timeout or socket_timeout or None
-        self.retry_on_timeout = retry_on_timeout
-        self.health_check_interval = health_check_interval
-        self.next_health_check = -1
-        self.encoder = Encoder(encoding, encoding_errors, decode_responses)
-        self._sock = None
-        self._reader = None
-        self._writer = None
-        self._parser = parser_class(socket_read_size=socket_read_size)
-        self._connect_callbacks = []
-        self._buffer_cutoff = 6000
-        self._lock = asyncio.Lock()
-
-    def repr_pieces(self) -> Iterable[Tuple[str, Union[str, int]]]:
-        pieces = [
-            ("path", self.path),
-            ("db", self.db),
-        ]
-        if self.client_name:
-            pieces.append(("client_name", self.client_name))
-        return pieces
-
-    async def _connect(self):
-        async with async_timeout.timeout(self.socket_connect_timeout):
-            reader, writer = await asyncio.open_unix_connection(path=self.path)
-        self._reader = reader
-        self._writer = writer
-        await self.on_connect()
-
-    def _error_message(self, exception):
-        # args for socket.error can either be (errno, "message")
-        # or just "message"
-        if len(exception.args) == 1:
-            return f"Error connecting to unix socket: {self.path}. {exception.args[0]}."
-        else:
-            return (
-                f"Error {exception.args[0]} connecting to unix socket: "
-                f"{self.path}. {exception.args[1]}."
-            )
-
-
-FALSE_STRINGS = ("0", "F", "FALSE", "N", "NO")
-
-
-def to_bool(value) -> Optional[bool]:
-    if value is None or value == "":
-        return None
-    if isinstance(value, str) and value.upper() in FALSE_STRINGS:
-        return False
-    return bool(value)
-
-
-URL_QUERY_ARGUMENT_PARSERS: Mapping[str, Callable[..., object]] = MappingProxyType(
-    {
-        "db": int,
-        "socket_timeout": float,
-        "socket_connect_timeout": float,
-        "socket_keepalive": to_bool,
-        "retry_on_timeout": to_bool,
-        "max_connections": int,
-        "health_check_interval": int,
-        "ssl_check_hostname": to_bool,
-    }
-)
-
-
-class ConnectKwargs(TypedDict, total=False):
-    username: str
-    password: str
-    connection_class: Type[Connection]
-    host: str
-    port: int
-    db: int
-    path: str
-
-
-def parse_url(url: str) -> ConnectKwargs:
-    parsed: ParseResult = urlparse(url)
-    kwargs: ConnectKwargs = {}
-
-    for name, value_list in parse_qs(parsed.query).items():
-        if value_list and len(value_list) > 0:
-            value = unquote(value_list[0])
-            parser = URL_QUERY_ARGUMENT_PARSERS.get(name)
-            if parser:
-                try:
-                    # We can't type this.
-                    kwargs[name] = parser(value)  # type: ignore[misc]
-                except (TypeError, ValueError):
-                    raise ValueError(f"Invalid value for `{name}` in connection URL.")
-            else:
-                kwargs[name] = value  # type: ignore[misc]
-
-    if parsed.username:
-        kwargs["username"] = unquote(parsed.username)
-    if parsed.password:
-        kwargs["password"] = unquote(parsed.password)
-
-    # We only support redis://, rediss:// and unix:// schemes.
-    if parsed.scheme == "unix":
-        if parsed.path:
-            kwargs["path"] = unquote(parsed.path)
-        kwargs["connection_class"] = UnixDomainSocketConnection
-
-    elif parsed.scheme in ("redis", "rediss"):
-        if parsed.hostname:
-            kwargs["host"] = unquote(parsed.hostname)
-        if parsed.port:
-            kwargs["port"] = int(parsed.port)
-
-        # If there's a path argument, use it as the db argument if a
-        # querystring value wasn't specified
-        if parsed.path and "db" not in kwargs:
-            try:
-                kwargs["db"] = int(unquote(parsed.path).replace("/", ""))
-            except (AttributeError, ValueError):
-                pass
-
-        if parsed.scheme == "rediss":
-            kwargs["connection_class"] = SSLConnection
-    else:
-        valid_schemes = "redis://, rediss://, unix://"
-        raise ValueError(
-            f"Redis URL must specify one of the following schemes ({valid_schemes})"
-        )
-
-    return kwargs
-
-
-_CP = TypeVar("_CP", bound="ConnectionPool")
-
-
-class ConnectionPool:
-    """
-    Create a connection pool. ``If max_connections`` is set, then this
-    object raises :py:class:`~redis.ConnectionError` when the pool's
-    limit is reached.
-
-    By default, TCP connections are created unless ``connection_class``
-    is specified. Use :py:class:`~redis.UnixDomainSocketConnection` for
-    unix sockets.
-
-    Any additional keyword arguments are passed to the constructor of
-    ``connection_class``.
-    """
-
-    @classmethod
-    def from_url(cls: Type[_CP], url: str, **kwargs) -> _CP:
-        """
-        Return a connection pool configured from the given URL.
-
-        For example::
-
-            redis://[[username]:[password]]@localhost:6379/0
-            rediss://[[username]:[password]]@localhost:6379/0
-            unix://[[username]:[password]]@/path/to/socket.sock?db=0
-
-        Three URL schemes are supported:
-
-        - `redis://` creates a TCP socket connection. See more at:
-          <https://www.iana.org/assignments/uri-schemes/prov/redis>
-        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
-          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
-        - ``unix://``: creates a Unix Domain Socket connection.
-
-        The username, password, hostname, path and all querystring values
-        are passed through urllib.parse.unquote in order to replace any
-        percent-encoded values with their corresponding characters.
-
-        There are several ways to specify a database number. The first value
-        found will be used:
-            1. A ``db`` querystring option, e.g. redis://localhost?db=0
-            2. If using the redis:// or rediss:// schemes, the path argument
-               of the url, e.g. redis://localhost/0
-            3. A ``db`` keyword argument to this function.
-
-        If none of these options are specified, the default db=0 is used.
-
-        All querystring options are cast to their appropriate Python types.
-        Boolean arguments can be specified with string values "True"/"False"
-        or "Yes"/"No". Values that cannot be properly cast cause a
-        ``ValueError`` to be raised. Once parsed, the querystring arguments
-        and keyword arguments are passed to the ``ConnectionPool``'s
-        class initializer. In the case of conflicting arguments, querystring
-        arguments always win.
-        """
-        url_options = parse_url(url)
-        kwargs.update(url_options)
-        return cls(**kwargs)
-
-    def __init__(
-        self,
-        connection_class: Type[Connection] = Connection,
-        max_connections: Optional[int] = None,
-        **connection_kwargs,
-    ):
-        max_connections = max_connections or 2 ** 31
-        if not isinstance(max_connections, int) or max_connections < 0:
-            raise ValueError('"max_connections" must be a positive integer')
-
-        self.connection_class = connection_class
-        self.connection_kwargs = connection_kwargs
-        self.max_connections = max_connections
-
-        # a lock to protect the critical section in _checkpid().
-        # this lock is acquired when the process id changes, such as
-        # after a fork. during this time, multiple threads in the child
-        # process could attempt to acquire this lock. the first thread
-        # to acquire the lock will reset the data structures and lock
-        # object of this pool. subsequent threads acquiring this lock
-        # will notice the first thread already did the work and simply
-        # release the lock.
-        self._fork_lock = threading.Lock()
-        self._lock = asyncio.Lock()
-        self._created_connections: int
-        self._available_connections: List[Connection]
-        self._in_use_connections: Set[Connection]
-        self.reset()  # lgtm [py/init-calls-subclass]
-        self.encoder_class = self.connection_kwargs.get("encoder_class", Encoder)
-
-    def __repr__(self):
-        return (
-            f"{self.__class__.__name__}"
-            f"<{self.connection_class(**self.connection_kwargs)!r}>"
-        )
-
-    def reset(self):
-        self._lock = asyncio.Lock()
-        self._created_connections = 0
-        self._available_connections = []
-        self._in_use_connections = set()
-
-        # this must be the last operation in this method. while reset() is
-        # called when holding _fork_lock, other threads in this process
-        # can call _checkpid() which compares self.pid and os.getpid() without
-        # holding any lock (for performance reasons). keeping this assignment
-        # as the last operation ensures that those other threads will also
-        # notice a pid difference and block waiting for the first thread to
-        # release _fork_lock. when each of these threads eventually acquire
-        # _fork_lock, they will notice that another thread already called
-        # reset() and they will immediately release _fork_lock and continue on.
-        self.pid = os.getpid()
-
-    def _checkpid(self):
-        # _checkpid() attempts to keep ConnectionPool fork-safe on modern
-        # systems. this is called by all ConnectionPool methods that
-        # manipulate the pool's state such as get_connection() and release().
-        #
-        # _checkpid() determines whether the process has forked by comparing
-        # the current process id to the process id saved on the ConnectionPool
-        # instance. if these values are the same, _checkpid() simply returns.
-        #
-        # when the process ids differ, _checkpid() assumes that the process
-        # has forked and that we're now running in the child process. the child
-        # process cannot use the parent's file descriptors (e.g., sockets).
-        # therefore, when _checkpid() sees the process id change, it calls
-        # reset() in order to reinitialize the child's ConnectionPool. this
-        # will cause the child to make all new connection objects.
-        #
-        # _checkpid() is protected by self._fork_lock to ensure that multiple
-        # threads in the child process do not call reset() multiple times.
-        #
-        # there is an extremely small chance this could fail in the following
-        # scenario:
-        #   1. process A calls _checkpid() for the first time and acquires
-        #      self._fork_lock.
-        #   2. while holding self._fork_lock, process A forks (the fork()
-        #      could happen in a different thread owned by process A)
-        #   3. process B (the forked child process) inherits the
-        #      ConnectionPool's state from the parent. that state includes
-        #      a locked _fork_lock. process B will not be notified when
-        #      process A releases the _fork_lock and will thus never be
-        #      able to acquire the _fork_lock.
-        #
-        # to mitigate this possible deadlock, _checkpid() will only wait 5
-        # seconds to acquire _fork_lock. if _fork_lock cannot be acquired in
-        # that time it is assumed that the child is deadlocked and a
-        # redis.ChildDeadlockedError error is raised.
-        if self.pid != os.getpid():
-            acquired = self._fork_lock.acquire(timeout=5)
-            if not acquired:
-                raise ChildDeadlockedError
-            # reset() the instance for the new process if another thread
-            # hasn't already done so
-            try:
-                if self.pid != os.getpid():
-                    self.reset()
-            finally:
-                self._fork_lock.release()
-
-    async def get_connection(self, command_name, *keys, **options):
-        """Get a connection from the pool"""
-        self._checkpid()
-        async with self._lock:
-            try:
-                connection = self._available_connections.pop()
-            except IndexError:
-                connection = self.make_connection()
-            self._in_use_connections.add(connection)
-
-        try:
-            # ensure this connection is connected to Redis
-            await connection.connect()
-            # connections that the pool provides should be ready to send
-            # a command. if not, the connection was either returned to the
-            # pool before all data has been read or the socket has been
-            # closed. either way, reconnect and verify everything is good.
-            try:
-                if await connection.can_read():
-                    raise ConnectionError("Connection has data") from None
-            except ConnectionError:
-                await connection.disconnect()
-                await connection.connect()
-                if await connection.can_read():
-                    raise ConnectionError("Connection not ready") from None
-        except BaseException:
-            # release the connection back to the pool so that we don't
-            # leak it
-            await self.release(connection)
-            raise
-
-        return connection
-
-    def get_encoder(self):
-        """Return an encoder based on encoding settings"""
-        kwargs = self.connection_kwargs
-        return self.encoder_class(
-            encoding=kwargs.get("encoding", "utf-8"),
-            encoding_errors=kwargs.get("encoding_errors", "strict"),
-            decode_responses=kwargs.get("decode_responses", False),
-        )
-
-    def make_connection(self):
-        """Create a new connection"""
-        if self._created_connections >= self.max_connections:
-            raise ConnectionError("Too many connections")
-        self._created_connections += 1
-        return self.connection_class(**self.connection_kwargs)
-
-    async def release(self, connection: Connection):
-        """Releases the connection back to the pool"""
-        self._checkpid()
-        async with self._lock:
-            try:
-                self._in_use_connections.remove(connection)
-            except KeyError:
-                # Gracefully fail when a connection is returned to this pool
-                # that the pool doesn't actually own
-                pass
-
-            if self.owns_connection(connection):
-                self._available_connections.append(connection)
-            else:
-                # pool doesn't own this connection. do not add it back
-                # to the pool and decrement the count so that another
-                # connection can take its place if needed
-                self._created_connections -= 1
-                await connection.disconnect()
-                return
-
-    def owns_connection(self, connection: Connection):
-        return connection.pid == self.pid
-
-    async def disconnect(self, inuse_connections: bool = True):
-        """
-        Disconnects connections in the pool
-
-        If ``inuse_connections`` is True, disconnect connections that are
-        current in use, potentially by other tasks. Otherwise only disconnect
-        connections that are idle in the pool.
-        """
-        self._checkpid()
-        async with self._lock:
-            if inuse_connections:
-                connections: Iterable[Connection] = chain(
-                    self._available_connections, self._in_use_connections
-                )
-            else:
-                connections = self._available_connections
-            resp = await asyncio.gather(
-                *(connection.disconnect() for connection in connections),
-                return_exceptions=True,
-            )
-            exc = next((r for r in resp if isinstance(r, BaseException)), None)
-            if exc:
-                raise exc
-
-
-class BlockingConnectionPool(ConnectionPool):
-    """
-    Thread-safe blocking connection pool::
-
-        >>> from aioredis.client import Redis
-        >>> client = Redis(connection_pool=BlockingConnectionPool())
-
-    It performs the same function as the default
-    :py:class:`~redis.ConnectionPool` implementation, in that,
-    it maintains a pool of reusable connections that can be shared by
-    multiple redis clients (safely across threads if required).
-
-    The difference is that, in the event that a client tries to get a
-    connection from the pool when all of connections are in use, rather than
-    raising a :py:class:`~redis.ConnectionError` (as the default
-    :py:class:`~redis.ConnectionPool` implementation does), it
-    makes the client wait ("blocks") for a specified number of seconds until
-    a connection becomes available.
-
-    Use ``max_connections`` to increase / decrease the pool size::
-
-        >>> pool = BlockingConnectionPool(max_connections=10)
-
-    Use ``timeout`` to tell it either how many seconds to wait for a connection
-    to become available, or to block forever:
-
-        >>> # Block forever.
-        >>> pool = BlockingConnectionPool(timeout=None)
-
-        >>> # Raise a ``ConnectionError`` after five seconds if a connection is
-        >>> # not available.
-        >>> pool = BlockingConnectionPool(timeout=5)
-    """
-
-    def __init__(
-        self,
-        max_connections: int = 50,
-        timeout: Optional[int] = 20,
-        connection_class: Type[Connection] = Connection,
-        queue_class: Type[asyncio.Queue] = asyncio.LifoQueue,
-        **connection_kwargs,
-    ):
-
-        self.queue_class = queue_class
-        self.timeout = timeout
-        self._connections: List[Connection]
-        super().__init__(
-            connection_class=connection_class,
-            max_connections=max_connections,
-            **connection_kwargs,
-        )
-
-    def reset(self):
-        # Create and fill up a thread safe queue with ``None`` values.
-        self.pool = self.queue_class(self.max_connections)
-        while True:
-            try:
-                self.pool.put_nowait(None)
-            except asyncio.QueueFull:
-                break
-
-        # Keep a list of actual connection instances so that we can
-        # disconnect them later.
-        self._connections = []
-
-        # this must be the last operation in this method. while reset() is
-        # called when holding _fork_lock, other threads in this process
-        # can call _checkpid() which compares self.pid and os.getpid() without
-        # holding any lock (for performance reasons). keeping this assignment
-        # as the last operation ensures that those other threads will also
-        # notice a pid difference and block waiting for the first thread to
-        # release _fork_lock. when each of these threads eventually acquire
-        # _fork_lock, they will notice that another thread already called
-        # reset() and they will immediately release _fork_lock and continue on.
-        self.pid = os.getpid()
-
-    def make_connection(self):
-        """Make a fresh connection."""
-        connection = self.connection_class(**self.connection_kwargs)
-        self._connections.append(connection)
-        return connection
-
-    async def get_connection(self, command_name, *keys, **options):
-        """
-        Get a connection, blocking for ``self.timeout`` until a connection
-        is available from the pool.
-
-        If the connection returned is ``None`` then creates a new connection.
-        Because we use a last-in first-out queue, the existing connections
-        (having been returned to the pool after the initial ``None`` values
-        were added) will be returned before ``None`` values. This means we only
-        create new connections when we need to, i.e.: the actual number of
-        connections will only increase in response to demand.
-        """
-        # Make sure we haven't changed process.
-        self._checkpid()
-
-        # Try and get a connection from the pool. If one isn't available within
-        # self.timeout then raise a ``ConnectionError``.
-        connection = None
-        try:
-            async with async_timeout.timeout(self.timeout):
-                connection = await self.pool.get()
-        except (asyncio.QueueEmpty, asyncio.TimeoutError):
-            # Note that this is not caught by the redis client and will be
-            # raised unless handled by application code. If you want never to
-            raise ConnectionError("No connection available.")
-
-        # If the ``connection`` is actually ``None`` then that's a cue to make
-        # a new connection to add to the pool.
-        if connection is None:
-            connection = self.make_connection()
-
-        try:
-            # ensure this connection is connected to Redis
-            await connection.connect()
-            # connections that the pool provides should be ready to send
-            # a command. if not, the connection was either returned to the
-            # pool before all data has been read or the socket has been
-            # closed. either way, reconnect and verify everything is good.
-            try:
-                if await connection.can_read():
-                    raise ConnectionError("Connection has data") from None
-            except ConnectionError:
-                await connection.disconnect()
-                await connection.connect()
-                if await connection.can_read():
-                    raise ConnectionError("Connection not ready") from None
-        except BaseException:
-            # release the connection back to the pool so that we don't leak it
-            await self.release(connection)
-            raise
-
-        return connection
-
-    async def release(self, connection: Connection):
-        """Releases the connection back to the pool."""
-        # Make sure we haven't changed process.
-        self._checkpid()
-        if not self.owns_connection(connection):
-            # pool doesn't own this connection. do not add it back
-            # to the pool. instead add a None value which is a placeholder
-            # that will cause the pool to recreate the connection if
-            # its needed.
-            await connection.disconnect()
-            self.pool.put_nowait(None)
-            return
-
-        # Put the connection back into the pool.
-        try:
-            self.pool.put_nowait(connection)
-        except asyncio.QueueFull:
-            # perhaps the pool has been reset() after a fork? regardless,
-            # we don't want this connection
-            pass
-
-    async def disconnect(self, inuse_connections: bool = True):
-        """Disconnects all connections in the pool."""
-        self._checkpid()
-        async with self._lock:
-            resp = await asyncio.gather(
-                *(connection.disconnect() for connection in self._connections),
-                return_exceptions=True,
-            )
-            exc = next((r for r in resp if isinstance(r, BaseException)), None)
-            if exc:
-                raise exc
+import asyncio
+import enum
+import errno
+import inspect
+import io
+import os
+import socket
+import ssl
+import threading
+import warnings
+from distutils.version import StrictVersion
+from itertools import chain
+from types import MappingProxyType
+from typing import (
+    Any,
+    Callable,
+    Iterable,
+    List,
+    Mapping,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
+from urllib.parse import ParseResult, parse_qs, unquote, urlparse
+
+import async_timeout
+
+from .compat import Protocol, TypedDict
+from .exceptions import (
+    AuthenticationError,
+    AuthenticationWrongNumberOfArgsError,
+    BusyLoadingError,
+    ChildDeadlockedError,
+    ConnectionError,
+    DataError,
+    ExecAbortError,
+    InvalidResponse,
+    ModuleError,
+    NoPermissionError,
+    NoScriptError,
+    ReadOnlyError,
+    RedisError,
+    ResponseError,
+    TimeoutError,
+)
+from .utils import str_if_bytes
+
+NONBLOCKING_EXCEPTION_ERROR_NUMBERS = {
+    BlockingIOError: errno.EWOULDBLOCK,
+    ssl.SSLWantReadError: 2,
+    ssl.SSLWantWriteError: 2,
+    ssl.SSLError: 2,
+}
+
+NONBLOCKING_EXCEPTIONS = tuple(NONBLOCKING_EXCEPTION_ERROR_NUMBERS.keys())
+
+try:
+    import hiredis
+
+except (ImportError, ModuleNotFoundError):
+    HIREDIS_AVAILABLE = False
+else:
+    HIREDIS_AVAILABLE = True
+    hiredis_version = StrictVersion(hiredis.__version__)
+    if hiredis_version < StrictVersion("1.0.0"):
+        warnings.warn(
+            "aioredis supports hiredis @ 1.0.0 or higher. "
+            f"You have hiredis @ {hiredis.__version__}. "
+            "Pure-python parser will be used instead."
+        )
+        HIREDIS_AVAILABLE = False
+
+SYM_STAR = b"*"
+SYM_DOLLAR = b"$"
+SYM_CRLF = b"\r\n"
+SYM_LF = b"\n"
+SYM_EMPTY = b""
+
+SERVER_CLOSED_CONNECTION_ERROR = "Connection closed by server."
+
+
+class _Sentinel(enum.Enum):
+    sentinel = object()
+
+
+SENTINEL = _Sentinel.sentinel
+MODULE_LOAD_ERROR = "Error loading the extension. Please check the server logs."
+NO_SUCH_MODULE_ERROR = "Error unloading module: no such module with that name"
+MODULE_UNLOAD_NOT_POSSIBLE_ERROR = "Error unloading module: operation not possible."
+MODULE_EXPORTS_DATA_TYPES_ERROR = (
+    "Error unloading module: the module "
+    "exports one or more module-side data "
+    "types, can't unload"
+)
+
+EncodedT = Union[bytes, memoryview]
+DecodedT = Union[str, int, float]
+EncodableT = Union[EncodedT, DecodedT]
+
+
+class _HiredisReaderArgs(TypedDict, total=False):
+    protocolError: Callable[[str], Exception]
+    replyError: Callable[[str], Exception]
+    encoding: Optional[str]
+    errors: Optional[str]
+
+
+class Encoder:
+    """Encode strings to bytes-like and decode bytes-like to strings"""
+
+    __slots__ = "encoding", "encoding_errors", "decode_responses"
+
+    def __init__(self, encoding: str, encoding_errors: str, decode_responses: bool):
+        self.encoding = encoding
+        self.encoding_errors = encoding_errors
+        self.decode_responses = decode_responses
+
+    def encode(self, value: EncodableT) -> EncodedT:
+        """Return a bytestring or bytes-like representation of the value"""
+        if isinstance(value, (bytes, memoryview)):
+            return value
+        if isinstance(value, bool):
+            # special case bool since it is a subclass of int
+            raise DataError(
+                "Invalid input of type: 'bool'. "
+                "Convert to a bytes, string, int or float first."
+            )
+        if isinstance(value, (int, float)):
+            return repr(value).encode()
+        if not isinstance(value, str):
+            # a value we don't know how to deal with. throw an error
+            typename = value.__class__.__name__  # type: ignore[unreachable]
+            raise DataError(
+                f"Invalid input of type: {typename!r}. "
+                "Convert to a bytes, string, int or float first."
+            )
+        return value.encode(self.encoding, self.encoding_errors)
+
+    def decode(self, value: EncodableT, force=False) -> EncodableT:
+        """Return a unicode string from the bytes-like representation"""
+        if self.decode_responses or force:
+            if isinstance(value, memoryview):
+                return value.tobytes().decode(self.encoding, self.encoding_errors)
+            if isinstance(value, bytes):
+                return value.decode(self.encoding, self.encoding_errors)
+        return value
+
+
+ExceptionMappingT = Mapping[str, Union[Type[Exception], Mapping[str, Type[Exception]]]]
+
+
+class BaseParser:
+    """Plain Python parsing class"""
+
+    __slots__ = "_stream", "_buffer", "_read_size"
+
+    EXCEPTION_CLASSES: ExceptionMappingT = {
+        "ERR": {
+            "max number of clients reached": ConnectionError,
+            "Client sent AUTH, but no password is set": AuthenticationError,
+            "invalid password": AuthenticationError,
+            # some Redis server versions report invalid command syntax
+            # in lowercase
+            "wrong number of arguments for 'auth' command": AuthenticationWrongNumberOfArgsError,
+            # some Redis server versions report invalid command syntax
+            # in uppercase
+            "wrong number of arguments for 'AUTH' command": AuthenticationWrongNumberOfArgsError,
+            MODULE_LOAD_ERROR: ModuleError,
+            MODULE_EXPORTS_DATA_TYPES_ERROR: ModuleError,
+            NO_SUCH_MODULE_ERROR: ModuleError,
+            MODULE_UNLOAD_NOT_POSSIBLE_ERROR: ModuleError,
+        },
+        "EXECABORT": ExecAbortError,
+        "LOADING": BusyLoadingError,
+        "NOSCRIPT": NoScriptError,
+        "READONLY": ReadOnlyError,
+        "NOAUTH": AuthenticationError,
+        "NOPERM": NoPermissionError,
+    }
+
+    def __init__(self, socket_read_size: int):
+        self._stream: Optional[asyncio.StreamReader] = None
+        self._buffer: Optional[SocketBuffer] = None
+        self._read_size = socket_read_size
+
+    def __del__(self):
+        try:
+            self.on_disconnect()
+        except BaseException :
+            pass
+
+    def parse_error(self, response: str) -> ResponseError:
+        """Parse an error response"""
+        error_code = response.split(" ")[0]
+        if error_code in self.EXCEPTION_CLASSES:
+            response = response[len(error_code) + 1 :]
+            exception_class_or_dict = self.EXCEPTION_CLASSES[error_code]
+            if isinstance(exception_class_or_dict, dict):
+                exception_class = exception_class_or_dict.get(response, ResponseError)
+            else:
+                exception_class = exception_class_or_dict
+            return exception_class(response)
+        return ResponseError(response)
+
+    def on_disconnect(self):
+        raise NotImplementedError()
+
+    def on_connect(self, connection: "Connection"):
+        raise NotImplementedError()
+
+    async def can_read(self, timeout: float) -> bool:
+        raise NotImplementedError()
+
+    async def read_response(
+        self,
+    ) -> Union[EncodableT, ResponseError, None, List[EncodableT]]:
+        raise NotImplementedError()
+
+
+class SocketBuffer:
+    """Async-friendly re-impl of redis-py's SocketBuffer.
+
+    TODO: We're currently passing through two buffers,
+        the asyncio.StreamReader and this. I imagine we can reduce the layers here
+        while maintaining compliance with prior art.
+    """
+
+    def __init__(
+        self,
+        stream_reader: asyncio.StreamReader,
+        socket_read_size: int,
+        socket_timeout: Optional[float],
+    ):
+        self._stream: Optional[asyncio.StreamReader] = stream_reader
+        self.socket_read_size = socket_read_size
+        self.socket_timeout = socket_timeout
+        self._buffer: Optional[io.BytesIO] = io.BytesIO()
+        # number of bytes written to the buffer from the socket
+        self.bytes_written = 0
+        # number of bytes read from the buffer
+        self.bytes_read = 0
+
+    @property
+    def length(self):
+        return self.bytes_written - self.bytes_read
+
+    async def _read_from_socket(
+        self,
+        length: Optional[int] = None,
+        timeout: Union[float, None, _Sentinel] = SENTINEL,
+        raise_on_timeout: bool = True,
+    ) -> bool:
+        buf = self._buffer
+        if buf is None or self._stream is None:
+            raise RedisError("Buffer is closed.")
+        buf.seek(self.bytes_written)
+        marker = 0
+        timeout = timeout if timeout is not SENTINEL else self.socket_timeout
+
+        try:
+            while True:
+                async with async_timeout.timeout(timeout):
+                    data = await self._stream.read(self.socket_read_size)
+                # an empty string indicates the server shutdown the socket
+                if isinstance(data, bytes) and len(data) == 0:
+                    raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
+                buf.write(data)
+                data_length = len(data)
+                self.bytes_written += data_length
+                marker += data_length
+
+                if length is not None and length > marker:
+                    continue
+                return True
+        except (socket.timeout, asyncio.TimeoutError):
+            if raise_on_timeout:
+                raise TimeoutError("Timeout reading from socket")
+            return False
+        except NONBLOCKING_EXCEPTIONS as ex:
+            # if we're in nonblocking mode and the recv raises a
+            # blocking error, simply return False indicating that
+            # there's no data to be read. otherwise raise the
+            # original exception.
+            allowed = NONBLOCKING_EXCEPTION_ERROR_NUMBERS.get(ex.__class__, -1)
+            if not raise_on_timeout and ex.errno == allowed:
+                return False
+            raise ConnectionError(f"Error while reading from socket: {ex.args}")
+
+    async def can_read(self, timeout: float) -> bool:
+        return bool(self.length) or await self._read_from_socket(
+            timeout=timeout, raise_on_timeout=False
+        )
+
+    async def read(self, length: int) -> bytes:
+        length = length + 2  # make sure to read the \r\n terminator
+        # make sure we've read enough data from the socket
+        if length > self.length:
+            await self._read_from_socket(length - self.length)
+
+        if self._buffer is None:
+            raise RedisError("Buffer is closed.")
+
+        self._buffer.seek(self.bytes_read)
+        data = self._buffer.read(length)
+        self.bytes_read += len(data)
+
+        # purge the buffer when we've consumed it all so it doesn't
+        # grow forever
+        if self.bytes_read == self.bytes_written:
+            self.purge()
+
+        return data[:-2]
+
+    async def readline(self) -> bytes:
+        buf = self._buffer
+        if buf is None:
+            raise RedisError("Buffer is closed.")
+
+        buf.seek(self.bytes_read)
+        data = buf.readline()
+        while not data.endswith(SYM_CRLF):
+            # there's more data in the socket that we need
+            await self._read_from_socket()
+            buf.seek(self.bytes_read)
+            data = buf.readline()
+
+        self.bytes_read += len(data)
+
+        # purge the buffer when we've consumed it all so it doesn't
+        # grow forever
+        if self.bytes_read == self.bytes_written:
+            self.purge()
+
+        return data[:-2]
+
+    def purge(self):
+        if self._buffer is None:
+            raise RedisError("Buffer is closed.")
+
+        self._buffer.seek(0)
+        self._buffer.truncate()
+        self.bytes_written = 0
+        self.bytes_read = 0
+
+    def close(self):
+        try:
+            self.purge()
+            self._buffer.close()  # type: ignore[union-attr]
+        except BaseException :
+            # issue #633 suggests the purge/close somehow raised a
+            # BadFileDescriptor error. Perhaps the client ran out of
+            # memory or something else? It's probably OK to ignore
+            # any error being raised from purge/close since we're
+            # removing the reference to the instance below.
+            pass
+        self._buffer = None
+        self._stream = None
+
+
+class PythonParser(BaseParser):
+    """Plain Python parsing class"""
+
+    __slots__ = BaseParser.__slots__ + ("encoder",)
+
+    def __init__(self, socket_read_size: int):
+        super().__init__(socket_read_size)
+        self.encoder: Optional[Encoder] = None
+
+    def on_connect(self, connection: "Connection"):
+        """Called when the stream connects"""
+        self._stream = connection._reader
+        if self._stream is None:
+            raise RedisError("Buffer is closed.")
+
+        self._buffer = SocketBuffer(
+            self._stream, self._read_size, connection.socket_timeout
+        )
+        self.encoder = connection.encoder
+
+    def on_disconnect(self):
+        """Called when the stream disconnects"""
+        if self._stream is not None:
+            self._stream = None
+        if self._buffer is not None:
+            self._buffer.close()
+            self._buffer = None
+        self.encoder = None
+
+    async def can_read(self, timeout: float):
+        return self._buffer and bool(await self._buffer.can_read(timeout))
+
+    async def read_response(self) -> Union[EncodableT, ResponseError, None]:
+        if not self._buffer or not self.encoder:
+            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
+        raw = await self._buffer.readline()
+        if not raw:
+            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
+        response: Any
+        byte, response = raw[:1], raw[1:]
+
+        if byte not in (b"-", b"+", b":", b"$", b"*"):
+            raise InvalidResponse(f"Protocol Error: {raw!r}")
+
+        # server returned an error
+        if byte == b"-":
+            response = response.decode("utf-8", errors="replace")
+            error = self.parse_error(response)
+            # if the error is a ConnectionError, raise immediately so the user
+            # is notified
+            if isinstance(error, ConnectionError):
+                raise error
+            # otherwise, we're dealing with a ResponseError that might belong
+            # inside a pipeline response. the connection's read_response()
+            # and/or the pipeline's execute() will raise this error if
+            # necessary, so just return the exception instance here.
+            return error
+        # single value
+        elif byte == b"+":
+            pass
+        # int value
+        elif byte == b":":
+            response = int(response)
+        # bulk response
+        elif byte == b"$":
+            length = int(response)
+            if length == -1:
+                return None
+            response = await self._buffer.read(length)
+        # multi-bulk response
+        elif byte == b"*":
+            length = int(response)
+            if length == -1:
+                return None
+            response = [(await self.read_response()) for _ in range(length)]
+        if isinstance(response, bytes):
+            response = self.encoder.decode(response)
+        return response
+
+
+class HiredisParser(BaseParser):
+    """Parser class for connections using Hiredis"""
+
+    __slots__ = BaseParser.__slots__ + ("_next_response", "_reader", "_socket_timeout")
+
+    _next_response: bool
+
+    def __init__(self, socket_read_size: int):
+        if not HIREDIS_AVAILABLE:
+            raise RedisError("Hiredis is not available.")
+        super().__init__(socket_read_size=socket_read_size)
+        self._reader: Optional[hiredis.Reader] = None
+        self._socket_timeout: Optional[float] = None
+
+    def on_connect(self, connection: "Connection"):
+        self._stream = connection._reader
+        kwargs: _HiredisReaderArgs = {
+            "protocolError": InvalidResponse,
+            "replyError": self.parse_error,
+        }
+        if connection.encoder.decode_responses:
+            kwargs["encoding"] = connection.encoder.encoding
+            kwargs["errors"] = connection.encoder.encoding_errors
+
+        self._reader = hiredis.Reader(**kwargs)
+        self._next_response = False
+        self._socket_timeout = connection.socket_timeout
+
+    def on_disconnect(self):
+        self._stream = None
+        self._reader = None
+        self._next_response = False
+
+    async def can_read(self, timeout: float):
+        if not self._reader:
+            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR)
+
+        if self._next_response is False:
+            self._next_response = self._reader.gets()
+        if self._next_response is False:
+            return await self.read_from_socket(timeout=timeout, raise_on_timeout=False)
+        return True
+
+    async def read_from_socket(
+        self,
+        timeout: Union[float, None, _Sentinel] = SENTINEL,
+        raise_on_timeout: bool = True,
+    ):
+        if self._stream is None or self._reader is None:
+            raise RedisError("Parser already closed.")
+
+        timeout = self._socket_timeout if timeout is SENTINEL else timeout
+        try:
+            async with async_timeout.timeout(timeout):
+                buffer = await self._stream.read(self._read_size)
+            if not isinstance(buffer, bytes) or len(buffer) == 0:
+                raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR) from None
+            self._reader.feed(buffer)
+            # data was read from the socket and added to the buffer.
+            # return True to indicate that data was read.
+            return True
+        except asyncio.CancelledError:
+            raise
+        except (socket.timeout, asyncio.TimeoutError):
+            if raise_on_timeout:
+                raise TimeoutError("Timeout reading from socket") from None
+            return False
+        except NONBLOCKING_EXCEPTIONS as ex:
+            # if we're in nonblocking mode and the recv raises a
+            # blocking error, simply return False indicating that
+            # there's no data to be read. otherwise raise the
+            # original exception.
+            allowed = NONBLOCKING_EXCEPTION_ERROR_NUMBERS.get(ex.__class__, -1)
+            if not raise_on_timeout and ex.errno == allowed:
+                return False
+            raise ConnectionError(f"Error while reading from socket: {ex.args}")
+
+    async def read_response(self) -> Union[EncodableT, List[EncodableT]]:
+        if not self._stream or not self._reader:
+            self.on_disconnect()
+            raise ConnectionError(SERVER_CLOSED_CONNECTION_ERROR) from None
+
+        response: Union[
+            EncodableT, ConnectionError, List[Union[EncodableT, ConnectionError]]
+        ]
+        # _next_response might be cached from a can_read() call
+        if self._next_response is not False:
+            response = self._next_response
+            self._next_response = False
+            return response
+
+        response = self._reader.gets()
+        while response is False:
+            await self.read_from_socket()
+            response = self._reader.gets()
+
+        # if the response is a ConnectionError or the response is a list and
+        # the first item is a ConnectionError, raise it as something bad
+        # happened
+        if isinstance(response, ConnectionError):
+            raise response
+        elif (
+            isinstance(response, list)
+            and response
+            and isinstance(response[0], ConnectionError)
+        ):
+            raise response[0]
+        # cast as there won't be a ConnectionError here.
+        return cast(Union[EncodableT, List[EncodableT]], response)
+
+
+DefaultParser: Type[Union[PythonParser, HiredisParser]]
+if HIREDIS_AVAILABLE:
+    DefaultParser = HiredisParser
+else:
+    DefaultParser = PythonParser
+
+
+class ConnectCallbackProtocol(Protocol):
+    def __call__(self, connection: "Connection"):
+        ...
+
+
+class AsyncConnectCallbackProtocol(Protocol):
+    async def __call__(self, connection: "Connection"):
+        ...
+
+
+ConnectCallbackT = Union[ConnectCallbackProtocol, AsyncConnectCallbackProtocol]
+
+
+class Connection:
+    """Manages TCP communication to and from a Redis server"""
+
+    __slots__ = (
+        "pid",
+        "host",
+        "port",
+        "db",
+        "username",
+        "client_name",
+        "password",
+        "socket_timeout",
+        "socket_connect_timeout",
+        "socket_keepalive",
+        "socket_keepalive_options",
+        "socket_type",
+        "retry_on_timeout",
+        "health_check_interval",
+        "next_health_check",
+        "last_active_at",
+        "encoder",
+        "ssl_context",
+        "_reader",
+        "_writer",
+        "_parser",
+        "_connect_callbacks",
+        "_buffer_cutoff",
+        "_lock",
+        "__dict__",
+    )
+
+    def __init__(
+        self,
+        *,
+        host: str = "localhost",
+        port: Union[str, int] = 6379,
+        db: Union[str, int] = 0,
+        password: Optional[str] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        socket_keepalive: bool = False,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        socket_type: int = 0,
+        retry_on_timeout: bool = False,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        parser_class: Type[BaseParser] = DefaultParser,
+        socket_read_size: int = 65536,
+        health_check_interval: float = 0,
+        client_name: Optional[str] = None,
+        username: Optional[str] = None,
+        encoder_class: Type[Encoder] = Encoder,
+    ):
+        self.pid = os.getpid()
+        self.host = host
+        self.port = int(port)
+        self.db = db
+        self.username = username
+        self.client_name = client_name
+        self.password = password
+        self.socket_timeout = socket_timeout
+        self.socket_connect_timeout = socket_connect_timeout or socket_timeout or None
+        self.socket_keepalive = socket_keepalive
+        self.socket_keepalive_options = socket_keepalive_options or {}
+        self.socket_type = socket_type
+        self.retry_on_timeout = retry_on_timeout
+        self.health_check_interval = health_check_interval
+        self.next_health_check: float = -1
+        self.ssl_context: Optional[RedisSSLContext] = None
+        self.encoder = encoder_class(encoding, encoding_errors, decode_responses)
+        self._reader: Optional[asyncio.StreamReader] = None
+        self._writer: Optional[asyncio.StreamWriter] = None
+        self._parser = parser_class(
+            socket_read_size=socket_read_size,
+        )
+        self._connect_callbacks: List[ConnectCallbackT] = []
+        self._buffer_cutoff = 6000
+        self._lock = asyncio.Lock()
+
+    def __repr__(self):
+        repr_args = ",".join((f"{k}={v}" for k, v in self.repr_pieces()))
+        return f"{self.__class__.__name__}<{repr_args}>"
+
+    def repr_pieces(self):
+        pieces = [("host", self.host), ("port", self.port), ("db", self.db)]
+        if self.client_name:
+            pieces.append(("client_name", self.client_name))
+        return pieces
+
+    def __del__(self):
+        try:
+            if self.is_connected:
+                loop = asyncio.get_event_loop()
+                coro = self.disconnect()
+                if loop.is_running():
+                    loop.create_task(coro)
+                else:
+                    loop.run_until_complete(coro)
+        except BaseException :
+            pass
+
+    @property
+    def is_connected(self):
+        return bool(self._reader and self._writer)
+
+    def register_connect_callback(self, callback):
+        self._connect_callbacks.append(callback)
+
+    def clear_connect_callbacks(self):
+        self._connect_callbacks = []
+
+    async def connect(self):
+        """Connects to the Redis server if not already connected"""
+        if self.is_connected:
+            return
+        try:
+            await self._connect()
+        except asyncio.CancelledError:
+            raise
+        except (socket.timeout, asyncio.TimeoutError):
+            raise TimeoutError("Timeout connecting to server")
+        except OSError as e:
+            raise ConnectionError(self._error_message(e))
+        except BaseException as exc:
+            raise ConnectionError(exc) from exc
+
+        try:
+            await self.on_connect()
+        except RedisError:
+            # clean up after any error in on_connect
+            await self.disconnect()
+            raise
+
+        # run any user callbacks. right now the only internal callback
+        # is for pubsub channel/pattern resubscription
+        for callback in self._connect_callbacks:
+            task = callback(self)
+            if task and inspect.isawaitable(task):
+                await task
+
+    async def _connect(self):
+        """Create a TCP socket connection"""
+        async with async_timeout.timeout(self.socket_connect_timeout):
+            reader, writer = await asyncio.open_connection(
+                host=self.host,
+                port=self.port,
+                ssl=self.ssl_context.get() if self.ssl_context else None,
+            )
+        self._reader = reader
+        self._writer = writer
+        sock = writer.transport.get_extra_info("socket")
+        if sock is not None:
+            sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+            try:
+                # TCP_KEEPALIVE
+                if self.socket_keepalive:
+                    sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+                    for k, v in self.socket_keepalive_options.items():
+                        sock.setsockopt(socket.SOL_TCP, k, v)
+
+            except (OSError, TypeError):
+                # `socket_keepalive_options` might contain invalid options
+                # causing an error. Do not leave the connection open.
+                writer.close()
+                raise
+
+    def _error_message(self, exception):
+        # args for socket.error can either be (errno, "message")
+        # or just "message"
+        if len(exception.args) == 1:
+            return f"Error connecting to {self.host}:{self.port}. {exception.args[0]}."
+        else:
+            return (
+                f"Error {exception.args[0]} connecting to {self.host}:{self.port}. "
+                f"{exception.args[0]}."
+            )
+
+    async def on_connect(self):
+        """Initialize the connection, authenticate and select a database"""
+        self._parser.on_connect(self)
+
+        # if username and/or password are set, authenticate
+        if self.username or self.password:
+            auth_args: Union[Tuple[str], Tuple[str, str]]
+            if self.username:
+                auth_args = (self.username, self.password or "")
+            else:
+                # Mypy bug: https://github.com/python/mypy/issues/10944
+                auth_args = (self.password or "",)
+            # avoid checking health here -- PING will fail if we try
+            # to check the health prior to the AUTH
+            await self.send_command("AUTH", *auth_args, check_health=False)
+
+            try:
+                auth_response = await self.read_response()
+            except AuthenticationWrongNumberOfArgsError:
+                # a username and password were specified but the Redis
+                # server seems to be < 6.0.0 which expects a single password
+                # arg. retry auth with just the password.
+                # https://github.com/andymccurdy/redis-py/issues/1274
+                await self.send_command("AUTH", self.password, check_health=False)
+                auth_response = await self.read_response()
+
+            if str_if_bytes(auth_response) != "OK":
+                raise AuthenticationError("Invalid Username or Password")
+
+        # if a client_name is given, set it
+        if self.client_name:
+            await self.send_command("CLIENT", "SETNAME", self.client_name)
+            if str_if_bytes(await self.read_response()) != "OK":
+                raise ConnectionError("Error setting client name")
+
+        # if a database is specified, switch to it
+        if self.db:
+            await self.send_command("SELECT", self.db)
+            if str_if_bytes(await self.read_response()) != "OK":
+                raise ConnectionError("Invalid Database")
+
+    async def disconnect(self):
+        """Disconnects from the Redis server"""
+        try:
+            async with async_timeout.timeout(self.socket_connect_timeout):
+                self._parser.on_disconnect()
+                if not self.is_connected:
+                    return
+                try:
+                    if os.getpid() == self.pid:
+                        self._writer.close()  # type: ignore[union-attr]
+                        # py3.6 doesn't have this method
+                        if hasattr(self._writer, "wait_closed"):
+                            await self._writer.wait_closed()  # type: ignore[union-attr]
+                except OSError:
+                    pass
+                self._reader = None
+                self._writer = None
+        except asyncio.TimeoutError:
+            raise TimeoutError(
+                f"Timed out closing connection after {self.socket_connect_timeout}"
+            ) from None
+
+    async def check_health(self):
+        """Check the health of the connection with a PING/PONG"""
+        if (
+            self.health_check_interval
+            and asyncio.get_event_loop().time() > self.next_health_check
+        ):
+            try:
+                await self.send_command("PING", check_health=False)
+                if str_if_bytes(await self.read_response()) != "PONG":
+                    raise ConnectionError("Bad response from PING health check")
+            except (ConnectionError, TimeoutError) as err:
+                await self.disconnect()
+                try:
+                    await self.send_command("PING", check_health=False)
+                    if str_if_bytes(await self.read_response()) != "PONG":
+                        raise ConnectionError(
+                            "Bad response from PING health check"
+                        ) from None
+                except BaseException as err2:
+                    raise err2 from err
+
+    async def _send_packed_command(self, command: Iterable[bytes]) -> None:
+        if self._writer is None:
+            raise RedisError("Connection already closed.")
+
+        self._writer.writelines(command)
+        await self._writer.drain()
+
+    async def send_packed_command(
+        self,
+        command: Union[bytes, str, Iterable[bytes]],
+        check_health: bool = True,
+    ):
+        """Send an already packed command to the Redis server"""
+        if not self._writer:
+            await self.connect()
+        # guard against health check recursion
+        if check_health:
+            await self.check_health()
+        try:
+            if isinstance(command, str):
+                command = command.encode()
+            if isinstance(command, bytes):
+                command = [command]
+            await asyncio.wait_for(
+                self._send_packed_command(command),
+                self.socket_timeout,
+            )
+        except asyncio.TimeoutError:
+            await self.disconnect()
+            raise TimeoutError("Timeout writing to socket") from None
+        except OSError as e:
+            await self.disconnect()
+            if len(e.args) == 1:
+                err_no, errmsg = "UNKNOWN", e.args[0]
+            else:
+                err_no = e.args[0]
+                errmsg = e.args[1]
+            raise ConnectionError(
+                f"Error {err_no} while writing to socket. {errmsg}."
+            ) from e
+        except BaseException:
+            await self.disconnect()
+            raise
+
+    async def send_command(self, *args, **kwargs):
+        """Pack and send a command to the Redis server"""
+        if not self.is_connected:
+            await self.connect()
+        await self.send_packed_command(
+            self.pack_command(*args), check_health=kwargs.get("check_health", True)
+        )
+
+    async def can_read(self, timeout: float = 0):
+        """Poll the socket to see if there's data that can be read."""
+        if not self.is_connected:
+            await self.connect()
+        return await self._parser.can_read(timeout)
+
+    async def read_response(self):
+        """Read the response from a previously sent command"""
+        try:
+            async with self._lock:
+                async with async_timeout.timeout(self.socket_timeout):
+                    response = await self._parser.read_response()
+        except asyncio.TimeoutError:
+            await self.disconnect()
+            raise TimeoutError(f"Timeout reading from {self.host}:{self.port}")
+        except OSError as e:
+            await self.disconnect()
+            raise ConnectionError(
+                f"Error while reading from {self.host}:{self.port} : {e.args}"
+            )
+        except BaseException:
+            await self.disconnect()
+            raise
+
+        if self.health_check_interval:
+            self.next_health_check = (
+                asyncio.get_event_loop().time() + self.health_check_interval
+            )
+
+        if isinstance(response, ResponseError):
+            raise response from None
+        return response
+
+    def pack_command(self, *args: EncodableT) -> List[bytes]:
+        """Pack a series of arguments into the Redis protocol"""
+        output = []
+        # the client might have included 1 or more literal arguments in
+        # the command name, e.g., 'CONFIG GET'. The Redis server expects these
+        # arguments to be sent separately, so split the first argument
+        # manually. These arguments should be bytestrings so that they are
+        # not encoded.
+        assert not isinstance(args[0], float)
+        if isinstance(args[0], str):
+            args = tuple(args[0].encode().split()) + args[1:]
+        elif b" " in args[0]:
+            args = tuple(args[0].split()) + args[1:]
+
+        buff = SYM_EMPTY.join((SYM_STAR, str(len(args)).encode(), SYM_CRLF))
+
+        buffer_cutoff = self._buffer_cutoff
+        for arg in map(self.encoder.encode, args):
+            # to avoid large string mallocs, chunk the command into the
+            # output list if we're sending large values or memoryviews
+            arg_length = len(arg)
+            if (
+                len(buff) > buffer_cutoff
+                or arg_length > buffer_cutoff
+                or isinstance(arg, memoryview)
+            ):
+                buff = SYM_EMPTY.join(
+                    (buff, SYM_DOLLAR, str(arg_length).encode(), SYM_CRLF)
+                )
+                output.append(buff)
+                output.append(arg)
+                buff = SYM_CRLF
+            else:
+                buff = SYM_EMPTY.join(
+                    (
+                        buff,
+                        SYM_DOLLAR,
+                        str(arg_length).encode(),
+                        SYM_CRLF,
+                        arg,
+                        SYM_CRLF,
+                    )
+                )
+        output.append(buff)
+        return output
+
+    def pack_commands(self, commands: Iterable[Iterable[EncodableT]]) -> List[bytes]:
+        """Pack multiple commands into the Redis protocol"""
+        output: List[bytes] = []
+        pieces: List[bytes] = []
+        buffer_length = 0
+        buffer_cutoff = self._buffer_cutoff
+
+        for cmd in commands:
+            for chunk in self.pack_command(*cmd):
+                chunklen = len(chunk)
+                if (
+                    buffer_length > buffer_cutoff
+                    or chunklen > buffer_cutoff
+                    or isinstance(chunk, memoryview)
+                ):
+                    output.append(SYM_EMPTY.join(pieces))
+                    buffer_length = 0
+                    pieces = []
+
+                if chunklen > buffer_cutoff or isinstance(chunk, memoryview):
+                    output.append(chunk)
+                else:
+                    pieces.append(chunk)
+                    buffer_length += chunklen
+
+        if pieces:
+            output.append(SYM_EMPTY.join(pieces))
+        return output
+
+
+class SSLConnection(Connection):
+    def __init__(
+        self,
+        ssl_keyfile: Optional[str] = None,
+        ssl_certfile: Optional[str] = None,
+        ssl_cert_reqs: str = "required",
+        ssl_ca_certs: Optional[str] = None,
+        ssl_check_hostname: bool = False,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.ssl_context: RedisSSLContext = RedisSSLContext(
+            keyfile=ssl_keyfile,
+            certfile=ssl_certfile,
+            cert_reqs=ssl_cert_reqs,
+            ca_certs=ssl_ca_certs,
+            check_hostname=ssl_check_hostname,
+        )
+
+    @property
+    def keyfile(self):
+        return self.ssl_context.keyfile
+
+    @property
+    def certfile(self):
+        return self.ssl_context.certfile
+
+    @property
+    def cert_reqs(self):
+        return self.ssl_context.cert_reqs
+
+    @property
+    def ca_certs(self):
+        return self.ssl_context.ca_certs
+
+    @property
+    def check_hostname(self):
+        return self.ssl_context.check_hostname
+
+
+class RedisSSLContext:
+    __slots__ = (
+        "keyfile",
+        "certfile",
+        "cert_reqs",
+        "ca_certs",
+        "context",
+        "check_hostname",
+    )
+
+    def __init__(
+        self,
+        keyfile: Optional[str] = None,
+        certfile: Optional[str] = None,
+        cert_reqs: Optional[str] = None,
+        ca_certs: Optional[str] = None,
+        check_hostname: bool = False,
+    ):
+        self.keyfile = keyfile
+        self.certfile = certfile
+        if cert_reqs is None:
+            self.cert_reqs = ssl.CERT_NONE
+        elif isinstance(cert_reqs, str):
+            CERT_REQS = {
+                "none": ssl.CERT_NONE,
+                "optional": ssl.CERT_OPTIONAL,
+                "required": ssl.CERT_REQUIRED,
+            }
+            if cert_reqs not in CERT_REQS:
+                raise RedisError(
+                    f"Invalid SSL Certificate Requirements Flag: {cert_reqs}"
+                )
+            self.cert_reqs = CERT_REQS[cert_reqs]
+        self.ca_certs = ca_certs
+        self.check_hostname = check_hostname
+        self.context: Optional[ssl.SSLContext] = None
+
+    def get(self) -> ssl.SSLContext:
+        if not self.context:
+            context = ssl.create_default_context()
+            context.check_hostname = self.check_hostname
+            context.verify_mode = self.cert_reqs
+            if self.certfile and self.keyfile:
+                context.load_cert_chain(certfile=self.certfile, keyfile=self.keyfile)
+            if self.ca_certs:
+                context.load_verify_locations(self.ca_certs)
+            self.context = context
+        return self.context
+
+
+class UnixDomainSocketConnection(Connection):  # lgtm [py/missing-call-to-init]
+    def __init__(
+        self,
+        *,
+        path: str = "",
+        db: Union[str, int] = 0,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        retry_on_timeout: bool = False,
+        parser_class: Type[BaseParser] = DefaultParser,
+        socket_read_size: int = 65536,
+        health_check_interval: float = 0.0,
+        client_name=None,
+    ):
+        self.pid = os.getpid()
+        self.path = path
+        self.db = db
+        self.username = username
+        self.client_name = client_name
+        self.password = password
+        self.socket_timeout = socket_timeout
+        self.socket_connect_timeout = socket_connect_timeout or socket_timeout or None
+        self.retry_on_timeout = retry_on_timeout
+        self.health_check_interval = health_check_interval
+        self.next_health_check = -1
+        self.encoder = Encoder(encoding, encoding_errors, decode_responses)
+        self._sock = None
+        self._reader = None
+        self._writer = None
+        self._parser = parser_class(socket_read_size=socket_read_size)
+        self._connect_callbacks = []
+        self._buffer_cutoff = 6000
+        self._lock = asyncio.Lock()
+
+    def repr_pieces(self) -> Iterable[Tuple[str, Union[str, int]]]:
+        pieces = [
+            ("path", self.path),
+            ("db", self.db),
+        ]
+        if self.client_name:
+            pieces.append(("client_name", self.client_name))
+        return pieces
+
+    async def _connect(self):
+        async with async_timeout.timeout(self.socket_connect_timeout):
+            reader, writer = await asyncio.open_unix_connection(path=self.path)
+        self._reader = reader
+        self._writer = writer
+        await self.on_connect()
+
+    def _error_message(self, exception):
+        # args for socket.error can either be (errno, "message")
+        # or just "message"
+        if len(exception.args) == 1:
+            return f"Error connecting to unix socket: {self.path}. {exception.args[0]}."
+        else:
+            return (
+                f"Error {exception.args[0]} connecting to unix socket: "
+                f"{self.path}. {exception.args[1]}."
+            )
+
+
+FALSE_STRINGS = ("0", "F", "FALSE", "N", "NO")
+
+
+def to_bool(value) -> Optional[bool]:
+    if value is None or value == "":
+        return None
+    if isinstance(value, str) and value.upper() in FALSE_STRINGS:
+        return False
+    return bool(value)
+
+
+URL_QUERY_ARGUMENT_PARSERS: Mapping[str, Callable[..., object]] = MappingProxyType(
+    {
+        "db": int,
+        "socket_timeout": float,
+        "socket_connect_timeout": float,
+        "socket_keepalive": to_bool,
+        "retry_on_timeout": to_bool,
+        "max_connections": int,
+        "health_check_interval": int,
+        "ssl_check_hostname": to_bool,
+    }
+)
+
+
+class ConnectKwargs(TypedDict, total=False):
+    username: str
+    password: str
+    connection_class: Type[Connection]
+    host: str
+    port: int
+    db: int
+    path: str
+
+
+def parse_url(url: str) -> ConnectKwargs:
+    parsed: ParseResult = urlparse(url)
+    kwargs: ConnectKwargs = {}
+
+    for name, value_list in parse_qs(parsed.query).items():
+        if value_list and len(value_list) > 0:
+            value = unquote(value_list[0])
+            parser = URL_QUERY_ARGUMENT_PARSERS.get(name)
+            if parser:
+                try:
+                    # We can't type this.
+                    kwargs[name] = parser(value)  # type: ignore[misc]
+                except (TypeError, ValueError):
+                    raise ValueError(f"Invalid value for `{name}` in connection URL.")
+            else:
+                kwargs[name] = value  # type: ignore[misc]
+
+    if parsed.username:
+        kwargs["username"] = unquote(parsed.username)
+    if parsed.password:
+        kwargs["password"] = unquote(parsed.password)
+
+    # We only support redis://, rediss:// and unix:// schemes.
+    if parsed.scheme == "unix":
+        if parsed.path:
+            kwargs["path"] = unquote(parsed.path)
+        kwargs["connection_class"] = UnixDomainSocketConnection
+
+    elif parsed.scheme in ("redis", "rediss"):
+        if parsed.hostname:
+            kwargs["host"] = unquote(parsed.hostname)
+        if parsed.port:
+            kwargs["port"] = int(parsed.port)
+
+        # If there's a path argument, use it as the db argument if a
+        # querystring value wasn't specified
+        if parsed.path and "db" not in kwargs:
+            try:
+                kwargs["db"] = int(unquote(parsed.path).replace("/", ""))
+            except (AttributeError, ValueError):
+                pass
+
+        if parsed.scheme == "rediss":
+            kwargs["connection_class"] = SSLConnection
+    else:
+        valid_schemes = "redis://, rediss://, unix://"
+        raise ValueError(
+            f"Redis URL must specify one of the following schemes ({valid_schemes})"
+        )
+
+    return kwargs
+
+
+_CP = TypeVar("_CP", bound="ConnectionPool")
+
+
+class ConnectionPool:
+    """
+    Create a connection pool. ``If max_connections`` is set, then this
+    object raises :py:class:`~redis.ConnectionError` when the pool's
+    limit is reached.
+
+    By default, TCP connections are created unless ``connection_class``
+    is specified. Use :py:class:`~redis.UnixDomainSocketConnection` for
+    unix sockets.
+
+    Any additional keyword arguments are passed to the constructor of
+    ``connection_class``.
+    """
+
+    @classmethod
+    def from_url(cls: Type[_CP], url: str, **kwargs) -> _CP:
+        """
+        Return a connection pool configured from the given URL.
+
+        For example::
+
+            redis://[[username]:[password]]@localhost:6379/0
+            rediss://[[username]:[password]]@localhost:6379/0
+            unix://[[username]:[password]]@/path/to/socket.sock?db=0
+
+        Three URL schemes are supported:
+
+        - `redis://` creates a TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/redis>
+        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
+        - ``unix://``: creates a Unix Domain Socket connection.
+
+        The username, password, hostname, path and all querystring values
+        are passed through urllib.parse.unquote in order to replace any
+        percent-encoded values with their corresponding characters.
+
+        There are several ways to specify a database number. The first value
+        found will be used:
+            1. A ``db`` querystring option, e.g. redis://localhost?db=0
+            2. If using the redis:// or rediss:// schemes, the path argument
+               of the url, e.g. redis://localhost/0
+            3. A ``db`` keyword argument to this function.
+
+        If none of these options are specified, the default db=0 is used.
+
+        All querystring options are cast to their appropriate Python types.
+        Boolean arguments can be specified with string values "True"/"False"
+        or "Yes"/"No". Values that cannot be properly cast cause a
+        ``ValueError`` to be raised. Once parsed, the querystring arguments
+        and keyword arguments are passed to the ``ConnectionPool``'s
+        class initializer. In the case of conflicting arguments, querystring
+        arguments always win.
+        """
+        url_options = parse_url(url)
+        kwargs.update(url_options)
+        return cls(**kwargs)
+
+    def __init__(
+        self,
+        connection_class: Type[Connection] = Connection,
+        max_connections: Optional[int] = None,
+        **connection_kwargs,
+    ):
+        max_connections = max_connections or 2 ** 31
+        if not isinstance(max_connections, int) or max_connections < 0:
+            raise ValueError('"max_connections" must be a positive integer')
+
+        self.connection_class = connection_class
+        self.connection_kwargs = connection_kwargs
+        self.max_connections = max_connections
+
+        # a lock to protect the critical section in _checkpid().
+        # this lock is acquired when the process id changes, such as
+        # after a fork. during this time, multiple threads in the child
+        # process could attempt to acquire this lock. the first thread
+        # to acquire the lock will reset the data structures and lock
+        # object of this pool. subsequent threads acquiring this lock
+        # will notice the first thread already did the work and simply
+        # release the lock.
+        self._fork_lock = threading.Lock()
+        self._lock = asyncio.Lock()
+        self._created_connections: int
+        self._available_connections: List[Connection]
+        self._in_use_connections: Set[Connection]
+        self.reset()  # lgtm [py/init-calls-subclass]
+        self.encoder_class = self.connection_kwargs.get("encoder_class", Encoder)
+
+    def __repr__(self):
+        return (
+            f"{self.__class__.__name__}"
+            f"<{self.connection_class(**self.connection_kwargs)!r}>"
+        )
+
+    def reset(self):
+        self._lock = asyncio.Lock()
+        self._created_connections = 0
+        self._available_connections = []
+        self._in_use_connections = set()
+
+        # this must be the last operation in this method. while reset() is
+        # called when holding _fork_lock, other threads in this process
+        # can call _checkpid() which compares self.pid and os.getpid() without
+        # holding any lock (for performance reasons). keeping this assignment
+        # as the last operation ensures that those other threads will also
+        # notice a pid difference and block waiting for the first thread to
+        # release _fork_lock. when each of these threads eventually acquire
+        # _fork_lock, they will notice that another thread already called
+        # reset() and they will immediately release _fork_lock and continue on.
+        self.pid = os.getpid()
+
+    def _checkpid(self):
+        # _checkpid() attempts to keep ConnectionPool fork-safe on modern
+        # systems. this is called by all ConnectionPool methods that
+        # manipulate the pool's state such as get_connection() and release().
+        #
+        # _checkpid() determines whether the process has forked by comparing
+        # the current process id to the process id saved on the ConnectionPool
+        # instance. if these values are the same, _checkpid() simply returns.
+        #
+        # when the process ids differ, _checkpid() assumes that the process
+        # has forked and that we're now running in the child process. the child
+        # process cannot use the parent's file descriptors (e.g., sockets).
+        # therefore, when _checkpid() sees the process id change, it calls
+        # reset() in order to reinitialize the child's ConnectionPool. this
+        # will cause the child to make all new connection objects.
+        #
+        # _checkpid() is protected by self._fork_lock to ensure that multiple
+        # threads in the child process do not call reset() multiple times.
+        #
+        # there is an extremely small chance this could fail in the following
+        # scenario:
+        #   1. process A calls _checkpid() for the first time and acquires
+        #      self._fork_lock.
+        #   2. while holding self._fork_lock, process A forks (the fork()
+        #      could happen in a different thread owned by process A)
+        #   3. process B (the forked child process) inherits the
+        #      ConnectionPool's state from the parent. that state includes
+        #      a locked _fork_lock. process B will not be notified when
+        #      process A releases the _fork_lock and will thus never be
+        #      able to acquire the _fork_lock.
+        #
+        # to mitigate this possible deadlock, _checkpid() will only wait 5
+        # seconds to acquire _fork_lock. if _fork_lock cannot be acquired in
+        # that time it is assumed that the child is deadlocked and a
+        # redis.ChildDeadlockedError error is raised.
+        if self.pid != os.getpid():
+            acquired = self._fork_lock.acquire(timeout=5)
+            if not acquired:
+                raise ChildDeadlockedError
+            # reset() the instance for the new process if another thread
+            # hasn't already done so
+            try:
+                if self.pid != os.getpid():
+                    self.reset()
+            finally:
+                self._fork_lock.release()
+
+    async def get_connection(self, command_name, *keys, **options):
+        """Get a connection from the pool"""
+        self._checkpid()
+        async with self._lock:
+            try:
+                connection = self._available_connections.pop()
+            except IndexError:
+                connection = self.make_connection()
+            self._in_use_connections.add(connection)
+
+        try:
+            # ensure this connection is connected to Redis
+            await connection.connect()
+            # connections that the pool provides should be ready to send
+            # a command. if not, the connection was either returned to the
+            # pool before all data has been read or the socket has been
+            # closed. either way, reconnect and verify everything is good.
+            try:
+                if await connection.can_read():
+                    raise ConnectionError("Connection has data") from None
+            except ConnectionError:
+                await connection.disconnect()
+                await connection.connect()
+                if await connection.can_read():
+                    raise ConnectionError("Connection not ready") from None
+        except BaseException:
+            # release the connection back to the pool so that we don't
+            # leak it
+            await self.release(connection)
+            raise
+
+        return connection
+
+    def get_encoder(self):
+        """Return an encoder based on encoding settings"""
+        kwargs = self.connection_kwargs
+        return self.encoder_class(
+            encoding=kwargs.get("encoding", "utf-8"),
+            encoding_errors=kwargs.get("encoding_errors", "strict"),
+            decode_responses=kwargs.get("decode_responses", False),
+        )
+
+    def make_connection(self):
+        """Create a new connection"""
+        if self._created_connections >= self.max_connections:
+            raise ConnectionError("Too many connections")
+        self._created_connections += 1
+        return self.connection_class(**self.connection_kwargs)
+
+    async def release(self, connection: Connection):
+        """Releases the connection back to the pool"""
+        self._checkpid()
+        async with self._lock:
+            try:
+                self._in_use_connections.remove(connection)
+            except KeyError:
+                # Gracefully fail when a connection is returned to this pool
+                # that the pool doesn't actually own
+                pass
+
+            if self.owns_connection(connection):
+                self._available_connections.append(connection)
+            else:
+                # pool doesn't own this connection. do not add it back
+                # to the pool and decrement the count so that another
+                # connection can take its place if needed
+                self._created_connections -= 1
+                await connection.disconnect()
+                return
+
+    def owns_connection(self, connection: Connection):
+        return connection.pid == self.pid
+
+    async def disconnect(self, inuse_connections: bool = True):
+        """
+        Disconnects connections in the pool
+
+        If ``inuse_connections`` is True, disconnect connections that are
+        current in use, potentially by other tasks. Otherwise only disconnect
+        connections that are idle in the pool.
+        """
+        self._checkpid()
+        async with self._lock:
+            if inuse_connections:
+                connections: Iterable[Connection] = chain(
+                    self._available_connections, self._in_use_connections
+                )
+            else:
+                connections = self._available_connections
+            resp = await asyncio.gather(
+                *(connection.disconnect() for connection in connections),
+                return_exceptions=True,
+            )
+            exc = next((r for r in resp if isinstance(r, BaseException)), None)
+            if exc:
+                raise exc
+
+
+class BlockingConnectionPool(ConnectionPool):
+    """
+    Thread-safe blocking connection pool::
+
+        >>> from aioredis.client import Redis
+        >>> client = Redis(connection_pool=BlockingConnectionPool())
+
+    It performs the same function as the default
+    :py:class:`~redis.ConnectionPool` implementation, in that,
+    it maintains a pool of reusable connections that can be shared by
+    multiple redis clients (safely across threads if required).
+
+    The difference is that, in the event that a client tries to get a
+    connection from the pool when all of connections are in use, rather than
+    raising a :py:class:`~redis.ConnectionError` (as the default
+    :py:class:`~redis.ConnectionPool` implementation does), it
+    makes the client wait ("blocks") for a specified number of seconds until
+    a connection becomes available.
+
+    Use ``max_connections`` to increase / decrease the pool size::
+
+        >>> pool = BlockingConnectionPool(max_connections=10)
+
+    Use ``timeout`` to tell it either how many seconds to wait for a connection
+    to become available, or to block forever:
+
+        >>> # Block forever.
+        >>> pool = BlockingConnectionPool(timeout=None)
+
+        >>> # Raise a ``ConnectionError`` after five seconds if a connection is
+        >>> # not available.
+        >>> pool = BlockingConnectionPool(timeout=5)
+    """
+
+    def __init__(
+        self,
+        max_connections: int = 50,
+        timeout: Optional[int] = 20,
+        connection_class: Type[Connection] = Connection,
+        queue_class: Type[asyncio.Queue] = asyncio.LifoQueue,
+        **connection_kwargs,
+    ):
+
+        self.queue_class = queue_class
+        self.timeout = timeout
+        self._connections: List[Connection]
+        super().__init__(
+            connection_class=connection_class,
+            max_connections=max_connections,
+            **connection_kwargs,
+        )
+
+    def reset(self):
+        # Create and fill up a thread safe queue with ``None`` values.
+        self.pool = self.queue_class(self.max_connections)
+        while True:
+            try:
+                self.pool.put_nowait(None)
+            except asyncio.QueueFull:
+                break
+
+        # Keep a list of actual connection instances so that we can
+        # disconnect them later.
+        self._connections = []
+
+        # this must be the last operation in this method. while reset() is
+        # called when holding _fork_lock, other threads in this process
+        # can call _checkpid() which compares self.pid and os.getpid() without
+        # holding any lock (for performance reasons). keeping this assignment
+        # as the last operation ensures that those other threads will also
+        # notice a pid difference and block waiting for the first thread to
+        # release _fork_lock. when each of these threads eventually acquire
+        # _fork_lock, they will notice that another thread already called
+        # reset() and they will immediately release _fork_lock and continue on.
+        self.pid = os.getpid()
+
+    def make_connection(self):
+        """Make a fresh connection."""
+        connection = self.connection_class(**self.connection_kwargs)
+        self._connections.append(connection)
+        return connection
+
+    async def get_connection(self, command_name, *keys, **options):
+        """
+        Get a connection, blocking for ``self.timeout`` until a connection
+        is available from the pool.
+
+        If the connection returned is ``None`` then creates a new connection.
+        Because we use a last-in first-out queue, the existing connections
+        (having been returned to the pool after the initial ``None`` values
+        were added) will be returned before ``None`` values. This means we only
+        create new connections when we need to, i.e.: the actual number of
+        connections will only increase in response to demand.
+        """
+        # Make sure we haven't changed process.
+        self._checkpid()
+
+        # Try and get a connection from the pool. If one isn't available within
+        # self.timeout then raise a ``ConnectionError``.
+        connection = None
+        try:
+            async with async_timeout.timeout(self.timeout):
+                connection = await self.pool.get()
+        except (asyncio.QueueEmpty, asyncio.TimeoutError):
+            # Note that this is not caught by the redis client and will be
+            # raised unless handled by application code. If you want never to
+            raise ConnectionError("No connection available.")
+
+        # If the ``connection`` is actually ``None`` then that's a cue to make
+        # a new connection to add to the pool.
+        if connection is None:
+            connection = self.make_connection()
+
+        try:
+            # ensure this connection is connected to Redis
+            await connection.connect()
+            # connections that the pool provides should be ready to send
+            # a command. if not, the connection was either returned to the
+            # pool before all data has been read or the socket has been
+            # closed. either way, reconnect and verify everything is good.
+            try:
+                if await connection.can_read():
+                    raise ConnectionError("Connection has data") from None
+            except ConnectionError:
+                await connection.disconnect()
+                await connection.connect()
+                if await connection.can_read():
+                    raise ConnectionError("Connection not ready") from None
+        except BaseException:
+            # release the connection back to the pool so that we don't leak it
+            await self.release(connection)
+            raise
+
+        return connection
+
+    async def release(self, connection: Connection):
+        """Releases the connection back to the pool."""
+        # Make sure we haven't changed process.
+        self._checkpid()
+        if not self.owns_connection(connection):
+            # pool doesn't own this connection. do not add it back
+            # to the pool. instead add a None value which is a placeholder
+            # that will cause the pool to recreate the connection if
+            # its needed.
+            await connection.disconnect()
+            self.pool.put_nowait(None)
+            return
+
+        # Put the connection back into the pool.
+        try:
+            self.pool.put_nowait(connection)
+        except asyncio.QueueFull:
+            # perhaps the pool has been reset() after a fork? regardless,
+            # we don't want this connection
+            pass
+
+    async def disconnect(self, inuse_connections: bool = True):
+        """Disconnects all connections in the pool."""
+        self._checkpid()
+        async with self._lock:
+            resp = await asyncio.gather(
+                *(connection.disconnect() for connection in self._connections),
+                return_exceptions=True,
+            )
+            exc = next((r for r in resp if isinstance(r, BaseException)), None)
+            if exc:
+                raise exc
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py

 * *Ordering differences only*

```diff
@@ -1,96 +1,96 @@
-"""Core exceptions raised by the Redis client"""
-import asyncio
-import builtins
-
-
-class RedisError(Exception):
-    pass
-
-
-class ConnectionError(RedisError):
-    pass
-
-
-''' 这个在python3.11有问题'''
-# class TimeoutError(asyncio.TimeoutError, builtins.TimeoutError, RedisError):
-#     pass
-
-class TimeoutError(asyncio.TimeoutError, RedisError):
-    pass
-
-
-class AuthenticationError(ConnectionError):
-    pass
-
-
-class BusyLoadingError(ConnectionError):
-    pass
-
-
-class InvalidResponse(RedisError):
-    pass
-
-
-class ResponseError(RedisError):
-    pass
-
-
-class DataError(RedisError):
-    pass
-
-
-class PubSubError(RedisError):
-    pass
-
-
-class WatchError(RedisError):
-    pass
-
-
-class NoScriptError(ResponseError):
-    pass
-
-
-class ExecAbortError(ResponseError):
-    pass
-
-
-class ReadOnlyError(ResponseError):
-    pass
-
-
-class NoPermissionError(ResponseError):
-    pass
-
-
-class ModuleError(ResponseError):
-    pass
-
-
-class LockError(RedisError, ValueError):
-    """Errors acquiring or releasing a lock"""
-
-    # NOTE: For backwards compatibility, this class derives from ValueError.
-    # This was originally chosen to behave like threading.Lock.
-    pass
-
-
-class LockNotOwnedError(LockError):
-    """Error trying to extend or release a lock that is (no longer) owned"""
-
-    pass
-
-
-class ChildDeadlockedError(Exception):
-    """Error indicating that a child process is deadlocked after a fork()"""
-
-    pass
-
-
-class AuthenticationWrongNumberOfArgsError(ResponseError):
-    """
-    An error to indicate that the wrong number of args
-    were sent to the AUTH command
-    """
-
-    pass
+"""Core exceptions raised by the Redis client"""
+import asyncio
+import builtins
+
+
+class RedisError(Exception):
+    pass
+
+
+class ConnectionError(RedisError):
+    pass
+
+
+''' 这个在python3.11有问题'''
+# class TimeoutError(asyncio.TimeoutError, builtins.TimeoutError, RedisError):
+#     pass
+
+class TimeoutError(asyncio.TimeoutError, RedisError):
+    pass
+
+
+class AuthenticationError(ConnectionError):
+    pass
+
+
+class BusyLoadingError(ConnectionError):
+    pass
+
+
+class InvalidResponse(RedisError):
+    pass
+
+
+class ResponseError(RedisError):
+    pass
+
+
+class DataError(RedisError):
+    pass
+
+
+class PubSubError(RedisError):
+    pass
+
+
+class WatchError(RedisError):
+    pass
+
+
+class NoScriptError(ResponseError):
+    pass
+
+
+class ExecAbortError(ResponseError):
+    pass
+
+
+class ReadOnlyError(ResponseError):
+    pass
+
+
+class NoPermissionError(ResponseError):
+    pass
+
+
+class ModuleError(ResponseError):
+    pass
+
+
+class LockError(RedisError, ValueError):
+    """Errors acquiring or releasing a lock"""
+
+    # NOTE: For backwards compatibility, this class derives from ValueError.
+    # This was originally chosen to behave like threading.Lock.
+    pass
+
+
+class LockNotOwnedError(LockError):
+    """Error trying to extend or release a lock that is (no longer) owned"""
+
+    pass
+
+
+class ChildDeadlockedError(Exception):
+    """Error indicating that a child process is deadlocked after a fork()"""
+
+    pass
+
+
+class AuthenticationWrongNumberOfArgsError(ResponseError):
+    """
+    An error to indicate that the wrong number of args
+    were sent to the AUTH command
+    """
+
+    pass
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py

 * *Ordering differences only*

```diff
@@ -1,306 +1,306 @@
-import asyncio
-import threading
-import uuid
-from types import SimpleNamespace
-from typing import TYPE_CHECKING, Awaitable, NoReturn, Optional, Union
-
-from aioredis.exceptions import LockError, LockNotOwnedError
-
-if TYPE_CHECKING:
-    from aioredis import Redis
-
-
-class Lock:
-    """
-    A shared, distributed Lock. Using Redis for locking allows the Lock
-    to be shared across processes and/or machines.
-
-    It's left to the user to resolve deadlock issues and make sure
-    multiple clients play nicely together.
-    """
-
-    lua_release = None
-    lua_extend = None
-    lua_reacquire = None
-
-    # KEYS[1] - lock name
-    # ARGV[1] - token
-    # return 1 if the lock was released, otherwise 0
-    LUA_RELEASE_SCRIPT = """
-        local token = redis.call('get', KEYS[1])
-        if not token or token ~= ARGV[1] then
-            return 0
-        end
-        redis.call('del', KEYS[1])
-        return 1
-    """
-
-    # KEYS[1] - lock name
-    # ARGV[1] - token
-    # ARGV[2] - additional milliseconds
-    # ARGV[3] - "0" if the additional time should be added to the lock's
-    #           existing ttl or "1" if the existing ttl should be replaced
-    # return 1 if the locks time was extended, otherwise 0
-    LUA_EXTEND_SCRIPT = """
-        local token = redis.call('get', KEYS[1])
-        if not token or token ~= ARGV[1] then
-            return 0
-        end
-        local expiration = redis.call('pttl', KEYS[1])
-        if not expiration then
-            expiration = 0
-        end
-        if expiration < 0 then
-            return 0
-        end
-
-        local newttl = ARGV[2]
-        if ARGV[3] == "0" then
-            newttl = ARGV[2] + expiration
-        end
-        redis.call('pexpire', KEYS[1], newttl)
-        return 1
-    """
-
-    # KEYS[1] - lock name
-    # ARGV[1] - token
-    # ARGV[2] - milliseconds
-    # return 1 if the locks time was reacquired, otherwise 0
-    LUA_REACQUIRE_SCRIPT = """
-        local token = redis.call('get', KEYS[1])
-        if not token or token ~= ARGV[1] then
-            return 0
-        end
-        redis.call('pexpire', KEYS[1], ARGV[2])
-        return 1
-    """
-
-    def __init__(
-        self,
-        redis: "Redis",
-        name: Union[str, bytes, memoryview],
-        timeout: Optional[float] = None,
-        sleep: float = 0.1,
-        blocking: bool = True,
-        blocking_timeout: Optional[float] = None,
-        thread_local: bool = True,
-    ):
-        """
-        Create a new Lock instance named ``name`` using the Redis client
-        supplied by ``redis``.
-
-        ``timeout`` indicates a maximum life for the lock.
-        By default, it will remain locked until release() is called.
-        ``timeout`` can be specified as a float or integer, both representing
-        the number of seconds to wait.
-
-        ``sleep`` indicates the amount of time to sleep per loop iteration
-        when the lock is in blocking mode and another client is currently
-        holding the lock.
-
-        ``blocking`` indicates whether calling ``acquire`` should block until
-        the lock has been acquired or to fail immediately, causing ``acquire``
-        to return False and the lock not being acquired. Defaults to True.
-        Note this value can be overridden by passing a ``blocking``
-        argument to ``acquire``.
-
-        ``blocking_timeout`` indicates the maximum amount of time in seconds to
-        spend trying to acquire the lock. A value of ``None`` indicates
-        continue trying forever. ``blocking_timeout`` can be specified as a
-        float or integer, both representing the number of seconds to wait.
-
-        ``thread_local`` indicates whether the lock token is placed in
-        thread-local storage. By default, the token is placed in thread local
-        storage so that a thread only sees its token, not a token set by
-        another thread. Consider the following timeline:
-
-            time: 0, thread-1 acquires `my-lock`, with a timeout of 5 seconds.
-                     thread-1 sets the token to "abc"
-            time: 1, thread-2 blocks trying to acquire `my-lock` using the
-                     Lock instance.
-            time: 5, thread-1 has not yet completed. redis expires the lock
-                     key.
-            time: 5, thread-2 acquired `my-lock` now that it's available.
-                     thread-2 sets the token to "xyz"
-            time: 6, thread-1 finishes its work and calls release(). if the
-                     token is *not* stored in thread local storage, then
-                     thread-1 would see the token value as "xyz" and would be
-                     able to successfully release the thread-2's lock.
-
-        In some use cases it's necessary to disable thread local storage. For
-        example, if you have code where one thread acquires a lock and passes
-        that lock instance to a worker thread to release later. If thread
-        local storage isn't disabled in this case, the worker thread won't see
-        the token set by the thread that acquired the lock. Our assumption
-        is that these cases aren't common and as such default to using
-        thread local storage.
-        """
-        self.redis = redis
-        self.name = name
-        self.timeout = timeout
-        self.sleep = sleep
-        self.blocking = blocking
-        self.blocking_timeout = blocking_timeout
-        self.thread_local = bool(thread_local)
-        self.local = threading.local() if self.thread_local else SimpleNamespace()
-        self.local.token = None
-        self.register_scripts()
-
-    def register_scripts(self):
-        cls = self.__class__
-        client = self.redis
-        if cls.lua_release is None:
-            cls.lua_release = client.register_script(cls.LUA_RELEASE_SCRIPT)
-        if cls.lua_extend is None:
-            cls.lua_extend = client.register_script(cls.LUA_EXTEND_SCRIPT)
-        if cls.lua_reacquire is None:
-            cls.lua_reacquire = client.register_script(cls.LUA_REACQUIRE_SCRIPT)
-
-    async def __aenter__(self):
-        if await self.acquire():
-            return self
-        raise LockError("Unable to acquire lock within the time specified")
-
-    async def __aexit__(self, exc_type, exc_value, traceback):
-        await self.release()
-
-    async def acquire(
-        self,
-        blocking: Optional[bool] = None,
-        blocking_timeout: Optional[float] = None,
-        token: Optional[Union[str, bytes]] = None,
-    ):
-        """
-        Use Redis to hold a shared, distributed lock named ``name``.
-        Returns True once the lock is acquired.
-
-        If ``blocking`` is False, always return immediately. If the lock
-        was acquired, return True, otherwise return False.
-
-        ``blocking_timeout`` specifies the maximum number of seconds to
-        wait trying to acquire the lock.
-
-        ``token`` specifies the token value to be used. If provided, token
-        must be a bytes object or a string that can be encoded to a bytes
-        object with the default encoding. If a token isn't specified, a UUID
-        will be generated.
-        """
-        loop = asyncio.get_event_loop()
-        sleep = self.sleep
-        if token is None:
-            token = uuid.uuid1().hex.encode()
-        else:
-            encoder = self.redis.connection_pool.get_encoder()
-            token = encoder.encode(token)
-        if blocking is None:
-            blocking = self.blocking
-        if blocking_timeout is None:
-            blocking_timeout = self.blocking_timeout
-        stop_trying_at = None
-        if blocking_timeout is not None:
-            stop_trying_at = loop.time() + blocking_timeout
-        while True:
-            if await self.do_acquire(token):
-                self.local.token = token
-                return True
-            if not blocking:
-                return False
-            next_try_at = loop.time() + sleep
-            if stop_trying_at is not None and next_try_at > stop_trying_at:
-                return False
-            await asyncio.sleep(sleep)
-
-    async def do_acquire(self, token: Union[str, bytes]) -> bool:
-        if self.timeout:
-            # convert to milliseconds
-            timeout = int(self.timeout * 1000)
-        else:
-            timeout = None
-        if await self.redis.set(self.name, token, nx=True, px=timeout):
-            return True
-        return False
-
-    async def locked(self) -> bool:
-        """
-        Returns True if this key is locked by any process, otherwise False.
-        """
-        return await self.redis.get(self.name) is not None
-
-    async def owned(self) -> bool:
-        """
-        Returns True if this key is locked by this lock, otherwise False.
-        """
-        stored_token = await self.redis.get(self.name)
-        # need to always compare bytes to bytes
-        # TODO: this can be simplified when the context manager is finished
-        if stored_token and not isinstance(stored_token, bytes):
-            encoder = self.redis.connection_pool.get_encoder()
-            stored_token = encoder.encode(stored_token)
-        return self.local.token is not None and stored_token == self.local.token
-
-    def release(self) -> Awaitable[NoReturn]:
-        """Releases the already acquired lock"""
-        expected_token = self.local.token
-        if expected_token is None:
-            raise LockError("Cannot release an unlocked lock")
-        self.local.token = None
-        return self.do_release(expected_token)
-
-    async def do_release(self, expected_token: bytes):
-        if not bool(
-            await self.lua_release(
-                keys=[self.name], args=[expected_token], client=self.redis
-            )
-        ):
-            raise LockNotOwnedError("Cannot release a lock" " that's no longer owned")
-
-    def extend(
-        self, additional_time: float, replace_ttl: bool = False
-    ) -> Awaitable[bool]:
-        """
-        Adds more time to an already acquired lock.
-
-        ``additional_time`` can be specified as an integer or a float, both
-        representing the number of seconds to add.
-
-        ``replace_ttl`` if False (the default), add `additional_time` to
-        the lock's existing ttl. If True, replace the lock's ttl with
-        `additional_time`.
-        """
-        if self.local.token is None:
-            raise LockError("Cannot extend an unlocked lock")
-        if self.timeout is None:
-            raise LockError("Cannot extend a lock with no timeout")
-        return self.do_extend(additional_time, replace_ttl)
-
-    async def do_extend(self, additional_time, replace_ttl) -> bool:
-        additional_time = int(additional_time * 1000)
-        if not bool(
-            await self.lua_extend(
-                keys=[self.name],
-                args=[self.local.token, additional_time, replace_ttl and "1" or "0"],
-                client=self.redis,
-            )
-        ):
-            raise LockNotOwnedError("Cannot extend a lock that's" " no longer owned")
-        return True
-
-    def reacquire(self) -> Awaitable[bool]:
-        """
-        Resets a TTL of an already acquired lock back to a timeout value.
-        """
-        if self.local.token is None:
-            raise LockError("Cannot reacquire an unlocked lock")
-        if self.timeout is None:
-            raise LockError("Cannot reacquire a lock with no timeout")
-        return self.do_reacquire()
-
-    async def do_reacquire(self) -> bool:
-        timeout = int(self.timeout * 1000)
-        if not bool(
-            await self.lua_reacquire(
-                keys=[self.name], args=[self.local.token, timeout], client=self.redis
-            )
-        ):
-            raise LockNotOwnedError("Cannot reacquire a lock that's" " no longer owned")
-        return True
+import asyncio
+import threading
+import uuid
+from types import SimpleNamespace
+from typing import TYPE_CHECKING, Awaitable, NoReturn, Optional, Union
+
+from aioredis.exceptions import LockError, LockNotOwnedError
+
+if TYPE_CHECKING:
+    from aioredis import Redis
+
+
+class Lock:
+    """
+    A shared, distributed Lock. Using Redis for locking allows the Lock
+    to be shared across processes and/or machines.
+
+    It's left to the user to resolve deadlock issues and make sure
+    multiple clients play nicely together.
+    """
+
+    lua_release = None
+    lua_extend = None
+    lua_reacquire = None
+
+    # KEYS[1] - lock name
+    # ARGV[1] - token
+    # return 1 if the lock was released, otherwise 0
+    LUA_RELEASE_SCRIPT = """
+        local token = redis.call('get', KEYS[1])
+        if not token or token ~= ARGV[1] then
+            return 0
+        end
+        redis.call('del', KEYS[1])
+        return 1
+    """
+
+    # KEYS[1] - lock name
+    # ARGV[1] - token
+    # ARGV[2] - additional milliseconds
+    # ARGV[3] - "0" if the additional time should be added to the lock's
+    #           existing ttl or "1" if the existing ttl should be replaced
+    # return 1 if the locks time was extended, otherwise 0
+    LUA_EXTEND_SCRIPT = """
+        local token = redis.call('get', KEYS[1])
+        if not token or token ~= ARGV[1] then
+            return 0
+        end
+        local expiration = redis.call('pttl', KEYS[1])
+        if not expiration then
+            expiration = 0
+        end
+        if expiration < 0 then
+            return 0
+        end
+
+        local newttl = ARGV[2]
+        if ARGV[3] == "0" then
+            newttl = ARGV[2] + expiration
+        end
+        redis.call('pexpire', KEYS[1], newttl)
+        return 1
+    """
+
+    # KEYS[1] - lock name
+    # ARGV[1] - token
+    # ARGV[2] - milliseconds
+    # return 1 if the locks time was reacquired, otherwise 0
+    LUA_REACQUIRE_SCRIPT = """
+        local token = redis.call('get', KEYS[1])
+        if not token or token ~= ARGV[1] then
+            return 0
+        end
+        redis.call('pexpire', KEYS[1], ARGV[2])
+        return 1
+    """
+
+    def __init__(
+        self,
+        redis: "Redis",
+        name: Union[str, bytes, memoryview],
+        timeout: Optional[float] = None,
+        sleep: float = 0.1,
+        blocking: bool = True,
+        blocking_timeout: Optional[float] = None,
+        thread_local: bool = True,
+    ):
+        """
+        Create a new Lock instance named ``name`` using the Redis client
+        supplied by ``redis``.
+
+        ``timeout`` indicates a maximum life for the lock.
+        By default, it will remain locked until release() is called.
+        ``timeout`` can be specified as a float or integer, both representing
+        the number of seconds to wait.
+
+        ``sleep`` indicates the amount of time to sleep per loop iteration
+        when the lock is in blocking mode and another client is currently
+        holding the lock.
+
+        ``blocking`` indicates whether calling ``acquire`` should block until
+        the lock has been acquired or to fail immediately, causing ``acquire``
+        to return False and the lock not being acquired. Defaults to True.
+        Note this value can be overridden by passing a ``blocking``
+        argument to ``acquire``.
+
+        ``blocking_timeout`` indicates the maximum amount of time in seconds to
+        spend trying to acquire the lock. A value of ``None`` indicates
+        continue trying forever. ``blocking_timeout`` can be specified as a
+        float or integer, both representing the number of seconds to wait.
+
+        ``thread_local`` indicates whether the lock token is placed in
+        thread-local storage. By default, the token is placed in thread local
+        storage so that a thread only sees its token, not a token set by
+        another thread. Consider the following timeline:
+
+            time: 0, thread-1 acquires `my-lock`, with a timeout of 5 seconds.
+                     thread-1 sets the token to "abc"
+            time: 1, thread-2 blocks trying to acquire `my-lock` using the
+                     Lock instance.
+            time: 5, thread-1 has not yet completed. redis expires the lock
+                     key.
+            time: 5, thread-2 acquired `my-lock` now that it's available.
+                     thread-2 sets the token to "xyz"
+            time: 6, thread-1 finishes its work and calls release(). if the
+                     token is *not* stored in thread local storage, then
+                     thread-1 would see the token value as "xyz" and would be
+                     able to successfully release the thread-2's lock.
+
+        In some use cases it's necessary to disable thread local storage. For
+        example, if you have code where one thread acquires a lock and passes
+        that lock instance to a worker thread to release later. If thread
+        local storage isn't disabled in this case, the worker thread won't see
+        the token set by the thread that acquired the lock. Our assumption
+        is that these cases aren't common and as such default to using
+        thread local storage.
+        """
+        self.redis = redis
+        self.name = name
+        self.timeout = timeout
+        self.sleep = sleep
+        self.blocking = blocking
+        self.blocking_timeout = blocking_timeout
+        self.thread_local = bool(thread_local)
+        self.local = threading.local() if self.thread_local else SimpleNamespace()
+        self.local.token = None
+        self.register_scripts()
+
+    def register_scripts(self):
+        cls = self.__class__
+        client = self.redis
+        if cls.lua_release is None:
+            cls.lua_release = client.register_script(cls.LUA_RELEASE_SCRIPT)
+        if cls.lua_extend is None:
+            cls.lua_extend = client.register_script(cls.LUA_EXTEND_SCRIPT)
+        if cls.lua_reacquire is None:
+            cls.lua_reacquire = client.register_script(cls.LUA_REACQUIRE_SCRIPT)
+
+    async def __aenter__(self):
+        if await self.acquire():
+            return self
+        raise LockError("Unable to acquire lock within the time specified")
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.release()
+
+    async def acquire(
+        self,
+        blocking: Optional[bool] = None,
+        blocking_timeout: Optional[float] = None,
+        token: Optional[Union[str, bytes]] = None,
+    ):
+        """
+        Use Redis to hold a shared, distributed lock named ``name``.
+        Returns True once the lock is acquired.
+
+        If ``blocking`` is False, always return immediately. If the lock
+        was acquired, return True, otherwise return False.
+
+        ``blocking_timeout`` specifies the maximum number of seconds to
+        wait trying to acquire the lock.
+
+        ``token`` specifies the token value to be used. If provided, token
+        must be a bytes object or a string that can be encoded to a bytes
+        object with the default encoding. If a token isn't specified, a UUID
+        will be generated.
+        """
+        loop = asyncio.get_event_loop()
+        sleep = self.sleep
+        if token is None:
+            token = uuid.uuid1().hex.encode()
+        else:
+            encoder = self.redis.connection_pool.get_encoder()
+            token = encoder.encode(token)
+        if blocking is None:
+            blocking = self.blocking
+        if blocking_timeout is None:
+            blocking_timeout = self.blocking_timeout
+        stop_trying_at = None
+        if blocking_timeout is not None:
+            stop_trying_at = loop.time() + blocking_timeout
+        while True:
+            if await self.do_acquire(token):
+                self.local.token = token
+                return True
+            if not blocking:
+                return False
+            next_try_at = loop.time() + sleep
+            if stop_trying_at is not None and next_try_at > stop_trying_at:
+                return False
+            await asyncio.sleep(sleep)
+
+    async def do_acquire(self, token: Union[str, bytes]) -> bool:
+        if self.timeout:
+            # convert to milliseconds
+            timeout = int(self.timeout * 1000)
+        else:
+            timeout = None
+        if await self.redis.set(self.name, token, nx=True, px=timeout):
+            return True
+        return False
+
+    async def locked(self) -> bool:
+        """
+        Returns True if this key is locked by any process, otherwise False.
+        """
+        return await self.redis.get(self.name) is not None
+
+    async def owned(self) -> bool:
+        """
+        Returns True if this key is locked by this lock, otherwise False.
+        """
+        stored_token = await self.redis.get(self.name)
+        # need to always compare bytes to bytes
+        # TODO: this can be simplified when the context manager is finished
+        if stored_token and not isinstance(stored_token, bytes):
+            encoder = self.redis.connection_pool.get_encoder()
+            stored_token = encoder.encode(stored_token)
+        return self.local.token is not None and stored_token == self.local.token
+
+    def release(self) -> Awaitable[NoReturn]:
+        """Releases the already acquired lock"""
+        expected_token = self.local.token
+        if expected_token is None:
+            raise LockError("Cannot release an unlocked lock")
+        self.local.token = None
+        return self.do_release(expected_token)
+
+    async def do_release(self, expected_token: bytes):
+        if not bool(
+            await self.lua_release(
+                keys=[self.name], args=[expected_token], client=self.redis
+            )
+        ):
+            raise LockNotOwnedError("Cannot release a lock" " that's no longer owned")
+
+    def extend(
+        self, additional_time: float, replace_ttl: bool = False
+    ) -> Awaitable[bool]:
+        """
+        Adds more time to an already acquired lock.
+
+        ``additional_time`` can be specified as an integer or a float, both
+        representing the number of seconds to add.
+
+        ``replace_ttl`` if False (the default), add `additional_time` to
+        the lock's existing ttl. If True, replace the lock's ttl with
+        `additional_time`.
+        """
+        if self.local.token is None:
+            raise LockError("Cannot extend an unlocked lock")
+        if self.timeout is None:
+            raise LockError("Cannot extend a lock with no timeout")
+        return self.do_extend(additional_time, replace_ttl)
+
+    async def do_extend(self, additional_time, replace_ttl) -> bool:
+        additional_time = int(additional_time * 1000)
+        if not bool(
+            await self.lua_extend(
+                keys=[self.name],
+                args=[self.local.token, additional_time, replace_ttl and "1" or "0"],
+                client=self.redis,
+            )
+        ):
+            raise LockNotOwnedError("Cannot extend a lock that's" " no longer owned")
+        return True
+
+    def reacquire(self) -> Awaitable[bool]:
+        """
+        Resets a TTL of an already acquired lock back to a timeout value.
+        """
+        if self.local.token is None:
+            raise LockError("Cannot reacquire an unlocked lock")
+        if self.timeout is None:
+            raise LockError("Cannot reacquire a lock with no timeout")
+        return self.do_reacquire()
+
+    async def do_reacquire(self) -> bool:
+        timeout = int(self.timeout * 1000)
+        if not bool(
+            await self.lua_reacquire(
+                keys=[self.name], args=[self.local.token, timeout], client=self.redis
+            )
+        ):
+            raise LockNotOwnedError("Cannot reacquire a lock that's" " no longer owned")
+        return True
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py

 * *Ordering differences only*

```diff
@@ -1,15 +1,15 @@
-import logging
-import os
-import sys
-
-logger = logging.getLogger("aioredis")
-sentinel_logger = logger.getChild("sentinel")
-
-if os.environ.get("AIOREDIS_DEBUG"):
-    logger.setLevel(logging.DEBUG)
-    handler = logging.StreamHandler(stream=sys.stderr)
-    handler.setFormatter(
-        logging.Formatter("%(asctime)s %(name)s %(levelname)s %(message)s")
-    )
-    logger.addHandler(handler)
-    os.environ["AIOREDIS_DEBUG"] = ""
+import logging
+import os
+import sys
+
+logger = logging.getLogger("aioredis")
+sentinel_logger = logger.getChild("sentinel")
+
+if os.environ.get("AIOREDIS_DEBUG"):
+    logger.setLevel(logging.DEBUG)
+    handler = logging.StreamHandler(stream=sys.stderr)
+    handler.setFormatter(
+        logging.Formatter("%(asctime)s %(name)s %(levelname)s %(message)s")
+    )
+    logger.addHandler(handler)
+    os.environ["AIOREDIS_DEBUG"] = ""
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py

 * *Ordering differences only*

```diff
@@ -1,329 +1,329 @@
-import random
-import weakref
-from typing import AsyncIterator, Iterable, Mapping, Sequence, Tuple, Type
-
-from aioredis.client import Redis
-from aioredis.connection import Connection, ConnectionPool, EncodableT, SSLConnection
-from aioredis.exceptions import (
-    ConnectionError,
-    ReadOnlyError,
-    ResponseError,
-    TimeoutError,
-)
-from aioredis.utils import str_if_bytes
-
-
-class MasterNotFoundError(ConnectionError):
-    pass
-
-
-class SlaveNotFoundError(ConnectionError):
-    pass
-
-
-class SentinelManagedConnection(SSLConnection):
-    def __init__(self, **kwargs):
-        self.connection_pool = kwargs.pop("connection_pool")
-        if not kwargs.pop("ssl", False):
-            # use constructor from Connection class
-            super(SSLConnection, self).__init__(**kwargs)
-        else:
-            # use constructor from SSLConnection class
-            super().__init__(**kwargs)
-
-    def __repr__(self):
-        pool = self.connection_pool
-        s = f"{self.__class__.__name__}<service={pool.service_name}"
-        if self.host:
-            host_info = f",host={self.host},port={self.port}"
-            s += host_info
-        return s + ">"
-
-    async def connect_to(self, address):
-        self.host, self.port = address
-        await super().connect()
-        if self.connection_pool.check_connection:
-            await self.send_command("PING")
-            if str_if_bytes(await self.read_response()) != "PONG":
-                raise ConnectionError("PING failed")
-
-    async def connect(self):
-        if self._reader:
-            return  # already connected
-        if self.connection_pool.is_master:
-            await self.connect_to(await self.connection_pool.get_master_address())
-        else:
-            async for slave in self.connection_pool.rotate_slaves():
-                try:
-                    return await self.connect_to(slave)
-                except ConnectionError:
-                    continue
-            raise SlaveNotFoundError  # Never be here
-
-    async def read_response(self):
-        try:
-            return await super().read_response()
-        except ReadOnlyError:
-            if self.connection_pool.is_master:
-                # When talking to a master, a ReadOnlyError when likely
-                # indicates that the previous master that we're still connected
-                # to has been demoted to a slave and there's a new master.
-                # calling disconnect will force the connection to re-query
-                # sentinel during the next connect() attempt.
-                await self.disconnect()
-                raise ConnectionError("The previous master is now a slave")
-            raise
-
-
-class SentinelConnectionPool(ConnectionPool):
-    """
-    Sentinel backed connection pool.
-
-    If ``check_connection`` flag is set to True, SentinelManagedConnection
-    sends a PING command right after establishing the connection.
-    """
-
-    def __init__(self, service_name, sentinel_manager, **kwargs):
-        kwargs["connection_class"] = kwargs.get(
-            "connection_class", SentinelManagedConnection
-        )
-        self.is_master = kwargs.pop("is_master", True)
-        self.check_connection = kwargs.pop("check_connection", False)
-        super().__init__(**kwargs)
-        self.connection_kwargs["connection_pool"] = weakref.proxy(self)
-        self.service_name = service_name
-        self.sentinel_manager = sentinel_manager
-        self.master_address = None
-        self.slave_rr_counter = None
-
-    def __repr__(self):
-        return (
-            f"{self.__class__.__name__}"
-            f"<service={self.service_name}({self.is_master and 'master' or 'slave'})>"
-        )
-
-    def reset(self):
-        super().reset()
-        self.master_address = None
-        self.slave_rr_counter = None
-
-    def owns_connection(self, connection: Connection):
-        check = not self.is_master or (
-            self.is_master and self.master_address == (connection.host, connection.port)
-        )
-        return check and super().owns_connection(connection)
-
-    async def get_master_address(self):
-        master_address = await self.sentinel_manager.discover_master(self.service_name)
-        if self.is_master:
-            if self.master_address != master_address:
-                self.master_address = master_address
-                # disconnect any idle connections so that they reconnect
-                # to the new master the next time that they are used.
-                await self.disconnect(inuse_connections=False)
-        return master_address
-
-    async def rotate_slaves(self) -> AsyncIterator:
-        """Round-robin slave balancer"""
-        slaves = await self.sentinel_manager.discover_slaves(self.service_name)
-        if slaves:
-            if self.slave_rr_counter is None:
-                self.slave_rr_counter = random.randint(0, len(slaves) - 1)
-            for _ in range(len(slaves)):
-                self.slave_rr_counter = (self.slave_rr_counter + 1) % len(slaves)
-                slave = slaves[self.slave_rr_counter]
-                yield slave
-        # Fallback to the master connection
-        try:
-            yield await self.get_master_address()
-        except MasterNotFoundError:
-            pass
-        raise SlaveNotFoundError(f"No slave found for {self.service_name!r}")
-
-
-class Sentinel:
-    """
-    Redis Sentinel cluster client
-
-    >>> from aioredis.sentinel import Sentinel
-    >>> sentinel = Sentinel([('localhost', 26379)], socket_timeout=0.1)
-    >>> master = sentinel.master_for('mymaster', socket_timeout=0.1)
-    >>> await master.set('foo', 'bar')
-    >>> slave = sentinel.slave_for('mymaster', socket_timeout=0.1)
-    >>> await slave.get('foo')
-    b'bar'
-
-    ``sentinels`` is a list of sentinel nodes. Each node is represented by
-    a pair (hostname, port).
-
-    ``min_other_sentinels`` defined a minimum number of peers for a sentinel.
-    When querying a sentinel, if it doesn't meet this threshold, responses
-    from that sentinel won't be considered valid.
-
-    ``sentinel_kwargs`` is a dictionary of connection arguments used when
-    connecting to sentinel instances. Any argument that can be passed to
-    a normal Redis connection can be specified here. If ``sentinel_kwargs`` is
-    not specified, any socket_timeout and socket_keepalive options specified
-    in ``connection_kwargs`` will be used.
-
-    ``connection_kwargs`` are keyword arguments that will be used when
-    establishing a connection to a Redis server.
-    """
-
-    def __init__(
-        self,
-        sentinels,
-        min_other_sentinels=0,
-        sentinel_kwargs=None,
-        **connection_kwargs,
-    ):
-        # if sentinel_kwargs isn't defined, use the socket_* options from
-        # connection_kwargs
-        if sentinel_kwargs is None:
-            sentinel_kwargs = {
-                k: v for k, v in connection_kwargs.items() if k.startswith("socket_")
-            }
-        self.sentinel_kwargs = sentinel_kwargs
-
-        self.sentinels = [
-            Redis(host=hostname, port=port, **self.sentinel_kwargs)
-            for hostname, port in sentinels
-        ]
-        self.min_other_sentinels = min_other_sentinels
-        self.connection_kwargs = connection_kwargs
-
-    def __repr__(self):
-        sentinel_addresses = []
-        for sentinel in self.sentinels:
-            sentinel_addresses.append(
-                f"{sentinel.connection_pool.connection_kwargs['host']}:"
-                f"{sentinel.connection_pool.connection_kwargs['port']}"
-            )
-        return f"{self.__class__.__name__}<sentinels=[{','.join(sentinel_addresses)}]>"
-
-    def check_master_state(self, state: dict, service_name: str) -> bool:
-        if not state["is_master"] or state["is_sdown"] or state["is_odown"]:
-            return False
-        # Check if our sentinel doesn't see other nodes
-        if state["num-other-sentinels"] < self.min_other_sentinels:
-            return False
-        return True
-
-    async def discover_master(self, service_name: str):
-        """
-        Asks sentinel servers for the Redis master's address corresponding
-        to the service labeled ``service_name``.
-
-        Returns a pair (address, port) or raises MasterNotFoundError if no
-        master is found.
-        """
-        for sentinel_no, sentinel in enumerate(self.sentinels):
-            try:
-                masters = await sentinel.sentinel_masters()
-            except (ConnectionError, TimeoutError):
-                continue
-            state = masters.get(service_name)
-            if state and self.check_master_state(state, service_name):
-                # Put this sentinel at the top of the list
-                self.sentinels[0], self.sentinels[sentinel_no] = (
-                    sentinel,
-                    self.sentinels[0],
-                )
-                return state["ip"], state["port"]
-        raise MasterNotFoundError(f"No master found for {service_name!r}")
-
-    def filter_slaves(
-        self, slaves: Iterable[Mapping]
-    ) -> Sequence[Tuple[EncodableT, EncodableT]]:
-        """Remove slaves that are in an ODOWN or SDOWN state"""
-        slaves_alive = []
-        for slave in slaves:
-            if slave["is_odown"] or slave["is_sdown"]:
-                continue
-            slaves_alive.append((slave["ip"], slave["port"]))
-        return slaves_alive
-
-    async def discover_slaves(
-        self, service_name: str
-    ) -> Sequence[Tuple[EncodableT, EncodableT]]:
-        """Returns a list of alive slaves for service ``service_name``"""
-        for sentinel in self.sentinels:
-            try:
-                slaves = await sentinel.sentinel_slaves(service_name)
-            except (ConnectionError, ResponseError, TimeoutError):
-                continue
-            slaves = self.filter_slaves(slaves)
-            if slaves:
-                return slaves
-        return []
-
-    def master_for(
-        self,
-        service_name: str,
-        redis_class: Type[Redis] = Redis,
-        connection_pool_class: Type[SentinelConnectionPool] = SentinelConnectionPool,
-        **kwargs,
-    ):
-        """
-        Returns a redis client instance for the ``service_name`` master.
-
-        A :py:class:`~redis.sentinel.SentinelConnectionPool` class is
-        used to retrive the master's address before establishing a new
-        connection.
-
-        NOTE: If the master's address has changed, any cached connections to
-        the old master are closed.
-
-        By default clients will be a :py:class:`~redis.Redis` instance.
-        Specify a different class to the ``redis_class`` argument if you
-        desire something different.
-
-        The ``connection_pool_class`` specifies the connection pool to
-        use.  The :py:class:`~redis.sentinel.SentinelConnectionPool`
-        will be used by default.
-
-        All other keyword arguments are merged with any connection_kwargs
-        passed to this class and passed to the connection pool as keyword
-        arguments to be used to initialize Redis connections.
-        """
-        kwargs["is_master"] = True
-        connection_kwargs = dict(self.connection_kwargs)
-        connection_kwargs.update(kwargs)
-        return redis_class(
-            connection_pool=connection_pool_class(
-                service_name, self, **connection_kwargs
-            )
-        )
-
-    def slave_for(
-        self,
-        service_name: str,
-        redis_class: Type[Redis] = Redis,
-        connection_pool_class: Type[SentinelConnectionPool] = SentinelConnectionPool,
-        **kwargs,
-    ):
-        """
-        Returns redis client instance for the ``service_name`` slave(s).
-
-        A SentinelConnectionPool class is used to retrive the slave's
-        address before establishing a new connection.
-
-        By default clients will be a :py:class:`~redis.Redis` instance.
-        Specify a different class to the ``redis_class`` argument if you
-        desire something different.
-
-        The ``connection_pool_class`` specifies the connection pool to use.
-        The SentinelConnectionPool will be used by default.
-
-        All other keyword arguments are merged with any connection_kwargs
-        passed to this class and passed to the connection pool as keyword
-        arguments to be used to initialize Redis connections.
-        """
-        kwargs["is_master"] = False
-        connection_kwargs = dict(self.connection_kwargs)
-        connection_kwargs.update(kwargs)
-        return redis_class(
-            connection_pool=connection_pool_class(
-                service_name, self, **connection_kwargs
-            )
-        )
+import random
+import weakref
+from typing import AsyncIterator, Iterable, Mapping, Sequence, Tuple, Type
+
+from aioredis.client import Redis
+from aioredis.connection import Connection, ConnectionPool, EncodableT, SSLConnection
+from aioredis.exceptions import (
+    ConnectionError,
+    ReadOnlyError,
+    ResponseError,
+    TimeoutError,
+)
+from aioredis.utils import str_if_bytes
+
+
+class MasterNotFoundError(ConnectionError):
+    pass
+
+
+class SlaveNotFoundError(ConnectionError):
+    pass
+
+
+class SentinelManagedConnection(SSLConnection):
+    def __init__(self, **kwargs):
+        self.connection_pool = kwargs.pop("connection_pool")
+        if not kwargs.pop("ssl", False):
+            # use constructor from Connection class
+            super(SSLConnection, self).__init__(**kwargs)
+        else:
+            # use constructor from SSLConnection class
+            super().__init__(**kwargs)
+
+    def __repr__(self):
+        pool = self.connection_pool
+        s = f"{self.__class__.__name__}<service={pool.service_name}"
+        if self.host:
+            host_info = f",host={self.host},port={self.port}"
+            s += host_info
+        return s + ">"
+
+    async def connect_to(self, address):
+        self.host, self.port = address
+        await super().connect()
+        if self.connection_pool.check_connection:
+            await self.send_command("PING")
+            if str_if_bytes(await self.read_response()) != "PONG":
+                raise ConnectionError("PING failed")
+
+    async def connect(self):
+        if self._reader:
+            return  # already connected
+        if self.connection_pool.is_master:
+            await self.connect_to(await self.connection_pool.get_master_address())
+        else:
+            async for slave in self.connection_pool.rotate_slaves():
+                try:
+                    return await self.connect_to(slave)
+                except ConnectionError:
+                    continue
+            raise SlaveNotFoundError  # Never be here
+
+    async def read_response(self):
+        try:
+            return await super().read_response()
+        except ReadOnlyError:
+            if self.connection_pool.is_master:
+                # When talking to a master, a ReadOnlyError when likely
+                # indicates that the previous master that we're still connected
+                # to has been demoted to a slave and there's a new master.
+                # calling disconnect will force the connection to re-query
+                # sentinel during the next connect() attempt.
+                await self.disconnect()
+                raise ConnectionError("The previous master is now a slave")
+            raise
+
+
+class SentinelConnectionPool(ConnectionPool):
+    """
+    Sentinel backed connection pool.
+
+    If ``check_connection`` flag is set to True, SentinelManagedConnection
+    sends a PING command right after establishing the connection.
+    """
+
+    def __init__(self, service_name, sentinel_manager, **kwargs):
+        kwargs["connection_class"] = kwargs.get(
+            "connection_class", SentinelManagedConnection
+        )
+        self.is_master = kwargs.pop("is_master", True)
+        self.check_connection = kwargs.pop("check_connection", False)
+        super().__init__(**kwargs)
+        self.connection_kwargs["connection_pool"] = weakref.proxy(self)
+        self.service_name = service_name
+        self.sentinel_manager = sentinel_manager
+        self.master_address = None
+        self.slave_rr_counter = None
+
+    def __repr__(self):
+        return (
+            f"{self.__class__.__name__}"
+            f"<service={self.service_name}({self.is_master and 'master' or 'slave'})>"
+        )
+
+    def reset(self):
+        super().reset()
+        self.master_address = None
+        self.slave_rr_counter = None
+
+    def owns_connection(self, connection: Connection):
+        check = not self.is_master or (
+            self.is_master and self.master_address == (connection.host, connection.port)
+        )
+        return check and super().owns_connection(connection)
+
+    async def get_master_address(self):
+        master_address = await self.sentinel_manager.discover_master(self.service_name)
+        if self.is_master:
+            if self.master_address != master_address:
+                self.master_address = master_address
+                # disconnect any idle connections so that they reconnect
+                # to the new master the next time that they are used.
+                await self.disconnect(inuse_connections=False)
+        return master_address
+
+    async def rotate_slaves(self) -> AsyncIterator:
+        """Round-robin slave balancer"""
+        slaves = await self.sentinel_manager.discover_slaves(self.service_name)
+        if slaves:
+            if self.slave_rr_counter is None:
+                self.slave_rr_counter = random.randint(0, len(slaves) - 1)
+            for _ in range(len(slaves)):
+                self.slave_rr_counter = (self.slave_rr_counter + 1) % len(slaves)
+                slave = slaves[self.slave_rr_counter]
+                yield slave
+        # Fallback to the master connection
+        try:
+            yield await self.get_master_address()
+        except MasterNotFoundError:
+            pass
+        raise SlaveNotFoundError(f"No slave found for {self.service_name!r}")
+
+
+class Sentinel:
+    """
+    Redis Sentinel cluster client
+
+    >>> from aioredis.sentinel import Sentinel
+    >>> sentinel = Sentinel([('localhost', 26379)], socket_timeout=0.1)
+    >>> master = sentinel.master_for('mymaster', socket_timeout=0.1)
+    >>> await master.set('foo', 'bar')
+    >>> slave = sentinel.slave_for('mymaster', socket_timeout=0.1)
+    >>> await slave.get('foo')
+    b'bar'
+
+    ``sentinels`` is a list of sentinel nodes. Each node is represented by
+    a pair (hostname, port).
+
+    ``min_other_sentinels`` defined a minimum number of peers for a sentinel.
+    When querying a sentinel, if it doesn't meet this threshold, responses
+    from that sentinel won't be considered valid.
+
+    ``sentinel_kwargs`` is a dictionary of connection arguments used when
+    connecting to sentinel instances. Any argument that can be passed to
+    a normal Redis connection can be specified here. If ``sentinel_kwargs`` is
+    not specified, any socket_timeout and socket_keepalive options specified
+    in ``connection_kwargs`` will be used.
+
+    ``connection_kwargs`` are keyword arguments that will be used when
+    establishing a connection to a Redis server.
+    """
+
+    def __init__(
+        self,
+        sentinels,
+        min_other_sentinels=0,
+        sentinel_kwargs=None,
+        **connection_kwargs,
+    ):
+        # if sentinel_kwargs isn't defined, use the socket_* options from
+        # connection_kwargs
+        if sentinel_kwargs is None:
+            sentinel_kwargs = {
+                k: v for k, v in connection_kwargs.items() if k.startswith("socket_")
+            }
+        self.sentinel_kwargs = sentinel_kwargs
+
+        self.sentinels = [
+            Redis(host=hostname, port=port, **self.sentinel_kwargs)
+            for hostname, port in sentinels
+        ]
+        self.min_other_sentinels = min_other_sentinels
+        self.connection_kwargs = connection_kwargs
+
+    def __repr__(self):
+        sentinel_addresses = []
+        for sentinel in self.sentinels:
+            sentinel_addresses.append(
+                f"{sentinel.connection_pool.connection_kwargs['host']}:"
+                f"{sentinel.connection_pool.connection_kwargs['port']}"
+            )
+        return f"{self.__class__.__name__}<sentinels=[{','.join(sentinel_addresses)}]>"
+
+    def check_master_state(self, state: dict, service_name: str) -> bool:
+        if not state["is_master"] or state["is_sdown"] or state["is_odown"]:
+            return False
+        # Check if our sentinel doesn't see other nodes
+        if state["num-other-sentinels"] < self.min_other_sentinels:
+            return False
+        return True
+
+    async def discover_master(self, service_name: str):
+        """
+        Asks sentinel servers for the Redis master's address corresponding
+        to the service labeled ``service_name``.
+
+        Returns a pair (address, port) or raises MasterNotFoundError if no
+        master is found.
+        """
+        for sentinel_no, sentinel in enumerate(self.sentinels):
+            try:
+                masters = await sentinel.sentinel_masters()
+            except (ConnectionError, TimeoutError):
+                continue
+            state = masters.get(service_name)
+            if state and self.check_master_state(state, service_name):
+                # Put this sentinel at the top of the list
+                self.sentinels[0], self.sentinels[sentinel_no] = (
+                    sentinel,
+                    self.sentinels[0],
+                )
+                return state["ip"], state["port"]
+        raise MasterNotFoundError(f"No master found for {service_name!r}")
+
+    def filter_slaves(
+        self, slaves: Iterable[Mapping]
+    ) -> Sequence[Tuple[EncodableT, EncodableT]]:
+        """Remove slaves that are in an ODOWN or SDOWN state"""
+        slaves_alive = []
+        for slave in slaves:
+            if slave["is_odown"] or slave["is_sdown"]:
+                continue
+            slaves_alive.append((slave["ip"], slave["port"]))
+        return slaves_alive
+
+    async def discover_slaves(
+        self, service_name: str
+    ) -> Sequence[Tuple[EncodableT, EncodableT]]:
+        """Returns a list of alive slaves for service ``service_name``"""
+        for sentinel in self.sentinels:
+            try:
+                slaves = await sentinel.sentinel_slaves(service_name)
+            except (ConnectionError, ResponseError, TimeoutError):
+                continue
+            slaves = self.filter_slaves(slaves)
+            if slaves:
+                return slaves
+        return []
+
+    def master_for(
+        self,
+        service_name: str,
+        redis_class: Type[Redis] = Redis,
+        connection_pool_class: Type[SentinelConnectionPool] = SentinelConnectionPool,
+        **kwargs,
+    ):
+        """
+        Returns a redis client instance for the ``service_name`` master.
+
+        A :py:class:`~redis.sentinel.SentinelConnectionPool` class is
+        used to retrive the master's address before establishing a new
+        connection.
+
+        NOTE: If the master's address has changed, any cached connections to
+        the old master are closed.
+
+        By default clients will be a :py:class:`~redis.Redis` instance.
+        Specify a different class to the ``redis_class`` argument if you
+        desire something different.
+
+        The ``connection_pool_class`` specifies the connection pool to
+        use.  The :py:class:`~redis.sentinel.SentinelConnectionPool`
+        will be used by default.
+
+        All other keyword arguments are merged with any connection_kwargs
+        passed to this class and passed to the connection pool as keyword
+        arguments to be used to initialize Redis connections.
+        """
+        kwargs["is_master"] = True
+        connection_kwargs = dict(self.connection_kwargs)
+        connection_kwargs.update(kwargs)
+        return redis_class(
+            connection_pool=connection_pool_class(
+                service_name, self, **connection_kwargs
+            )
+        )
+
+    def slave_for(
+        self,
+        service_name: str,
+        redis_class: Type[Redis] = Redis,
+        connection_pool_class: Type[SentinelConnectionPool] = SentinelConnectionPool,
+        **kwargs,
+    ):
+        """
+        Returns redis client instance for the ``service_name`` slave(s).
+
+        A SentinelConnectionPool class is used to retrive the slave's
+        address before establishing a new connection.
+
+        By default clients will be a :py:class:`~redis.Redis` instance.
+        Specify a different class to the ``redis_class`` argument if you
+        desire something different.
+
+        The ``connection_pool_class`` specifies the connection pool to use.
+        The SentinelConnectionPool will be used by default.
+
+        All other keyword arguments are merged with any connection_kwargs
+        passed to this class and passed to the connection pool as keyword
+        arguments to be used to initialize Redis connections.
+        """
+        kwargs["is_master"] = False
+        connection_kwargs = dict(self.connection_kwargs)
+        connection_kwargs.update(kwargs)
+        return redis_class(
+            connection_pool=connection_pool_class(
+                service_name, self, **connection_kwargs
+            )
+        )
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py

 * *Ordering differences only*

```diff
@@ -1,61 +1,61 @@
-from typing import TYPE_CHECKING, TypeVar, overload
-
-if TYPE_CHECKING:
-    from aioredis import Redis
-    from aioredis.client import Pipeline
-
-
-try:
-    import hiredis  # noqa
-
-    HIREDIS_AVAILABLE = True
-except ImportError:
-    HIREDIS_AVAILABLE = False
-
-
-_T = TypeVar("_T")
-
-
-def from_url(url, **kwargs):
-    """
-    Returns an active Redis client generated from the given database URL.
-
-    Will attempt to extract the database id from the path url fragment, if
-    none is provided.
-    """
-    from aioredis.client import Redis
-
-    return Redis.from_url(url, **kwargs)
-
-
-class pipeline:
-    def __init__(self, redis_obj: "Redis"):
-        self.p: "Pipeline" = redis_obj.pipeline()
-
-    async def __aenter__(self) -> "Pipeline":
-        return self.p
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.p.execute()
-        del self.p
-
-
-# Mypy bug: https://github.com/python/mypy/issues/11005
-@overload
-def str_if_bytes(value: bytes) -> str:  # type: ignore[misc]
-    ...
-
-
-@overload
-def str_if_bytes(value: _T) -> _T:
-    ...
-
-
-def str_if_bytes(value: object) -> object:
-    return (
-        value.decode("utf-8", errors="replace") if isinstance(value, bytes) else value
-    )
-
-
-def safe_str(value: object) -> str:
-    return str(str_if_bytes(value))
+from typing import TYPE_CHECKING, TypeVar, overload
+
+if TYPE_CHECKING:
+    from aioredis import Redis
+    from aioredis.client import Pipeline
+
+
+try:
+    import hiredis  # noqa
+
+    HIREDIS_AVAILABLE = True
+except ImportError:
+    HIREDIS_AVAILABLE = False
+
+
+_T = TypeVar("_T")
+
+
+def from_url(url, **kwargs):
+    """
+    Returns an active Redis client generated from the given database URL.
+
+    Will attempt to extract the database id from the path url fragment, if
+    none is provided.
+    """
+    from aioredis.client import Redis
+
+    return Redis.from_url(url, **kwargs)
+
+
+class pipeline:
+    def __init__(self, redis_obj: "Redis"):
+        self.p: "Pipeline" = redis_obj.pipeline()
+
+    async def __aenter__(self) -> "Pipeline":
+        return self.p
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.p.execute()
+        del self.p
+
+
+# Mypy bug: https://github.com/python/mypy/issues/11005
+@overload
+def str_if_bytes(value: bytes) -> str:  # type: ignore[misc]
+    ...
+
+
+@overload
+def str_if_bytes(value: _T) -> _T:
+    ...
+
+
+def str_if_bytes(value: object) -> object:
+    return (
+        value.decode("utf-8", errors="replace") if isinstance(value, bytes) else value
+    )
+
+
+def safe_str(value: object) -> str:
+    return str(str_if_bytes(value))
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 27 10:21:45 2023 UTC, .py size: 1223 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3984 fc63 c704 0000  a.......9..c....
+00000000: 610d 0d0a 0000 0000 506d 4a64 0205 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar 23 05:34:26 2023 UTC, .py size: 182652 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e2e4 1b64 7cc9 0200  a..........d|...
+00000000: 610d 0d0a 0000 0000 506d 4a64 40dc 0200  a.......PmJd@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0018 0000 0040 0000 0073 d004 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c07 5a07 6400 6402 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
@@ -1011,20 +1011,20 @@
 00003f20: 0029 047a 670a 2020 2020 5061 7273 696e  .).zg.    Parsin
 00003f30: 6720 636c 6965 6e74 2d69 6e66 6f20 696e  g client-info in
 00003f40: 2041 434c 204c 6f67 2069 6e20 666f 6c6c   ACL Log in foll
 00003f50: 6f77 696e 6720 666f 726d 6174 2e0a 2020  owing format..  
 00003f60: 2020 226b 6579 313d 7661 6c75 6531 206b    "key1=value1 k
 00003f70: 6579 323d 7661 6c75 6532 206b 6579 333d  ey2=value2 key3=
 00003f80: 7661 6c75 6533 220a 2020 2020 72f7 0000  value3".    r...
-00003f90: 0072 7e00 0000 3e0c 0000 00da 046f 6d65  .r~...>......ome
-00003fa0: 6dda 0264 62da 0471 6275 66da 0361 6765  m..db..qbuf..age
-00003fb0: 7a09 7162 7566 2d66 7265 65da 0373 7562  z.qbuf-free..sub
-00003fc0: da04 6964 6c65 da03 6f62 6cda 036f 6c6c  ..idle..obl..oll
-00003fd0: da04 7073 7562 7204 0100 00da 056d 756c  ..psubr......mul
-00003fe0: 7469 2902 724f 0000 0072 4600 0000 2906  ti).rO...rF...).
+00003f90: 0072 7e00 0000 3e0c 0000 00da 0373 7562  .r~...>......sub
+00003fa0: da04 6f6d 656d da04 7162 7566 da02 6462  ..omem..qbuf..db
+00003fb0: da03 6167 6572 0401 0000 da04 6964 6c65  ..ager......idle
+00003fc0: da03 6f62 6c7a 0971 6275 662d 6672 6565  ..oblz.qbuf-free
+00003fd0: da03 6f6c 6cda 056d 756c 7469 da04 7073  ..oll..multi..ps
+00003fe0: 7562 2902 724f 0000 0072 4600 0000 2906  ub).rO...rF...).
 00003ff0: 7283 0000 0072 3e01 0000 da05 696e 666f  r....r>.....info
 00004000: 7372 9300 0000 7295 0000 00da 0769 6e74  sr....r......int
 00004010: 5f6b 6579 7243 0000 0072 4300 0000 7244  _keyrC...rC...rD
 00004020: 0000 0072 3b01 0000 5002 0000 7310 0000  ...r;...P...s...
 00004030: 0000 0504 010a 0108 010e 010a 0308 0e12  ................
 00004040: 0172 3b01 0000 6301 0000 0000 0000 0000  .r;...c.........
 00004050: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
@@ -1927,15 +1927,15 @@
 00007860: 7372 a201 0000 729a 0000 0072 a401 0000  sr....r....r....
 00007870: 7243 0000 0072 4300 0000 7244 0000 0072  rC...rC...rD...r
 00007880: a501 0000 1503 0000 7304 0000 0000 2912  ........s.....).
 00007890: 017a 0e52 6564 6973 2e66 726f 6d5f 7572  .z.Redis.from_ur
 000078a0: 6cda 096c 6f63 616c 686f 7374 69eb 1800  l..localhosti...
 000078b0: 0072 0100 0000 4e7a 0575 7466 2d38 da06  .r....Nz.utf-8..
 000078c0: 7374 7269 6374 46da 0872 6571 7569 7265  strictF..require
-000078d0: 6429 19da 0468 6f73 7472 9d00 0000 7241  d)...hostr....rA
+000078d0: 6429 19da 0468 6f73 7472 9d00 0000 7243  d)...hostr....rC
 000078e0: 0100 00da 0870 6173 7377 6f72 64da 0e73  .....password..s
 000078f0: 6f63 6b65 745f 7469 6d65 6f75 74da 1673  ocket_timeout..s
 00007900: 6f63 6b65 745f 636f 6e6e 6563 745f 7469  ocket_connect_ti
 00007910: 6d65 6f75 74da 1073 6f63 6b65 745f 6b65  meout..socket_ke
 00007920: 6570 616c 6976 65da 1873 6f63 6b65 745f  epalive..socket_
 00007930: 6b65 6570 616c 6976 655f 6f70 7469 6f6e  keepalive_option
 00007940: 7372 a401 0000 da10 756e 6978 5f73 6f63  sr......unix_soc
@@ -1961,30 +1961,30 @@
 00007a80: 7401 6402 9c02 a101 0100 6e32 7c1a a000  t.d.......n2|...
 00007a90: 7c01 7c02 7c06 7c07 7c08 6403 9c05 a101  |.|.|.|.|.d.....
 00007aa0: 0100 7c0f 726c 7c1a a000 7402 7c10 7c11  ..|.rl|...t.|.|.
 00007ab0: 7c12 7c13 7c14 6404 9c06 a101 0100 7403  |.|.|.d.......t.
 00007ac0: 6600 6900 7c1a a401 8e01 7d09 7c09 7c00  f.i.|.....}.|.|.
 00007ad0: 5f04 7c16 7c00 5f05 6400 7c00 5f06 7407  _.|.|._.d.|._.t.
 00007ae0: 7c00 6a08 6a09 8301 7c00 5f0a 6400 5300  |.j.j...|._.d.S.
-00007af0: 2905 4e29 0b72 4101 0000 72be 0100 0072  ).N).rA...r....r
+00007af0: 2905 4e29 0b72 4301 0000 72be 0100 0072  ).N).rC...r....r
 00007b00: ab01 0000 72ac 0100 0072 b101 0000 72b2  ....r....r....r.
 00007b10: 0100 0072 0101 0000 72b3 0100 0072 ba01  ...r....r....r..
 00007b20: 0000 72bc 0100 0072 bd01 0000 2902 da04  ..r....r....)...
 00007b30: 7061 7468 da10 636f 6e6e 6563 7469 6f6e  path..connection
 00007b40: 5f63 6c61 7373 2905 72aa 0100 0072 9d00  _class).r....r..
 00007b50: 0000 72ad 0100 0072 ae01 0000 72af 0100  ..r....r....r...
 00007b60: 0029 0672 c001 0000 72b5 0100 0072 b601  .).r....r....r..
 00007b70: 0000 72b7 0100 0072 b801 0000 72b9 0100  ..r....r....r...
 00007b80: 0029 0b72 6500 0000 721c 0000 0072 1b00  .).re...r....r..
 00007b90: 0000 7219 0000 0072 a401 0000 72bb 0100  ..r....r....r...
 00007ba0: 00da 0a63 6f6e 6e65 6374 696f 6e72 5300  ...connectionrS.
 00007bb0: 0000 725f 0000 00da 1252 4553 504f 4e53  ..r_.....RESPONS
 00007bc0: 455f 4341 4c4c 4241 434b 5372 a101 0000  E_CALLBACKSr....
 00007bd0: 291b 7256 0000 0072 aa01 0000 729d 0000  ).rV...r....r...
-00007be0: 0072 4101 0000 72ab 0100 0072 ac01 0000  .rA...r....r....
+00007be0: 0072 4301 0000 72ab 0100 0072 ac01 0000  .rC...r....r....
 00007bf0: 72ad 0100 0072 ae01 0000 72af 0100 0072  r....r....r....r
 00007c00: a401 0000 72b0 0100 0072 b101 0000 72b2  ....r....r....r.
 00007c10: 0100 0072 0101 0000 72b3 0100 0072 b401  ...r....r....r..
 00007c20: 0000 72b5 0100 0072 b601 0000 72b7 0100  ..r....r....r...
 00007c30: 0072 b801 0000 72b9 0100 0072 ba01 0000  .r....r....r....
 00007c40: 72bb 0100 0072 bc01 0000 72bd 0100 0072  r....r....r....r
 00007c50: be01 0000 729a 0000 0072 4300 0000 7243  ....r....rC...rC
@@ -4152,23 +4152,23 @@
 00010370: 6572 6174 696f 6e20 7761 7320 7375 6363  eration was succ
 00010380: 6573 7366 756c 2e0a 2020 2020 2020 2020  essful..        
 00010390: da06 4d53 4554 4e58 72c9 0200 0072 ca02  ..MSETNXr....r..
 000103a0: 0000 7243 0000 0072 4300 0000 7244 0000  ..rC...rC...rD..
 000103b0: 00da 066d 7365 746e 787f 0700 0073 0800  ...msetnx....s..
 000103c0: 0000 0007 0401 0c01 0c01 7a0c 5265 6469  ..........z.Redi
 000103d0: 732e 6d73 6574 6e78 2903 72b2 0000 0072  s.msetnx).r....r
-000103e0: 4101 0000 7238 0000 0063 0300 0000 0000  A...r8...c......
+000103e0: 4301 0000 7238 0000 0063 0300 0000 0000  C...r8...c......
 000103f0: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
 00010400: 0000 730e 0000 007c 00a0 0064 017c 017c  ..s....|...d.|.|
 00010410: 02a1 0353 0029 027a 3b4d 6f76 6573 2074  ...S.).z;Moves t
 00010420: 6865 206b 6579 2060 606e 616d 6560 6020  he key ``name`` 
 00010430: 746f 2061 2064 6966 6665 7265 6e74 2052  to a different R
 00010440: 6564 6973 2064 6174 6162 6173 6520 6060  edis database ``
 00010450: 6462 6060 da04 4d4f 5645 7209 0200 0029  db``..MOVEr....)
-00010460: 0372 5600 0000 72b2 0000 0072 4101 0000  .rV...r....rA...
+00010460: 0372 5600 0000 72b2 0000 0072 4301 0000  .rV...r....rC...
 00010470: 7243 0000 0072 4300 0000 7244 0000 00da  rC...rC...rD....
 00010480: 046d 6f76 658b 0700 0073 0200 0000 0002  .move....s......
 00010490: 7a0a 5265 6469 732e 6d6f 7665 6302 0000  z.Redis.movec...
 000104a0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 000104b0: 0043 0000 0073 0c00 0000 7c00 a000 6401  .C...s....|...d.
 000104c0: 7c01 a102 5300 2902 7a21 5265 6d6f 7665  |...S.).z!Remove
 000104d0: 7320 616e 2065 7870 6972 6174 696f 6e20  s an expiration 
@@ -8066,15 +8066,15 @@
 0001f810: 2c18 0716 0763 0000 0000 0000 0000 0000  ,....c..........
 0001f820: 0000 0000 0000 0300 0000 4000 0000 733e  ..........@...s>
 0001f830: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
 0001f840: 0464 013c 0065 0565 0464 023c 0065 0665  .d.<.e.e.d.<.e.e
 0001f850: 0464 033c 0065 0665 0464 043c 0065 0665  .d.<.e.e.d.<.e.e
 0001f860: 0464 053c 0065 0665 0464 063c 0064 0753  .d.<.e.e.d.<.d.S
 0001f870: 0029 08da 124d 6f6e 6974 6f72 436f 6d6d  .)...MonitorComm
-0001f880: 616e 6449 6e66 6f72 8602 0000 7241 0100  andInfor....rA..
+0001f880: 616e 6449 6e66 6f72 8602 0000 7243 0100  andInfor....rC..
 0001f890: 00da 0e63 6c69 656e 745f 6164 6472 6573  ...client_addres
 0001f8a0: 73da 0b63 6c69 656e 745f 706f 7274 da0b  s..client_port..
 0001f8b0: 636c 6965 6e74 5f74 7970 6572 0701 0000  client_typer....
 0001f8c0: 4e29 0772 6700 0000 7268 0000 0072 6900  N).rg...rh...ri.
 0001f8d0: 0000 7281 0000 0072 3d04 0000 7246 0000  ..r....r=...rF..
 0001f8e0: 0072 3d00 0000 7243 0000 0072 4300 0000  .r=...rC...rC...
 0001f8f0: 7243 0000 0072 4400 0000 724c 0400 00f5  rC...rD...rL....
@@ -8172,15 +8172,15 @@
 0001feb0: 7a1a 436f 6e6e 6563 7469 6f6e 2061 6c72  z.Connection alr
 0001fec0: 6561 6479 2063 6c6f 7365 642e 5472 1e02  eady closed.Tr..
 0001fed0: 0000 72f7 0000 0072 8000 0000 7a19 496e  ..r....r....z.In
 0001fee0: 7661 6c69 6420 636f 6d6d 616e 6420 7265  valid command re
 0001fef0: 6365 6976 6564 2e7a 025c 22fa 0122 da03  ceived.z.\".."..
 0001ff00: 6c75 6172 3a01 0000 da04 756e 6978 e905  luar:.....unix..
 0001ff10: 0000 0072 6d00 0000 da03 7463 7029 0672  ...rm.....tcp).r
-0001ff20: 8602 0000 7241 0100 0072 4d04 0000 724e  ....rA...rM...rN
+0001ff20: 8602 0000 7243 0100 0072 4d04 0000 724e  ....rC...rM...rN
 0001ff30: 0400 0072 4f04 0000 7207 0100 0029 1472  ...rO...r....).r
 0001ff40: c101 0000 7223 0000 0072 5104 0000 7206  ....r#...rQ...r.
 0001ff50: 0200 0072 3b00 0000 723c 0000 0072 2402  ...r;...r<...r$.
 0001ff60: 0000 7223 0200 0072 4f00 0000 da0a 6d6f  ..r#...rO.....mo
 0001ff70: 6e69 746f 725f 7265 7245 0300 0072 ca00  nitor_rerE...r..
 0001ff80: 0000 7208 0100 00da 0a63 6f6d 6d61 6e64  ..r......command
 0001ff90: 5f72 65da 0766 696e 6461 6c6c 7264 0200  _re..findallrd..
@@ -8947,16 +8947,16 @@
 00022f20: 2020 5265 7370 6f6e 7365 4572 726f 7220    ResponseError 
 00022f30: 6578 6365 7074 696f 6e73 2c20 7375 6368  exceptions, such
 00022f40: 2061 7320 7468 6f73 6520 7261 6973 6564   as those raised
 00022f50: 2077 6865 6e20 6973 7375 696e 6720 6120   when issuing a 
 00022f60: 636f 6d6d 616e 640a 2020 2020 6f6e 2061  command.    on a
 00022f70: 206b 6579 206f 6620 6120 6469 6666 6572   key of a differ
 00022f80: 656e 7420 6461 7461 7479 7065 2e0a 2020  ent datatype..  
-00022f90: 2020 3e03 0000 00da 0755 4e57 4154 4348    >......UNWATCH
-00022fa0: da07 4449 5343 4152 44da 0445 5845 4329  ..DISCARD..EXEC)
+00022f90: 2020 3e03 0000 00da 0744 4953 4341 5244    >......DISCARD
+00022fa0: da07 554e 5741 5443 48da 0445 5845 4329  ..UNWATCH..EXEC)
 00022fb0: 0472 a401 0000 72a1 0100 0072 ce01 0000  .r....r....r....
 00022fc0: 72cf 0100 0063 0500 0000 0000 0000 0000  r....c..........
 00022fd0: 0000 0500 0000 0200 0000 4300 0000 733c  ..........C...s<
 00022fe0: 0000 007c 017c 005f 0064 007c 005f 017c  ...|.|._.d.|._.|
 00022ff0: 027c 005f 027c 037c 005f 037c 047c 005f  .|._.|.|._.|.|._
 00023000: 0464 017c 005f 0567 007c 005f 0674 0783  .d.|._.g.|._.t..
 00023010: 007c 005f 0864 017c 005f 0964 0053 0029  .|._.d.|._.d.S.)
@@ -9026,15 +9026,15 @@
 00023410: 0100 7c00 6a04 a006 a100 4900 6400 4800  ..|.j.....I.d.H.
 00023420: 0100 5700 6e28 0400 7407 7968 0100 0100  ..W.n(..t.yh....
 00023430: 0100 7c00 6a04 7264 7c00 6a04 a008 a100  ..|.j.rd|.j.....
 00023440: 4900 6400 4800 0100 5900 6e02 3000 6402  I.d.H...Y.n.0.d.
 00023450: 7c00 5f03 6402 7c00 5f09 7c00 6a04 7296  |._.d.|._.|.j.r.
 00023460: 7c00 6a0a a00b 7c00 6a04 a101 4900 6400  |.j...|.j...I.d.
 00023470: 4800 0100 6400 7c00 5f04 6400 5300 2903  H...d.|._.d.S.).
-00023480: 4e72 9e04 0000 4629 0c72 a304 0000 72b0  Nr....F).r....r.
+00023480: 4e72 9f04 0000 4629 0c72 a304 0000 72b0  Nr....F).r....r.
 00023490: 0000 0072 a404 0000 72a2 0400 0072 c101  ...r....r....r..
 000234a0: 0000 72fe 0100 0072 0602 0000 721d 0000  ..r....r....r...
 000234b0: 0072 0002 0000 72a5 0400 0072 a401 0000  .r....r....r....
 000234c0: 72fb 0100 0072 c501 0000 7243 0000 0072  r....r....rC...r
 000234d0: 4300 0000 7244 0000 0072 1902 0000 0f11  C...rD...r......
 000234e0: 0000 731c 0000 0000 0106 0108 030c 0102  ..s.............
 000234f0: 0312 0114 010c 0206 0116 0206 0106 0306  ................
@@ -9057,15 +9057,15 @@
 00023600: 6564 2063 616c 6c73 2074 6f20 4d55 4c54  ed calls to MULT
 00023610: 497a 3a43 6f6d 6d61 6e64 7320 7769 7468  Iz:Commands with
 00023620: 6f75 7420 616e 2069 6e69 7469 616c 2057  out an initial W
 00023630: 4154 4348 2068 6176 6520 616c 7265 6164  ATCH have alread
 00023640: 7920 6265 656e 2069 7373 7565 6454 4e29  y been issuedTN)
 00023650: 0372 a504 0000 7223 0000 0072 a304 0000  .r....r#...r....
 00023660: 72c5 0100 0072 4300 0000 7243 0000 0072  r....rC...rC...r
-00023670: 4400 0000 7249 0100 0027 1100 0073 0e00  D...rI...'...s..
+00023670: 4400 0000 7248 0100 0027 1100 0073 0e00  D...rH...'...s..
 00023680: 0000 0005 0601 0801 0601 0201 02ff 0403  ................
 00023690: 7a0e 5069 7065 6c69 6e65 2e6d 756c 7469  z.Pipeline.multi
 000236a0: 72e5 0100 0063 0100 0000 0000 0000 0000  r....c..........
 000236b0: 0000 0300 0000 0400 0000 4f00 0000 7338  ..........O...s8
 000236c0: 0000 007c 006a 0073 127c 0164 0119 0064  ...|.j.s.|.d...d
 000236d0: 026b 0272 287c 006a 0173 287c 006a 027c  .k.r(|.j.s(|.j.|
 000236e0: 0169 007c 02a4 018e 0153 007c 006a 037c  .i.|.....S.|.j.|
@@ -9430,28 +9430,28 @@
 00024d50: 0000 0000 0206 0108 017a 0e50 6970 656c  .........z.Pipel
 00024d60: 696e 652e 7761 7463 6863 0100 0000 0000  ine.watchc......
 00024d70: 0000 0000 0000 0100 0000 0300 0000 c300  ................
 00024d80: 0000 731a 0000 007c 006a 0072 167c 00a0  ..s....|.j.r.|..
 00024d90: 0164 01a1 0149 0064 0248 0070 1864 0353  .d...I.d.H.p.d.S
 00024da0: 0029 047a 2755 6e77 6174 6368 6573 2061  .).z'Unwatches a
 00024db0: 6c6c 2070 7265 7669 6f75 736c 7920 7370  ll previously sp
-00024dc0: 6563 6966 6965 6420 6b65 7973 729e 0400  ecified keysr...
+00024dc0: 6563 6966 6965 6420 6b65 7973 729f 0400  ecified keysr...
 00024dd0: 004e 5429 0272 a204 0000 7204 0200 0072  .NT).r....r....r
 00024de0: c501 0000 7243 0000 0072 4300 0000 7244  ....rC...rC...rD
 00024df0: 0000 00da 0775 6e77 6174 6368 2a12 0000  .....unwatch*...
 00024e00: 7302 0000 0000 027a 1050 6970 656c 696e  s......z.Pipelin
 00024e10: 652e 756e 7761 7463 6829 0154 292e 7267  e.unwatch).T).rg
 00024e20: 0000 0072 6800 0000 7269 0000 0072 6a00  ...rh...ri...rj.
 00024e30: 0000 72bf 0400 0072 1900 0000 720b 0000  ..r....r....r...
 00024e40: 0072 1300 0000 723d 0000 0072 3c00 0000  .r....r=...r<...
 00024e50: 723c 0400 0072 5a01 0000 720d 0000 0072  r<...rZ...r....r
 00024e60: 5a00 0000 7232 0000 0072 ea01 0000 72f0  Z...r2...r....r.
 00024e70: 0100 0072 c801 0000 72f6 0100 0072 a704  ...r....r....r..
 00024e80: 0000 72a8 0400 0072 a604 0000 7219 0200  ..r....r....r...
-00024e90: 0072 4901 0000 7205 0000 0072 0402 0000  .rI...r....r....
+00024e90: 0072 4801 0000 7205 0000 0072 0402 0000  .rH...r....r....
 00024ea0: 72aa 0400 0072 ab04 0000 7218 0000 00da  r....r....r.....
 00024eb0: 0d43 6f6d 6d61 6e64 5374 6163 6b54 72bb  .CommandStackTr.
 00024ec0: 0400 0072 bc04 0000 7208 0000 0072 0300  ...r....r....r..
 00024ed0: 0000 72b2 0400 0072 b304 0000 7246 0000  ..r....r....rF..
 00024ee0: 0072 6802 0000 72b0 0400 0072 ff01 0000  .rh...r....r....
 00024ef0: 72c5 0400 0072 d801 0000 723f 0400 0072  r....r....r?...r
 00024f00: d501 0000 72c7 0400 0072 6b00 0000 7243  ....r....rk...rC
@@ -9810,19 +9810,19 @@
 00026510: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
 00026520: 5a0d 6169 6f72 6564 6973 2e6c 6f63 6b72  Z.aioredis.lockr
 00026530: 2800 0000 da0e 6169 6f72 6564 6973 2e75  (.....aioredis.u
 00026540: 7469 6c73 7229 0000 0072 2a00 0000 7246  tilsr)...r*...rF
 00026550: 0000 0072 4204 0000 72ab 0200 0072 4104  ...rB...r....rA.
 00026560: 0000 7281 0000 0072 3d00 0000 7249 0400  ..r....r=...rI..
 00026570: 0072 d904 0000 723c 0000 0072 4000 0000  .r....r<...r@...
-00026580: 5a0c 5f53 7472 696e 674c 696b 6554 723f  Z._StringLikeTr?
+00026580: da0c 5f53 7472 696e 674c 696b 6554 723f  .._StringLikeTr?
 00026590: 0400 0072 4304 0000 7247 0400 0072 4004  ...rC...rG...r@.
 000265a0: 0000 724a 0400 0072 4504 0000 7248 0400  ..rJ...rE...rH..
 000265b0: 0072 4604 0000 724b 0400 0072 4404 0000  .rF...rK...rD...
-000265c0: 722b 0000 0072 2c00 0000 5a0b 416e 7943  r+...r,...Z.AnyC
+000265c0: 722b 0000 0072 2c00 0000 da0b 416e 7943  r+...r,.....AnyC
 000265d0: 6861 6e6e 656c 5472 9804 0000 da09 5359  hannelTr......SY
 000265e0: 4d5f 454d 5054 5972 2e00 0000 722f 0000  M_EMPTYr....r/..
 000265f0: 0072 3100 0000 7232 0000 0072 6802 0000  .r1...r2...rh...
 00026600: 7234 0000 0072 4500 0000 724c 0000 0072  r4...rE...rL...r
 00026610: 5200 0000 724d 0000 0072 5300 0000 7278  R...rM...rS...rx
 00026620: 0000 0072 7c00 0000 7296 0000 0072 9c00  ...r|...r....r..
 00026630: 0000 72af 0000 0072 b400 0000 72b7 0000  ..r....r....r...
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 27 10:21:45 2023 UTC, .py size: 183 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,22 +1,22 @@
-00000000: 610d 0d0a 0000 0000 3984 fc63 b700 0000  a.......9..c....
+00000000: 610d 0d0a 0000 0000 506d 4a64 bf00 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6500 6a01 6402 6b05 7224  d.l.Z.e.j.d.k.r$
 00000040: 6400 6403 6c02 6d03 5a03 6d04 5a04 0100  d.d.l.m.Z.m.Z...
 00000050: 6e10 6400 6403 6c05 6d03 5a03 6d04 5a04  n.d.d.l.m.Z.m.Z.
 00000060: 0100 6403 5a06 6401 5300 2904 e900 0000  ..d.Z.d.S.).....
 00000070: 004e 2902 e903 0000 00e9 0800 0000 2902  .N)...........).
 00000080: da08 5072 6f74 6f63 6f6c da09 5479 7065  ..Protocol..Type
 00000090: 6444 6963 7429 07da 0373 7973 da0c 7665  dDict)...sys..ve
 000000a0: 7273 696f 6e5f 696e 666f da06 7479 7069  rsion_info..typi
-000000b0: 6e67 7204 0000 0072 0500 0000 5a11 7479  ngr....r....Z.ty
+000000b0: 6e67 7204 0000 0072 0500 0000 da11 7479  ngr....r......ty
 000000c0: 7069 6e67 5f65 7874 656e 7369 6f6e 73da  ping_extensions.
-000000d0: 075f 5f61 6c6c 5f5f a900 720a 0000 0072  .__all__..r....r
-000000e0: 0a00 0000 fa55 443a 5c63 6f64 6573 5c66  .....UD:\codes\f
+000000d0: 075f 5f61 6c6c 5f5f a900 720b 0000 0072  .__all__..r....r
+000000e0: 0b00 0000 fa55 443a 5c63 6f64 6573 5c66  .....UD:\codes\f
 000000f0: 756e 626f 6f73 745c 6675 6e62 6f6f 7374  unboost\funboost
 00000100: 5c75 7469 6c73 5c64 6570 656e 6465 6e63  \utils\dependenc
 00000110: 795f 7061 636b 6167 6573 5f69 6e5f 7079  y_packages_in_py
 00000120: 7468 6f6e 7061 7468 5c61 696f 7265 6469  thonpath\aioredi
 00000130: 735c 636f 6d70 6174 2e70 79da 083c 6d6f  s\compat.py..<mo
 00000140: 6475 6c65 3e01 0000 0073 0800 0000 0802  dule>....s......
 00000150: 0a01 1202 1002                           ......
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar 23 05:34:26 2023 UTC, .py size: 62239 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e2e4 1b64 1ff3 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 506d 4a64 a3f9 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 c203 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6401 6c02 5a02 6400 6401 6c03 5a03  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6401 6c04 5a04 6400 6401 6c05 5a05  d.d.l.Z.d.d.l.Z.
 00000060: 6400 6401 6c06 5a06 6400 6401 6c07 5a07  d.d.l.Z.d.d.l.Z.
 00000070: 6400 6401 6c08 5a08 6400 6401 6c09 5a09  d.d.l.Z.d.d.l.Z.
@@ -2609,15 +2609,15 @@
 0000a300: 696f 6eda 0477 6172 6e72 4a01 0000 724c  ion..warnrJ...rL
 0000a310: 0100 0072 ae00 0000 5a06 5359 4d5f 4c46  ...r....Z.SYM_LF
 0000a320: 7249 0100 0072 9a00 0000 da04 456e 756d  rI...r......Enum
 0000a330: 722d 0000 0072 3200 0000 7297 0000 0072  r-...r2...r....r
 0000a340: 8300 0000 7285 0000 0072 8600 0000 7284  ....r....r....r.
 0000a350: 0000 0072 4800 0000 7249 0000 0072 5700  ...rH...rI...rW.
 0000a360: 0000 723a 0000 0072 4b00 0000 724c 0000  ..r:...rK...rL..
-0000a370: 005a 0844 6563 6f64 6564 5472 5600 0000  .Z.DecodedTrV...
+0000a370: 00da 0844 6563 6f64 6564 5472 5600 0000  ...DecodedTrV...
 0000a380: 7235 0000 0072 3e00 0000 723b 0000 0072  r5...r>...r;...r
 0000a390: 8700 0000 7258 0000 0072 8800 0000 72b3  ....rX...r....r.
 0000a3a0: 0000 0072 c600 0000 723c 0000 0072 d300  ...r....r<...r..
 0000a3b0: 0000 72d4 0000 0072 d700 0000 5a10 436f  ..r....r....Z.Co
 0000a3c0: 6e6e 6563 7443 616c 6c62 6163 6b54 7278  nnectCallbackTrx
 0000a3d0: 0000 0072 5801 0000 7265 0100 0072 7201  ...rX...re...rr.
 0000a3e0: 0000 727b 0100 0072 4a00 0000 727c 0100  ..r{...rJ...r|..
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar  9 11:46:09 2023 UTC, .py size: 1586 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 01c7 0964 3206 0000  a..........d2...
+00000000: 610d 0d0a 0000 0000 506d 4a64 9206 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4e01 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 4700 6403 6404 8400 6404 6503 8303  Z.G.d.d...d.e...
 00000050: 5a04 4700 6405 6406 8400 6406 6504 8303  Z.G.d.d...d.e...
 00000060: 5a05 4700 6407 6408 8400 6408 6501 6a06  Z.G.d.d...d.e.j.
 00000070: 6504 8304 5a06 4700 6409 640a 8400 640a  e...Z.G.d.d...d.
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 27 10:21:45 2023 UTC, .py size: 11651 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3984 fc63 832d 0000  a.......9..c.-..
+00000000: 610d 0d0a 0000 0000 506d 4a64 b52e 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6404 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6506  d.l.m.Z.m.Z...e.
```

## funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 27 10:21:45 2023 UTC, .py size: 1284 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3984 fc63 0405 0000  a.......9..c....
+00000000: 610d 0d0a 0000 0000 506d 4a64 4105 0000  a.......PmJdA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6501 7230 6400 6402 6c04 6d05 5a05  ..e.r0d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 7a10  ..d.d.l.m.Z...z.
 00000060: 6400 6404 6c08 5a08 6405 5a09 5700 6e16  d.d.l.Z.d.Z.W.n.
 00000070: 0400 650a 7956 0100 0100 0100 6406 5a09  ..e.yV......d.Z.
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py

 * *Ordering differences only*

```diff
@@ -1,133 +1,133 @@
-'''
-    Copyright (c) 2016, 2017, 2019 Timothy Savannah All Rights Reserved.
-
-    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
-    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
-'''
-
-import os
-import ctypes
-import threading
-
-__all__ = ('StoppableThread', 'JoinThread')
-
-class StoppableThread(threading.Thread):
-    '''
-        StoppableThread - A thread that can be stopped by forcing an exception in the execution context.
-
-          This works both to interrupt code that is in C or in python code, at either the next call to a python function,
-           or the next line in python code.
-
-        It is recommended that if you call stop ( @see StoppableThread.stop ) that you use an exception that inherits BaseException, to ensure it likely isn't caught.
-
-         Also, beware unmarked exception handlers in your code. Code like this:
-
-            while True:
-                try:
-                    doSomething()
-                except:
-                    continue
-
-        will never be able to abort, because the exception you raise is immediately caught.
-
-        The exception is raised over and over, with a specifed delay (default 2.0 seconds)
-    '''
-
-
-    def _stopThread(self, exception, raiseEvery=2.0):
-        '''
-            _stopThread - @see StoppableThread.stop
-        '''
-        if self.is_alive() is False:
-            return True
-
-        self._stderr = open(os.devnull, 'w')
-
-        # Create "joining" thread which will raise the provided exception
-        #  on a repeat, until the thread stops.
-        joinThread = JoinThread(self, exception, repeatEvery=raiseEvery)
-
-        # Try to prevent spurrious prints
-        joinThread._stderr = self._stderr
-        joinThread.start()
-        joinThread._stderr = self._stderr
-
-
-    def stop(self, exception, raiseEvery=2.0):
-        '''
-            Stops the thread by raising a given exception.
-
-            @param exception <Exception type> - Exception to throw. Likely, you want to use something
-
-              that inherits from BaseException (so except BaseException as e: continue; isn't a problem)
-
-              This should be a class/type, NOT an instance, i.e.  MyExceptionType   not  MyExceptionType()
-
-
-            @param raiseEvery <float> Default 2.0 - We will keep raising this exception every #raiseEvery seconds,
-
-                until the thread terminates.
-
-                If your code traps a specific exception type, this will allow you #raiseEvery seconds to cleanup before exit.
-
-                If you're calling third-party code you can't control, which catches BaseException, set this to a low number
-
-                  to break out of their exception handler.
-
-
-             @return <None>
-        '''
-        return self._stopThread(exception, raiseEvery)
-
-
-class JoinThread(threading.Thread):
-    '''
-        JoinThread - The workhouse that stops the StoppableThread.
-
-            Takes an exception, and upon being started immediately raises that exception in the current context
-              of the thread's execution (so next line of python gets it, or next call to a python api function in C code ).
-
-            @see StoppableThread for more details
-    '''
-
-    def __init__(self, otherThread, exception, repeatEvery=2.0):
-        '''
-            __init__ - Create a JoinThread (don't forget to call .start() ! )
-
-                @param otherThread <threading.Thread> - A thread
-
-                @param exception <BaseException> - An exception. Should be a BaseException, to prevent "catch Exception as e: continue" type code
-                  from never being terminated. If such code is unavoidable, you can try setting #repeatEvery to a very low number, like .00001,
-                  and it will hopefully raise within the context of the catch, and be able to break free.
-
-                @param repeatEvery <float> Default 2.0 - After starting, the given exception is immediately raised. Then, every #repeatEvery seconds,
-                  it is raised again, until the thread terminates.
-        '''
-        threading.Thread.__init__(self)
-        self.otherThread = otherThread
-        self.exception = exception
-        self.repeatEvery = repeatEvery
-        self.daemon = True
-
-    def run(self):
-        '''
-            run - The thread main. Will attempt to stop and join the attached thread.
-        '''
-
-        # Try to silence default exception printing.
-        self.otherThread._Thread__stderr = self._stderr
-        if hasattr(self.otherThread, '_Thread__stop'):
-            # If py2, call this first to start thread termination cleanly.
-            #   Python3 does not need such ( nor does it provide.. )
-            self.otherThread._Thread__stop()
-        while self.otherThread.is_alive():
-            # We loop raising exception incase it's caught hopefully this breaks us far out.
-            ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(self.otherThread.ident), ctypes.py_object(self.exception))
-            self.otherThread.join(self.repeatEvery)
-
-        try:
-            self._stderr.close()
-        except:
-            pass
-
-# vim: set ts=4 sw=4 expandtab :
+'''
+    Copyright (c) 2016, 2017, 2019 Timothy Savannah All Rights Reserved.
+
+    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
+    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
+'''
+
+import os
+import ctypes
+import threading
+
+__all__ = ('StoppableThread', 'JoinThread')
+
+class StoppableThread(threading.Thread):
+    '''
+        StoppableThread - A thread that can be stopped by forcing an exception in the execution context.
+
+          This works both to interrupt code that is in C or in python code, at either the next call to a python function,
+           or the next line in python code.
+
+        It is recommended that if you call stop ( @see StoppableThread.stop ) that you use an exception that inherits BaseException, to ensure it likely isn't caught.
+
+         Also, beware unmarked exception handlers in your code. Code like this:
+
+            while True:
+                try:
+                    doSomething()
+                except:
+                    continue
+
+        will never be able to abort, because the exception you raise is immediately caught.
+
+        The exception is raised over and over, with a specifed delay (default 2.0 seconds)
+    '''
+
+
+    def _stopThread(self, exception, raiseEvery=2.0):
+        '''
+            _stopThread - @see StoppableThread.stop
+        '''
+        if self.is_alive() is False:
+            return True
+
+        self._stderr = open(os.devnull, 'w')
+
+        # Create "joining" thread which will raise the provided exception
+        #  on a repeat, until the thread stops.
+        joinThread = JoinThread(self, exception, repeatEvery=raiseEvery)
+
+        # Try to prevent spurrious prints
+        joinThread._stderr = self._stderr
+        joinThread.start()
+        joinThread._stderr = self._stderr
+
+
+    def stop(self, exception, raiseEvery=2.0):
+        '''
+            Stops the thread by raising a given exception.
+
+            @param exception <Exception type> - Exception to throw. Likely, you want to use something
+
+              that inherits from BaseException (so except BaseException as e: continue; isn't a problem)
+
+              This should be a class/type, NOT an instance, i.e.  MyExceptionType   not  MyExceptionType()
+
+
+            @param raiseEvery <float> Default 2.0 - We will keep raising this exception every #raiseEvery seconds,
+
+                until the thread terminates.
+
+                If your code traps a specific exception type, this will allow you #raiseEvery seconds to cleanup before exit.
+
+                If you're calling third-party code you can't control, which catches BaseException, set this to a low number
+
+                  to break out of their exception handler.
+
+
+             @return <None>
+        '''
+        return self._stopThread(exception, raiseEvery)
+
+
+class JoinThread(threading.Thread):
+    '''
+        JoinThread - The workhouse that stops the StoppableThread.
+
+            Takes an exception, and upon being started immediately raises that exception in the current context
+              of the thread's execution (so next line of python gets it, or next call to a python api function in C code ).
+
+            @see StoppableThread for more details
+    '''
+
+    def __init__(self, otherThread, exception, repeatEvery=2.0):
+        '''
+            __init__ - Create a JoinThread (don't forget to call .start() ! )
+
+                @param otherThread <threading.Thread> - A thread
+
+                @param exception <BaseException> - An exception. Should be a BaseException, to prevent "catch Exception as e: continue" type code
+                  from never being terminated. If such code is unavoidable, you can try setting #repeatEvery to a very low number, like .00001,
+                  and it will hopefully raise within the context of the catch, and be able to break free.
+
+                @param repeatEvery <float> Default 2.0 - After starting, the given exception is immediately raised. Then, every #repeatEvery seconds,
+                  it is raised again, until the thread terminates.
+        '''
+        threading.Thread.__init__(self)
+        self.otherThread = otherThread
+        self.exception = exception
+        self.repeatEvery = repeatEvery
+        self.daemon = True
+
+    def run(self):
+        '''
+            run - The thread main. Will attempt to stop and join the attached thread.
+        '''
+
+        # Try to silence default exception printing.
+        self.otherThread._Thread__stderr = self._stderr
+        if hasattr(self.otherThread, '_Thread__stop'):
+            # If py2, call this first to start thread termination cleanly.
+            #   Python3 does not need such ( nor does it provide.. )
+            self.otherThread._Thread__stop()
+        while self.otherThread.is_alive():
+            # We loop raising exception incase it's caught hopefully this breaks us far out.
+            ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(self.otherThread.ident), ctypes.py_object(self.exception))
+            self.otherThread.join(self.repeatEvery)
+
+        try:
+            self._stderr.close()
+        except:
+            pass
+
+# vim: set ts=4 sw=4 expandtab :
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
-'''
-    Copyright (c) 2016, 2017, 2019 Tim Savannah All Rights Reserved.
-
-    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
-    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
-'''
-
-
-__version__ = '4.3.5'
-__version_tuple__ = (4, 3, 5)
-
-__all__ = ('func_timeout', 'func_set_timeout', 'FunctionTimedOut', 'StoppableThread')
-
-from .exceptions import FunctionTimedOut
-from .dafunc import func_timeout, func_set_timeout
-from .StoppableThread import StoppableThread
+'''
+    Copyright (c) 2016, 2017, 2019 Tim Savannah All Rights Reserved.
+
+    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
+    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
+'''
+
+
+__version__ = '4.3.5'
+__version_tuple__ = (4, 3, 5)
+
+__all__ = ('func_timeout', 'func_set_timeout', 'FunctionTimedOut', 'StoppableThread')
+
+from .exceptions import FunctionTimedOut
+from .dafunc import func_timeout, func_set_timeout
+from .StoppableThread import StoppableThread
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py

 * *Ordering differences only*

```diff
@@ -1,234 +1,234 @@
-
-# vim: set ts=4 sw=4 expandtab :
-
-'''
-    Copyright (c) 2016, 2017 Tim Savannah All Rights Reserved.
-
-    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
-    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
-'''
-
-import copy
-import inspect
-import threading
-import time
-import types
-import sys
-
-from .exceptions import FunctionTimedOut
-from .StoppableThread import StoppableThread
-
-
-from .py3_raise import raise_exception
-
-
-from functools import wraps
-
-__all__ = ('func_timeout', 'func_set_timeout')
-
-
-def func_timeout(timeout, func, args=(), kwargs=None):
-    '''
-        func_timeout - Runs the given function for up to #timeout# seconds.
-
-        Raises any exceptions #func# would raise, returns what #func# would return (unless timeout is exceeded), in which case it raises FunctionTimedOut
-
-        @param timeout <float> - Maximum number of seconds to run #func# before terminating
-
-        @param func <function> - The function to call
-
-        @param args    <tuple> - Any ordered arguments to pass to the function
-
-        @param kwargs  <dict/None> - Keyword arguments to pass to the function.
-
-
-        @raises - FunctionTimedOut if #timeout# is exceeded, otherwise anything #func# could raise will be raised
-
-        If the timeout is exceeded, FunctionTimedOut will be raised within the context of the called function every two seconds until it terminates,
-        but will not block the calling thread (a new thread will be created to perform the join). If possible, you should try/except FunctionTimedOut
-        to return cleanly, but in most cases it will 'just work'.
-
-        @return - The return value that #func# gives
-    '''
-
-    if not kwargs:
-        kwargs = {}
-    if not args:
-        args = ()
-
-    ret = []
-    exception = []
-    isStopped = False
-
-    def funcwrap(args2, kwargs2):
-        try:
-            ret.append( func(*args2, **kwargs2) )
-        except FunctionTimedOut:
-            # Don't print traceback to stderr if we time out
-            pass
-        except BaseException as e:
-            exc_info = sys.exc_info()
-            if isStopped is False:
-                # Assemble the alternate traceback, excluding this function
-                #  from the trace (by going to next frame)
-                # Pytohn3 reads native from __traceback__,
-                # python2 has a different form for "raise"
-                e.__traceback__ = exc_info[2].tb_next
-                exception.append( e )
-
-    thread = StoppableThread(target=funcwrap, args=(args, kwargs))
-    thread.daemon = True
-
-    thread.start()
-    thread.join(timeout)
-
-    stopException = None
-    if thread.is_alive():
-        isStopped = True
-
-        class FunctionTimedOutTempType(FunctionTimedOut):
-            def __init__(self):
-                return FunctionTimedOut.__init__(self, '', timeout, func, args, kwargs)
-
-        FunctionTimedOutTemp = type('FunctionTimedOut' + str( hash( "%d_%d_%d_%d" %(id(timeout), id(func), id(args), id(kwargs))) ), FunctionTimedOutTempType.__bases__, dict(FunctionTimedOutTempType.__dict__))
-
-        stopException = FunctionTimedOutTemp
-        # raise FunctionTimedOut('', timeout, func, args, kwargs)
-        thread._stopThread(stopException)
-        thread.join(min(.1, timeout / 50.0))
-        raise FunctionTimedOut('', timeout, func, args, kwargs)
-    else:
-        # We can still cleanup the thread here..
-        # Still give a timeout... just... cuz..
-        thread.join(.5)
-
-    if exception:
-        raise_exception(exception)
-
-    if ret:
-        return ret[0]
-
-
-def func_set_timeout(timeout, allowOverride=False):
-    '''
-        func_set_timeout - Decorator to run a function with a given/calculated timeout (max execution time).
-            Optionally (if #allowOverride is True), adds a paramater, "forceTimeout", to the
-            function which, if provided, will override the default timeout for that invocation.
-
-            If #timeout is provided as a lambda/function, it will be called
-              prior to each invocation of the decorated function to calculate the timeout to be used
-              for that call, based on the arguments passed to the decorated function.
-
-              For example, you may have a "processData" function whose execution time
-              depends on the number of "data" elements, so you may want a million elements to have a
-              much higher timeout than seven elements.)
-
-            If #allowOverride is True AND a kwarg of "forceTimeout" is passed to the wrapped function, that timeout
-             will be used for that single call.
-
-        @param timeout <float OR lambda/function> -
-
-            **If float:**
-                Default number of seconds max to allow function to execute
-                  before throwing FunctionTimedOut
-
-            **If lambda/function:
-
-                 If a function/lambda is provided, it will be called for every
-                  invocation of the decorated function (unless #allowOverride=True and "forceTimeout" was passed)
-                  to determine the timeout to use based on the arguments to the decorated function.
-
-                    The arguments as passed into the decorated function will be passed to this function.
-                     They either must match exactly to what the decorated function has, OR
-                      if you prefer to get the *args (list of ordered args) and **kwargs ( key : value  keyword args form),
-                      define your calculate function like:
-
-                        def calculateTimeout(*args, **kwargs):
-                            ...
-
-                      or lambda like:
-
-                        calculateTimeout = lambda *args, **kwargs : ...
-
-                    otherwise the args to your calculate function should match exactly the decorated function.
-
-
-        @param allowOverride <bool> Default False, if True adds a keyword argument to the decorated function,
-            "forceTimeout" which, if provided, will override the #timeout. If #timeout was provided as a lambda / function, it
-             will not be called.
-
-        @throws FunctionTimedOut If time alloted passes without function returning naturally
-
-        @see func_timeout
-    '''
-    # Try to be as efficent as possible... don't compare the args more than once
-
-    #  Helps closure issue on some versions of python
-    defaultTimeout = copy.copy(timeout)
-
-    isTimeoutAFunction = bool( issubclass(timeout.__class__, (types.FunctionType, types.MethodType, types.LambdaType, types.BuiltinFunctionType, types.BuiltinMethodType) ) )
-
-    if not isTimeoutAFunction:
-        if not issubclass(timeout.__class__, (float, int)):
-            try:
-                timeout = float(timeout)
-            except:
-                raise ValueError('timeout argument must be a float/int for number of seconds, or a function/lambda which gets passed the function arguments and returns a calculated timeout (as float or int). Passed type: < %s > is not of any of these, and cannot be converted to a float.' %( timeout.__class__.__name__, ))
-
-
-    if not allowOverride and not isTimeoutAFunction:
-        # Only defaultTimeout provided. Simple function wrapper
-        def _function_decorator(func):
-
-            return wraps(func)(lambda *args, **kwargs : func_timeout(defaultTimeout, func, args=args, kwargs=kwargs))
-
-#            def _function_wrapper(*args, **kwargs):
-#                return func_timeout(defaultTimeout, func, args=args, kwargs=kwargs)
-#            return _function_wrapper
-        return _function_decorator
-
-    if not isTimeoutAFunction:
-        # allowOverride is True and timeout is not a function. Simple conditional on every call
-        def _function_decorator(func):
-            def _function_wrapper(*args, **kwargs):
-                if 'forceTimeout' in kwargs:
-                    useTimeout = kwargs.pop('forceTimeout')
-                else:
-                    useTimeout = defaultTimeout
-
-                return func_timeout(useTimeout, func, args=args, kwargs=kwargs)
-
-            return wraps(func)(_function_wrapper)
-        return _function_decorator
-
-
-    # At this point, timeout IS known to be a function.
-    timeoutFunction = timeout
-
-    if allowOverride:
-        # Could use a lambda here... but want traceback to highlight the calculate function,
-        #  and not the invoked function
-        def _function_decorator(func):
-            def _function_wrapper(*args, **kwargs):
-                if 'forceTimeout' in kwargs:
-                    useTimeout = kwargs.pop('forceTimeout')
-                else:
-                    useTimeout = timeoutFunction(*args, **kwargs)
-
-                return func_timeout(useTimeout, func, args=args, kwargs=kwargs)
-
-            return wraps(func)(_function_wrapper)
-        return _function_decorator
-
-    # Cannot override, and calculate timeout function
-    def _function_decorator(func):
-        def _function_wrapper(*args, **kwargs):
-            useTimeout = timeoutFunction(*args, **kwargs)
-
-            return func_timeout(useTimeout, func, args=args, kwargs=kwargs)
-
-        return wraps(func)(_function_wrapper)
-    return _function_decorator
-
-
-# vim: set ts=4 sw=4 expandtab :
+
+# vim: set ts=4 sw=4 expandtab :
+
+'''
+    Copyright (c) 2016, 2017 Tim Savannah All Rights Reserved.
+
+    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
+    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
+'''
+
+import copy
+import inspect
+import threading
+import time
+import types
+import sys
+
+from .exceptions import FunctionTimedOut
+from .StoppableThread import StoppableThread
+
+
+from .py3_raise import raise_exception
+
+
+from functools import wraps
+
+__all__ = ('func_timeout', 'func_set_timeout')
+
+
+def func_timeout(timeout, func, args=(), kwargs=None):
+    '''
+        func_timeout - Runs the given function for up to #timeout# seconds.
+
+        Raises any exceptions #func# would raise, returns what #func# would return (unless timeout is exceeded), in which case it raises FunctionTimedOut
+
+        @param timeout <float> - Maximum number of seconds to run #func# before terminating
+
+        @param func <function> - The function to call
+
+        @param args    <tuple> - Any ordered arguments to pass to the function
+
+        @param kwargs  <dict/None> - Keyword arguments to pass to the function.
+
+
+        @raises - FunctionTimedOut if #timeout# is exceeded, otherwise anything #func# could raise will be raised
+
+        If the timeout is exceeded, FunctionTimedOut will be raised within the context of the called function every two seconds until it terminates,
+        but will not block the calling thread (a new thread will be created to perform the join). If possible, you should try/except FunctionTimedOut
+        to return cleanly, but in most cases it will 'just work'.
+
+        @return - The return value that #func# gives
+    '''
+
+    if not kwargs:
+        kwargs = {}
+    if not args:
+        args = ()
+
+    ret = []
+    exception = []
+    isStopped = False
+
+    def funcwrap(args2, kwargs2):
+        try:
+            ret.append( func(*args2, **kwargs2) )
+        except FunctionTimedOut:
+            # Don't print traceback to stderr if we time out
+            pass
+        except BaseException as e:
+            exc_info = sys.exc_info()
+            if isStopped is False:
+                # Assemble the alternate traceback, excluding this function
+                #  from the trace (by going to next frame)
+                # Pytohn3 reads native from __traceback__,
+                # python2 has a different form for "raise"
+                e.__traceback__ = exc_info[2].tb_next
+                exception.append( e )
+
+    thread = StoppableThread(target=funcwrap, args=(args, kwargs))
+    thread.daemon = True
+
+    thread.start()
+    thread.join(timeout)
+
+    stopException = None
+    if thread.is_alive():
+        isStopped = True
+
+        class FunctionTimedOutTempType(FunctionTimedOut):
+            def __init__(self):
+                return FunctionTimedOut.__init__(self, '', timeout, func, args, kwargs)
+
+        FunctionTimedOutTemp = type('FunctionTimedOut' + str( hash( "%d_%d_%d_%d" %(id(timeout), id(func), id(args), id(kwargs))) ), FunctionTimedOutTempType.__bases__, dict(FunctionTimedOutTempType.__dict__))
+
+        stopException = FunctionTimedOutTemp
+        # raise FunctionTimedOut('', timeout, func, args, kwargs)
+        thread._stopThread(stopException)
+        thread.join(min(.1, timeout / 50.0))
+        raise FunctionTimedOut('', timeout, func, args, kwargs)
+    else:
+        # We can still cleanup the thread here..
+        # Still give a timeout... just... cuz..
+        thread.join(.5)
+
+    if exception:
+        raise_exception(exception)
+
+    if ret:
+        return ret[0]
+
+
+def func_set_timeout(timeout, allowOverride=False):
+    '''
+        func_set_timeout - Decorator to run a function with a given/calculated timeout (max execution time).
+            Optionally (if #allowOverride is True), adds a paramater, "forceTimeout", to the
+            function which, if provided, will override the default timeout for that invocation.
+
+            If #timeout is provided as a lambda/function, it will be called
+              prior to each invocation of the decorated function to calculate the timeout to be used
+              for that call, based on the arguments passed to the decorated function.
+
+              For example, you may have a "processData" function whose execution time
+              depends on the number of "data" elements, so you may want a million elements to have a
+              much higher timeout than seven elements.)
+
+            If #allowOverride is True AND a kwarg of "forceTimeout" is passed to the wrapped function, that timeout
+             will be used for that single call.
+
+        @param timeout <float OR lambda/function> -
+
+            **If float:**
+                Default number of seconds max to allow function to execute
+                  before throwing FunctionTimedOut
+
+            **If lambda/function:
+
+                 If a function/lambda is provided, it will be called for every
+                  invocation of the decorated function (unless #allowOverride=True and "forceTimeout" was passed)
+                  to determine the timeout to use based on the arguments to the decorated function.
+
+                    The arguments as passed into the decorated function will be passed to this function.
+                     They either must match exactly to what the decorated function has, OR
+                      if you prefer to get the *args (list of ordered args) and **kwargs ( key : value  keyword args form),
+                      define your calculate function like:
+
+                        def calculateTimeout(*args, **kwargs):
+                            ...
+
+                      or lambda like:
+
+                        calculateTimeout = lambda *args, **kwargs : ...
+
+                    otherwise the args to your calculate function should match exactly the decorated function.
+
+
+        @param allowOverride <bool> Default False, if True adds a keyword argument to the decorated function,
+            "forceTimeout" which, if provided, will override the #timeout. If #timeout was provided as a lambda / function, it
+             will not be called.
+
+        @throws FunctionTimedOut If time alloted passes without function returning naturally
+
+        @see func_timeout
+    '''
+    # Try to be as efficent as possible... don't compare the args more than once
+
+    #  Helps closure issue on some versions of python
+    defaultTimeout = copy.copy(timeout)
+
+    isTimeoutAFunction = bool( issubclass(timeout.__class__, (types.FunctionType, types.MethodType, types.LambdaType, types.BuiltinFunctionType, types.BuiltinMethodType) ) )
+
+    if not isTimeoutAFunction:
+        if not issubclass(timeout.__class__, (float, int)):
+            try:
+                timeout = float(timeout)
+            except:
+                raise ValueError('timeout argument must be a float/int for number of seconds, or a function/lambda which gets passed the function arguments and returns a calculated timeout (as float or int). Passed type: < %s > is not of any of these, and cannot be converted to a float.' %( timeout.__class__.__name__, ))
+
+
+    if not allowOverride and not isTimeoutAFunction:
+        # Only defaultTimeout provided. Simple function wrapper
+        def _function_decorator(func):
+
+            return wraps(func)(lambda *args, **kwargs : func_timeout(defaultTimeout, func, args=args, kwargs=kwargs))
+
+#            def _function_wrapper(*args, **kwargs):
+#                return func_timeout(defaultTimeout, func, args=args, kwargs=kwargs)
+#            return _function_wrapper
+        return _function_decorator
+
+    if not isTimeoutAFunction:
+        # allowOverride is True and timeout is not a function. Simple conditional on every call
+        def _function_decorator(func):
+            def _function_wrapper(*args, **kwargs):
+                if 'forceTimeout' in kwargs:
+                    useTimeout = kwargs.pop('forceTimeout')
+                else:
+                    useTimeout = defaultTimeout
+
+                return func_timeout(useTimeout, func, args=args, kwargs=kwargs)
+
+            return wraps(func)(_function_wrapper)
+        return _function_decorator
+
+
+    # At this point, timeout IS known to be a function.
+    timeoutFunction = timeout
+
+    if allowOverride:
+        # Could use a lambda here... but want traceback to highlight the calculate function,
+        #  and not the invoked function
+        def _function_decorator(func):
+            def _function_wrapper(*args, **kwargs):
+                if 'forceTimeout' in kwargs:
+                    useTimeout = kwargs.pop('forceTimeout')
+                else:
+                    useTimeout = timeoutFunction(*args, **kwargs)
+
+                return func_timeout(useTimeout, func, args=args, kwargs=kwargs)
+
+            return wraps(func)(_function_wrapper)
+        return _function_decorator
+
+    # Cannot override, and calculate timeout function
+    def _function_decorator(func):
+        def _function_wrapper(*args, **kwargs):
+            useTimeout = timeoutFunction(*args, **kwargs)
+
+            return func_timeout(useTimeout, func, args=args, kwargs=kwargs)
+
+        return wraps(func)(_function_wrapper)
+    return _function_decorator
+
+
+# vim: set ts=4 sw=4 expandtab :
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py

 * *Ordering differences only*

```diff
@@ -1,98 +1,98 @@
-'''
-    Copyright (c) 2016 Tim Savannah All Rights Reserved.
-
-    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
-    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
-'''
-
-__all__ = ('FunctionTimedOut', 'RETRY_SAME_TIMEOUT')
-
-RETRY_SAME_TIMEOUT = 'RETRY_SAME_TIMEOUT'
-
-class FunctionTimedOut(BaseException):
-    '''
-        FunctionTimedOut - Exception raised when a function times out
-
-        @property timedOutAfter - Number of seconds before timeout was triggered
-
-        @property timedOutFunction - Function called which timed out
-        @property timedOutArgs - Ordered args to function
-        @property timedOutKwargs - Keyword args to function
-
-        @method retry - Retries the function with same arguments, with option to run with original timeout, no timeout, or a different
-          explicit timeout. @see FunctionTimedOut.retry
-    '''
-
-
-    def __init__(self, msg='', timedOutAfter=None, timedOutFunction=None, timedOutArgs=None, timedOutKwargs=None):
-        '''
-            __init__ - Create this exception type.
-
-                You should not need to do this outside of testing, it will be created by the func_timeout API
-
-                    @param msg <str> - A predefined message, otherwise we will attempt to generate one from the other arguments.
-
-                    @param timedOutAfter <None/float> - Number of seconds before timing-out. Filled-in by API, None will produce "Unknown"
-
-                    @param timedOutFunction <None/function> - Reference to the function that timed-out. Filled-in by API." None will produce "Unknown Function"
-
-                    @param timedOutArgs <None/tuple/list> - List of fixed-order arguments ( *args ), or None for no args.
-
-                    @param timedOutKwargs <None/dict> - Dict of keyword arg ( **kwargs ) names to values, or None for no kwargs.
-
-        '''
-
-        self.timedOutAfter = timedOutAfter
-
-        self.timedOutFunction = timedOutFunction
-        self.timedOutArgs = timedOutArgs
-        self.timedOutKwargs = timedOutKwargs
-
-        if not msg:
-            msg = self.getMsg()
-
-        BaseException.__init__(self, msg)
-
-        self.msg = msg
-
-
-    def getMsg(self):
-        '''
-            getMsg - Generate a default message based on parameters to FunctionTimedOut exception'
-
-            @return <str> - Message
-        '''
-        # Try to gather the function name, if available.
-        # If it is not, default to an "unknown" string to allow default instantiation
-        if self.timedOutFunction is not None:
-            timedOutFuncName = self.timedOutFunction.__name__
-        else:
-            timedOutFuncName = 'Unknown Function'
-        if self.timedOutAfter is not None:
-            timedOutAfterStr = "%f" %(self.timedOutAfter, )
-        else:
-            timedOutAfterStr = "Unknown"
-
-        return 'Function %s (args=%s) (kwargs=%s) timed out after %s seconds.\n' %(timedOutFuncName, repr(self.timedOutArgs), repr(self.timedOutKwargs), timedOutAfterStr)
-
-    def retry(self, timeout=RETRY_SAME_TIMEOUT):
-        '''
-            retry - Retry the timed-out function with same arguments.
-
-            @param timeout <float/RETRY_SAME_TIMEOUT/None> Default RETRY_SAME_TIMEOUT
-
-                If RETRY_SAME_TIMEOUT : Will retry the function same args, same timeout
-                If a float/int : Will retry the function same args with provided timeout
-                If None : Will retry function same args no timeout
-
-            @return - Returnval from function
-        '''
-        if timeout is None:
-            return self.timedOutFunction(*(self.timedOutArgs), **self.timedOutKwargs)
-
-        from .dafunc import func_timeout
-
-        if timeout == RETRY_SAME_TIMEOUT:
-            timeout = self.timedOutAfter
-
-        return func_timeout(timeout, self.timedOutFunction, args=self.timedOutArgs, kwargs=self.timedOutKwargs)
+'''
+    Copyright (c) 2016 Tim Savannah All Rights Reserved.
+
+    Licensed under the Lesser GNU Public License Version 3, LGPLv3. You should have recieved a copy of this with the source distribution as
+    LICENSE, otherwise it is available at https://github.com/kata198/func_timeout/LICENSE
+'''
+
+__all__ = ('FunctionTimedOut', 'RETRY_SAME_TIMEOUT')
+
+RETRY_SAME_TIMEOUT = 'RETRY_SAME_TIMEOUT'
+
+class FunctionTimedOut(BaseException):
+    '''
+        FunctionTimedOut - Exception raised when a function times out
+
+        @property timedOutAfter - Number of seconds before timeout was triggered
+
+        @property timedOutFunction - Function called which timed out
+        @property timedOutArgs - Ordered args to function
+        @property timedOutKwargs - Keyword args to function
+
+        @method retry - Retries the function with same arguments, with option to run with original timeout, no timeout, or a different
+          explicit timeout. @see FunctionTimedOut.retry
+    '''
+
+
+    def __init__(self, msg='', timedOutAfter=None, timedOutFunction=None, timedOutArgs=None, timedOutKwargs=None):
+        '''
+            __init__ - Create this exception type.
+
+                You should not need to do this outside of testing, it will be created by the func_timeout API
+
+                    @param msg <str> - A predefined message, otherwise we will attempt to generate one from the other arguments.
+
+                    @param timedOutAfter <None/float> - Number of seconds before timing-out. Filled-in by API, None will produce "Unknown"
+
+                    @param timedOutFunction <None/function> - Reference to the function that timed-out. Filled-in by API." None will produce "Unknown Function"
+
+                    @param timedOutArgs <None/tuple/list> - List of fixed-order arguments ( *args ), or None for no args.
+
+                    @param timedOutKwargs <None/dict> - Dict of keyword arg ( **kwargs ) names to values, or None for no kwargs.
+
+        '''
+
+        self.timedOutAfter = timedOutAfter
+
+        self.timedOutFunction = timedOutFunction
+        self.timedOutArgs = timedOutArgs
+        self.timedOutKwargs = timedOutKwargs
+
+        if not msg:
+            msg = self.getMsg()
+
+        BaseException.__init__(self, msg)
+
+        self.msg = msg
+
+
+    def getMsg(self):
+        '''
+            getMsg - Generate a default message based on parameters to FunctionTimedOut exception'
+
+            @return <str> - Message
+        '''
+        # Try to gather the function name, if available.
+        # If it is not, default to an "unknown" string to allow default instantiation
+        if self.timedOutFunction is not None:
+            timedOutFuncName = self.timedOutFunction.__name__
+        else:
+            timedOutFuncName = 'Unknown Function'
+        if self.timedOutAfter is not None:
+            timedOutAfterStr = "%f" %(self.timedOutAfter, )
+        else:
+            timedOutAfterStr = "Unknown"
+
+        return 'Function %s (args=%s) (kwargs=%s) timed out after %s seconds.\n' %(timedOutFuncName, repr(self.timedOutArgs), repr(self.timedOutKwargs), timedOutAfterStr)
+
+    def retry(self, timeout=RETRY_SAME_TIMEOUT):
+        '''
+            retry - Retry the timed-out function with same arguments.
+
+            @param timeout <float/RETRY_SAME_TIMEOUT/None> Default RETRY_SAME_TIMEOUT
+
+                If RETRY_SAME_TIMEOUT : Will retry the function same args, same timeout
+                If a float/int : Will retry the function same args with provided timeout
+                If None : Will retry function same args no timeout
+
+            @return - Returnval from function
+        '''
+        if timeout is None:
+            return self.timedOutFunction(*(self.timedOutArgs), **self.timedOutKwargs)
+
+        from .dafunc import func_timeout
+
+        if timeout == RETRY_SAME_TIMEOUT:
+            timeout = self.timedOutAfter
+
+        return func_timeout(timeout, self.timedOutFunction, args=self.timedOutArgs, kwargs=self.timedOutKwargs)
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-
-
-# Python2 allows specifying an alternate traceback.
-def raise_exception(exception):
-    '''
-    raise exception[0] , None , exception[0].__traceback__  # noqa
-    '''
+
+
+# Python2 allows specifying an alternate traceback.
+def raise_exception(exception):
+    '''
+    raise exception[0] , None , exception[0].__traceback__  # noqa
+    '''
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-
-# PEP 409 - Raise with the chained exception context disabled
-#  This, in effect, prevents the "funcwrap" wrapper ( chained
-#   in context to an exception raised here, due to scope )
-# Only available in python3.3+
-def raise_exception(exception):
-    raise exception[0] from None
+
+# PEP 409 - Raise with the chained exception context disabled
+#  This, in effect, prevents the "funcwrap" wrapper ( chained
+#   in context to an exception raised here, due to scope )
+# Only available in python3.3+
+def raise_exception(exception):
+    raise exception[0] from None
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar 23 05:32:55 2023 UTC, .py size: 5246 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 87e4 1b64 7e14 0000  a..........d~...
+00000000: 610d 0d0a 0000 0000 506d 4a64 0315 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6403 5a04 4700  Z.d.d.l.Z.d.Z.G.
 00000050: 6404 6405 8400 6405 6503 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 4700 6406 6407 8400 6407 6503 6a05 8303  G.d.d...d.e.j...
 00000070: 5a07 6402 5300 2908 6131 0100 000a 2020  Z.d.S.).a1....
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar  9 04:50:23 2023 UTC, .py size: 587 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8f65 0964 4b02 0000  a........e.dK...
+00000000: 610d 0d0a 0000 0000 506d 4a64 5b02 0000  a.......PmJd[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 6405 6c04 6d05 5a05 0100 6404 6406 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 6d08 5a08 0100 6404 6407 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6408 5300 2909 612d 0100  m.Z...d.S.).a-..
 00000070: 000a 2020 2020 436f 7079 7269 6768 7420  ..    Copyright
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar 23 05:32:56 2023 UTC, .py size: 9297 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 88e4 1b64 5124 0000  a..........dQ$..
+00000000: 610d 0d0a 0000 0000 506d 4a64 3b25 0000  a.......PmJd;%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6403 6404 6c07 6d08 5a08 0100 6403  Z.d.d.l.m.Z...d.
 00000070: 6405 6c09 6d09 5a09 0100 6403 6406 6c0a  d.l.m.Z...d.d.l.
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar  9 04:14:50 2023 UTC, .py size: 3974 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3a5d 0964 860f 0000  a.......:].d....
+00000000: 610d 0d0a 0000 0000 506d 4a64 e80f 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 5a01 6402 5a02 4700 6403 6404  Z.d.Z.d.Z.G.d.d.
 00000040: 8400 6404 6503 8303 5a04 6405 5300 2906  ..d.e...Z.d.S.).
 00000050: 6121 0100 000a 2020 2020 436f 7079 7269  a!....    Copyri
 00000060: 6768 7420 2863 2920 3230 3136 2054 696d  ght (c) 2016 Tim
 00000070: 2053 6176 616e 6e61 6820 416c 6c20 5269   Savannah All Ri
```

## funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar  9 04:14:50 2023 UTC, .py size: 280 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3a5d 0964 1801 0000  a.......:].d....
+00000000: 610d 0d0a 0000 0000 506d 4a64 1f01 0000  a.......PmJd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 6401 8400 5a00 6402 5300 2903 6301 0000  d...Z.d.S.).c...
 00000040: 0000 0000 0000 0000 0001 0000 0002 0000  ................
 00000050: 0043 0000 0073 0e00 0000 7c00 6401 1900  .C...s....|.d...
 00000060: 6400 8202 6400 5300 2902 4ee9 0000 0000  d...d.S.).N.....
 00000070: a900 2901 da09 6578 6365 7074 696f 6e72  ..)...exceptionr
```

## funboost/utils/times/__init__.py

 * *Ordering differences only*

```diff
@@ -1,85 +1,85 @@
-import datetime
-import sys
-
-import arrow
-
-from .version import VERSION
-
-PY3 = sys.version_info[0] == 3
-if PY3:
-    string_types = str
-else:
-    string_types = basestring
-
-
-__author__ = 'Vincent Driessen <vincent@3rdcloud.com>'
-__version__ = VERSION
-
-
-def to_universal(local_dt, timezone=None):
-    """
-    Converts the given local datetime or UNIX timestamp to a universal
-    datetime.
-    """
-    if isinstance(local_dt, (int, float)):
-        if timezone is not None:
-            raise ValueError('Timezone argument illegal when using UNIX timestamps.')
-        return from_unix(local_dt)
-    elif isinstance(local_dt, string_types):
-        local_dt = arrow.get(local_dt).to('UTC').naive
-
-    return from_local(local_dt, timezone)
-
-
-def from_local(local_dt, timezone=None):
-    """Converts the given local datetime to a universal datetime."""
-    if not isinstance(local_dt, datetime.datetime):
-        raise TypeError('Expected a datetime object')
-
-    if timezone is None:
-        a = arrow.get(local_dt)
-    else:
-        a = arrow.get(local_dt, timezone)
-    return a.to('UTC').naive
-
-
-def from_unix(ut):
-    """
-    Converts a UNIX timestamp, as returned by `time.time()`, to universal
-    time.  Assumes the input is in UTC, as `time.time()` does.
-    """
-    if not isinstance(ut, (int, float)):
-        raise TypeError('Expected an int or float value')
-
-    return arrow.get(ut).naive
-
-
-def to_local(dt, timezone):
-    """Converts universal datetime to a local representation in given timezone."""
-    if dt.tzinfo is not None:
-        raise ValueError(
-            'First argument to to_local() should be a universal time.'
-        )
-    if not isinstance(timezone, string_types):
-        raise TypeError('expected a timezone name (string), but got {} instead'.format(type(timezone)))
-    return arrow.get(dt).to(timezone).datetime
-
-
-def to_unix(dt):
-    """Converts a datetime object to unixtime"""
-    if not isinstance(dt, datetime.datetime):
-        raise TypeError('Expected a datetime object')
-
-    return arrow.get(dt).timestamp
-
-
-def format(dt, timezone, fmt=None):
-    """Formats the given universal time for display in the given time zone."""
-    local = to_local(dt, timezone)
-    if fmt is None:
-        return local.isoformat()
-    else:
-        return local.strftime(fmt)
-
-
-now = datetime.datetime.utcnow
+import datetime
+import sys
+
+import arrow
+
+from .version import VERSION
+
+PY3 = sys.version_info[0] == 3
+if PY3:
+    string_types = str
+else:
+    string_types = basestring
+
+
+__author__ = 'Vincent Driessen <vincent@3rdcloud.com>'
+__version__ = VERSION
+
+
+def to_universal(local_dt, timezone=None):
+    """
+    Converts the given local datetime or UNIX timestamp to a universal
+    datetime.
+    """
+    if isinstance(local_dt, (int, float)):
+        if timezone is not None:
+            raise ValueError('Timezone argument illegal when using UNIX timestamps.')
+        return from_unix(local_dt)
+    elif isinstance(local_dt, string_types):
+        local_dt = arrow.get(local_dt).to('UTC').naive
+
+    return from_local(local_dt, timezone)
+
+
+def from_local(local_dt, timezone=None):
+    """Converts the given local datetime to a universal datetime."""
+    if not isinstance(local_dt, datetime.datetime):
+        raise TypeError('Expected a datetime object')
+
+    if timezone is None:
+        a = arrow.get(local_dt)
+    else:
+        a = arrow.get(local_dt, timezone)
+    return a.to('UTC').naive
+
+
+def from_unix(ut):
+    """
+    Converts a UNIX timestamp, as returned by `time.time()`, to universal
+    time.  Assumes the input is in UTC, as `time.time()` does.
+    """
+    if not isinstance(ut, (int, float)):
+        raise TypeError('Expected an int or float value')
+
+    return arrow.get(ut).naive
+
+
+def to_local(dt, timezone):
+    """Converts universal datetime to a local representation in given timezone."""
+    if dt.tzinfo is not None:
+        raise ValueError(
+            'First argument to to_local() should be a universal time.'
+        )
+    if not isinstance(timezone, string_types):
+        raise TypeError('expected a timezone name (string), but got {} instead'.format(type(timezone)))
+    return arrow.get(dt).to(timezone).datetime
+
+
+def to_unix(dt):
+    """Converts a datetime object to unixtime"""
+    if not isinstance(dt, datetime.datetime):
+        raise TypeError('Expected a datetime object')
+
+    return arrow.get(dt).timestamp
+
+
+def format(dt, timezone, fmt=None):
+    """Formats the given universal time for display in the given time zone."""
+    local = to_local(dt, timezone)
+    if fmt is None:
+        return local.isoformat()
+    else:
+        return local.strftime(fmt)
+
+
+now = datetime.datetime.utcnow
```

## funboost/utils/times/version.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-VERSION = '0.7'
+VERSION = '0.7'
```

## Comparing `funboost-23.3.dist-info/LICENSE` & `funboost-23.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-23.3.dist-info/METADATA` & `funboost-23.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 23.3
+Version: 23.4
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -438,8 +438,7 @@
 ```
 
 [查看分布式函数调度框架完整文档](https://funboost.readthedocs.io/zh/latest/index.html)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=distributed_framework)
 
 <div> </div>
-
```

## Comparing `funboost-23.3.dist-info/RECORD` & `funboost-23.4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-funboost/__init__.py,sha256=b0QCToD6xthLiftBpMU5u_ISXKA4oDe0k_yJAtteD7E,2341
+funboost/__init__.py,sha256=eBTjiQBcy0DoDZiOdcRJpgb5RHwv8d1ekgVwDkhoHoc,2402
 funboost/__init__old.py,sha256=cSzw-ZQqtAAp5_-7eONXQT5fwz_JbZlRjDQPASDLUHk,20378
-funboost/constant.py,sha256=X_foUR_tggz8VO_-9z3egC191fBPiq2XxSe1p1ftSkc,6261
-funboost/funboost_config_deafult.py,sha256=CSawbw5Yzkk73wMNOxhxkrkncS-OOSEYismtbK547xA,7358
+funboost/constant.py,sha256=tSdHQ8nrZH63jOKKZFtOfTo2melCsiMrk-O1lFcsIKA,6489
+funboost/funboost_config_deafult.py,sha256=xpmiZBCVylJe4pC4fG2J-LZZ0c0QJsYXOM1YxQMcMtw,7399
 funboost/set_frame_config.py,sha256=hz_38C-IXEulYpHQdr1fhsMcdEDCHIsF2la8MkHiIjA,9149
 funboost/assist/celery_helper.py,sha256=YvKP21xUzgazZHeFGq4FTgtd0A1g3BGNWzKLQ3gNygc,4186
 funboost/assist/dramatiq_helper.py,sha256=lRNouO8MyCB_Qj2ppYG4FbMpf-2Aok8QhtGZLH1zWkg,2089
 funboost/assist/huey_helper.py,sha256=VEzMdQDVJJ-ujcOXKw7chrTgvieLz4si3hrjt8gIK38,1760
 funboost/assist/rq_helper.py,sha256=-tUZ00FzkczwBAkbbISPHF-8J0K7HLSZsue39WiF-cM,1509
 funboost/assist/rq_windows_worker.py,sha256=jQlGmU0FWPVoKVP8cyuwTuAca9VfSd75F5Qw_hR04y0,4831
 funboost/beggar_version_implementation/beggar_redis_consumer.py,sha256=aiucCkj7-GWbLMIWHhevdQrAsxzyc55AL69fue8esYs,3930
@@ -22,15 +22,15 @@
 funboost/concurrent_pool/custom_threadpool_executor000.py,sha256=jJLXy3h-bELap6nZA6yLtdozzTWcvCtZ7IY6MTqLEAM,9317
 funboost/concurrent_pool/single_thread_executor.py,sha256=NDWOegh8Nxpb-Bp-lUlj-DONWvepSmA9qepL1yNgdQI,373
 funboost/concurrent_pool/backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/concurrent_pool/backup/async_pool_executor0223.py,sha256=iTxxJFk2lu1P9ZAIkBip3euq3oEQ4_qTODy3xUaOecY,9548
 funboost/concurrent_pool/backup/async_pool_executor_back.py,sha256=vIgUUyF4Zb0jIRPWgNPqyO09YEkQP32kkpGBldqm4qA,9568
 funboost/concurrent_pool/backup/async_pool_executor_janus.py,sha256=OHMWJ9l3EYTpPpcrPrGGKd4K0tmQ2PN8HiX0Dta0EOo,5728
 funboost/consumers/__init__.py,sha256=ZXY_6Kut1VYNQiF5aWEgIWobsW1ht9YUP0TdRZRWFqI,126
-funboost/consumers/base_consumer.py,sha256=G-hmhk6H0F7tbKrwkXSUv1n37J1LXJ_yTffaPMfrJ50,82870
+funboost/consumers/base_consumer.py,sha256=oIA1IiXL8SADzxpxCeoGIq1QJg7FB0LVfkYbzBX1CDM,85359
 funboost/consumers/celery_consumer.py,sha256=6CqorZH5pbxIjVwn5gNzcxSbos5YWT8eYqxYyYjgUcY,7574
 funboost/consumers/celery_consumer000.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
 funboost/consumers/confirm_mixin.py,sha256=oVBQ1RayIBFOzGNTJ69HdBR_kLd46xd0VfCOKfqDpLA,6033
 funboost/consumers/dramatiq_consumer.py,sha256=kiHM1wpSZykYDomtSGZ2PlMInCDn_8GOGEHqHUD9m0o,2144
 funboost/consumers/http_consumer.py,sha256=3HF8tsH90fUPX3iOmVid_nqW_7hZCFaL7feOkuAM36U,2025
 funboost/consumers/http_consumer000.py,sha256=NXOSiN1qpLAJfJkuF6SjFpWQ28YxMDULzWCBTNMwYe8,4463
 funboost/consumers/httpsqs_consumer.py,sha256=LICZzovaMVrZsJY4GgLrk3EaHz8f9ZZBLKZtWl3frMc,1080
@@ -67,60 +67,59 @@
 funboost/consumers/udp_consumer.py,sha256=J-G1ZYktXZ_er_1fg3FdSPVl4V_eEIHZXlBadCNpJmE,1643
 funboost/consumers/zeromq_consumer.py,sha256=7V1RwZKtPDDpjKTKj4GWGuz1AGZ83EBHCnWuYN4ooSM,4157
 funboost/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/contrib/queue2queue.py,sha256=I6e1d2s_TQ_29rbwSs3KuA7Tuj9B905EcJruT287CnM,4680
 funboost/contrib/redis_consume_latest_msg_broker.py,sha256=V-8-pOyotOXNbs2olS7vig-yN1PxRdw_MeLOtpUufJc,1817
 funboost/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/core/active_cousumer_info_getter.py,sha256=VwVRxsApdKqnoBdg1PsHEkyWiOFJMm0_qWIdCFbPOWg,4984
-funboost/core/booster.py,sha256=4uMrOpS_nsBVZDmPoJUJV_lcl1t-JGBotRXXrjK2kdY,16372
+funboost/core/booster.py,sha256=9jqNczG36-bEs9x708PHWqsugk5Y0gjOZcPO_zq3kmU,16688
 funboost/core/exit_signal.py,sha256=GDP3si_hNm7-iNZeeRaON62He47j_jX5weOOsDYW68Y,576
 funboost/core/fabric_deploy_helper.py,sha256=yIdWhlJAR1rCpzvcSme-KrU7RwKH8B7tdwHG-q6QH0U,8875
 funboost/core/function_result_status_config.py,sha256=CE7xaGoL7vT2VsLTHvv-EnJE7K83XVWivBimHVmVfnQ,1570
-funboost/core/function_result_status_saver.py,sha256=6dMLpa74t3zsHF20lqfgAdCeRD1yc1oJcw--Usk-A3c,8819
+funboost/core/function_result_status_saver.py,sha256=tNYRvUfb2T59mda9fLWDftbPbLvyKQg7Sph6BTBy_J4,8886
 funboost/core/get_booster.py,sha256=YlImXa5yjvuON_9JOa2yAlPw0tHj7RET5jBjmbj1gcM,1169
 funboost/core/global_boosters.py,sha256=CDrnKhxEEb-GxTL7JhrDTD1tyhLj7ciAtO1Cy2iyi1Q,340
-funboost/core/helper_funs.py,sha256=JDIawL6BWViC37rOJ9gFS8f4vCaispiA8Y7Zch-VM_o,1193
+funboost/core/helper_funs.py,sha256=SKSMKytJTOFQJsuMKWJ-_mQg6e_Bgpq1ANDzjjBAcio,1192
+funboost/core/kill_remote_task.py,sha256=jLvwcEDEQ0n0MBVB8oV8nki1yuCMg5bM2yAV-udUFFE,5388
 funboost/core/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
 funboost/core/muliti_process_enhance.py,sha256=zNodv3Ww5yCmwO6xCh7k8HntFHjIYYJ9EPaGinvPV9Q,3814
 funboost/factories/__init__.py,sha256=s7kKKjR1HU5eMjPD6r5b-SXTVMo1zBp2JjOAtkyt5Yo,178
-funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=00VqI85iEh566n_Zb6hs4QFtPzR3ZAejT-gXJFiYbbI,8976
+funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=Ig1Kze8keS04_vXMNenZSDxibBSjxVrcMkDHviPsxnQ,8976
 funboost/factories/consumer_factory.py,sha256=KFvYkx1a7egtSiTLuVsoRMKLUAotx-QJX1jAI8Xzo3s,946
 funboost/factories/publisher_factotry.py,sha256=Vz66GrCxMt7GV5iqyIXSzZcC_eHF8fj-2kYduzbTTpg,2281
 funboost/function_result_web/app.py,sha256=xUSDBwwDA5wQVWFdFBXj9Y1s7BOh2itUw5pCZl0URMw,4841
 funboost/function_result_web/functions.py,sha256=OIPMxc4jv51qnhBxFGfTZnpMx5p4lQflPoTviDTbJUc,7345
-funboost/function_result_web/__pycache__/app.cpython-37.pyc,sha256=p-jwU7xf31KOJhmhNXqj6J79PTxjMbiTU16gAotpSEw,4045
-funboost/function_result_web/__pycache__/functions.cpython-37.pyc,sha256=KuU8DnYhFpYN0p9rdDXE9mqFuE7eKkcXHCNze3aAdOw,3921
 funboost/function_result_web/static/assets/css/custom.css,sha256=3brvjy2aBOTIXcTUK4NV6dX5wFRqx6K2aLu_jQn63jM,7674
 funboost/function_result_web/static/assets/css/jquery.mCustomScrollbar.min.css,sha256=JHGEmB629pipTkMag9aMaw32I8zle24p3FpsEeI6oZU,42839
 funboost/function_result_web/static/assets/img/user.jpg,sha256=Vz1A99gho-0bKV67Pt2s_zT25mWhNcPe0mWG-0mRl9U,23610
 funboost/function_result_web/static/assets/js/custom.js,sha256=-BDtMX9tRvSFkJr6654cQd4rIYxasI1uA0TGlB8xzZs,1106
 funboost/function_result_web/static/assets/js/jquery.mCustomScrollbar.concat.min.js,sha256=WrXxn5vUpN3PFCNfwWhO7-fPv7wz8KH85mGxPeQwkr4,45483
 funboost/function_result_web/static/css/style.css,sha256=780a8qm6IrrbawetpIGDp3l8BUoSQvD1R86_BGAhhbU,11065
 funboost/function_result_web/static/images/bg.jpg,sha256=qOk3I6ElZHnigPWaIk_Qq_SCNAdi8N5OI_hdNiIhNXQ,1153168
 funboost/function_result_web/static/images/password.png,sha256=0jRivuQAhWKtkS73p8f_KiLy3D39_flqVTrpFKJPNqk,546
 funboost/function_result_web/static/images/tick.png,sha256=S9dZYN4HQzw7JsWPw3ut1dQp4OTJ_Uh2Qp2KUDF1Jv8,2912
 funboost/function_result_web/static/images/user.png,sha256=HxLjNc83WZzZEscZRdmVhGKlPXNdp_EKmmYxafuyb3g,622
 funboost/function_result_web/static/js/jquery-1.11.0.min.js,sha256=ryQZ3RXgnqkTz-lNEw-YcEhnMuV3ZODwLqOEbyBBRu4,96383
 funboost/function_result_web/templates/index.html,sha256=dWe-JFQhsDpoNjSsBF4P6SJWp_KvHX8EP_yECS5r7_o,19501
 funboost/function_result_web/templates/login.html,sha256=q37dj7O0LeyiV38Zd5P1Qn_qmhjdFomuYTRY1Yk48Bo,2007
 funboost/publishers/__init__.py,sha256=xqBHlvsJQVPfbdvP84G0LHmVB7-pFBS7vDnX1Uo9pVY,131
-funboost/publishers/base_publisher.py,sha256=2eLwOgi6TnuGTRzQmaB7dXg5q52Cl1_10xd_CeXGujk,15844
-funboost/publishers/celery_publisher.py,sha256=ePnHIlO-XevW6zRvAgdnpQixiC5ogZsT0cNYeptcmCE,3073
+funboost/publishers/base_publisher.py,sha256=CU0xjCpt1tsQRcy6Orhuxd8bwsmIJ80wmMZw0JDHevY,15860
+funboost/publishers/celery_publisher.py,sha256=XCR-xvkHEQhbJSluuhrlMPv-V4RTlpA9Ot10mfe4a3E,3081
 funboost/publishers/celery_publisher000.py,sha256=ag2s7MzPPrnNdza3u8vcbDJqtiqbQw4lJJzAVuJ6GF0,3897
 funboost/publishers/confluent_kafka_publisher.py,sha256=cpbyWvZ0T_kM62LWeBKRUuEuMkJAKOof97UUMSz6-Dk,3541
 funboost/publishers/dramatiq_publisher.py,sha256=RoZzfvkS5H-XXcmHGBomuvkQRQBlVyiaCdWpgy0LL9o,1410
 funboost/publishers/http_publisher.py,sha256=pS3z_AVqH6h4PAgqB7usihvzLJP5ZzfPKQRMQfHrJHQ,753
 funboost/publishers/httpsqs_publisher.py,sha256=7cf5ijwrbp4smq6ofndrKisruAqG0Wzfo_d_7bnLUk4,2783
 funboost/publishers/huey_publisher.py,sha256=z1CF18YZkQY6lqeoc6tiJkaYsRjRicbhYYeoHSvdD-w,1101
 funboost/publishers/kafka_publisher.py,sha256=cmlJ0mvwq0Ajlth4VQqwnoe6v_bZ4eIz49GgkiJr-ZU,2160
 funboost/publishers/kombu_publisher.py,sha256=TJt24M_Y4x8wjXHFl2hp6z3Dat6rjuA_xGiqA8RbRLg,5321
 funboost/publishers/local_python_queue_publisher.py,sha256=veskMS5tjeneYU9HmrJLXZSK9_UT48NzHzcljjOoy3g,1365
 funboost/publishers/mongomq_publisher.py,sha256=xQr3KMQEKksX4OEvzPlCl8v1VeBHaoZtYw2QujOUyGo,1874
 funboost/publishers/mqtt_publisher.py,sha256=NKVDE5R12QL99IXgRjJtF4phyW8QaXKxHkqW5p_kXr4,3050
-funboost/publishers/nameko_publisher.py,sha256=k1XHZQgtRz0b9A22rLYrnGB5ghtDsq5MfMuqdk1Lqw0,1662
+funboost/publishers/nameko_publisher.py,sha256=2sqRe08mTjBlvnDe-mE55wFMxllzHCPKA4WtMABnKZ0,1670
 funboost/publishers/nats_publisher.py,sha256=hFfaQovij9dm8w-iRN0SgiHHoS_TlrTAjw42dPwCLSA,776
 funboost/publishers/nsq_publisher.py,sha256=Go4UjLd_Vt4JuVtfkmCuuXrmxUXv1y6NaBQJX6s1XUo,1302
 funboost/publishers/peewee_publisher.py,sha256=RsYAqBKf_ZLxkGJeZPWExzG4cpUac7weCeNhcSQ9hZc,1095
 funboost/publishers/persist_queue_publisher.py,sha256=x6qRiR3Ln-jX9KPC5GvBzUzAlmZ0HDjU1KTnILXVJrw,2540
 funboost/publishers/pulsar_publisher.py,sha256=3BqDtywExvTIw1KZWG4kT1uz029uw2YkntLggZ-Ao6A,1238
 funboost/publishers/rabbitmq_amqpstorm_publisher.py,sha256=C32sQZpjv1iJtFDD6g_q0wI7Arw9i0RDsRVVOBRKzi4,3137
 funboost/publishers/rabbitmq_pika_publisher.py,sha256=jZZw3DUiZ4VqJ6FqZGdv7qo3F_ltzHuKsy_5-j4jkCs,2343
@@ -145,17 +144,18 @@
 funboost/timing_job/apscheduler_use_mysql_store.py,sha256=zIeK2LETm8m3VX7K6but8YAQOZomfO-P6AKLqeluxys,418
 funboost/timing_job/apscheduler_use_redis_store.py,sha256=zG2QSJYnDm6pgTwbyU3wvtr3GHKhlR9fonc5Fba1F5I,876
 funboost/utils/__init__.py,sha256=9YTXH5jt-_MulaWy5cbIpiJghy-fVQU9Gd1RHSajI94,1951
 funboost/utils/apscheduler_monkey.py,sha256=CcUISbqX6nMWSxr_QjZ26IvvhUk_ojYZWRaKenpsKfE,3124
 funboost/utils/block_exit.py,sha256=BnfxNYo3lnmhk686RAEoc4u3D4RU_iEMMMgu5L8gIuI,96
 funboost/utils/bulk_operation.py,sha256=jty8pvQWCPVUmfqeP6DnilveGc6YGjCMwVbnOAV4eRg,9972
 funboost/utils/custom_pysnooper.py,sha256=7yXLKEMY_JjPRRt0Y0N-wV2CFhILlYNh40Y6uRBUaj8,5923
-funboost/utils/decorators.py,sha256=vkshA4qHflg7G5xWuc6NcZyTKDMhS7ctGUZXlAeI_i4,24296
+funboost/utils/decorators.py,sha256=VNbWxlQzP8JkTuJdrv1-4GGWI9m9f7nhAvfkkszqrGA,24671
 funboost/utils/develop_log.py,sha256=f82JHBPBjdF_By5P_Ft4wMREeIHtF8MmqGFYa_pZbyA,251
-funboost/utils/kill_thread.py,sha256=qdqgFfWJjBimBLOKUQ0xDOn-H0AmmXIJM4_2NEUdaN8,2837
+funboost/utils/expire_lock.py,sha256=AOkd1KlvZeIwQaz8ZoKxLpGxWgqQ4mfNHcFphh04o8Q,4732
+funboost/utils/kill_thread.py,sha256=PPw1WQ1zZmINVgzGByMCj2aevFcHKB7KyrN9iyeJdGE,3412
 funboost/utils/mongo_util.py,sha256=9oAWgYMBdP1rqY2KySW_VEuEBq8Xdsf5lgml4484OzM,2984
 funboost/utils/monkey_color_log.py,sha256=QChhQMTB6phZ2eBaPq-9tFZF1n7pWeJgmJPIB_ugkvs,7367
 funboost/utils/monkey_patches.py,sha256=Q0_jKxOfFrSgrIDSuSZFrgNh6w_LRGaKAITghrIpEwI,2882
 funboost/utils/mqtt_util.py,sha256=BfCmyYwI-B8VL9499_IuYlJDCbv6ZhwyWThMf8dANOU,3199
 funboost/utils/paramiko_util.py,sha256=pu67zkgptqNSV9m2Lznezb3zF1AFYvkWJp_6DVKFSPU,4901
 funboost/utils/rabbitmq_factory.py,sha256=NPzTwG-INZG9aJgkzp-QVk3TgV0rjiuTVT5lmRT77zg,2963
 funboost/utils/redis_manager.py,sha256=2Hg9UT-X6nS5TkZ-YrTRxRK-WPHZaLOsuvTxYuD1cCc,4628
@@ -171,76 +171,50 @@
 funboost/utils/dependency_packages/mongomq/mongomq.py,sha256=A-_Y0OXmCqGHiCdOFWW4V0ciMyp6gIaPPVK95uaqd_k,7902
 funboost/utils/dependency_packages/mongomq/mongomq0000.py,sha256=DEZ_41VvmQD5eao5KOjF_s5_t-kso6zIsipFREm6ckY,7867
 funboost/utils/dependency_packages/mongomq/test.py,sha256=Tcmme3U3KXFSkdknO71bge4aLcWbZkTcyL5ufNZkco4,4811
 funboost/utils/dependency_packages/mongomq/utils.py,sha256=ljhcLhNf3yOc7IgnuRdFqLtwTGynRNd2uXZNRvStAL0,377
 funboost/utils/dependency_packages_in_pythonpath/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py,sha256=eOaK0Cr1yAmLcHhOM5-nV9XxXhQFZQkiaBECY65sFuc,341
 funboost/utils/dependency_packages_in_pythonpath/readme.md,sha256=fazVs-DBVTKan8X-2Jjqo5jxV4Abdaywj4SLzb_BLcA,814
-funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-37.pyc,sha256=Oy1-_q-VLcFLQ7RRp8B-fbBkNOb2SepePLYW4L5DQ6U,165
-funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc,sha256=sWX6OxFSOtD3N3H4ndWNS5xusjqwp54NNzddJ8dxMc0,475
-funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-37.pyc,sha256=Y9-hpQ_g0oRz3GWiUhB4GUW8rpxoQlQ4rQV17pPscLo,312
-funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc,sha256=KoT6tPC8DlM-7KwaYL3tNlnnd9PCjzYJK61JYuRTcKc,316
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py,sha256=DPdTb309wR_E5zR3RVoUYuR1jotheJL3PXdqNBHi2yg,1223
-funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py,sha256=o0SVW1qgNTAmKDAO6GoznN9EnibdgBB7XvLU49RXfeg,182652
-funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py,sha256=yplKtDh6CsO-sWqowLgyF5D3kwzcw7npEjlOGA3465k,183
-funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py,sha256=n_Z9ggf3AxW5fXvLEumEUA6gTtovytoXhMD1CWFk6tw,62239
-funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py,sha256=SOmdITVAwi5waYPiJa48YOxzUZQv184_6QD_wL0NCD8,1586
-funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py,sha256=CnB9LpvykAEXEdQyBEcgUU7iHxwNF3xuGzX7UYuUbiQ,11651
-funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py,sha256=qTxLRo5EqoHZIGqMguzLm90mtThBRYje_FaZz-fDbhg,427
+funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-39.pyc,sha256=3hoi1Y_c-4y78h666mYwuElx-QdC7R8WtjYQtn8xNzo,169
+funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc,sha256=xqlN_DIhqF6VSGZ5NVmXSD2UZhNbmdyM0B_tS1iDBVo,316
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py,sha256=J3gI6IwEN0nWEFTXZEpO7Xcw2oFEEWIy_DggeBiUjRI,1282
+funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py,sha256=HRzervUy2QlcMNSOfZJr30ZCC0o08X3aozKfXIUBCOY,187456
+funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py,sha256=p21NOSATlSQLWmMIiy11I-yGnbSb2cZ6Mn31JxnNei4,191
+funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py,sha256=d7sZla_PbT7nJQrSb3xtSfrNCI7RemUPfTCRZrsHjQM,63907
+funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py,sha256=3k0Nk-sSKiF5wU_1rSygc3_wYlZ8EpI5K3J_UQIHcnU,1682
+funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py,sha256=ylvjdSJl6RAjB2rY_Mq6hhyd1k2vF_EsH4cIehIfNKU,11957
+funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py,sha256=8f8NOEgWPXQvBFBJ-Sc2ZV11y0xx9y8-MpfM_x4JO4M,442
 funboost/utils/dependency_packages_in_pythonpath/aioredis/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md,sha256=BUZVchvn4henUdpA48IuF6SSSsnzdsMSff8l0MU4R2A,617
-funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py,sha256=ldPwRIOWVskKsItBwFqbqPfraMlFsGs42_ZDXtxza5U,12536
-funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py,sha256=90Dgj62Q9ABGVAwAPwufo3OKM2s0ws6LeQMZg8ifJb0,1284
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-311.pyc,sha256=PGpc0JrGU6UjKZ7WgxlpsCL2OuhJhWpE9WrxMHREtPc,1696
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-37.pyc,sha256=aKCGPo7i9v2xUiGebdBM06w7ZUcwnbZV2Xq0aPCiN4g,1272
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-39.pyc,sha256=4XwbdobWJgVOrdJ7fMJH2PiQM4B-Qm8_sCKH1DGGyi8,1208
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-311.pyc,sha256=0u-lJEwnkot6b2BDJIVL4WbTT3bym5n2QOsuVCewld8,238822
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-37.pyc,sha256=XEPgeY4Nwi3mdh94wLC6tJH8KjWZ9pVnTNrncaelPnQ,158582
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-39.pyc,sha256=wjxUkZih51SnrtAHWyYhZD1Z_jMa9OvBZLXHkSuyKaA,157873
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-311.pyc,sha256=PmG4dGsitvRfEp1NmL1VkXHH00D1CtFuEfInc1ECiwU,439
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-37.pyc,sha256=EqzTiVtVfotFy3QMnAnOxzfuFfK2iPv_FHXc14Pw9Rg,338
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-39.pyc,sha256=M1BnLliiDPk3Nwc1eBZwYY37TM5yo6a2_hnsTj3PwpE,342
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-311.pyc,sha256=59GzmrfW3YjWXbU4EYSrZJR1CU4FX-XlqoZmkjJmwiw,79446
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-37.pyc,sha256=OX0ujlOfU7fCg4Gjdh2yjV65KJm3nCEidHzvC9o_O1M,41714
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-39.pyc,sha256=31cVyJj5nyTDzml35fBmTPVRHQnTnTrhnK-O844-_Sc,42233
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-311.pyc,sha256=AZW20P5qRKwoXZmXsEzFeNRcMyGj48PXmzp2SWwtKUg,4280
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-37.pyc,sha256=aM5jObc-2kR-NMZ1BsoWmnkyNrzbJPTGxRwh6Nirl8s,3274
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-39.pyc,sha256=whw8BamPoqjNAt4IJ3mLY2dcCRt7vg0tYgEeCQzFzFM,3135
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-311.pyc,sha256=CPAHXDNMxcCsRl_iEYT-9yInKM0CloSxN2D2e1Dr1Lk,14348
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-37.pyc,sha256=LfwSKV3i9Vauewx-KKbmjZ7yzu0N2FBB0J9KjbGYAsE,10139
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-39.pyc,sha256=QtoJhsh-Nka2uFMYz6UVWqkxOrnCeLI_Jfaqotx8Kys,10198
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-311.pyc,sha256=l9RbPBAjUu3whHG4cOdbViCV7Kmjwq2U-YXwbVP6o4o,2926
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-37.pyc,sha256=TzdWPsHptgf4gjacx9gjwVw3749nbYHTQDmSWcajpyQ,1971
-funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-39.pyc,sha256=UyZJDglEyha0S4-6X4Jno7rAOPbXq6E-km0Fi_JnsJU,2017
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py,sha256=mvlE6n4bPDVem2cVBJLItEG_JEQhCogLjukFkJKF8c8,5246
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py,sha256=rnAnFnfFPy5_x3lw4xcRJ_fzjHZuxWrdLdVujqglHwg,587
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py,sha256=_eLe328DPJcHmKwjTwsazi7Hg9eNAYXopT35d_iGF0U,9297
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py,sha256=tUEaspemq_dS460EQvUMMSxeeyjIbgfEHIdxIC6ZhaU,3974
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py,sha256=9tpZLQ3-zIgU_ixazydwZmw8rFg7ybjI9alNYfSvwRk,169
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py,sha256=Odvg1FtXTEC--Ru1EIfsHASamBpOm9hdXY7OnlEUObA,280
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-311.pyc,sha256=p5cyFCQdCfGIlm8aTAIHqS0liMFAoadD_k26adyHXTo,6480
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-37.pyc,sha256=Fta8NkEzLOtLDgT5Ocol895uDx4-JwrfnLdnLouoJ4g,5063
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-39.pyc,sha256=b7vh_ZagGkh-37J89HLDCe9AFJdQ5uNYqjzADqp2TGw,5083
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-311.pyc,sha256=UBbUeoQg10pza2zo-5ELiOzE_Q-WclM1dafrFDRKZVs,857
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-37.pyc,sha256=ACdP5kS3R-5Bt2Qk-sq6RHF3LaOyywwVyM9R7L8m1-Q,763
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-39.pyc,sha256=5J3PkkFxVDKw4aFL59LwtJC5SDtteQT9ibIBR_1DkF8,767
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-311.pyc,sha256=Km9cH-VaZbCjtcRnCmZGkx7XupRT81jorraHlQ_UYQU,11443
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-37.pyc,sha256=9BDSFUqtY6nNXyULNlC5YgqU1jIC33FBwaQsGqglTQQ,8208
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-39.pyc,sha256=aYRhjAhdcweDRI_wlh1UU_tFnWHr9at5Ywz-p6tw0QI,8001
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-311.pyc,sha256=9v_YQPA5cUlVs-3UHbVwfiIE8UBzPD1HyWzApfBSR7Y,4592
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-37.pyc,sha256=UXQJRMqqUOpudiCLxFYM2RWF8JXerjUttXl6Fiw55OE,3708
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-39.pyc,sha256=xd7rk8scXgeE1EiNlHjeDmzlEa_DDeiX3tBVyFgDRuY,3732
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-311.pyc,sha256=i27JG81WYNUWCTqdYZLl5u-C7iPQbdxtzFFt_fRIsRE,357
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc,sha256=67Zqz4tjErzQSm9FM9mGaY3uMHYOUj3QYKtPqJQvQpE,303
-funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc,sha256=a1ajayGg3JjQz--IC3-6YQHRFStG9etoieY8mXEdJ6Q,311
+funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py,sha256=kDMNxjbm1s_hOOtjjLni8RoS003cVdm41jEPI4nbuCQ,12865
+funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py,sha256=KkQBFio0kQQeMTDLAr8INiFYuzC4UMowRtGvCl2Nw1s,1345
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-39.pyc,sha256=NnXOIpw-2Gegdjsl6SQYFWm4wi3z4FaDyDaH4u1KKI0,1208
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-39.pyc,sha256=7X3plofwsv5RIPhUE-sd4pKEgQZ41y9CwppBB2fqP0c,157873
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-39.pyc,sha256=cY1uALstkHOm--xJ5qIx-zT37DcejHTbUjOGd9hH6-M,342
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-39.pyc,sha256=xZQLxyc3yYd_cKUOkpRfbjTImNDrKukE_PU35Vn7Odg,42233
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-39.pyc,sha256=EL9HO-DGiUifKhsYJb1IhBXTkiPKYh_6tAOPgCrlzFc,3135
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-39.pyc,sha256=8toq_bQ96ifLGuoKqZAW4fG06lTBt31y7m3ZYB-ayXU,10198
+funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-39.pyc,sha256=1Qi5z-nd1F1LsWV6KVi2upaJ8NvfIhtYT5GVpjtgGlA,2017
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py,sha256=v15aAZDBtS42hDn4x5tjKBs6MGUKICztv0rUJ7aPcAQ,5379
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py,sha256=P3gPbNKNWi0P9ASJcFBnxsxiyII-3neM-FsVjwT_IeU,603
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py,sha256=iMNrcBHdXZ6jXDgdV5rczHF-Ld4MYFvEGYOnPDQms9A,9531
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py,sha256=ilz6xOeq-H0qspAraXfScQTBEQ8TME3i9FItDscm3H0,4072
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py,sha256=HS-jk-HqLm4jHK82bw8P_FmrrifAG8DAol_gEmIW6nE,176
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py,sha256=lrJ3yWuym8-rcQ_s___E5w7bzJ1dFGpXtmWo3RPpJoE,287
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-39.pyc,sha256=kvj4jhPh6HHMUw3aWdBImNa5T-vQyuu85ozqEjG4lSg,5083
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-39.pyc,sha256=m4vNDlsjMFuAOjmudVIWvyp_7Td0NlpjA_nRGZvPbQk,767
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-39.pyc,sha256=um1uluR-Wnwqj0qs0yucNGZXEhgiAJzn7uuhfd4tIwQ,8001
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-39.pyc,sha256=pzFmbSiuiYivY1RIUFOMXc12EJSIZc0gKO96KitxPoE,3732
+funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc,sha256=zE4fCYsao9dA1bC8aBT0fzYT8yTYuTQqMk9LFPClCyc,311
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
-funboost/utils/times/__init__.py,sha256=Y4bQD3SIA_E7W2YvHq2Qdi0dGM4H2DxyFNdDOuFOq1w,2417
-funboost/utils/times/version.py,sha256=11XfnZVVzOgIhXXdeN_mYfdXThfrsbQHpA0wCjz-hpg,17
-funboost-23.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-23.3.dist-info/METADATA,sha256=_tShdyF1bWkC8_jhJQyBBkloVBs1g9iLqLY3cXAd8j0,26616
-funboost-23.3.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-funboost-23.3.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-23.3.dist-info/RECORD,,
+funboost/utils/times/__init__.py,sha256=z-KQTxXapfu2ScJxISGe7QGffASuyJYL6JGsLXxD6O0,2332
+funboost/utils/times/version.py,sha256=JiZLGTB-HYyBOV4xS0rnx2K2OqVMTebUj30sZRbrleE,16
+funboost-23.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-23.4.dist-info/METADATA,sha256=7U8JVYTqu-PoU-TkMwN82y2eHK0fkqUni7YWcEmmnO8,26615
+funboost-23.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+funboost-23.4.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-23.4.dist-info/RECORD,,
```

