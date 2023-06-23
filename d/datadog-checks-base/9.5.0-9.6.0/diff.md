# Comparing `tmp/datadog_checks_base-9.5.0-py2.py3-none-any.whl.zip` & `tmp/datadog_checks_base-9.6.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,127 +1,134 @@
-Zip file size: 133122 bytes, number of entries: 125
+Zip file size: 140231 bytes, number of entries: 132
 -rw-rw-rw-  2.0 fat      172 b- defN 19-May-25 19:31 datadog_checks/__init__.py
--rw-rw-rw-  2.0 fat      190 b- defN 19-Aug-23 03:30 datadog_checks/config.py
--rw-rw-rw-  2.0 fat      149 b- defN 19-Aug-23 03:30 datadog_checks/errors.py
--rw-rw-rw-  2.0 fat      295 b- defN 19-Aug-23 03:30 datadog_checks/log.py
--rw-rw-rw-  2.0 fat      130 b- defN 19-Oct-22 23:48 datadog_checks/base/__about__.py
--rw-rw-rw-  2.0 fat      889 b- defN 19-Sep-29 22:03 datadog_checks/base/__init__.py
+-rw-rw-rw-  2.0 fat      190 b- defN 19-Nov-08 02:17 datadog_checks/config.py
+-rw-rw-rw-  2.0 fat      149 b- defN 19-Nov-08 02:17 datadog_checks/errors.py
+-rw-rw-rw-  2.0 fat      295 b- defN 19-Nov-08 02:17 datadog_checks/log.py
+-rw-rw-rw-  2.0 fat      135 b- defN 19-Nov-28 15:40 datadog_checks/base/__about__.py
+-rw-rw-rw-  2.0 fat      889 b- defN 19-Nov-08 02:17 datadog_checks/base/__init__.py
 -rw-rw-rw-  2.0 fat      556 b- defN 19-May-25 19:31 datadog_checks/base/config.py
 -rw-rw-rw-  2.0 fat      228 b- defN 19-May-25 19:31 datadog_checks/base/constants.py
--rw-rw-rw-  2.0 fat     4238 b- defN 19-Sep-03 18:41 datadog_checks/base/ddyaml.py
--rw-rw-rw-  2.0 fat      329 b- defN 19-Jun-05 22:17 datadog_checks/base/errors.py
--rw-rw-rw-  2.0 fat     3475 b- defN 19-Oct-01 04:40 datadog_checks/base/log.py
--rw-rw-rw-  2.0 fat      425 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/__init__.py
--rw-rw-rw-  2.0 fat    35126 b- defN 19-Oct-18 19:33 datadog_checks/base/checks/base.py
--rw-rw-rw-  2.0 fat     1960 b- defN 19-Oct-18 19:33 datadog_checks/base/checks/network.py
+-rw-rw-rw-  2.0 fat     4217 b- defN 19-Nov-09 13:26 datadog_checks/base/ddyaml.py
+-rw-rw-rw-  2.0 fat      329 b- defN 19-Nov-08 02:17 datadog_checks/base/errors.py
+-rw-rw-rw-  2.0 fat     3475 b- defN 19-Nov-08 02:17 datadog_checks/base/log.py
+-rw-rw-rw-  2.0 fat      425 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/__init__.py
+-rw-rw-rw-  2.0 fat    35688 b- defN 19-Nov-25 00:57 datadog_checks/base/checks/base.py
+-rw-rw-rw-  2.0 fat     1960 b- defN 19-Nov-08 18:27 datadog_checks/base/checks/network.py
 -rw-rw-rw-  2.0 fat      327 b- defN 19-May-25 19:31 datadog_checks/base/checks/kube_leader/__init__.py
--rw-rw-rw-  2.0 fat      700 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/kube_leader/base_check.py
--rw-rw-rw-  2.0 fat     4097 b- defN 19-May-25 19:31 datadog_checks/base/checks/kube_leader/mixins.py
+-rw-rw-rw-  2.0 fat      700 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/kube_leader/base_check.py
+-rw-rw-rw-  2.0 fat     4090 b- defN 19-Nov-09 13:26 datadog_checks/base/checks/kube_leader/mixins.py
 -rw-rw-rw-  2.0 fat     2715 b- defN 19-May-25 19:31 datadog_checks/base/checks/kube_leader/record.py
 -rw-rw-rw-  2.0 fat        0 b- defN 19-May-25 19:31 datadog_checks/base/checks/libs/__init__.py
--rw-rw-rw-  2.0 fat    24477 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/libs/thread_pool.py
--rw-rw-rw-  2.0 fat      577 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/libs/timer.py
+-rw-rw-rw-  2.0 fat    24477 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/libs/thread_pool.py
+-rw-rw-rw-  2.0 fat      577 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/libs/timer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 19-May-25 19:31 datadog_checks/base/checks/libs/vmware/__init__.py
--rw-rw-rw-  2.0 fat    73070 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/libs/vmware/all_metrics.py
--rw-rw-rw-  2.0 fat     3280 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/libs/vmware/basic_metrics.py
--rw-rw-rw-  2.0 fat      190 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/openmetrics/__init__.py
--rw-rw-rw-  2.0 fat     3405 b- defN 19-Oct-01 04:40 datadog_checks/base/checks/openmetrics/base_check.py
--rw-rw-rw-  2.0 fat    42842 b- defN 19-Oct-22 19:33 datadog_checks/base/checks/openmetrics/mixins.py
--rw-rw-rw-  2.0 fat      567 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/prometheus/__init__.py
--rw-rw-rw-  2.0 fat     8362 b- defN 19-Sep-03 18:41 datadog_checks/base/checks/prometheus/base_check.py
--rw-rw-rw-  2.0 fat    32355 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/prometheus/mixins.py
--rw-rw-rw-  2.0 fat     3903 b- defN 19-Sep-03 18:41 datadog_checks/base/checks/prometheus/prometheus_base.py
--rw-rw-rw-  2.0 fat      403 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/win/__init__.py
--rw-rw-rw-  2.0 fat    10811 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/win/winpdh.py
--rw-rw-rw-  2.0 fat     7294 b- defN 19-Jun-21 03:34 datadog_checks/base/checks/win/winpdh_base.py
--rw-rw-rw-  2.0 fat      388 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/win/winpdh_stub.py
--rw-rw-rw-  2.0 fat    12614 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/win/wmi/__init__.py
--rw-rw-rw-  2.0 fat     5767 b- defN 19-Jun-05 22:17 datadog_checks/base/checks/win/wmi/counter_type.py
--rw-rw-rw-  2.0 fat    18968 b- defN 19-Sep-03 18:41 datadog_checks/base/checks/win/wmi/sampler.py
--rw-rw-rw-  2.0 fat     1757 b- defN 19-Oct-20 15:15 datadog_checks/base/data/agent_requirements.in
--rw-rw-rw-  2.0 fat      223 b- defN 19-Jun-05 22:17 datadog_checks/base/stubs/__init__.py
+-rw-rw-rw-  2.0 fat    73070 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/libs/vmware/all_metrics.py
+-rw-rw-rw-  2.0 fat     3280 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/libs/vmware/basic_metrics.py
+-rw-rw-rw-  2.0 fat      190 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/openmetrics/__init__.py
+-rw-rw-rw-  2.0 fat     3891 b- defN 19-Nov-09 13:26 datadog_checks/base/checks/openmetrics/base_check.py
+-rw-rw-rw-  2.0 fat    42950 b- defN 19-Nov-28 15:39 datadog_checks/base/checks/openmetrics/mixins.py
+-rw-rw-rw-  2.0 fat      567 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/prometheus/__init__.py
+-rw-rw-rw-  2.0 fat     8362 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/prometheus/base_check.py
+-rw-rw-rw-  2.0 fat    32431 b- defN 19-Nov-28 15:39 datadog_checks/base/checks/prometheus/mixins.py
+-rw-rw-rw-  2.0 fat     3903 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/prometheus/prometheus_base.py
+-rw-rw-rw-  2.0 fat      403 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/win/__init__.py
+-rw-rw-rw-  2.0 fat    10792 b- defN 19-Nov-09 13:26 datadog_checks/base/checks/win/winpdh.py
+-rw-rw-rw-  2.0 fat     7294 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/win/winpdh_base.py
+-rw-rw-rw-  2.0 fat      388 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/win/winpdh_stub.py
+-rw-rw-rw-  2.0 fat    12614 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/win/wmi/__init__.py
+-rw-rw-rw-  2.0 fat     5767 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/win/wmi/counter_type.py
+-rw-rw-rw-  2.0 fat    18968 b- defN 19-Nov-08 02:17 datadog_checks/base/checks/win/wmi/sampler.py
+-rw-rw-rw-  2.0 fat     1795 b- defN 19-Nov-28 15:39 datadog_checks/base/data/agent_requirements.in
+-rw-rw-rw-  2.0 fat      264 b- defN 19-Nov-09 13:26 datadog_checks/base/stubs/__init__.py
 -rw-rw-rw-  2.0 fat     1169 b- defN 19-May-25 19:31 datadog_checks/base/stubs/_util.py
--rw-rw-rw-  2.0 fat    15907 b- defN 19-Oct-18 19:33 datadog_checks/base/stubs/aggregator.py
--rw-rw-rw-  2.0 fat      468 b- defN 19-Oct-18 19:33 datadog_checks/base/stubs/common.py
--rw-rw-rw-  2.0 fat      583 b- defN 19-Oct-18 19:33 datadog_checks/base/stubs/datadog_agent.py
--rw-rw-rw-  2.0 fat      828 b- defN 19-Oct-01 04:40 datadog_checks/base/stubs/log.py
--rw-rw-rw-  2.0 fat     5867 b- defN 19-Oct-18 19:33 datadog_checks/base/stubs/similar.py
--rw-rw-rw-  2.0 fat     1431 b- defN 19-Jun-05 22:17 datadog_checks/base/stubs/tagging.py
--rw-rw-rw-  2.0 fat      346 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/__init__.py
--rw-rw-rw-  2.0 fat     1964 b- defN 19-Oct-18 19:33 datadog_checks/base/utils/common.py
--rw-rw-rw-  2.0 fat      881 b- defN 19-May-25 19:31 datadog_checks/base/utils/containers.py
--rw-rw-rw-  2.0 fat     2780 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/date.py
--rw-rw-rw-  2.0 fat     1305 b- defN 19-Sep-03 18:41 datadog_checks/base/utils/headers.py
--rw-rw-rw-  2.0 fat    14229 b- defN 19-Oct-19 00:04 datadog_checks/base/utils/http.py
--rw-rw-rw-  2.0 fat     2559 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/limiter.py
--rw-rw-rw-  2.0 fat     2497 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/platform.py
+-rw-rw-rw-  2.0 fat    15907 b- defN 19-Nov-08 18:27 datadog_checks/base/stubs/aggregator.py
+-rw-rw-rw-  2.0 fat      468 b- defN 19-Nov-08 18:27 datadog_checks/base/stubs/common.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 19-Nov-09 13:26 datadog_checks/base/stubs/datadog_agent.py
+-rw-rw-rw-  2.0 fat      828 b- defN 19-Nov-08 02:17 datadog_checks/base/stubs/log.py
+-rw-rw-rw-  2.0 fat     5867 b- defN 19-Nov-08 18:27 datadog_checks/base/stubs/similar.py
+-rw-rw-rw-  2.0 fat     1431 b- defN 19-Nov-08 02:17 datadog_checks/base/stubs/tagging.py
+-rw-rw-rw-  2.0 fat      346 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/__init__.py
+-rw-rw-rw-  2.0 fat     2877 b- defN 19-Nov-09 13:26 datadog_checks/base/utils/common.py
+-rw-rw-rw-  2.0 fat      298 b- defN 19-Nov-25 00:57 datadog_checks/base/utils/constants.py
+-rw-rw-rw-  2.0 fat      881 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/containers.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/date.py
+-rw-rw-rw-  2.0 fat     1305 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/headers.py
+-rw-rw-rw-  2.0 fat    14440 b- defN 19-Nov-28 15:39 datadog_checks/base/utils/http.py
+-rw-rw-rw-  2.0 fat     2506 b- defN 19-Nov-09 13:26 datadog_checks/base/utils/limiter.py
+-rw-rw-rw-  2.0 fat     2497 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/platform.py
 -rw-rw-rw-  2.0 fat     1280 b- defN 19-May-25 19:31 datadog_checks/base/utils/proxy.py
