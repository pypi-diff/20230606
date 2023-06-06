# Comparing `tmp/propan-0.1.2.8.tar.gz` & `tmp/propan-0.1.2.9.tar.gz`

## Comparing `propan-0.1.2.8.tar` & `propan-0.1.2.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.8/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/__about__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/__main__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/py.typed
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/app.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/nats.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/redis.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/sqs.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.2.8/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.8/LICENSE
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.8/README.md
--rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.8/pyproject.toml
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.9/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/__about__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/__main__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/py.typed
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/app.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/nats.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/redis.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/sqs.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.2.9/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.9/LICENSE
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.9/README.md
+-rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 propan-0.1.2.9/pyproject.toml
+-rw-r--r--   0        0        0    16155 2020-02-02 00:00:00.000000 propan-0.1.2.9/PKG-INFO
```

### Comparing `propan-0.1.2.8/CONTRIBUTING.md` & `propan-0.1.2.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/SECURITY.md` & `propan-0.1.2.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.2.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.2.9/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/.github/workflows/documentation.yml` & `propan-0.1.2.9/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/.github/workflows/publish_coverage.yml` & `propan-0.1.2.9/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/.github/workflows/publish_pypi.yml` & `propan-0.1.2.9/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/.github/workflows/tests.yml` & `propan-0.1.2.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/3_lifespan_events.py` & `propan-0.1.2.9/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.9/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/5_publishing.py` & `propan-0.1.2.9/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/6_arguments_casting.py` & `propan-0.1.2.9/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/7_handler_errors_processing.py` & `propan-0.1.2.9/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.9/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.9/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.9/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.9/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.9/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/dependencies/7_annotated.py` & `propan-0.1.2.9/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.9/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.9/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.9/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.9/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.9/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.9/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.9/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/rabbit/direct.py` & `propan-0.1.2.9/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/rabbit/fanout.py` & `propan-0.1.2.9/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/rabbit/header.py` & `propan-0.1.2.9/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/rabbit/topic.py` & `propan-0.1.2.9/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/redis/direct.py` & `propan-0.1.2.9/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/examples/redis/pattern.py` & `propan-0.1.2.9/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/__about__.py` & `propan-0.1.2.9/propan/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.2.8"
+__version__ = "0.1.2.9"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.2.8/propan/__init__.py` & `propan-0.1.2.9/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/annotations.py` & `propan-0.1.2.9/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/types.py` & `propan-0.1.2.9/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/push_back_watcher.py` & `propan-0.1.2.9/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/_model/broker_usecase.py` & `propan-0.1.2.9/propan/brokers/_model/broker_usecase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 import json
 import logging
 from abc import ABC, abstractmethod
 from functools import wraps
