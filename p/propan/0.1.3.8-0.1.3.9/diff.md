# Comparing `tmp/propan-0.1.3.8.tar.gz` & `tmp/propan-0.1.3.9.tar.gz`

## Comparing `propan-0.1.3.8.tar` & `propan-0.1.3.9.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.8/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/gen_py_code.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/grpc_encoding.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/message.proto
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/__about__.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/__main__.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/py.typed
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/app.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/nats.py
--rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/redis.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/sqs.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/context/main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.8/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.8/LICENSE
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.8/README.md
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 propan-0.1.3.8/pyproject.toml
--rw-r--r--   0        0        0    17608 2020-02-02 00:00:00.000000 propan-0.1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.9/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/gen_py_code.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/grpc_encoding.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/message.proto
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/__about__.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/__main__.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/py.typed
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    11988 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/app.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/nats.py
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/redis.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/sqs.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.9/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.9/LICENSE
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.9/README.md
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 propan-0.1.3.9/pyproject.toml
+-rw-r--r--   0        0        0    17672 2020-02-02 00:00:00.000000 propan-0.1.3.9/PKG-INFO
```

### Comparing `propan-0.1.3.8/CONTRIBUTING.md` & `propan-0.1.3.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/SECURITY.md` & `propan-0.1.3.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.3.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.3.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.3.9/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/.github/workflows/documentation.yml` & `propan-0.1.3.9/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/.github/workflows/publish_coverage.yml` & `propan-0.1.3.9/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/.github/workflows/publish_pypi.yml` & `propan-0.1.3.9/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/.github/workflows/tests.yml` & `propan-0.1.3.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/3_lifespan_events.py` & `propan-0.1.3.9/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/4_cli_attributes_promotion.py` & `propan-0.1.3.9/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/5_publishing.py` & `propan-0.1.3.9/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/6_arguments_casting.py` & `propan-0.1.3.9/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/7_handler_errors_processing.py` & `propan-0.1.3.9/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/dependencies/1_dependency_injection.py` & `propan-0.1.3.9/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.3.9/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.3.9/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.3.9/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.3.9/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/dependencies/7_annotated.py` & `propan-0.1.3.9/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/grpc/grpc_encoding.py` & `propan-0.1.3.9/examples/grpc/grpc_encoding.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.3.9/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.3.9/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.3.9/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.3.9/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/http_frameworks_integrations/quart.py` & `propan-0.1.3.9/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.3.9/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.3.9/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/rabbit/direct.py` & `propan-0.1.3.9/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/rabbit/fanout.py` & `propan-0.1.3.9/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/rabbit/header.py` & `propan-0.1.3.9/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/rabbit/topic.py` & `propan-0.1.3.9/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/redis/direct.py` & `propan-0.1.3.9/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/examples/redis/pattern.py` & `propan-0.1.3.9/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/__about__.py` & `propan-0.1.3.9/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.3.8"
+__version__ = "0.1.3.9"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.3.8/propan/__init__.py` & `propan-0.1.3.9/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/annotations.py` & `propan-0.1.3.9/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/types.py` & `propan-0.1.3.9/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/__init__.py` & `propan-0.1.3.9/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/channels.py` & `propan-0.1.3.9/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/info.py` & `propan-0.1.3.9/propan/asyncapi/info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib.util
 from typing import Optional
 
 from pydantic import BaseModel, Field, HttpUrl
 
 if importlib.util.find_spec("email_validator"):
     from pydantic import EmailStr
-else:
+else:  # pragma: no cover
     EmailStr = str  # type: ignore
 
 
 class AsyncAPIContact(BaseModel):
     name: str
     url: HttpUrl
     email: Optional[EmailStr] = None
```

### Comparing `propan-0.1.3.8/propan/asyncapi/main.py` & `propan-0.1.3.9/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/message.py` & `propan-0.1.3.9/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/security.py` & `propan-0.1.3.9/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/subscription.py` & `propan-0.1.3.9/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/bindings/amqp.py` & `propan-0.1.3.9/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/bindings/kafka.py` & `propan-0.1.3.9/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/bindings/main.py` & `propan-0.1.3.9/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/asyncapi/bindings/redis.py` & `propan-0.1.3.9/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/push_back_watcher.py` & `propan-0.1.3.9/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/_model/broker_usecase.py` & `propan-0.1.3.9/propan/brokers/_model/broker_usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,14 @@
         async def wrapper(message: PropanMessage[MsgType]) -> T:
             if decoder is not None:
                 msg = await decoder(message, self._decode_message)
             else:
                 msg = await self._decode_message(message)
 
             message.decoded_body = msg
-
             if _raw is True:
                 return await func(message)
 
             elif is_unwrap is True and isinstance(msg, Mapping):
                 return await func(**msg)
 
             else:
```

### Comparing `propan-0.1.3.8/propan/brokers/_model/schemas.py` & `propan-0.1.3.9/propan/brokers/_model/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,21 +49,15 @@
             response_model: Type[BaseModel] = dependant.response_model
             return_field = list(response_model.__fields__.values())[0]
 
             if (
                 return_field.annotation != Any  # NOTE: 3.7-3.10 compatibility
                 and issubclass(return_field.annotation, BaseModel)
             ):
-                response_model = return_field.annotation
-
-                schema_extra = response_model.Config.schema_extra
-                if not isinstance(schema_extra, dict) or not schema_extra.get(
-                    "example"
-                ):
-                    response_model = add_example_to_model(response_model)
+                response_model = add_example_to_model(return_field.annotation)
 
                 return_info = jsonref.replace_refs(
                     response_model.schema(), jsonschema=True, proxies=False
                 )
                 return_info["examples"] = [return_info.pop("example", None)]
 
             else:
@@ -84,59 +78,48 @@
         else:
             return_info = None
 
         payload_title = f"{self.title}Payload"
         params = dependant.flat_params
         params_number = len(params)
 
-        gen_examples: bool
         use_original_model = False
         if params_number == 0:
             model = None
 
         elif params_number == 1:
             name, param = list(params.items())[0]
             info = getattr(param, "field_info", param)
 