--rw-rw-rw-  2.0 fat     2610 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/subprocess_output.py
--rw-rw-rw-  2.0 fat      190 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/tagging.py
--rw-rw-rw-  2.0 fat     3500 b- defN 19-May-25 19:31 datadog_checks/base/utils/tailfile.py
--rw-rw-rw-  2.0 fat     2014 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/timeout.py
--rw-rw-rw-  2.0 fat      841 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/tracing.py
--rw-rw-rw-  2.0 fat      107 b- defN 19-May-25 19:31 datadog_checks/base/utils/agent/__init__.py
--rw-rw-rw-  2.0 fat      158 b- defN 19-Sep-25 03:14 datadog_checks/base/utils/agent/common.py
--rw-rw-rw-  2.0 fat     2266 b- defN 19-May-25 19:31 datadog_checks/base/utils/agent/debug.py
--rw-rw-rw-  2.0 fat    10506 b- defN 19-Oct-18 02:14 datadog_checks/base/utils/agent/memory.py
--rw-rw-rw-  2.0 fat      500 b- defN 19-Jun-21 03:34 datadog_checks/base/utils/agent/packages.py
--rw-rw-rw-  2.0 fat      891 b- defN 19-Oct-18 19:33 datadog_checks/base/utils/agent/utils.py
--rw-rw-rw-  2.0 fat      141 b- defN 19-Oct-18 19:33 datadog_checks/base/utils/metadata/__init__.py
--rw-rw-rw-  2.0 fat      456 b- defN 19-Oct-18 19:33 datadog_checks/base/utils/metadata/constants.py
--rw-rw-rw-  2.0 fat     6329 b- defN 19-Oct-18 19:33 datadog_checks/base/utils/metadata/core.py
--rw-rw-rw-  2.0 fat      373 b- defN 19-Oct-18 19:33 datadog_checks/base/utils/metadata/utils.py
--rw-rw-rw-  2.0 fat     1677 b- defN 19-Oct-18 19:33 datadog_checks/base/utils/metadata/version.py
+-rw-rw-rw-  2.0 fat     2585 b- defN 19-Nov-09 13:26 datadog_checks/base/utils/subprocess_output.py
+-rw-rw-rw-  2.0 fat      190 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/tagging.py
+-rw-rw-rw-  2.0 fat     3494 b- defN 19-Nov-09 13:26 datadog_checks/base/utils/tailfile.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/timeout.py
+-rw-rw-rw-  2.0 fat      841 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/tracing.py
+-rw-rw-rw-  2.0 fat      962 b- defN 19-Nov-28 15:39 datadog_checks/base/utils/warnings_util.py
+-rw-rw-rw-  2.0 fat      107 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/agent/__init__.py
+-rw-rw-rw-  2.0 fat      158 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/agent/common.py
+-rw-rw-rw-  2.0 fat     2266 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/agent/debug.py
+-rw-rw-rw-  2.0 fat    10506 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/agent/memory.py
+-rw-rw-rw-  2.0 fat      500 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/agent/packages.py
+-rw-rw-rw-  2.0 fat      891 b- defN 19-Nov-08 18:27 datadog_checks/base/utils/agent/utils.py
+-rw-rw-rw-  2.0 fat      163 b- defN 19-Nov-25 00:57 datadog_checks/base/utils/db/__init__.py
+-rw-rw-rw-  2.0 fat     4541 b- defN 19-Nov-25 00:57 datadog_checks/base/utils/db/core.py
+-rw-rw-rw-  2.0 fat     4237 b- defN 19-Nov-25 00:57 datadog_checks/base/utils/db/query.py
+-rw-rw-rw-  2.0 fat     4322 b- defN 19-Nov-25 00:57 datadog_checks/base/utils/db/transform.py
+-rw-rw-rw-  2.0 fat      487 b- defN 19-Nov-25 00:57 datadog_checks/base/utils/db/utils.py
+-rw-rw-rw-  2.0 fat      141 b- defN 19-Nov-08 18:27 datadog_checks/base/utils/metadata/__init__.py
+-rw-rw-rw-  2.0 fat      456 b- defN 19-Nov-08 18:27 datadog_checks/base/utils/metadata/constants.py
+-rw-rw-rw-  2.0 fat     6350 b- defN 19-Nov-09 13:26 datadog_checks/base/utils/metadata/core.py
+-rw-rw-rw-  2.0 fat      373 b- defN 19-Nov-08 18:27 datadog_checks/base/utils/metadata/utils.py
+-rw-rw-rw-  2.0 fat     1917 b- defN 19-Nov-09 13:26 datadog_checks/base/utils/metadata/version.py
 -rw-rw-rw-  2.0 fat      159 b- defN 19-May-25 19:31 datadog_checks/base/utils/prometheus/__init__.py
--rw-rw-rw-  2.0 fat     1032 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/prometheus/functions.py
--rw-rw-rw-  2.0 fat    25002 b- defN 19-Jun-05 22:17 datadog_checks/base/utils/prometheus/metrics_pb2.py
--rw-rw-rw-  2.0 fat      211 b- defN 19-Sep-25 15:24 datadog_checks/checks/__init__.py
--rw-rw-rw-  2.0 fat      155 b- defN 19-Aug-23 03:30 datadog_checks/checks/base.py
--rw-rw-rw-  2.0 fat      183 b- defN 19-Aug-23 03:30 datadog_checks/checks/network.py
--rw-rw-rw-  2.0 fat      300 b- defN 19-Sep-25 15:24 datadog_checks/checks/network_checks.py
--rw-rw-rw-  2.0 fat      332 b- defN 19-Sep-25 15:24 datadog_checks/checks/winwmi_check.py
--rw-rw-rw-  2.0 fat      239 b- defN 19-Sep-25 15:24 datadog_checks/checks/libs/__init__.py
--rw-rw-rw-  2.0 fat      167 b- defN 19-Aug-23 03:30 datadog_checks/checks/libs/thread_pool.py
--rw-rw-rw-  2.0 fat      161 b- defN 19-Aug-23 03:30 datadog_checks/checks/libs/timer.py
+-rw-rw-rw-  2.0 fat     1032 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/prometheus/functions.py
+-rw-rw-rw-  2.0 fat    25002 b- defN 19-Nov-08 02:17 datadog_checks/base/utils/prometheus/metrics_pb2.py
+-rw-rw-rw-  2.0 fat      211 b- defN 19-Nov-08 02:17 datadog_checks/checks/__init__.py
+-rw-rw-rw-  2.0 fat      155 b- defN 19-Nov-08 02:17 datadog_checks/checks/base.py
+-rw-rw-rw-  2.0 fat      183 b- defN 19-Nov-08 02:17 datadog_checks/checks/network.py
+-rw-rw-rw-  2.0 fat      300 b- defN 19-Nov-08 02:17 datadog_checks/checks/network_checks.py
+-rw-rw-rw-  2.0 fat      332 b- defN 19-Nov-08 02:17 datadog_checks/checks/winwmi_check.py
+-rw-rw-rw-  2.0 fat      239 b- defN 19-Nov-08 02:17 datadog_checks/checks/libs/__init__.py
+-rw-rw-rw-  2.0 fat      167 b- defN 19-Nov-08 02:17 datadog_checks/checks/libs/thread_pool.py
+-rw-rw-rw-  2.0 fat      161 b- defN 19-Nov-08 02:17 datadog_checks/checks/libs/timer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 19-Aug-23 03:30 datadog_checks/checks/libs/vmware/__init__.py
--rw-rw-rw-  2.0 fat      175 b- defN 19-Aug-23 03:30 datadog_checks/checks/libs/vmware/all_metrics.py
--rw-rw-rw-  2.0 fat      177 b- defN 19-Aug-23 03:30 datadog_checks/checks/libs/vmware/basic_metrics.py
--rw-rw-rw-  2.0 fat      239 b- defN 19-Sep-25 15:24 datadog_checks/checks/libs/wmi/__init__.py
--rw-rw-rw-  2.0 fat     1154 b- defN 19-Sep-25 15:24 datadog_checks/checks/libs/wmi/sampler.py
--rw-rw-rw-  2.0 fat      163 b- defN 19-Aug-23 03:30 datadog_checks/checks/openmetrics/__init__.py
--rw-rw-rw-  2.0 fat      174 b- defN 19-Aug-23 03:30 datadog_checks/checks/openmetrics/base_check.py
--rw-rw-rw-  2.0 fat      170 b- defN 19-Aug-23 03:30 datadog_checks/checks/openmetrics/mixins.py
--rw-rw-rw-  2.0 fat       80 b- defN 19-Aug-23 03:30 datadog_checks/checks/prometheus/__init__.py
--rw-rw-rw-  2.0 fat      173 b- defN 19-Aug-23 03:30 datadog_checks/checks/prometheus/base_check.py
--rw-rw-rw-  2.0 fat      169 b- defN 19-Aug-23 03:30 datadog_checks/checks/prometheus/mixins.py
--rw-rw-rw-  2.0 fat      178 b- defN 19-Aug-23 03:30 datadog_checks/checks/prometheus/prometheus_base.py
--rw-rw-rw-  2.0 fat      180 b- defN 19-Sep-25 15:24 datadog_checks/checks/prometheus_check/__init__.py
--rw-rw-rw-  2.0 fat      155 b- defN 19-Aug-23 03:30 datadog_checks/checks/win/__init__.py
--rw-rw-rw-  2.0 fat      162 b- defN 19-Aug-23 03:30 datadog_checks/checks/win/winpdh.py
--rw-rw-rw-  2.0 fat      167 b- defN 19-Aug-23 03:30 datadog_checks/checks/win/winpdh_base.py
--rw-rw-rw-  2.0 fat      166 b- defN 19-Aug-23 03:30 datadog_checks/checks/win/winpdh_stub.py
--rw-rw-rw-  2.0 fat      160 b- defN 19-Aug-23 03:30 datadog_checks/checks/win/wmi/__init__.py
--rw-rw-rw-  2.0 fat      173 b- defN 19-Aug-23 03:30 datadog_checks/checks/win/wmi/counter_type.py
--rw-rw-rw-  2.0 fat      168 b- defN 19-Aug-23 03:30 datadog_checks/checks/win/wmi/sampler.py
--rw-rw-rw-  2.0 fat      149 b- defN 19-Aug-23 03:30 datadog_checks/stubs/__init__.py
--rw-rw-rw-  2.0 fat      155 b- defN 19-Aug-23 03:30 datadog_checks/stubs/_util.py
--rw-rw-rw-  2.0 fat      160 b- defN 19-Aug-23 03:30 datadog_checks/stubs/aggregator.py
--rw-rw-rw-  2.0 fat      163 b- defN 19-Aug-23 03:30 datadog_checks/stubs/datadog_agent.py
+-rw-rw-rw-  2.0 fat      175 b- defN 19-Nov-08 02:17 datadog_checks/checks/libs/vmware/all_metrics.py
+-rw-rw-rw-  2.0 fat      177 b- defN 19-Nov-08 02:17 datadog_checks/checks/libs/vmware/basic_metrics.py
+-rw-rw-rw-  2.0 fat      239 b- defN 19-Nov-08 02:17 datadog_checks/checks/libs/wmi/__init__.py
+-rw-rw-rw-  2.0 fat     1154 b- defN 19-Nov-08 02:17 datadog_checks/checks/libs/wmi/sampler.py
+-rw-rw-rw-  2.0 fat      163 b- defN 19-Nov-08 02:17 datadog_checks/checks/openmetrics/__init__.py
+-rw-rw-rw-  2.0 fat      174 b- defN 19-Nov-08 02:17 datadog_checks/checks/openmetrics/base_check.py
+-rw-rw-rw-  2.0 fat      170 b- defN 19-Nov-08 02:17 datadog_checks/checks/openmetrics/mixins.py
+-rw-rw-rw-  2.0 fat       80 b- defN 19-Nov-08 02:17 datadog_checks/checks/prometheus/__init__.py
+-rw-rw-rw-  2.0 fat      173 b- defN 19-Nov-08 02:17 datadog_checks/checks/prometheus/base_check.py
+-rw-rw-rw-  2.0 fat      169 b- defN 19-Nov-08 02:17 datadog_checks/checks/prometheus/mixins.py
+-rw-rw-rw-  2.0 fat      178 b- defN 19-Nov-08 02:17 datadog_checks/checks/prometheus/prometheus_base.py
+-rw-rw-rw-  2.0 fat      180 b- defN 19-Nov-08 02:17 datadog_checks/checks/prometheus_check/__init__.py
+-rw-rw-rw-  2.0 fat      155 b- defN 19-Nov-08 02:17 datadog_checks/checks/win/__init__.py
+-rw-rw-rw-  2.0 fat      162 b- defN 19-Nov-08 02:17 datadog_checks/checks/win/winpdh.py
+-rw-rw-rw-  2.0 fat      167 b- defN 19-Nov-08 02:17 datadog_checks/checks/win/winpdh_base.py
+-rw-rw-rw-  2.0 fat      166 b- defN 19-Nov-08 02:17 datadog_checks/checks/win/winpdh_stub.py
+-rw-rw-rw-  2.0 fat      160 b- defN 19-Nov-08 02:17 datadog_checks/checks/win/wmi/__init__.py
+-rw-rw-rw-  2.0 fat      173 b- defN 19-Nov-08 02:17 datadog_checks/checks/win/wmi/counter_type.py
+-rw-rw-rw-  2.0 fat      168 b- defN 19-Nov-08 02:17 datadog_checks/checks/win/wmi/sampler.py
+-rw-rw-rw-  2.0 fat      149 b- defN 19-Nov-08 02:17 datadog_checks/stubs/__init__.py
+-rw-rw-rw-  2.0 fat      155 b- defN 19-Nov-08 02:17 datadog_checks/stubs/_util.py
+-rw-rw-rw-  2.0 fat      160 b- defN 19-Nov-08 02:17 datadog_checks/stubs/aggregator.py
+-rw-rw-rw-  2.0 fat      163 b- defN 19-Nov-08 02:17 datadog_checks/stubs/datadog_agent.py
 -rw-rw-rw-  2.0 fat        0 b- defN 19-Aug-23 03:30 datadog_checks/utils/__init__.py