-from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
+from fast_depends.construct import get_dependant
+from fast_depends.model import Dependant
+from pydantic.fields import ModelField
 from typing_extensions import Self
 
 from propan.brokers._model.schemas import (
     ContentType,
     ContentTypes,
     PropanMessage,
     SendableModel,
@@ -160,20 +175,26 @@
     def _wrap_handler(
         self,
         func: AnyCallable,
         retry: Union[bool, int] = False,
         _raw: bool = False,
         **broker_args: Any,
     ) -> DecoratedAsync:
+        dependant: Dependant = get_dependant(path="", call=func)
+
         f = to_async(func)
 
         if self._is_apply_types is True:
             f = apply_types(f)
 
-        f = self._wrap_decode_message(f, _raw=_raw)
+        f = self._wrap_decode_message(
+            f,
+            _raw=_raw,
+            params=dependant.real_params,
+        )
 
         if self.logger is not None:
             f = self._log_execution(**broker_args)(f)
 
         f = self._process_message(f, get_watcher(self.logger, retry))
 
         f = self._wrap_parse_message(f)
@@ -183,27 +204,34 @@
         f = suppress_decor(f)
 
         return f
 
     def _wrap_decode_message(
         self,
         func: Callable[..., Awaitable[T]],
+        params: Sequence[ModelField] = (),
         _raw: bool = False,
     ) -> Callable[[PropanMessage], Awaitable[T]]:
         decode: Callable[
             [PropanMessage], Awaitable[Union[PropanMessage, DecodedMessage]]
         ]
         if _raw is True:
             decode = _fake_decode
         else:
             decode = self._decode_message
 
+        is_unwrap = len(params) > 1
+
         @wraps(func)
         async def wrapper(message: PropanMessage) -> T:
-            return await func(await decode(message))
+            msg = await decode(message)
+            if is_unwrap is True and isinstance(msg, Mapping):
+                return await func(**msg)
+            else:
+                return await func(msg)
 
         return wrapper
 
     def _wrap_parse_message(
         self, func: Callable[[PropanMessage], Awaitable[T]]
     ) -> Callable[[Any], Awaitable[T]]:
         @wraps(func)
```

### Comparing `propan-0.1.2.8/propan/brokers/_model/schemas.py` & `propan-0.1.2.9/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/_model/utils.py` & `propan-0.1.2.9/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.9/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.9/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.9/propan/brokers/nats/nats_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,20 @@
     handlers: List[Handler]
     _connection: Optional[Client]
 
     __max_queue_len: int
     __max_subject_len: int
     __is_connected: bool
 
-    def __init__(self, *args: Any, log_fmt: Optional[str] = None, **kwargs: AnyDict):
+    def __init__(
+        self,
+        *args: Any,
+        log_fmt: Optional[str] = None,
+        **kwargs: AnyDict,
+    ):
         super().__init__(*args, log_fmt=log_fmt, **kwargs)
 
         self._connection = None
 
         self.__max_queue_len = 0
         self.__max_subject_len = 4
         self.__is_connected = True
```

### Comparing `propan-0.1.2.8/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.9/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.9/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/nats/schemas.py` & `propan-0.1.2.9/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.9/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.9/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.9/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/redis/schemas.py` & `propan-0.1.2.9/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/sqs/schema.py` & `propan-0.1.2.9/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.2.9/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.2.9/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/app.py` & `propan-0.1.2.9/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/main.py` & `propan-0.1.2.9/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/core.py` & `propan-0.1.2.9/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.9/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.9/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.9/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.9/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.9/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.9/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.2.9/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/supervisors/basereload.py` & `propan-0.1.2.9/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.9/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/supervisors/utils.py` & `propan-0.1.2.9/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.9/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/utils/imports.py` & `propan-0.1.2.9/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/utils/logs.py` & `propan-0.1.2.9/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/cli/utils/parser.py` & `propan-0.1.2.9/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/__init__.py` & `propan-0.1.2.9/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/core/route.py` & `propan-0.1.2.9/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/core/router.py` & `propan-0.1.2.9/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.9/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/nats/router.pyi` & `propan-0.1.2.9/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.9/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/redis/router.pyi` & `propan-0.1.2.9/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/fastapi/sqs/router.pyi` & `propan-0.1.2.9/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/log/formatter.py` & `propan-0.1.2.9/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/log/logging.py` & `propan-0.1.2.9/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/test/__init__.py` & `propan-0.1.2.9/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/test/kafka.py` & `propan-0.1.2.9/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/test/nats.py` & `propan-0.1.2.9/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/test/rabbit.py` & `propan-0.1.2.9/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/test/redis.py` & `propan-0.1.2.9/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/test/sqs.py` & `propan-0.1.2.9/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/test/utils.py` & `propan-0.1.2.9/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/utils/functions.py` & `propan-0.1.2.9/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/utils/context/main.py` & `propan-0.1.2.9/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/propan/utils/context/types.py` & `propan-0.1.2.9/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/LICENSE` & `propan-0.1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/README.md` & `propan-0.1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.8/pyproject.toml` & `propan-0.1.2.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "fast-depends>=1.1.4",
+    "fast-depends>=1.1.5",
     "watchfiles",
     "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
 
@@ -62,15 +62,15 @@
 
 [project.optional-dependencies]
 async-rabbit = [
     "aio-pika>=9",
 ]
 
 async-nats = [
-    "nats-py>=2"
+    "nats-py>=2,!=2.3.0",
 ]
 
 async-redis = [
     "redis>=4.2.0rc1"
 ]
 
 async-kafka = [
@@ -139,27 +139,37 @@
 features = [
   "dev",
 ]
 
 [tool.hatch.envs.test]
 features = [
   "test",
+  "async-sqs",
+  "async-kafka",
+  "async-nats",
+  "async-rabbit",
+  "async-redis",
 ]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
 [tool.hatch.envs.test.scripts]
 run = "pytest -q -m 'not slow'"
 run-all = "pytest -m 'all'"
 
 [tool.hatch.envs.test-last]
 python = "3.11"
 features = [
   "test",
+  "async-sqs",
+  "async-kafka",
+  "async-nats",
+  "async-rabbit",
+  "async-redis",
 ]
 
 [tool.hatch.envs.test-last.scripts]
 run = "pytest -q -m 'not slow'"
 run-all = "pytest -v -m 'all'"
 cov = "bash ./scripts/test-cov.sh -v -m 'all'"
```

### Comparing `propan-0.1.2.8/PKG-INFO` & `propan-0.1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.8
+Version: 0.1.2.9
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -31,22 +31,22 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: fast-depends>=1.1.4
+Requires-Dist: fast-depends>=1.1.5
 Requires-Dist: typer
 Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles
 Provides-Extra: async-kafka
 Requires-Dist: aiokafka>=0.8; extra == 'async-kafka'
 Provides-Extra: async-nats
-Requires-Dist: nats-py>=2; extra == 'async-nats'
+Requires-Dist: nats-py!=2.3.0,>=2; extra == 'async-nats'
 Provides-Extra: async-rabbit
 Requires-Dist: aio-pika>=9; extra == 'async-rabbit'
 Provides-Extra: async-redis
 Requires-Dist: redis>=4.2.0rc1; extra == 'async-redis'
 Provides-Extra: async-sqs
 Requires-Dist: aiobotocore; extra == 'async-sqs'
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.8 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.9 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -17,39 +17,39 @@
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Topic :: Internet Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Application Frameworks Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Classifier: Typing ::
-Typed Requires-Python: >=3.7 Requires-Dist: fast-depends>=1.1.4 Requires-Dist:
+Typed Requires-Python: >=3.7 Requires-Dist: fast-depends>=1.1.5 Requires-Dist:
 typer Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32'
 and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles Provides-Extra: async-kafka Requires-Dist:
 aiokafka>=0.8; extra == 'async-kafka' Provides-Extra: async-nats Requires-Dist:
-nats-py>=2; extra == 'async-nats' Provides-Extra: async-rabbit Requires-Dist:
-aio-pika>=9; extra == 'async-rabbit' Provides-Extra: async-redis Requires-Dist:
-redis>=4.2.0rc1; extra == 'async-redis' Provides-Extra: async-sqs Requires-
-Dist: aiobotocore; extra == 'async-sqs' Provides-Extra: dev Requires-Dist:
-black==23.3.0; extra == 'dev' Requires-Dist: isort>=5; extra == 'dev' Requires-
-Dist: mypy==1.1.1; extra == 'dev' Requires-Dist: propan[doc]; extra == 'dev'
-Requires-Dist: propan[test]; extra == 'dev' Requires-Dist: ruff==0.0.261; extra
-== 'dev' Requires-Dist: typer[all]; extra == 'dev' Requires-Dist: types-redis;
-extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-include<2.0.0,>=1.4.1;
-extra == 'doc' Requires-Dist: mkdocs-macros-plugin; extra == 'doc' Requires-
-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist: mkdocs-
-static-i18n; extra == 'doc' Requires-Dist: typer[all]; extra == 'doc' Provides-
-Extra: test Requires-Dist: asyncmock; python_version < '3.8' and extra ==
-'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist:
-fastapi; extra == 'test' Requires-Dist: propan[async-kafka]; extra == 'test'
-Requires-Dist: propan[async-nats]; extra == 'test' Requires-Dist: propan[async-
-rabbit]; extra == 'test' Requires-Dist: propan[async-redis]; extra == 'test'
-Requires-Dist: propan[async-sqs]; extra == 'test' Requires-Dist: pytest-
-asyncio>=0.21; extra == 'test' Requires-Dist: pytest>=7; extra == 'test'
-Description-Content-Type: text/markdown
+nats-py!=2.3.0,>=2; extra == 'async-nats' Provides-Extra: async-rabbit
+Requires-Dist: aio-pika>=9; extra == 'async-rabbit' Provides-Extra: async-redis
+Requires-Dist: redis>=4.2.0rc1; extra == 'async-redis' Provides-Extra: async-
+sqs Requires-Dist: aiobotocore; extra == 'async-sqs' Provides-Extra: dev
+Requires-Dist: black==23.3.0; extra == 'dev' Requires-Dist: isort>=5; extra ==
+'dev' Requires-Dist: mypy==1.1.1; extra == 'dev' Requires-Dist: propan[doc];
+extra == 'dev' Requires-Dist: propan[test]; extra == 'dev' Requires-Dist:
+ruff==0.0.261; extra == 'dev' Requires-Dist: typer[all]; extra == 'dev'
+Requires-Dist: types-redis; extra == 'dev' Provides-Extra: doc Requires-Dist:
+mdx-include<2.0.0,>=1.4.1; extra == 'doc' Requires-Dist: mkdocs-macros-plugin;
+extra == 'doc' Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
+Requires-Dist: mkdocs-static-i18n; extra == 'doc' Requires-Dist: typer[all];
+extra == 'doc' Provides-Extra: test Requires-Dist: asyncmock; python_version <
+'3.8' and extra == 'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test'
+Requires-Dist: fastapi; extra == 'test' Requires-Dist: propan[async-kafka];
+extra == 'test' Requires-Dist: propan[async-nats]; extra == 'test' Requires-
+Dist: propan[async-rabbit]; extra == 'test' Requires-Dist: propan[async-redis];
+extra == 'test' Requires-Dist: propan[async-sqs]; extra == 'test' Requires-
+Dist: pytest-asyncio>=0.21; extra == 'test' Requires-Dist: pytest>=7; extra ==
+'test' Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
 framework**. It's following by *fastapi*, simplify Message Brokers around code
 writing and provides a helpful development toolkit, which existed only in HTTP-
 frameworks world until now. It's designed to create reactive microservices
```