-            if (
-                param.annotation != Any  # NOTE: 3.7-3.10 compatibility
-                and issubclass(param.annotation, BaseModel)
+            if param.annotation != Any and issubclass(  # NOTE: 3.7-3.10 compatibility
+                param.annotation, BaseModel
             ):
                 model = param.annotation
-
-                schema_extra = model.Config.schema_extra
-                if isinstance(schema_extra, dict):
-                    gen_examples = schema_extra.get("example") is None
-                else:
-                    gen_examples = True
-
                 use_original_model = True
 
             else:
                 model = create_model(  # type: ignore
                     info.title or payload_title,
                     **{name: (param.annotation, info)},
                 )
-                gen_examples = True
+
         else:
             model = create_model(  # type: ignore
                 payload_title,
                 **{
                     i: (j.annotation, getattr(j, "field_info", j))
                     for i, j in params.items()
                 },
             )
-            gen_examples = True
 
         body: AnyDict
         if model is None:
             body = {"title": payload_title, "type": "null"}
         else:
-            if gen_examples is True:
-                model = add_example_to_model(model)
+            model = add_example_to_model(model)
             body = jsonref.replace_refs(model.schema(), jsonschema=True, proxies=False)
 
         body.pop("definitions", None)
         if return_info is not None:
             return_info.pop("definitions", None)
 
         if params_number == 1 and not use_original_model:
```

### Comparing `propan-0.1.3.8/propan/brokers/_model/utils.py` & `propan-0.1.3.9/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.3.9/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.3.9/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/kafka/schemas.py` & `propan-0.1.3.9/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/nats/nats_broker.py` & `propan-0.1.3.9/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.3.9/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.3.9/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/nats/schemas.py` & `propan-0.1.3.9/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/rabbit/schemas.py` & `propan-0.1.3.9/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/redis/redis_broker.py` & `propan-0.1.3.9/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.3.9/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/redis/schemas.py` & `propan-0.1.3.9/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/sqs/schema.py` & `propan-0.1.3.9/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.3.9/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.3.9/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/app.py` & `propan-0.1.3.9/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/main.py` & `propan-0.1.3.9/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/docs/app.py` & `propan-0.1.3.9/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/docs/gen.py` & `propan-0.1.3.9/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/docs/serving.py` & `propan-0.1.3.9/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/startproject/core.py` & `propan-0.1.3.9/propan/cli/startproject/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from pathlib import Path
 
+from fast_depends._compat import PYDANTIC_V2
+
 from propan.__about__ import __version__
 from propan.cli.startproject.utils import touch_dir, write_file
 
 
 def create_project_dir(dirname: Path, version: str) -> Path:
     project_dir = touch_dir(dirname)
     create_readme(project_dir)
@@ -52,14 +54,15 @@
 
 
 def create_requirements(project_dir: Path, version: str) -> None:
     write_file(
         project_dir / "requirements.txt",
         f"{version}=={__version__}",
         "python-dotenv",
+        "pydantic-settings>=2.0a1" if PYDANTIC_V2 else "",
     )
 
 
 def create_env(config_dir: Path, url: str) -> None:
     write_file(
         config_dir / ".env",
         "APP_DEBUG=True",
@@ -77,15 +80,18 @@
     config_dir = touch_dir(config)
 
     write_file(
         config_dir / "settings.py",
         "from pathlib import Path",
         "from typing import Optional",
         "",
-        "from pydantic import BaseSettings, BaseModel, Field",
+        "from pydantic import BaseModel, Field",
+        "from pydantic_settings import BaseSettings"
+        if PYDANTIC_V2
+        else "from pydantic import BaseSettings",
         "",
         "",
         "CONFIG_DIR = Path(__file__).resolve().parent",
         "BASE_DIR = CONFIG_DIR.parent",
         "",
         "",
         *broker_settings,
```

### Comparing `propan-0.1.3.8/propan/cli/startproject/async_app/app.py` & `propan-0.1.3.9/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/startproject/async_app/core.py` & `propan-0.1.3.9/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.3.9/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/startproject/async_app/nats.py` & `propan-0.1.3.9/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.3.9/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/startproject/async_app/redis.py` & `propan-0.1.3.9/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.3.9/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/supervisors/basereload.py` & `propan-0.1.3.9/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/supervisors/multiprocess.py` & `propan-0.1.3.9/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/supervisors/utils.py` & `propan-0.1.3.9/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/supervisors/watchfiles.py` & `propan-0.1.3.9/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/utils/imports.py` & `propan-0.1.3.9/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/utils/logs.py` & `propan-0.1.3.9/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/cli/utils/parser.py` & `propan-0.1.3.9/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/__init__.py` & `propan-0.1.3.9/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/core/route.py` & `propan-0.1.3.9/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/core/router.py` & `propan-0.1.3.9/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/kafka/router.pyi` & `propan-0.1.3.9/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/nats/router.pyi` & `propan-0.1.3.9/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/rabbit/router.pyi` & `propan-0.1.3.9/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/redis/router.pyi` & `propan-0.1.3.9/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/fastapi/sqs/router.pyi` & `propan-0.1.3.9/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/log/formatter.py` & `propan-0.1.3.9/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/log/logging.py` & `propan-0.1.3.9/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/test/__init__.py` & `propan-0.1.3.9/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/test/kafka.py` & `propan-0.1.3.9/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/test/nats.py` & `propan-0.1.3.9/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/test/rabbit.py` & `propan-0.1.3.9/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/test/redis.py` & `propan-0.1.3.9/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/test/sqs.py` & `propan-0.1.3.9/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/test/utils.py` & `propan-0.1.3.9/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/utils/functions.py` & `propan-0.1.3.9/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/utils/context/main.py` & `propan-0.1.3.9/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/propan/utils/context/types.py` & `propan-0.1.3.9/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/LICENSE` & `propan-0.1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/README.md` & `propan-0.1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.8/pyproject.toml` & `propan-0.1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "fast-depends==2.0.2",
+    "fast-depends>=2.0.3",
     "watchfiles",
     "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
 
@@ -75,15 +75,15 @@
 
 async-kafka = [
     "aiokafka>=0.8",
 ]
 
 doc = [
     "PyYAML",
-    "pydantic[email]",
+    "email-validator>=2.0.0",
     "polyfactory>=2.3.0; python_version > '3.7'",
     "jsonref",
     "fastapi",
     "uvicorn",
 ]
 
 async-sqs = [
@@ -97,14 +97,15 @@
     "propan[async-redis]",
     "propan[async-kafka]",
     "propan[async-sqs]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
+    "pydantic-settings>=2.0a1",
 
     "fastapi==0.100.0b1",
     "python-dotenv",
 
     "asyncmock; python_version < '3.8'",
 ]
```

### Comparing `propan-0.1.3.8/PKG-INFO` & `propan-0.1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -31,15 +31,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: fast-depends==2.0.2
+Requires-Dist: fast-depends>=2.0.3
 Requires-Dist: typer
 Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles
 Provides-Extra: async-kafka
 Requires-Dist: aiokafka>=0.8; extra == 'async-kafka'
 Provides-Extra: async-nats
 Requires-Dist: nats-py!=2.3.0,>=2; extra == 'async-nats'
@@ -63,30 +63,31 @@
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'dev-doc'
 Requires-Dist: mkdocs-glightbox; extra == 'dev-doc'
 Requires-Dist: mkdocs-macros-plugin; extra == 'dev-doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'dev-doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'dev-doc'
 Requires-Dist: typer[all]; extra == 'dev-doc'
 Provides-Extra: doc
+Requires-Dist: email-validator>=2.0.0; extra == 'doc'
 Requires-Dist: fastapi; extra == 'doc'
 Requires-Dist: jsonref; extra == 'doc'
 Requires-Dist: polyfactory>=2.3.0; python_version > '3.7' and extra == 'doc'
-Requires-Dist: pydantic[email]; extra == 'doc'
 Requires-Dist: pyyaml; extra == 'doc'
 Requires-Dist: uvicorn; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: fastapi==0.100.0b1; extra == 'test'
 Requires-Dist: propan[async-kafka]; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: propan[async-redis]; extra == 'test'
 Requires-Dist: propan[async-sqs]; extra == 'test'
 Requires-Dist: propan[doc]; extra == 'test'
+Requires-Dist: pydantic-settings>=2.0a1; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
 Requires-Dist: pytest>=7; extra == 'test'
 Requires-Dist: python-dotenv; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://lancetnik.github.io/Propan/" target="_blank">
```