--rw-rw-rw-  2.0 fat      156 b- defN 19-Aug-23 03:30 datadog_checks/utils/common.py
--rw-rw-rw-  2.0 fat      159 b- defN 19-Aug-23 03:30 datadog_checks/utils/containers.py
--rw-rw-rw-  2.0 fat      157 b- defN 19-Aug-23 03:30 datadog_checks/utils/headers.py
--rw-rw-rw-  2.0 fat      151 b- defN 19-Aug-23 03:30 datadog_checks/utils/limiter.py
--rw-rw-rw-  2.0 fat      158 b- defN 19-Aug-23 03:30 datadog_checks/utils/platform.py
--rw-rw-rw-  2.0 fat      155 b- defN 19-Aug-23 03:30 datadog_checks/utils/proxy.py
--rw-rw-rw-  2.0 fat      167 b- defN 19-Aug-23 03:30 datadog_checks/utils/subprocess_output.py
--rw-rw-rw-  2.0 fat      158 b- defN 19-Aug-23 03:30 datadog_checks/utils/tailfile.py
--rw-rw-rw-  2.0 fat      157 b- defN 19-Aug-23 03:30 datadog_checks/utils/timeout.py
--rw-rw-rw-  2.0 fat      151 b- defN 19-Aug-23 03:30 datadog_checks/utils/tracing.py
--rw-rw-rw-  2.0 fat      155 b- defN 19-Aug-23 03:30 datadog_checks/utils/prometheus/__init__.py
--rw-rw-rw-  2.0 fat      191 b- defN 19-Aug-23 03:30 datadog_checks/utils/prometheus/functions.py
--rw-rw-rw-  2.0 fat      167 b- defN 19-Aug-23 03:30 datadog_checks/utils/prometheus/metrics_pb2.py
--rw-rw-rw-  2.0 fat     3399 b- defN 19-Oct-22 23:49 datadog_checks_base-9.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      116 b- defN 19-Oct-22 23:49 datadog_checks_base-9.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 19-Oct-22 23:49 datadog_checks_base-9.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    11972 b- defN 19-Oct-22 23:49 datadog_checks_base-9.5.0.dist-info/RECORD
-125 files, 444242 bytes uncompressed, 113638 bytes compressed:  74.4%
+-rw-rw-rw-  2.0 fat      156 b- defN 19-Nov-08 02:17 datadog_checks/utils/common.py
+-rw-rw-rw-  2.0 fat      159 b- defN 19-Nov-08 02:17 datadog_checks/utils/containers.py
+-rw-rw-rw-  2.0 fat      157 b- defN 19-Nov-08 02:17 datadog_checks/utils/headers.py
+-rw-rw-rw-  2.0 fat      151 b- defN 19-Nov-08 02:17 datadog_checks/utils/limiter.py
+-rw-rw-rw-  2.0 fat      158 b- defN 19-Nov-08 02:17 datadog_checks/utils/platform.py
+-rw-rw-rw-  2.0 fat      155 b- defN 19-Nov-08 02:17 datadog_checks/utils/proxy.py
+-rw-rw-rw-  2.0 fat      167 b- defN 19-Nov-08 02:17 datadog_checks/utils/subprocess_output.py
+-rw-rw-rw-  2.0 fat      158 b- defN 19-Nov-08 02:17 datadog_checks/utils/tailfile.py
+-rw-rw-rw-  2.0 fat      157 b- defN 19-Nov-08 02:17 datadog_checks/utils/timeout.py
+-rw-rw-rw-  2.0 fat      151 b- defN 19-Nov-08 02:17 datadog_checks/utils/tracing.py
+-rw-rw-rw-  2.0 fat      155 b- defN 19-Nov-08 02:17 datadog_checks/utils/prometheus/__init__.py
+-rw-rw-rw-  2.0 fat      191 b- defN 19-Nov-08 02:17 datadog_checks/utils/prometheus/functions.py
+-rw-rw-rw-  2.0 fat      167 b- defN 19-Nov-08 02:17 datadog_checks/utils/prometheus/metrics_pb2.py
+-rw-rw-rw-  2.0 fat     3399 b- defN 19-Nov-28 15:41 datadog_checks_base-9.6.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      116 b- defN 19-Nov-28 15:41 datadog_checks_base-9.6.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 19-Nov-28 15:41 datadog_checks_base-9.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    12639 b- defN 19-Nov-28 15:41 datadog_checks_base-9.6.0.dist-info/RECORD
+132 files, 463027 bytes uncompressed, 119673 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -141,14 +141,17 @@
 
 Filename: datadog_checks/base/utils/__init__.py
 Comment: 
 
 Filename: datadog_checks/base/utils/common.py
 Comment: 
 
+Filename: datadog_checks/base/utils/constants.py
+Comment: 
+
 Filename: datadog_checks/base/utils/containers.py
 Comment: 
 
 Filename: datadog_checks/base/utils/date.py
 Comment: 
 
 Filename: datadog_checks/base/utils/headers.py
@@ -177,14 +180,17 @@
 
 Filename: datadog_checks/base/utils/timeout.py
 Comment: 
 
 Filename: datadog_checks/base/utils/tracing.py
 Comment: 
 
+Filename: datadog_checks/base/utils/warnings_util.py
+Comment: 
+
 Filename: datadog_checks/base/utils/agent/__init__.py
 Comment: 
 
 Filename: datadog_checks/base/utils/agent/common.py
 Comment: 
 
 Filename: datadog_checks/base/utils/agent/debug.py
@@ -195,14 +201,29 @@
 
 Filename: datadog_checks/base/utils/agent/packages.py
 Comment: 
 
 Filename: datadog_checks/base/utils/agent/utils.py
 Comment: 
 
+Filename: datadog_checks/base/utils/db/__init__.py
+Comment: 
+
+Filename: datadog_checks/base/utils/db/core.py
+Comment: 
+
+Filename: datadog_checks/base/utils/db/query.py
+Comment: 
+
+Filename: datadog_checks/base/utils/db/transform.py
+Comment: 
+
+Filename: datadog_checks/base/utils/db/utils.py
+Comment: 
+
 Filename: datadog_checks/base/utils/metadata/__init__.py
 Comment: 
 
 Filename: datadog_checks/base/utils/metadata/constants.py
 Comment: 
 
 Filename: datadog_checks/base/utils/metadata/core.py
@@ -357,20 +378,20 @@
 
 Filename: datadog_checks/utils/prometheus/functions.py
 Comment: 
 
 Filename: datadog_checks/utils/prometheus/metrics_pb2.py
 Comment: 
 
-Filename: datadog_checks_base-9.5.0.dist-info/METADATA
+Filename: datadog_checks_base-9.6.0.dist-info/METADATA
 Comment: 
 
-Filename: datadog_checks_base-9.5.0.dist-info/WHEEL
+Filename: datadog_checks_base-9.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: datadog_checks_base-9.5.0.dist-info/top_level.txt
+Filename: datadog_checks_base-9.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: datadog_checks_base-9.5.0.dist-info/RECORD
+Filename: datadog_checks_base-9.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datadog_checks/base/__about__.py

```diff
@@ -1,5 +1,5 @@
-# (C) Datadog, Inc. 2018
-# All rights reserved
-# Licensed under a 3-clause BSD style license (see LICENSE)
-
-__version__ = "9.5.0"
+# (C) Datadog, Inc. 2018
+# All rights reserved
+# Licensed under a 3-clause BSD style license (see LICENSE)
+
+__version__ = "9.6.0"
```

## datadog_checks/base/ddyaml.py

```diff
@@ -37,15 +37,15 @@
     explicit_start=None,
     explicit_end=None,
     version=None,
     tags=None,
 ):
     if Dumper != yDumper:
         stream_name = get_stream_name(stream)
-        log.debug("Unsafe dumping of YAML has been disabled - using safe dumper instead in {}".format(stream_name))
+        log.debug("Unsafe dumping of YAML has been disabled - using safe dumper instead in %s", stream_name)
 
     if pyyaml_dump_all:
         return pyyaml_dump_all(
             documents,
             stream,
             yDumper,
             default_style,
@@ -80,26 +80,26 @@
         tags,
     )
 
 
 def safe_yaml_load(stream, Loader=yLoader):
     if Loader != yLoader:
         stream_name = get_stream_name(stream)
-        log.debug("Unsafe loading of YAML has been disabled - using safe loader instead in {}".format(stream_name))
+        log.debug("Unsafe loading of YAML has been disabled - using safe loader instead in %s", stream_name)
 
     if pyyaml_load:
         return pyyaml_load(stream, Loader=yLoader)
 
     return yaml.load(stream, Loader=yLoader)
 
 
 def safe_yaml_load_all(stream, Loader=yLoader):
     if Loader != yLoader:
         stream_name = get_stream_name(stream)
-        log.debug("Unsafe loading of YAML has been disabled - using safe loader instead in {}".format(stream_name))
+        log.debug("Unsafe loading of YAML has been disabled - using safe loader instead in %s", stream_name)
 
     if pyyaml_load_all:
         return pyyaml_load_all(stream, Loader=yLoader)
 
     return yaml.load_all(stream, Loader=yLoader)
```

## datadog_checks/base/checks/base.py

```diff
@@ -93,27 +93,42 @@
 
     # Default fields to whitelist for metadata submission
     METADATA_DEFAULT_CONFIG_INIT_CONFIG = None
     METADATA_DEFAULT_CONFIG_INSTANCE = None
 
     FIRST_CAP_RE = re.compile(br'(.)([A-Z][a-z]+)')
     ALL_CAP_RE = re.compile(br'([a-z0-9])([A-Z])')
-    METRIC_REPLACEMENT = re.compile(br'([^a-zA-Z0-9_.]+)|(^[^a-zA-Z]+)')
+    METRIC_REPLACEMENT = re.compile(br'([^a-zA-Z0-9_.]+)|(^[^a-zA-Z]+)|__+')
     DOT_UNDERSCORE_CLEANUP = re.compile(br'_*\._*')
     DEFAULT_METRIC_LIMIT = 0
 
     def __init__(self, *args, **kwargs):
         """In general, you don't need to and you should not override anything from the base
         class except the :py:meth:`check` method but sometimes it might be useful for a Check to
         have its own constructor.
 
         When overriding `__init__` you have to remember that, depending on the configuration,
         the Agent might create several different Check instances and the method would be
         called as many times.
 
+        Agent 5 signature:
+
+            AgentCheck(name, init_config, agentConfig, instances=None)
+            AgentCheck.check(instance)
+
+        Agent 6,7 signature:
+
+            AgentCheck(name, init_config, instances)    # instances contain only 1 instance
+            AgentCheck.check(instance)
+
+        Agent 8 signature:
+
+            AgentCheck(name, init_config, instance)     # one instance
+            AgentCheck.check()                          # no more instance argument for check method
+
         :warning: when loading a Custom check, the Agent will inspect the module searching
             for a subclass of `AgentCheck`. If such a class exists but has been derived in
             turn, it'll be ignored - **you should never derive from an existing Check**.
 
         :param str name: the name of the check.
         :param dict init_config: the 'init_config' section of the configuration.
         :param list instances: a one-element list containing the instance options from the
@@ -130,15 +145,16 @@
         self.metric_limiter = None
 
         if len(args) > 0:
             self.name = args[0]
         if len(args) > 1:
             self.init_config = args[1]
         if len(args) > 2:
-            if len(args) > 3 or 'instances' in kwargs:
+            # agent pass instances as tuple but in test we are usually using list, so we are testing for both
+            if len(args) > 3 or not isinstance(args[2], (list, tuple)) or 'instances' in kwargs:
                 # old-style init: the 3rd argument is `agentConfig`
                 self.agentConfig = args[2]
                 if len(args) > 3:
                     self.instances = args[3]
             else:
                 # new-style init: the 3rd argument is `instances`
                 self.instances = args[2]
@@ -204,16 +220,16 @@
         # Setup metric limits
         try:
             metric_limit = self.instances[0].get('max_returned_metrics', self.DEFAULT_METRIC_LIMIT)
             # Do not allow to disable limiting if the class has set a non-zero default value
             if metric_limit == 0 and self.DEFAULT_METRIC_LIMIT > 0:
                 metric_limit = self.DEFAULT_METRIC_LIMIT
                 self.warning(
-                    'Setting max_returned_metrics to zero is not allowed, reverting '
-                    'to the default of {} metrics'.format(self.DEFAULT_METRIC_LIMIT)
+                    'Setting max_returned_metrics to zero is not allowed, reverting to the default of %s metrics',
+                    self.DEFAULT_METRIC_LIMIT,
                 )
         except Exception:
             metric_limit = self.DEFAULT_METRIC_LIMIT
         if metric_limit > 0:
             self.metric_limiter = Limiter(self.name, 'metrics', metric_limit, self.warning)
 
         # Functions that will be called exactly once (if successful) before the first check run
@@ -516,15 +532,15 @@
             new_tags = []
             for hostname, source_map in external_tags:
                 new_tags.append((to_string(hostname), source_map))
                 for src_name, tags in iteritems(source_map):
                     source_map[src_name] = self._normalize_tags_type(tags)
             datadog_agent.set_external_tags(new_tags)
         except IndexError:
-            self.log.exception('Unexpected external tags format: {}'.format(external_tags))
+            self.log.exception('Unexpected external tags format: %s', external_tags)
             raise
 
     def convert_to_underscore_separated(self, name):
         """
         Convert from CamelCase to camel_case
         And substitute illegal metric characters
         """
@@ -597,29 +613,32 @@
             metric = unicodedata.normalize('NFKD', metric).encode('ascii', 'ignore')
 
         if fix_case:
             name = self.convert_to_underscore_separated(metric)
             if prefix is not None:
                 prefix = self.convert_to_underscore_separated(prefix)
         else:
-            name = re.sub(br"[,\+\*\-/()\[\]{}\s]", b"_", metric)
-        # Eliminate multiple _
-        name = re.sub(br"__+", b"_", name)
-        # Don't start/end with _
-        name = re.sub(br"^_", b"", name)
-        name = re.sub(br"_$", b"", name)
-        # Drop ._ and _.
-        name = re.sub(br"\._", b".", name)
-        name = re.sub(br"_\.", b".", name)
+            name = self.METRIC_REPLACEMENT.sub(br'_', metric)
+            name = self.DOT_UNDERSCORE_CLEANUP.sub(br'.', name).strip(b'_')
 
         if prefix is not None:
             name = ensure_bytes(prefix) + b"." + name
 
         return to_string(name)
 
+    def normalize_tag(self, tag):
+        """Normalize tag values.
+
+        It doesn't entirely duplicate backend logic, as the cleanup will happen
+        here. It just removes leading underscores for consistency, and replaces
+        spaces for testing.
+        """
+        tag = tag.replace(' ', '_').strip('_')
+        return to_string(tag)
+
     def check(self, instance):
         raise NotImplementedError
 
     def run(self):
         try:
             while self.check_initializations:
                 initialization = self.check_initializations.popleft()
@@ -694,15 +713,15 @@
         for key, value in list(iteritems(event)):
             # transform any bytes objects to utf-8
             if isinstance(value, bytes):
                 try:
                     event[key] = event[key].decode('utf-8')
                 except UnicodeError:
                     self.log.warning(
-                        'Error decoding unicode field `{}` to utf-8 encoded string, cannot submit event'.format(key)
+                        'Error decoding unicode field `%s` to utf-8 encoded string, cannot submit event', key
                     )
                     return
 
         if event.get('tags'):
             event['tags'] = self._normalize_tags_type(event['tags'])
         if event.get('timestamp'):
             event['timestamp'] = int(event['timestamp'])
@@ -732,15 +751,15 @@
                 if tag is None:
                     continue
                 if not isinstance(tag, str):
                     try:
                         tag = tag.decode('utf-8')
                     except Exception:
                         self.log.warning(
-                            'Error decoding tag `{}` as utf-8 for metric `{}`, ignoring tag'.format(tag, metric_name)
+                            'Error decoding tag `%s` as utf-8 for metric `%s`, ignoring tag', tag, metric_name
                         )
                         continue
 
                 normalized_tags.append(tag)
 
         return normalized_tags
 
@@ -786,32 +805,26 @@
         normalized_tags = []
 
         if device_name:
             self._log_deprecation("device_name")
             device_tag = self._to_bytes("device:{}".format(device_name))
             if device_tag is None:
                 self.log.warning(
-                    'Error encoding device name `{}` to utf-8 for metric `{}`, ignoring tag'.format(
-                        repr(device_name), repr(metric_name)
-                    )
+                    'Error encoding device name `%r` to utf-8 for metric `%r`, ignoring tag', device_name, metric_name
                 )
             else:
                 normalized_tags.append(device_tag)
 
         if tags is not None:
             for tag in tags:
                 if tag is None:
                     continue
                 encoded_tag = self._to_bytes(tag)
                 if encoded_tag is None:
-                    self.log.warning(
-                        'Error encoding tag `{}` to utf-8 for metric `{}`, ignoring tag'.format(
-                            repr(tag), repr(metric_name)
-                        )
-                    )
+                    self.log.warning('Error encoding tag `%r` to utf-8 for metric `%r`, ignoring tag', tag, metric_name)
                     continue
                 normalized_tags.append(encoded_tag)
 
         return normalized_tags
 
     def _to_bytes(self, data):
         """
```

## datadog_checks/base/checks/kube_leader/mixins.py

```diff
@@ -44,15 +44,15 @@
         """
         try:
             record = self._get_record(
                 config.get("record_kind", ""), config.get("record_name", ""), config.get("record_namespace", "")
             )
             self._report_status(config, record)
         except Exception as e:
-            self.warning("Cannot retrieve leader election record {}: {}".format(config.get("record_name", ""), e))
+            self.warning("Cannot retrieve leader election record %s: %s", config.get("record_name", ""), e)
 
     @staticmethod
     def _get_record(kind, name, namespace):
         global client, config
         if client is config is None:
             from kubernetes import client, config  # noqa F401
```

## datadog_checks/base/checks/openmetrics/base_check.py

```diff
@@ -15,14 +15,25 @@
 
         instances:
         - prometheus_url: http://example.com/endpoint
             namespace: "foobar"
             metrics:
             - bar
             - foo
+
+
+    Agent 5 signature:
+
+        OpenMetricsBaseCheck(name, init_config, agentConfig, instances=None, default_instances=None,
+                             default_namespace=None)
+
+    Agent 6 signature:
+
+        OpenMetricsBaseCheck(name, init_config, instances, default_instances=None, default_namespace=None)
+
     """
 
     DEFAULT_METRIC_LIMIT = 2000
 
     def __init__(self, *args, **kwargs):
         args = list(args)
         default_instances = kwargs.pop('default_instances', None) or {}
@@ -38,20 +49,25 @@
 
         super(OpenMetricsBaseCheck, self).__init__(*args, **kwargs)
         self.config_map = {}
         self.default_instances = default_instances
         self.default_namespace = default_namespace
 
         # pre-generate the scraper configurations
+
         if 'instances' in kwargs:
             instances = kwargs['instances']
         elif len(args) == 4:
+            # instances from agent 5 signature
             instances = args[3]
-        else:
+        elif isinstance(args[2], (tuple, list)):
+            # instances from agent 6 signature
             instances = args[2]
+        else:
+            instances = None
 
         if instances is not None:
             for instance in instances:
                 self.get_scraper_config(instance)
 
     def check(self, instance):
         # Get the configuration for this specific instance
```

## datadog_checks/base/checks/openmetrics/mixins.py

```diff
@@ -5,20 +5,20 @@
 from fnmatch import fnmatchcase
 from math import isinf, isnan
 from os.path import isfile
 
 import requests
 from prometheus_client.parser import text_fd_to_metric_families
 from six import PY3, iteritems, itervalues, string_types
-from urllib3 import disable_warnings
 from urllib3.exceptions import InsecureRequestWarning
 
 from ...config import is_affirmative
 from ...errors import CheckException
 from ...utils.common import to_string
+from ...utils.warnings_util import disable_warnings_ctx
 from .. import AgentCheck
 
 if PY3:
     long = int
 
 
 class OpenMetricsScraperMixin(object):
@@ -487,15 +487,15 @@
         except KeyError:
             if metric_transformers is not None and metric.name in metric_transformers:
                 try:
                     # Get the transformer function for this specific metric
                     transformer = metric_transformers[metric.name]
                     transformer(metric, scraper_config)
                 except Exception as err:
-                    self.log.warning('Error handling metric: {} - error: {}'.format(metric.name, err))
+                    self.log.warning('Error handling metric: %s - error: %s', metric.name, err)
 
                 return
 
             # build the wildcard list if first pass
             if scraper_config['_metrics_wildcards'] is None:
                 scraper_config['_metrics_wildcards'] = [x for x in scraper_config['metrics_mapper'] if '*' in x]
 
@@ -531,15 +531,15 @@
         service_check_name = '{}{}'.format(scraper_config['namespace'], '.prometheus.health')
         service_check_tags = ['endpoint:{}'.format(endpoint)]
         service_check_tags.extend(scraper_config['custom_tags'])
 
         try:
             response = self.send_request(endpoint, scraper_config, headers)
         except requests.exceptions.SSLError:
-            self.log.error("Invalid SSL settings for requesting {} endpoint".format(endpoint))
+            self.log.error("Invalid SSL settings for requesting %s endpoint", endpoint)
             raise
         except IOError:
             if health_service_check:
                 self.service_check(service_check_name, AgentCheck.CRITICAL, tags=service_check_tags)
             raise
         try:
             response.raise_for_status()
@@ -575,33 +575,35 @@
                 cert = scraper_config['ssl_cert']
 
         verify = scraper_config['ssl_verify']
         # TODO: deprecate use as `ssl_verify` boolean
         if scraper_config['ssl_ca_cert'] is False:
             verify = False
 
+        disable_insecure_warnings = False
         if isinstance(scraper_config['ssl_ca_cert'], string_types):
             verify = scraper_config['ssl_ca_cert']
         elif verify is False:
-            disable_warnings(InsecureRequestWarning)
+            disable_insecure_warnings = True
 
         # Determine the authentication settings
         username = scraper_config['username']
         password = scraper_config['password']
         auth = (username, password) if username is not None and password is not None else None
 
-        return requests.get(
-            endpoint,
-            headers=headers,
-            stream=True,
-            timeout=scraper_config['prometheus_timeout'],
-            cert=cert,
-            verify=verify,
-            auth=auth,
-        )
+        with disable_warnings_ctx(InsecureRequestWarning, disable=disable_insecure_warnings):
+            return requests.get(
+                endpoint,
+                headers=headers,
+                stream=True,
+                timeout=scraper_config['prometheus_timeout'],
+                cert=cert,
+                verify=verify,
+                auth=auth,
+            )
 
     def get_hostname_for_sample(self, sample, scraper_config):
         """
         Expose the label_to_hostname mapping logic to custom handler methods
         """
         return self._get_hostname(None, sample, scraper_config)
 
@@ -619,15 +621,15 @@
         metric when sending the gauge to Datadog.
         """
         if metric.type in ["gauge", "counter", "rate"]:
             metric_name_with_namespace = '{}.{}'.format(scraper_config['namespace'], metric_name)
             for sample in metric.samples:
                 val = sample[self.SAMPLE_VALUE]
                 if not self._is_value_valid(val):
-                    self.log.debug("Metric value is not supported for metric {}".format(sample[self.SAMPLE_NAME]))
+                    self.log.debug("Metric value is not supported for metric %s", sample[self.SAMPLE_NAME])
                     continue
                 custom_hostname = self._get_hostname(hostname, sample, scraper_config)
                 # Determine the tags to send
                 tags = self._metric_tags(metric_name, val, sample, scraper_config, hostname=custom_hostname)
                 if metric.type == "counter" and scraper_config['send_monotonic_counter']:
                     self.monotonic_count(metric_name_with_namespace, val, tags=tags, hostname=custom_hostname)
                 elif metric.type == "rate":
@@ -635,15 +637,15 @@
                 else:
                     self.gauge(metric_name_with_namespace, val, tags=tags, hostname=custom_hostname)
         elif metric.type == "histogram":
             self._submit_gauges_from_histogram(metric_name, metric, scraper_config)
         elif metric.type == "summary":
             self._submit_gauges_from_summary(metric_name, metric, scraper_config)
         else:
-            self.log.error("Metric type {} unsupported for metric {}.".format(metric.type, metric_name))
+            self.log.error("Metric type %s unsupported for metric %s.", metric.type, metric_name)
 
     def _get_hostname(self, hostname, sample, scraper_config):
         """
         If hostname is None, look at label_to_hostname setting
         """
         if (
             hostname is None
@@ -660,15 +662,15 @@
     def _submit_gauges_from_summary(self, metric_name, metric, scraper_config, hostname=None):
         """
         Extracts metrics from a prometheus summary metric and sends them as gauges
         """
         for sample in metric.samples:
             val = sample[self.SAMPLE_VALUE]
             if not self._is_value_valid(val):
-                self.log.debug("Metric value is not supported for metric {}".format(sample[self.SAMPLE_NAME]))
+                self.log.debug("Metric value is not supported for metric %s", sample[self.SAMPLE_NAME])
                 continue
             custom_hostname = self._get_hostname(hostname, sample, scraper_config)
             if sample[self.SAMPLE_NAME].endswith("_sum"):
                 tags = self._metric_tags(metric_name, val, sample, scraper_config, hostname=custom_hostname)
                 self.gauge(
                     "{}.{}.sum".format(scraper_config['namespace'], metric_name),
                     val,
@@ -699,15 +701,15 @@
         Extracts metrics from a prometheus histogram and sends them as gauges
         """
         if scraper_config['non_cumulative_buckets']:
             self._decumulate_histogram_buckets(metric)
         for sample in metric.samples:
             val = sample[self.SAMPLE_VALUE]
             if not self._is_value_valid(val):
-                self.log.debug("Metric value is not supported for metric {}".format(sample[self.SAMPLE_NAME]))
+                self.log.debug("Metric value is not supported for metric %s", sample[self.SAMPLE_NAME])
                 continue
             custom_hostname = self._get_hostname(hostname, sample, scraper_config)
             if sample[self.SAMPLE_NAME].endswith("_sum") and not scraper_config['send_distribution_buckets']:
                 tags = self._metric_tags(metric_name, val, sample, scraper_config, hostname)
                 self.gauge(
                     "{}.{}.sum".format(scraper_config['namespace'], metric_name),
                     val,
@@ -806,25 +808,25 @@
             # Replacing the sample tuple
             sample[self.SAMPLE_LABELS]["lower_bound"] = str(matching_bucket_tuple[0])
             metric.samples[i] = (sample[self.SAMPLE_NAME], sample[self.SAMPLE_LABELS], matching_bucket_tuple[2])
 
     def _submit_sample_histogram_buckets(self, metric_name, sample, scraper_config, hostname=None):
         if "lower_bound" not in sample[self.SAMPLE_LABELS] or "le" not in sample[self.SAMPLE_LABELS]:
             self.log.warning(
-                "Metric: {} was not containing required bucket boundaries labels: {}".format(
-                    metric_name, sample[self.SAMPLE_LABELS]
-                )
+                "Metric: %s was not containing required bucket boundaries labels: %s",
+                metric_name,
+                sample[self.SAMPLE_LABELS],
             )
             return
         sample[self.SAMPLE_LABELS]["le"] = str(float(sample[self.SAMPLE_LABELS]["le"]))
         sample[self.SAMPLE_LABELS]["lower_bound"] = str(float(sample[self.SAMPLE_LABELS]["lower_bound"]))
         if sample[self.SAMPLE_LABELS]["le"] == sample[self.SAMPLE_LABELS]["lower_bound"]:
             # this can happen for -inf/-inf bucket that we don't want to send (always 0)
             self.log.warning(
-                "Metric: {} has bucket boundaries equal, skipping: {}".format(metric_name, sample[self.SAMPLE_LABELS])
+                "Metric: %s has bucket boundaries equal, skipping: %s", metric_name, sample[self.SAMPLE_LABELS]
             )
             return
         tags = self._metric_tags(metric_name, sample[self.SAMPLE_VALUE], sample, scraper_config, hostname)
         self.submit_histogram_bucket(
             "{}.{}".format(scraper_config['namespace'], metric_name),
             sample[self.SAMPLE_VALUE],
             float(sample[self.SAMPLE_LABELS]["lower_bound"]),
@@ -860,21 +862,21 @@
             return None
 
         path = None
         if bearer_token_path is not None:
             if isfile(bearer_token_path):
                 path = bearer_token_path
             else:
-                self.log.error("File not found: {}".format(bearer_token_path))
+                self.log.error("File not found: %s", bearer_token_path)
         elif isfile(self.KUBERNETES_TOKEN_PATH):
             path = self.KUBERNETES_TOKEN_PATH
 
         if path is None:
             self.log.error("Cannot get bearer token from bearer_token_path or auto discovery")
             raise IOError("Cannot get bearer token from bearer_token_path or auto discovery")
 
         try:
             with open(path, 'r') as f:
                 return f.read().rstrip()
         except Exception as err:
-            self.log.error("Cannot get bearer token from path: {} - error: {}".format(path, err))
+            self.log.error("Cannot get bearer token from path: %s - error: %s", path, err)
             raise
```

## datadog_checks/base/checks/prometheus/mixins.py

```diff
@@ -7,18 +7,18 @@
 from fnmatch import fnmatchcase
 from math import isinf, isnan
 
 import requests
 from google.protobuf.internal.decoder import _DecodeVarint32  # pylint: disable=E0611,E0401
 from prometheus_client.parser import text_fd_to_metric_families
 from six import PY3, iteritems, itervalues, string_types
-from urllib3 import disable_warnings
 from urllib3.exceptions import InsecureRequestWarning
 
 from ...utils.prometheus import metrics_pb2
+from ...utils.warnings_util import disable_warnings_ctx
 from .. import AgentCheck
 
 if PY3:
     long = int
 
 
 class PrometheusFormat:
@@ -194,15 +194,15 @@
 
                 # Lookup type overrides:
                 if self.type_overrides and message.name in self.type_overrides:
                     new_type = self.type_overrides[message.name]
                     if new_type in self.METRIC_TYPES:
                         message.type = self.METRIC_TYPES.index(new_type)
                     else:
-                        self.log.debug("type override %s for %s is not a valid type name" % (new_type, message.name))
+                        self.log.debug("type override %s for %s is not a valid type name", new_type, message.name)
                 yield message
 
         elif 'text/plain' in response.headers['Content-Type']:
             input_gen = response.iter_lines(chunk_size=self.REQUESTS_CHUNK_SIZE, decode_unicode=True)
             if self._text_filter_blacklist:
                 input_gen = self._text_filter_input(input_gen)
 
@@ -472,28 +472,28 @@
                 except KeyError:
                     if not ignore_unmapped:
                         # call magic method (non-generic check)
                         handler = getattr(self, message.name)  # Lookup will throw AttributeError if not found
                         try:
                             handler(message, **kwargs)
                         except Exception as err:
-                            self.log.warning("Error handling metric: {} - error: {}".format(message.name, err))
+                            self.log.warning("Error handling metric: %s - error: %s", message.name, err)
                     else:
                         # build the wildcard list if first pass
                         if self._metrics_wildcards is None:
                             self._metrics_wildcards = [x for x in self.metrics_mapper.keys() if '*' in x]
                         # try matching wildcard (generic check)
                         for wildcard in self._metrics_wildcards:
                             if fnmatchcase(message.name, wildcard):
                                 self._submit(
                                     message.name, message, send_histograms_buckets, send_monotonic_counter, custom_tags
                                 )
 
         except AttributeError as err:
-            self.log.debug("Unable to handle metric: {} - error: {}".format(message.name, err))
+            self.log.debug("Unable to handle metric: %s - error: %s", message.name, err)
 
     def poll(self, endpoint, pFormat=PrometheusFormat.PROTOBUF, headers=None):
         """
         Polls the metrics from the prometheus metrics endpoint provided.
         Defaults to the protobuf format, but can use the formats specified by
         the PrometheusFormat class.
         Custom headers can be added to the default headers.
@@ -519,25 +519,27 @@
         headers.update(self.extra_headers)
         cert = None
         if isinstance(self.ssl_cert, string_types):
             cert = self.ssl_cert
             if isinstance(self.ssl_private_key, string_types):
                 cert = (self.ssl_cert, self.ssl_private_key)
         verify = True
+        disable_insecure_warnings = False
         if isinstance(self.ssl_ca_cert, string_types):
             verify = self.ssl_ca_cert
         elif self.ssl_ca_cert is False:
-            disable_warnings(InsecureRequestWarning)
+            disable_insecure_warnings = True
             verify = False
         try:
-            response = requests.get(
-                endpoint, headers=headers, stream=False, timeout=self.prometheus_timeout, cert=cert, verify=verify
-            )
+            with disable_warnings_ctx(InsecureRequestWarning, disable=disable_insecure_warnings):
+                response = requests.get(
+                    endpoint, headers=headers, stream=False, timeout=self.prometheus_timeout, cert=cert, verify=verify
+                )
         except requests.exceptions.SSLError:
-            self.log.error("Invalid SSL settings for requesting {} endpoint".format(endpoint))
+            self.log.error("Invalid SSL settings for requesting %s endpoint", endpoint)
             raise
         except IOError:
             if self.health_service_check:
                 self._submit_service_check(
                     "{}{}".format(self.NAMESPACE, ".prometheus.health"),
                     AgentCheck.CRITICAL,
                     tags=["endpoint:" + endpoint],
@@ -588,33 +590,33 @@
                     val = getattr(metric, self.METRIC_TYPES[message.type]).value
                     if self._is_value_valid(val):
                         if send_monotonic_counter:
                             self._submit_monotonic_count(metric_name, val, metric, custom_tags, custom_hostname)
                         else:
                             self._submit_gauge(metric_name, val, metric, custom_tags, custom_hostname)
                     else:
-                        self.log.debug("Metric value is not supported for metric {}.".format(metric_name))
+                        self.log.debug("Metric value is not supported for metric %s.", metric_name)
                 elif message.type == 4:
                     self._submit_gauges_from_histogram(
                         metric_name, metric, send_histograms_buckets, custom_tags, custom_hostname
                     )
                 elif message.type == 2:
                     self._submit_gauges_from_summary(metric_name, metric, custom_tags, custom_hostname)
                 else:
                     val = getattr(metric, self.METRIC_TYPES[message.type]).value
                     if self._is_value_valid(val):
                         if message.name in self.rate_metrics:
                             self._submit_rate(metric_name, val, metric, custom_tags, custom_hostname)
                         else:
                             self._submit_gauge(metric_name, val, metric, custom_tags, custom_hostname)
                     else:
-                        self.log.debug("Metric value is not supported for metric {}.".format(metric_name))
+                        self.log.debug("Metric value is not supported for metric %s.", metric_name)
 
         else:
-            self.log.error("Metric type {} unsupported for metric {}.".format(message.type, message.name))
+            self.log.error("Metric type %s unsupported for metric %s.", message.type, message.name)
 
     def _get_hostname(self, hostname, metric):
         """
         If hostname is None, look at label_to_hostname setting
         """
         if hostname is None and self.label_to_hostname is not None:
             for label in metric.label:
@@ -637,33 +639,33 @@
         if custom_tags is None:
             custom_tags = []
         # summaries do not have a value attribute
         val = getattr(metric, self.METRIC_TYPES[2]).sample_count
         if self._is_value_valid(val):
             self._submit_gauge("{}.count".format(name), val, metric, custom_tags)
         else:
-            self.log.debug("Metric value is not supported for metric {}.count.".format(name))
+            self.log.debug("Metric value is not supported for metric %s.count.", name)
         val = getattr(metric, self.METRIC_TYPES[2]).sample_sum
         if self._is_value_valid(val):
             self._submit_gauge("{}.sum".format(name), val, metric, custom_tags)
         else:
-            self.log.debug("Metric value is not supported for metric {}.sum.".format(name))
+            self.log.debug("Metric value is not supported for metric %s.sum.", name)
         for quantile in getattr(metric, self.METRIC_TYPES[2]).quantile:
             val = quantile.value
             limit = quantile.quantile
             if self._is_value_valid(val):
                 self._submit_gauge(
                     "{}.quantile".format(name),
                     val,
                     metric,
                     custom_tags=custom_tags + ["quantile:{}".format(limit)],
                     hostname=hostname,
                 )
             else:
-                self.log.debug("Metric value is not supported for metric {}.quantile.".format(name))
+                self.log.debug("Metric value is not supported for metric %s.quantile.", name)
 
     def _submit_gauges_from_histogram(
         self, name, metric, send_histograms_buckets=True, custom_tags=None, hostname=None
     ):
         """
         Extracts metrics from a prometheus histogram and sends them as gauges
         """
@@ -673,34 +675,34 @@
         val = getattr(metric, self.METRIC_TYPES[4]).sample_count
         if self._is_value_valid(val):
             if send_histograms_buckets:
                 self._submit_gauge("{}.count".format(name), val, metric, custom_tags=custom_tags + ["upper_bound:none"])
             else:
                 self._submit_gauge("{}.count".format(name), val, metric, custom_tags)
         else:
-            self.log.debug("Metric value is not supported for metric {}.count.".format(name))
+            self.log.debug("Metric value is not supported for metric %s.count.", name)
         val = getattr(metric, self.METRIC_TYPES[4]).sample_sum
         if self._is_value_valid(val):
             self._submit_gauge("{}.sum".format(name), val, metric, custom_tags)
         else:
-            self.log.debug("Metric value is not supported for metric {}.sum.".format(name))
+            self.log.debug("Metric value is not supported for metric %s.sum.", name)
         if send_histograms_buckets:
             for bucket in getattr(metric, self.METRIC_TYPES[4]).bucket:
                 val = bucket.cumulative_count
                 limit = bucket.upper_bound
                 if self._is_value_valid(val):
                     self._submit_gauge(
                         "{}.count".format(name),
                         val,
                         metric,
                         custom_tags=custom_tags + ["upper_bound:{}".format(limit)],
                         hostname=hostname,
                     )
                 else:
-                    self.log.debug("Metric value is not supported for metric {}.count.".format(name))
+                    self.log.debug("Metric value is not supported for metric %s.count.", name)
 
     def _is_value_valid(self, val):
         return not (isnan(val) or isinf(val))
 
     def set_prometheus_timeout(self, instance, default_value=10):
         """ extract `prometheus_timeout` directly from the instance configuration """
         self.prometheus_timeout = instance.get('prometheus_timeout', default_value)
```

## datadog_checks/base/checks/win/winpdh.py

```diff
@@ -43,20 +43,20 @@
             self.logger.error("Exception loading counter strings %s", str(e))
             raise
 
         if WinPDHCounter._use_en_counter_names:
             self._class_name = class_name
         else:
             if len(class_name_index_list) == 0:
-                self.logger.warning("Class %s was not in counter name list, attempting english counter" % class_name)
+                self.logger.warning("Class %s was not in counter name list, attempting english counter", class_name)
                 self._class_name = class_name
             else:
                 if len(class_name_index_list) > 1:
                     self.logger.warning(
-                        "Class %s had multiple (%d) indices, using first" % (class_name, len(class_name_index_list))
+                        "Class %s had multiple (%d) indices, using first", class_name, len(class_name_index_list)
                     )
                 self._class_name = win32pdh.LookupPerfNameByIndex(None, int(class_name_index_list[0]))
 
         self.hq = win32pdh.OpenQuery()
         self.collect_counters()
 
         if len(self.counterdict) == 0:
@@ -154,46 +154,46 @@
             In this case, we don't have any translations.  Just attempt to make the
             counter path
             '''
             try:
                 path = win32pdh.MakeCounterPath((machine_name, self._class_name, instance_name, None, 0, counter_name))
                 self.logger.debug("Successfully created English-only path")
             except Exception as e:  # noqa: E722
-                self.logger.warning("Unable to create English-only path %s" % str(e))
+                self.logger.warning("Unable to create English-only path %s", e)
                 raise
             return path
 
         counter_name_index_list = WinPDHCounter.pdh_counter_dict[counter_name]
 
         for index in counter_name_index_list:
             c = win32pdh.LookupPerfNameByIndex(None, int(index))
             if c is None or len(c) == 0:
-                self.logger.debug("Index %s not found, skipping" % index)
+                self.logger.debug("Index %s not found, skipping", index)
                 continue
 
             # check to see if this counter is in the list of counters for this class
             if c not in counters:
                 try:
-                    self.logger.debug("Index %s counter %s not in counter list" % (index, text_type(c)))
+                    self.logger.debug("Index %s counter %s not in counter list", index, text_type(c))
                 except:  # noqa: E722
                     # some unicode characters are not translatable here.  Don't fail just
                     # because we couldn't log
-                    self.logger.debug("Index %s not in counter list" % index)
+                    self.logger.debug("Index %s not in counter list", index)
 
                 continue
 
             # see if we can create a counter
             try:
                 path = win32pdh.MakeCounterPath((machine_name, self._class_name, instance_name, None, 0, c))
                 break
             except:  # noqa: E722
                 try:
-                    self.logger.info("Unable to make path with counter %s, trying next available" % text_type(c))
+                    self.logger.info("Unable to make path with counter %s, trying next available", text_type(c))
                 except:  # noqa: E722
-                    self.logger.info("Unable to make path with counter index %s, trying next available" % index)
+                    self.logger.info("Unable to make path with counter index %s, trying next available", index)
         return path
 
     def collect_counters(self):
         counters, instances = win32pdh.EnumObjectItems(
             None, self._machine_name, self._class_name, win32pdh.PERF_DETAIL_WIZARD
         )
         if self._instance_name is None and len(instances) > 0:
@@ -202,48 +202,49 @@
                 path = self._make_counter_path(self._machine_name, self._counter_name, inst, counters)
                 if not path:
                     continue
                 all_instances.add(inst)
 
                 try:
                     if inst not in self.counterdict:
-                        self.logger.debug('Adding instance `{}`'.format(inst))
+                        self.logger.debug('Adding instance `%s`', inst)
                         self.counterdict[inst] = win32pdh.AddCounter(self.hq, path)
                 except:  # noqa: E722
                     self.logger.fatal(
                         "Failed to create counter.  No instances of %s\\%s" % (self._class_name, self._counter_name)
                     )
 
             expired_instances = set(self.counterdict) - all_instances
             for inst in expired_instances:
-                self.logger.debug('Removing expired instance `{}`'.format(inst))
+                self.logger.debug('Removing expired instance `%s`', inst)
                 del self.counterdict[inst]
         else:
             if self._instance_name is not None:
                 # check to see that it's valid
                 if len(instances) <= 0:
                     self.logger.error(
-                        "%s doesn't seem to be a multi-instance counter, but asked for specific instance %s"
-                        % (self._class_name, self._instance_name)
+                        "%s doesn't seem to be a multi-instance counter, but asked for specific instance %s",
+                        self._class_name,
+                        self._instance_name,
                     )
                     raise AttributeError("%s is not a multi-instance counter" % self._class_name)
                 if self._instance_name not in instances:
-                    self.logger.error("%s is not a counter instance in %s" % (self._instance_name, self._class_name))
+                    self.logger.error("%s is not a counter instance in %s", self._instance_name, self._class_name)
                     raise AttributeError("%s is not an instance of %s" % (self._instance_name, self._class_name))
 
             path = self._make_counter_path(self._machine_name, self._counter_name, self._instance_name, counters)
             if not path:
                 self.logger.warning("Empty path returned")
             elif win32pdh.ValidatePath(path) != 0:
                 # Multi-instance counter with no instances presently
                 pass
             else:
                 try:
                     if SINGLE_INSTANCE_KEY not in self.counterdict:
-                        self.logger.debug('Adding single instance for path `{}`'.format(path))
+                        self.logger.debug('Adding single instance for path `%s`', path)
                         self.counterdict[SINGLE_INSTANCE_KEY] = win32pdh.AddCounter(self.hq, path)
                 except:  # noqa: E722
                     self.logger.fatal(
                         "Failed to create counter.  No instances of %s\\%s" % (self._class_name, self._counter_name)
                     )
                     raise
                 self._is_single_instance = True
```

## datadog_checks/base/data/agent_requirements.in

```diff
@@ -1,64 +1,70 @@
-adodbapi==2.6.0.7; sys_platform == 'win32'
-aerospike==3.6.0; sys_platform != 'win32'
-beautifulsoup4==4.5.1
-binary==1.0.0
-boto==2.46.1
-contextlib2==0.5.5
-cryptography==2.7
-cx-oracle==7.2.0
-ddtrace==0.13.0
-dnspython==1.16.0
-flup==1.0.3.dev-20110405; python_version < '3.0'
-flup-py3==1.0.3; python_version > '3.0'
-gearman==2.0.2; sys_platform != 'win32' and python_version < '3.0'
-httplib2==0.10.3
-in-toto==0.3.0
-ipaddress==1.0.22; python_version < '3.0'
-jaydebeapi==1.1.1
-jpype1==0.7.0
-kafka-python==1.4.7; sys_platform != 'win32'
-kazoo==2.6.1; sys_platform != 'win32'
-kubernetes==8.0.1
-ldap3==2.5
-lxml==4.4.1
-meld3==1.0.2
-openstacksdk==0.24.0
-paramiko==2.6.0
-ply==3.10
-prometheus-client==0.3.0
-protobuf==3.7.0
-psutil==5.6.3
-psycopg2-binary==2.8.4
-pyasn1==0.4.6
-pycryptodomex==3.8.2
-pymongo==3.8.0
-pymqi==1.8.0; sys_platform != 'win32' and sys_platform != 'darwin'
-pymysql==0.9.3
-pyodbc==4.0.26; sys_platform != 'darwin'
-pyro4==4.73; sys_platform == 'win32'
-pysmi==0.2.2
-pysnmp==4.4.3
-pysnmp-mibs==0.1.6
-pysocks==1.7.0
-python-binary-memcached==0.26.1; sys_platform != 'win32'
-python-dateutil==2.8.0
-python3-gearman==0.1.0; sys_platform != 'win32' and python_version > '3.0'
-pyvmomi==v6.5.0.2017.5-1
-pywin32==225; sys_platform == 'win32'
-pyyaml==5.1
-redis==2.10.5
-requests==2.22.0
-requests-kerberos==0.12.0
-requests_ntlm==1.1.0
-scandir==1.8
-securesystemslib[crypto,pynacl]==0.11.3
-selectors34==1.2.0; sys_platform == 'win32' and python_version < '3.4'
-serpent==1.27; sys_platform == 'win32'
-service_identity[idna]==18.1.0
-simplejson==3.6.5
-six==1.12.0
-supervisor==4.0.1
-tuf==0.11.2.dev3
-uptime==3.0.1
-vertica-python==0.9.4
-win-inet-pton==1.1.0; sys_platform == 'win32' and python_version < '3.0'
+adodbapi==2.6.0.7; sys_platform == 'win32'
+aerospike==3.6.0; sys_platform != 'win32'
+beautifulsoup4==4.5.1
+binary==1.0.0
+boto==2.46.1
+boto3==1.10.27
+clickhouse-cityhash==1.0.2.3
+clickhouse-driver==0.1.2
+contextlib2==0.5.5
+cryptography==2.8
+cx-oracle==7.2.0
+ddtrace==0.13.0
+dnspython==1.16.0
+flup==1.0.3.dev-20110405; python_version < '3.0'
+flup-py3==1.0.3; python_version > '3.0'
+gearman==2.0.2; sys_platform != 'win32' and python_version < '3.0'
+httplib2==0.10.3
+in-toto==0.4.1
+ipaddress==1.0.22; python_version < '3.0'
+jaydebeapi==1.1.1
+jpype1==0.7.0
+kafka-python==1.4.7; sys_platform != 'win32'
+kazoo==2.6.1; sys_platform != 'win32'
+kubernetes==8.0.1
+ldap3==2.5
+lxml==4.4.1
+lz4==2.2.1
+meld3==1.0.2
+openstacksdk==0.24.0
+paramiko==2.6.0
+ply==3.10
+prometheus-client==0.3.0
+protobuf==3.7.0
+psutil==5.6.5
+psycopg2-binary==2.8.4
+pyasn1==0.4.6
+pycryptodomex==3.8.2
+pyhdb==0.3.4
+pymongo==3.8.0
+pymqi==1.8.0; sys_platform != 'win32' and sys_platform != 'darwin'
+pymysql==0.9.3
+pyodbc==4.0.26; sys_platform != 'darwin'
+pyro4==4.73; sys_platform == 'win32'
+pysmi==0.2.2
+pysnmp==4.4.3
+pysnmp-mibs==0.1.6
+pysocks==1.7.0
+python-binary-memcached==0.26.1; sys_platform != 'win32'
+python-dateutil==2.8.0
+python3-gearman==0.1.0; sys_platform != 'win32' and python_version > '3.0'
+pyvmomi==v6.5.0.2017.5-1
+pywin32==227; sys_platform == 'win32'
+pyyaml==5.1
+redis==2.10.5
+requests==2.22.0
+requests-kerberos==0.12.0
+requests_ntlm==1.1.0
+scandir==1.8
+securesystemslib[crypto,pynacl]==0.12.2
+selectors34==1.2.0; sys_platform == 'win32' and python_version < '3.4'
+semver==2.9.0
+serpent==1.27; sys_platform == 'win32'
+service_identity[idna]==18.1.0
+simplejson==3.6.5
+six==1.12.0
+supervisor==4.0.1
+tuf==0.12.1
+uptime==3.0.1
+vertica-python==0.9.4
+win-inet-pton==1.1.0; sys_platform == 'win32' and python_version < '3.0'
```

## datadog_checks/base/stubs/__init__.py

```diff
@@ -1,7 +1,8 @@
 # (C) Datadog, Inc. 2018
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 from .aggregator import aggregator
+from .datadog_agent import datadog_agent
 from .tagging import tagger
 
 __all__ = ['aggregator', 'datadog_agent', 'tagger']
```

## datadog_checks/base/stubs/datadog_agent.py

```diff
@@ -1,43 +1,47 @@
 # (C) Datadog, Inc. 2018
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 
 
-def get_hostname():
-    return 'stubbed.hostname'
+class DatadogAgentStub(object):
+    def __init__(self):
+        self._metadata = {}
 
+    def reset(self):
+        self._metadata.clear()
 
-def log(*args, **kwargs):
-    pass
+    def assert_metadata(self, check_id, data):
+        actual = {}
+        for name in data:
+            key = (check_id, name)
+            if key in self._metadata:
+                actual[name] = self._metadata[key]
+        assert data == actual
 
+    def assert_metadata_count(self, count):
+        assert len(self._metadata) == count
 
-def get_config(*args, **kwargs):
-    return ''
+    def get_hostname(self):
+        return 'stubbed.hostname'
 
+    def get_config(self, *args, **kwargs):
+        return ''
 
-def get_version():
-    return '0.0.0'
+    def get_version(self):
+        return '0.0.0'
 
+    def log(self, *args, **kwargs):
+        pass
 
-def warning(msg, *args, **kwargs):
-    pass
+    def set_check_metadata(self, check_id, name, value):
+        self._metadata[(check_id, name)] = value
 
+    def set_external_tags(self, *args, **kwargs):
+        pass
 
-def error(msg, *args, **kwargs):
-    pass
+    def tracemalloc_enabled(self, *args, **kwargs):
+        return False
 
 
-def debug(msg, *args, **kwargs):
-    pass
-
-
-def set_check_metadata(*args, **kwargs):
-    pass
-
-
-def set_external_tags(*args, **kwargs):
-    pass
-
-
-def tracemalloc_enabled(*args, **kwargs):
-    return False
+# Use the stub as a singleton
+datadog_agent = DatadogAgentStub()
```

## datadog_checks/base/utils/common.py

```diff
@@ -1,17 +1,21 @@
 # (C) Datadog, Inc. 2018
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
+from __future__ import division
+
 import os
 import re
 from decimal import ROUND_HALF_UP, Decimal
 
 from six import PY3, iteritems, text_type
 from six.moves.urllib.parse import urlparse
 
+from .constants import MILLISECOND
+
 
 def ensure_bytes(s):
     if isinstance(s, text_type):
         s = s.encode('utf-8')
     return s
 
 
@@ -20,14 +24,31 @@
         s = s.decode('utf-8')
     return s
 
 
 to_string = ensure_unicode if PY3 else ensure_bytes
 
 
+def total_time_to_temporal_percent(total_time, scale=MILLISECOND):
+    # This is really confusing, sorry.
+    #
+    # We get the `total_time` in `scale` since the start and we want to compute a percentage.
+    # Since the time is monotonically increasing we can't just submit a point-in-time value but
+    # rather it needs to be temporally aware, thus we submit the value as a rate.
+    #
+    # If we submit it as-is, that would be `scale` per second but we need seconds per second
+    # since the Agent's check run interval is internally represented as seconds. Hence we divide
+    # by 1000, for example, if the `scale` is milliseconds.
+    #
+    # At this point we have a number that will be no greater than 1 when compared to the last run.
+    #
+    # To turn it into a percentage we multiply by 100.
+    return total_time / scale * 100
+
+
 def exclude_undefined_keys(mapping):
     return {key: value for key, value in iteritems(mapping) if value is not None}
 
 
 def round_value(value, precision=0, rounding_method=ROUND_HALF_UP):
     precision = '0.{}'.format('0' * precision)
     return float(Decimal(str(value)).quantize(Decimal(precision), rounding=rounding_method))
```

## datadog_checks/base/utils/http.py

```diff
@@ -1,24 +1,23 @@
 # (C) Datadog, Inc. 2019
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import logging
 import os
-import threading
-import warnings
 from contextlib import contextmanager
 
 import requests
 from six import iteritems, string_types
 from six.moves.urllib.parse import urlparse
 from urllib3.exceptions import InsecureRequestWarning
 
 from ..config import is_affirmative
 from ..errors import ConfigurationError
 from .headers import get_default_headers, update_headers
+from .warnings_util import disable_warnings_ctx
 
 try:
     from contextlib import ExitStack
 except ImportError:
     from contextlib2 import ExitStack
 
 try:
@@ -34,14 +33,15 @@
 
 # The timeout should be slightly larger than a multiple of 3,
 # which is the default TCP packet retransmission window. See:
 # https://tools.ietf.org/html/rfc2988
 DEFAULT_TIMEOUT = 10
 
 STANDARD_FIELDS = {
+    'auth_type': '',
     'connect_timeout': None,
     'extra_headers': None,
     'headers': None,
     'kerberos_auth': None,
     'kerberos_cache': None,
     'kerberos_delegate': False,
     'kerberos_force_initiate': False,
@@ -89,18 +89,14 @@
         'logger',
         'no_proxy_uris',
         'options',
         'persist_connections',
         'request_hooks',
     )
 
-    # For modifying the warnings filter since the context
-    # manager that is provided changes module constants
-    warning_lock = threading.Lock()
-
     def __init__(self, instance, init_config, remapper=None, logger=None):
         self.logger = logger or LOGGER
         default_fields = dict(STANDARD_FIELDS)
 
         # Update the default behavior for global settings
         default_fields['log_requests'] = init_config.get('log_requests', default_fields['log_requests'])
         default_fields['skip_proxy'] = init_config.get('skip_proxy', default_fields['skip_proxy'])
@@ -166,15 +162,22 @@
         if config['extra_headers']:
             update_headers(headers, config['extra_headers'])
 
         # http://docs.python-requests.org/en/master/user/authentication/
         auth = None
         if config['password']:
             if config['username']:
-                auth = (config['username'], config['password'])
+                auth_type = config.get('auth_type', 'basic').lower()
+                if auth_type == 'digest':
+                    auth = requests.auth.HTTPDigestAuth(config['username'], config['password'])
+                else:
+                    if auth_type != 'basic':
+                        self.logger.debug('auth_type %s is not supported, defaulting to basic', auth_type)
+                    auth = (config['username'], config['password'])
+
             elif config['ntlm_domain']:
                 ensure_ntlm()
 
                 auth = requests_ntlm.HttpNtlmAuth(config['ntlm_domain'], config['password'])
 
         if auth is None and config['kerberos_auth']:
             ensure_kerberos()
@@ -264,15 +267,17 @@
         self.persist_connections = is_affirmative(config['persist_connections'])
         self._session = None
 
         # Whether or not to log request information like method and url
         self.log_requests = is_affirmative(config['log_requests'])
 
         # Context managers that should wrap all requests
-        self.request_hooks = [self.handle_tls_warning]
+        self.request_hooks = []
+        if self.ignore_tls_warning:
+            self.request_hooks.append(self.handle_tls_warning)
 
         if config['kerberos_keytab']:
             self.request_hooks.append(lambda: handle_kerberos_keytab(config['kerberos_keytab']))
         if config['kerberos_cache']:
             self.request_hooks.append(lambda: handle_kerberos_cache(config['kerberos_cache']))
 
     def get(self, url, **options):
@@ -291,15 +296,15 @@
         return self._request('patch', url, options)
 
     def delete(self, url, **options):
         return self._request('delete', url, options)
 
     def _request(self, method, url, options):
         if self.log_requests:
-            self.logger.debug(u'Sending {} request to {}'.format(method.upper(), url))
+            self.logger.debug(u'Sending %s request to %s', method.upper(), url)
 
         if self.no_proxy_uris:
             parsed_uri = urlparse(url)
 
             for no_proxy_uri in self.no_proxy_uris:
                 if no_proxy_uri in parsed_uri.netloc:
                     options.setdefault('proxies', PROXY_SETTINGS_DISABLED)
@@ -327,21 +332,16 @@
             # Make explicitly set options take precedence
             options.setdefault(option, value)
 
         return options
 
     @contextmanager
     def handle_tls_warning(self):
-        with self.warning_lock:
-
-            with warnings.catch_warnings():
-                if self.ignore_tls_warning:
-                    warnings.simplefilter('ignore', InsecureRequestWarning)
-
-                yield
+        with disable_warnings_ctx(InsecureRequestWarning, disable=True):
+            yield
 
     @property
     def session(self):
         if self._session is None:
             self._session = requests.Session()
 
             # Attributes can't be passed to the constructor
```

## datadog_checks/base/utils/limiter.py

```diff
@@ -55,17 +55,15 @@
             self.seen.add(uid)
         else:
             self.count += 1
 
         if self.count > self.limit:
             if self.warning:
                 self.warning(
-                    "Check {} exceeded limit of {} {}, ignoring next ones".format(
-                        self.check_name, self.limit, self.name
-                    )
+                    "Check %s exceeded limit of %s %s, ignoring next ones", self.check_name, self.limit, self.name
                 )
             self.reached_limit = True
             return True
         return False
 
     def get_status(self):
         """
```

## datadog_checks/base/utils/subprocess_output.py

```diff
@@ -50,20 +50,19 @@
     elif hasattr(type(command), '__iter__'):
         for arg in command:
             cmd_args.append(arg)
     else:
         raise TypeError('command must be a sequence or string')
 
     if log_debug:
-        log.debug('Running get_subprocess_output with cmd: {}'.format(cmd_args))
+        log.debug('Running get_subprocess_output with cmd: %s', cmd_args)
 
     out, err, returncode = subprocess_output(cmd_args, raise_on_empty_output)
 
     log.debug(
-        'get_subprocess_output returned '
-        '(len(out): {} ; len(err): {} ; returncode: {})'.format(len(out), len(err), returncode)
+        'get_subprocess_output returned (len(out): %s ; len(err): %s ; returncode: %s)', len(out), len(err), returncode
     )
 
     out = ensure_unicode(out) if out is not None else None
     err = ensure_unicode(err) if err is not None else None
 
     return out, err, returncode
```

## datadog_checks/base/utils/tailfile.py

```diff
@@ -63,18 +63,18 @@
 
         self._inode = inode
         self._size = size
         self._crc = crc
 
         self._f = open(self._path, 'r')
         if move_end:
-            self._log.debug("Opening file %s" % (self._path))
+            self._log.debug("Opening file %s", self._path)
             self._f.seek(0, os.SEEK_END)
         elif pos:
-            self._log.debug("Reopening file %s at %s" % (self._path, pos))
+            self._log.debug("Reopening file %s at %s", self._path, pos)
             self._f.seek(pos)
 
         return True
 
     def tail(self, line_by_line=True, move_end=True):
         """Read line-by-line and run callback on each line.
         line_by_line: yield each time a callback has returned True
```

## datadog_checks/base/utils/metadata/core.py

```diff
@@ -63,15 +63,15 @@
         scheme is defined then it will default to semver.
 
         The scheme may be set to ``regex`` in which case a ``pattern`` must also be defined. Any matching named
         subgroups will then be sent as ``version.<GROUP_NAME>``. In this case, the check name will be used as
         the value of ``version.scheme`` unless ``final_scheme`` is also set, which will take precedence.
         """
         scheme, version_parts = parse_version(version, options)
-        if scheme == 'regex':
+        if scheme == 'regex' or scheme == 'parts':
             scheme = options.get('final_scheme', self.check_name)
 
         data = {'version.{}'.format(part_name): part_value for part_name, part_value in iteritems(version_parts)}
         data['version.raw'] = version
         data['version.scheme'] = scheme
 
         return data
```

## datadog_checks/base/utils/metadata/version.py

```diff
@@ -46,19 +46,27 @@
     parts = match.groupdict()
     if not parts:
         raise ValueError('Regular expression pattern has no named subgroups')
 
     return exclude_undefined_keys(parts)
 
 
+def parse_raw(version, options):
+    part_map = options.get('part_map')
+    if not part_map:
+        raise ValueError('Version scheme `parts` requires a `part_map` option')
+
+    return exclude_undefined_keys(part_map)
+
+
 def parse_version(version, options):
     scheme = options.get('scheme')
 
     if not scheme:
         scheme = 'semver'
     elif scheme not in SCHEMES:
         raise ValueError('Unsupported version scheme `{}`'.format(scheme))
 
     return scheme, SCHEMES[scheme](version, options)
 
 
-SCHEMES = {'semver': parse_semver, 'regex': parse_regex}
+SCHEMES = {'semver': parse_semver, 'regex': parse_regex, 'parts': parse_raw}
```

## Comparing `datadog_checks_base-9.5.0.dist-info/METADATA` & `datadog_checks_base-9.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-checks-base
-Version: 9.5.0
+Version: 9.6.0
 Summary: The Datadog Check Toolkit
 Home-page: https://github.com/DataDog/integrations-core
 Author: Datadog
 Author-email: packages@datadoghq.com
 License: BSD
 Keywords: datadog agent checks
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 Requires-Dist: prometheus-client (==0.3.0) ; extra == 'deps'
 Requires-Dist: protobuf (==3.7.0) ; extra == 'deps'
 Requires-Dist: pyyaml (==5.1) ; extra == 'deps'
 Requires-Dist: requests (==2.22.0) ; extra == 'deps'
 Requires-Dist: simplejson (==3.6.5) ; extra == 'deps'
 Requires-Dist: six (==1.12.0) ; extra == 'deps'
 Requires-Dist: uptime (==3.0.1) ; extra == 'deps'
-Requires-Dist: pywin32 (==225) ; (sys_platform == "win32") and extra == 'deps'
+Requires-Dist: pywin32 (==227) ; (sys_platform == "win32") and extra == 'deps'
 Provides-Extra: http
 Requires-Dist: pysocks (==1.7.0) ; extra == 'http'
 Requires-Dist: requests-kerberos (==0.12.0) ; extra == 'http'
 Requires-Dist: requests-ntlm (==1.1.0) ; extra == 'http'
 Requires-Dist: win-inet-pton (==1.1.0) ; (sys_platform == "win32" and python_version < "3.0") and extra == 'http'
 Provides-Extra: kube
 Requires-Dist: kubernetes (==8.0.1) ; extra == 'kube'
```

## Comparing `datadog_checks_base-9.5.0.dist-info/RECORD` & `datadog_checks_base-9.6.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 datadog_checks/__init__.py,sha256=kYU6AgQ9Vpl9kNatd6zwAG_RtjYKsLTVCWe_iFkClug,172
 datadog_checks/config.py,sha256=ZZ3z2qCwTlD_JY5JPNY7nsh2GgjPLKub0L7cWv1HtPw,190
 datadog_checks/errors.py,sha256=QqXUOzdYqnP6j0GyKTH24rp4-Wx1brKD10Lpav7dToI,149
 datadog_checks/log.py,sha256=JK1Py6fnVPTrKBMyZwrVx5llYTgA7wJcBhkola-nsUc,295
-datadog_checks/base/__about__.py,sha256=EiGcMK3SiZOahPjuE4U_EjOQ2NhLnJ0lCX83emL7KPQ,130
+datadog_checks/base/__about__.py,sha256=y9_gv_X5BV53er2PDKZ762n95Jk7ZbwQ6c-9sLOYafE,135
 datadog_checks/base/__init__.py,sha256=HM91TYvzC0noiMfCLPY9MRVxbO-gOGnMZOoxHEWOW24,889
 datadog_checks/base/config.py,sha256=Rn1UcP7JIeB0_8n8CUcRgZ3EVkOtThch2DVd40-mUVc,556
 datadog_checks/base/constants.py,sha256=WWHamjtQanuJpwoHe_iZeiCuYzwrWXqKELjTcHi0t84,228
-datadog_checks/base/ddyaml.py,sha256=9k3pJghlTT-sQL54R48jE0R40HxDpQbkBU5O7m5iSa4,4238
+datadog_checks/base/ddyaml.py,sha256=4HGJDrdztJBfwXIz3vQvs5Spsn7TGaQE7-OL4G3mVi4,4217
 datadog_checks/base/errors.py,sha256=TFTWMcvkfYAYFRVSPEokC0DNGXd9PHGIE7rLvm4Zn9E,329
 datadog_checks/base/log.py,sha256=rGQgO2s9yh8G9HxeE46TVryFo8xqd55nd2_Mqi87d6c,3475
 datadog_checks/base/checks/__init__.py,sha256=-4Bp0zml2LeZWj-QDZxhaoqHQTANIs6HlKpg4FhRH6k,425
-datadog_checks/base/checks/base.py,sha256=njSxLxaHr345FWMjHhxcVRGjfsjVYLu4pG_iadw8FO0,35126
+datadog_checks/base/checks/base.py,sha256=BYGfCoIQerYCnXso9DlcZEdXop7ejwXgw5qNy6T3kSg,35688
 datadog_checks/base/checks/network.py,sha256=dSQh7eDSUqB7mlMc3ou1xqBGIg1-ms3XMMW8Y0KdYqE,1960
 datadog_checks/base/checks/kube_leader/__init__.py,sha256=MurA-evnRU95x7jQbDm23XSBwuiQFQ9rfUhChryx4jk,327
 datadog_checks/base/checks/kube_leader/base_check.py,sha256=qbd8CopcGxDd6usk87T8fLOgWWkYcd7ZoVKb6vnOIRQ,700
-datadog_checks/base/checks/kube_leader/mixins.py,sha256=ncCwDSpC4aTSaR0lllr9-lJl0LFxovjoNaRFRBfT_Kg,4097
+datadog_checks/base/checks/kube_leader/mixins.py,sha256=DYPHwmxNQgzrPOtNcMprYqC1zd5054lK1ShwRxEZxNQ,4090
 datadog_checks/base/checks/kube_leader/record.py,sha256=4KuJ2TzhNAJBwsYH-veQ_sp4RQr6V41RoD5peSXZphQ,2715
 datadog_checks/base/checks/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datadog_checks/base/checks/libs/thread_pool.py,sha256=pIdm2kpcz1aMLYuwgm1JOr11Lb7ap1SCVcYPoNF9big,24477
 datadog_checks/base/checks/libs/timer.py,sha256=8N3YqS38ypA5GYrLIJKVZZiU1WS9uE-joGnUZpEO54E,577
 datadog_checks/base/checks/libs/vmware/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datadog_checks/base/checks/libs/vmware/all_metrics.py,sha256=JRf5kr0_iN2UmQl01Qzy-obNpMAs15xP-VhXG2kVukU,73070
 datadog_checks/base/checks/libs/vmware/basic_metrics.py,sha256=P1RhpNI_lFYq7LoMofX2qw1jp0xTdyhKhkIpVEgI7bc,3280
 datadog_checks/base/checks/openmetrics/__init__.py,sha256=aHaNSc2EZrwQsQsVW7aVKJMyuFpi1bjtQJG9YP71fJ8,190
-datadog_checks/base/checks/openmetrics/base_check.py,sha256=tXQRCMRXl2spcfkW0LtHdWCYlrbS5EiMG-WclyProi0,3405
-datadog_checks/base/checks/openmetrics/mixins.py,sha256=9imlwF9Gysi99m99ee9J_YoWwRwlh5c0foYJgYTPUlI,42842
+datadog_checks/base/checks/openmetrics/base_check.py,sha256=sqtyWdJSE1dUUfvgM2nPSs0e_ZC1fFzQa5bG2yo37Kw,3891
+datadog_checks/base/checks/openmetrics/mixins.py,sha256=OVwzzdsKBPWTp6whP9uW8fI5jp5eP9tCblGbjR87Pxw,42950
 datadog_checks/base/checks/prometheus/__init__.py,sha256=wEJnzqt6rx8HfJ-GnElBvzsfaAeMzo5avtBSZUjrE_Q,567
 datadog_checks/base/checks/prometheus/base_check.py,sha256=0hOeVpbplsdueAzMB80tHYfJwZZqW1kRxncNIbBtHTM,8362
-datadog_checks/base/checks/prometheus/mixins.py,sha256=YQXokotkcgadozFhw7R4_9qb4YLFUg7SzKVBvGOZtK0,32355
+datadog_checks/base/checks/prometheus/mixins.py,sha256=OXl_E_PhfhVUp_-dARHzFP7qwJshQtR-90H_6hPmjBc,32431
 datadog_checks/base/checks/prometheus/prometheus_base.py,sha256=bh-YYDfaGIIbSskNHJQPq4SwgQVtlMUqCFDD5hGiO5A,3903
 datadog_checks/base/checks/win/__init__.py,sha256=cPJG07oUrLjMM45d2TtM-om9u3PIqsPHp30Pc9qq2-I,403
-datadog_checks/base/checks/win/winpdh.py,sha256=bkEwMSzOqxTkc-w5jfu0xnT6AYAPgWagvpprlLcjT1o,10811
+datadog_checks/base/checks/win/winpdh.py,sha256=FXX7p4qkS5b2lkRd1ZyvneSJ95ImeKVZQNon8a98Dmw,10792
 datadog_checks/base/checks/win/winpdh_base.py,sha256=Iccn8QEG8B33KchONumQ6kMdL-WFBIvFWN79uhfnPpE,7294
 datadog_checks/base/checks/win/winpdh_stub.py,sha256=wRIhLsxlh_oKQGnjuSp81WfGxs0LhRK7u_PEm5rorA4,388
 datadog_checks/base/checks/win/wmi/__init__.py,sha256=J92ge4eWxtn-WNNeSn85U43cadrjhm6SppNOJNAwpLw,12614
 datadog_checks/base/checks/win/wmi/counter_type.py,sha256=dOH0U8OFywXSC2THW9fCr2dZDLrNK2j3_nAtSTCstAY,5767
 datadog_checks/base/checks/win/wmi/sampler.py,sha256=EQGN3njdSM9EaHbQ33yWjUcqhE5HVYKLdK8eZyePI9I,18968
-datadog_checks/base/data/agent_requirements.in,sha256=GTlIE-SFNRy9jSGu3_yu7vlus9mQAXd8ID1lBkOPbPk,1757
-datadog_checks/base/stubs/__init__.py,sha256=SaA5loRN3t4wUnGVqPCOjSr5wdxwZTwLS50oZ92L6CI,223
+datadog_checks/base/data/agent_requirements.in,sha256=9KlhIJGCP-q6IXYwsfjtssId6y0mGW2nUZCvcOChYHw,1795
+datadog_checks/base/stubs/__init__.py,sha256=oloxeDLvOXK4pFyDEWbsYF0NlCukguEsBgeKNIM-5xY,264
 datadog_checks/base/stubs/_util.py,sha256=P43M85RLTYT-Fyr2RoItvqYYW4_NDkQyaGIV69BLGGg,1169
 datadog_checks/base/stubs/aggregator.py,sha256=eKPvPfDiEueheKhx75dhqAvEwjFAtWx2RmR2z4frRuc,15907
 datadog_checks/base/stubs/common.py,sha256=PxiJup93xZOnwRdfyADbxcTjFwmlBHbSggn8CVvYxHo,468
-datadog_checks/base/stubs/datadog_agent.py,sha256=eWbyeDCg6nDSHlXqCY0XE_-gWCA1LwBzO9V5UUR9V9Y,583
+datadog_checks/base/stubs/datadog_agent.py,sha256=PC307VnexujqlOboe8cGEVB5H3eDx8r55_f4CMPKlsI,1121
 datadog_checks/base/stubs/log.py,sha256=okNzs2bRAdE-anpnLulCfdNl5sXpwApPbjsMlrUX-gE,828
 datadog_checks/base/stubs/similar.py,sha256=zZ1bq5wPaQ-8cBY_HS-612spFR3UJ3vyFAaXVsGccBM,5867
 datadog_checks/base/stubs/tagging.py,sha256=ENSKyyMRi5MnKDbnvX9hY0BOL7DTxhCwdUPKZ3yCTnI,1431
 datadog_checks/base/utils/__init__.py,sha256=6UbUAtpaou6_tVpv-oIHxBOYIuIQsFs3FR3t5wWMkTs,346
-datadog_checks/base/utils/common.py,sha256=GHmOxBJgNU0037CBMax5Su-y82HMpdm8HasBe7CkNZ8,1964
+datadog_checks/base/utils/common.py,sha256=3Zx4DugGpld9eoL77k5xhjVNgWhD3BW5gt1wTZOJ3G0,2877
+datadog_checks/base/utils/constants.py,sha256=iA-n9FY3SuTKT14aNfTkVT5sATC3CoeqlY_A31skwYk,298
 datadog_checks/base/utils/containers.py,sha256=WbPR7CltQ449uS9Az5kFtpdPCOLLDcar8Bspp7aX3P4,881
 datadog_checks/base/utils/date.py,sha256=JJmqP84CgVcFJ0cvAmMu8EtM6v96tIESucQNm9eKeEc,2780
 datadog_checks/base/utils/headers.py,sha256=V5lM1NA-_jeEPFnfKE0GZO2g9MCv4P5XgDBA8pALPWM,1305
-datadog_checks/base/utils/http.py,sha256=-CSMusl-qDK_1AAD90iQTK7Z9AbH_AMFbp_yzc6xpuo,14229
-datadog_checks/base/utils/limiter.py,sha256=HHrdmJMYYMCGYct6m98Cpdi6EOj4Pki1TIU336bjRO0,2559
+datadog_checks/base/utils/http.py,sha256=yq1HInKGDoOAIl-oqyaEoApLWp4yrYjZzQVbsso4oHs,14440
+datadog_checks/base/utils/limiter.py,sha256=-xamq0wAn1KdC-N1e2gLs4B8FeJ4Phbu2sSyekzpaX0,2506
 datadog_checks/base/utils/platform.py,sha256=v80hcADsQ4E-l3ePoWGNe54bHeEMfFWidcZyCTLMxHQ,2497
 datadog_checks/base/utils/proxy.py,sha256=EIqMBcxQelV4wrWji8N69qE_ZJlsVroFNuh93C7qjKE,1280
-datadog_checks/base/utils/subprocess_output.py,sha256=U78L4ifERcA3aienWyLXU19d8y8BJAcQ8wnDotw5ZHA,2610
+datadog_checks/base/utils/subprocess_output.py,sha256=LvBvLAZNKWtPA9wQ79UgfKuhIaDY4LzRyUslFg76bsQ,2585
 datadog_checks/base/utils/tagging.py,sha256=i7j6B73iD5P0kbHKxCoSooJi1RoujIkjEYm8I43VUac,190
-datadog_checks/base/utils/tailfile.py,sha256=7xFBkA84UXxhZs_4s5lqsHGpW9pOEfJH7B3CGVY3Agg,3500
+datadog_checks/base/utils/tailfile.py,sha256=N_bM5szJFno9qArGGYIt8RzuZ5CnMqL1o4dvSbO6Nv8,3494
 datadog_checks/base/utils/timeout.py,sha256=YqikRCgXrtYwTxOC11avp_287IJRjb8WXWhF2tbZnHY,2014
 datadog_checks/base/utils/tracing.py,sha256=O8olet53uTYI6XH9tynGkln3P74QePOYHpxaRF94TDc,841
+datadog_checks/base/utils/warnings_util.py,sha256=lnfWtio70KYRudlnwqz80xpumt8h6lmZFmZYXvktyRw,962
 datadog_checks/base/utils/agent/__init__.py,sha256=c_Os0bocBwxPiqT5avfJBQepGJ_khNTVfTljh-5R5Uo,107
 datadog_checks/base/utils/agent/common.py,sha256=NFWP8N64PCnVviiS9FlKWsqFOOG_eF1pfY8IPZFal_A,158
 datadog_checks/base/utils/agent/debug.py,sha256=3upVyU0tjChsXb20xP8z6yu19vXXrOeLZjLy6Dp362k,2266
 datadog_checks/base/utils/agent/memory.py,sha256=79Lf0YPfbLejUHXiZMvBscsMWQ-ADb0Y93bNyySHcQQ,10506
 datadog_checks/base/utils/agent/packages.py,sha256=AcOVVNWS-b7nXpexkOYxmEZpVOl_eWc9EYv6A0vH9O4,500
 datadog_checks/base/utils/agent/utils.py,sha256=_RLlLMP7Vaq0fMiKmj3OpXgFXuQmkB3dXp7NhaxOi2o,891
+datadog_checks/base/utils/db/__init__.py,sha256=-qQ3L35Q9N78g8TB6mw1zOhQAXiOp2QgHVMF8fq6lsM,163
+datadog_checks/base/utils/db/core.py,sha256=3YvAp7J-IvOMap4-TxJFJ4k7aHo-6BlGSLzWOFGbDn4,4541
+datadog_checks/base/utils/db/query.py,sha256=pW3JUT-jfbTh6-49-tLxSU1BuJ6meAwDyeU1tp7kBto,4237
+datadog_checks/base/utils/db/transform.py,sha256=_lZmdCc_RxqbVRJG_yAbc_pkxQUOQuP6HtGBNCPnQPs,4322
+datadog_checks/base/utils/db/utils.py,sha256=ZWJ-qlr8mSCDYBXw62EaCiqclx2j5OqoG7erN1DFxnk,487
 datadog_checks/base/utils/metadata/__init__.py,sha256=AHcz7fimnrlZEcQzmIk5y-N2_IkEbUrRAPzuw0_yQDg,141
 datadog_checks/base/utils/metadata/constants.py,sha256=zxEI018tsz-5rdKXPxaB5i23BK1A-DjzGqT68yJpYeU,456
-datadog_checks/base/utils/metadata/core.py,sha256=PNTaIJNBDLncYHelSYkJ_T657FEb2zFHH9x0DoOCE58,6329
+datadog_checks/base/utils/metadata/core.py,sha256=6Lz3VxINp03zti_8LPLpRjz73FW18-ttMO8zX14ttFc,6350
 datadog_checks/base/utils/metadata/utils.py,sha256=n9NHE4mlfJ_3K4_vmEf9ryYkYJ31shuMEyOXOM5QwFE,373
-datadog_checks/base/utils/metadata/version.py,sha256=v8lxnjoO6phcR3sNP0HHIdtXS0L3OQrrUTYowboYLW4,1677
+datadog_checks/base/utils/metadata/version.py,sha256=5iDTme1b92U0SQWEotRJRjHnISaW76LcdnEXdtqjZyE,1917
 datadog_checks/base/utils/prometheus/__init__.py,sha256=ZVXmao3b38aRYB407hRoR27UXVj_fA3mS-vN-nPNPLg,159
 datadog_checks/base/utils/prometheus/functions.py,sha256=WTCRgpJ2SbvWf_kRX3pnKscRk62Jq98yo9QcB_wrkRg,1032
 datadog_checks/base/utils/prometheus/metrics_pb2.py,sha256=CVPPeyjo1fHUuXUmqySD72-YWhLwkaGjzBHefe6_Nsk,25002
 datadog_checks/checks/__init__.py,sha256=WuwRwBCWsqk6L-Fpk9Fq-68JlAITIp8_scs5hSQrvvc,211
 datadog_checks/checks/base.py,sha256=xT-t_xVs22lO14IlGmy2MpPZiILpsiWSOxi6X4mUYzQ,155
 datadog_checks/checks/network.py,sha256=Rp3-Utj7uzwz0gI1NC7rzkEik-ALpFlZujmccyMkEGc,183
 datadog_checks/checks/network_checks.py,sha256=HAAQhzI7q3ZYgdMD-BxYEv9iulLHpyVlevHFmsR-u58,300
@@ -115,11 +122,11 @@
 datadog_checks/utils/subprocess_output.py,sha256=rThDnMBs-qsxfl8Zn5qhOmfOe91P5voI_fTYnEZhDGk,167
 datadog_checks/utils/tailfile.py,sha256=82EgNicU5gfCP-upkXyfA93WbdC-p6ByzSjkiaFGsmI,158
 datadog_checks/utils/timeout.py,sha256=SfYg7yP8816YuORsKtZtvVSEd2awkIbEoHU-ba_TUyA,157
 datadog_checks/utils/tracing.py,sha256=9_xW-Cgavl_7uG7dhNp3tjJElc_X27eMnTtby9WCI1Y,151
 datadog_checks/utils/prometheus/__init__.py,sha256=46y-E1dqj4yefKYm5GWQ-Sgbhn7RO68VjKOh5HuBoDk,155
 datadog_checks/utils/prometheus/functions.py,sha256=pS0WtDAaxuElUGmppXH3d8WXJquYnDTndtGngeWQWk0,191
 datadog_checks/utils/prometheus/metrics_pb2.py,sha256=xf-IFi129qorec76EeJiXf8CJAqaJh1KMt9SBHCH9tU,167
-datadog_checks_base-9.5.0.dist-info/METADATA,sha256=ONNTuF31i9dGeYNi6MiuqkmCQszaO4UeGOg73VbPoMU,3399
-datadog_checks_base-9.5.0.dist-info/WHEEL,sha256=05Ahrak1u2K61DpLp9CDNSbUImLTITCMom_cqTFk6pE,116
-datadog_checks_base-9.5.0.dist-info/top_level.txt,sha256=lMOu0E4SYA9dF8PuBOreOD0EiE7Y356RW3Zwr8MCSBI,15
-datadog_checks_base-9.5.0.dist-info/RECORD,,
+datadog_checks_base-9.6.0.dist-info/METADATA,sha256=XC6O6rNWFMq81LVpDn7dT4e77tPLJa4ACsOCza_03jY,3399
+datadog_checks_base-9.6.0.dist-info/WHEEL,sha256=JZXtYepZFsf4IoivNpnSgKIc4qTHan08DRd56koo_DM,116
+datadog_checks_base-9.6.0.dist-info/top_level.txt,sha256=lMOu0E4SYA9dF8PuBOreOD0EiE7Y356RW3Zwr8MCSBI,15
+datadog_checks_base-9.6.0.dist-info/RECORD,,
```

