# Comparing `tmp/djangofoundry-0.0.5.tar.gz` & `tmp/djangofoundry-0.0.6.tar.gz`

## Comparing `djangofoundry-0.0.5.tar` & `djangofoundry-0.0.6.tar`

### file list

```diff
@@ -1,120 +1,121 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.dockerignore
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.prospector.yaml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/docker-compose.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/logging.conf
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/package.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/requirements.txt
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/urls.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/angular.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/detail.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/generic.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/list.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/memory.py
--rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/controllers/responses.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/__init__.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/queryset_filter.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/retry.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/decorators/timeout.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/exceptions/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/exceptions/app.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/logging.py
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/progress.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/encoders/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/encoders/json.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/exceptions.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hook.py
--rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hooks.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/waypoint.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/constants.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/types.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/queue/__init__.py
--rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/queue/queue.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/queue/signals.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/template.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/__init__.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/css.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/javascript.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/template.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/model.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/template.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/meta/__init__.py
--rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/helpers/render/meta/model.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/__init__.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/engine.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/fuzzy/__init__.py
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/matching/fuzzy/thefuzz.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/dirtyfields.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/hasParams.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/hookable.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/mixins/jsonResponse.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/choices.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/manager.py
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/model.py
--rw-r--r--   0        0        0    53639 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/queryset.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/serializer.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/viewset.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/exceptions/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/exceptions/get.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/boolean.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/char.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/date.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/number.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/objects.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/models/fields/relationships.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/options/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/options/request.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/README.md
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/__init__.py
--rw-r--r--   0        0        0    20059 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/app.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/db.py
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/lint.py
--rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/summarize.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/conf/sample-settings.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/__init__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/action.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/exceptions.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/settings.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/scripts/utils/types.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/signals/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/signals/abstract.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templates/memory.html
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templates/angular/base.html
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templates/jinja/model.py.jinja
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templatetags/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/src/djangofoundry/templatetags/syntax_highlight.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/test_matching.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/controllers/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/controllers/test_mixins.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/decorators/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/decorators/test_timeout.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/helpers/__init__.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/helpers/test_hooks.py
--rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/helpers/test_queue.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/models/__init__.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/models/test_choices.py
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/tests/foundry/models/test_queryset.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/.gitignore
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/LICENSE.md
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/README.md
--rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/.dockerignore
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/.prospector.yaml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/docker-compose.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/logging.conf
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/package.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/urls.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/controllers/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/controllers/angular.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/controllers/detail.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/controllers/generic.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/controllers/list.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/controllers/memory.py
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/controllers/responses.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/decorators/__init__.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/decorators/queryset_filter.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/decorators/retry.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/decorators/timeout.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/exceptions/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/exceptions/app.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/logging.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/progress.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/encoders/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/encoders/json.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/exceptions.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/hook.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/hooks.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/waypoint.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/meta/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/meta/constants.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/meta/types.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/queue/__init__.py
+-rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/queue/queue.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/queue/signals.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/template.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/__init__.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/__init__.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/css.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/javascript.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/template.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/python/__init__.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/python/model.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/python/template.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/meta/__init__.py
+-rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/helpers/render/meta/model.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/matching/__init__.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/matching/engine.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/matching/fuzzy/__init__.py
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/matching/fuzzy/thefuzz.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/mixins/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/mixins/dirtyfields.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/mixins/hasParams.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/mixins/hookable.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/mixins/jsonResponse.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/choices.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/manager.py
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/model.py
+-rw-r--r--   0        0        0    53639 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/queryset.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/serializer.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/viewset.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/exceptions/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/exceptions/get.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/fields/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/fields/boolean.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/fields/char.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/fields/date.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/fields/number.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/fields/objects.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/models/fields/relationships.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/options/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/options/request.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/README.md
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/__init__.py
+-rw-r--r--   0        0        0    20059 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/app.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/db.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/imports.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/lint.py
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/summarize.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/conf/sample-settings.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/utils/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/utils/__init__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/utils/action.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/utils/exceptions.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/utils/settings.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/scripts/utils/types.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/signals/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/signals/abstract.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/templates/memory.html
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/templates/angular/base.html
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/templates/jinja/model.py.jinja
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/templatetags/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/src/djangofoundry/templatetags/syntax_highlight.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/test_matching.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/controllers/__init__.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/controllers/test_mixins.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/decorators/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/decorators/test_timeout.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/helpers/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/helpers/test_hooks.py
+-rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/helpers/test_queue.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/models/__init__.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/models/test_choices.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/tests/foundry/models/test_queryset.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/README.md
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 djangofoundry-0.0.6/PKG-INFO
```

### Comparing `djangofoundry-0.0.5/.prospector.yaml` & `djangofoundry-0.0.6/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/Dockerfile` & `djangofoundry-0.0.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/package.json` & `djangofoundry-0.0.6/package.json`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/.devcontainer/docker-compose.yml` & `djangofoundry-0.0.6/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/urls.py` & `djangofoundry-0.0.6/src/djangofoundry/urls.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/controllers/__init__.py` & `djangofoundry-0.0.6/src/djangofoundry/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/controllers/angular.py` & `djangofoundry-0.0.6/src/djangofoundry/controllers/angular.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/controllers/detail.py` & `djangofoundry-0.0.6/src/djangofoundry/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/controllers/generic.py` & `djangofoundry-0.0.6/src/djangofoundry/controllers/generic.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/controllers/list.py` & `djangofoundry-0.0.6/src/djangofoundry/controllers/list.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/controllers/memory.py` & `djangofoundry-0.0.6/src/djangofoundry/controllers/memory.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/controllers/responses.py` & `djangofoundry-0.0.6/src/djangofoundry/controllers/responses.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/decorators/queryset_filter.py` & `djangofoundry-0.0.6/src/djangofoundry/decorators/queryset_filter.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/decorators/retry.py` & `djangofoundry-0.0.6/src/djangofoundry/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/decorators/timeout.py` & `djangofoundry-0.0.6/src/djangofoundry/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/exceptions/app.py` & `djangofoundry-0.0.6/src/djangofoundry/exceptions/app.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/logging.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/progress.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
 		# Update to running if we 1) haven't yet and 2) have done anything at all.
 		# -- otherwise, trust the end user to update states appropriately
 		if not ProgressStates.has_started(self.state) and (self._current > 0 or self._description):
 			self._state = PROGRESS_STATE
 
 		# If we don't have a task, there's nothing to refresh
-		if self.task is None:
+		if not hasattr(self, 'task') or not self.task:
 			return
 
 		# Refresh the state of the task we have based on our local values here
 		self.task.update_state(
 			state=self.state,
 			meta=self.meta
 		)
```

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/__init__.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/exceptions.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hook.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/hooks.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/waypoint.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/waypoint.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/constants.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/meta/constants.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/hooks/meta/types.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/hooks/meta/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/queue/queue.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/queue/queue.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/queue/signals.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/queue/signals.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/template.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/template.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/css.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/css.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/javascript.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/javascript.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/template.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/model.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/python/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/jinja/code/python/template.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/jinja/code/python/template.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/helpers/render/meta/model.py` & `djangofoundry-0.0.6/src/djangofoundry/helpers/render/meta/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/matching/engine.py` & `djangofoundry-0.0.6/src/djangofoundry/matching/engine.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/matching/fuzzy/thefuzz.py` & `djangofoundry-0.0.6/src/djangofoundry/matching/fuzzy/thefuzz.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/mixins/dirtyfields.py` & `djangofoundry-0.0.6/src/djangofoundry/mixins/dirtyfields.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/mixins/hasParams.py` & `djangofoundry-0.0.6/src/djangofoundry/mixins/hasParams.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/mixins/hookable.py` & `djangofoundry-0.0.6/src/djangofoundry/mixins/hookable.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/mixins/jsonResponse.py` & `djangofoundry-0.0.6/src/djangofoundry/mixins/jsonResponse.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/__init__.py` & `djangofoundry-0.0.6/src/djangofoundry/models/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 		-----
 
 		Copyright (c) 2022 Jess Mann
 
 """
 # Generic imports
 from djangofoundry.models.exceptions import DoesNotExist, NotUnique
-from djangofoundry.models.queryset import QuerySet
-from djangofoundry.models.manager import Manager, PostgresManager
-from djangofoundry.models.model import Model
-from djangofoundry.models.viewset import ViewSet
-from djangofoundry.models.serializer import Serializer
 from djangofoundry.models.choices import TextChoices
 from djangofoundry.models.fields import (
 	IntegerField,
 	CharField,
 	TextField,
 	DateTimeField,
 	DateGroupField,
@@ -47,8 +42,13 @@
 	HStoreField,
 	JsonFloatValues,
 	PickledObjectField,
 	BooleanField,
 	ForeignKey,
 	OneToOneField,
 	JSONField,
-)
+)
+from djangofoundry.models.queryset import QuerySet
+from djangofoundry.models.manager import Manager, PostgresManager
+from djangofoundry.models.model import Model
+from djangofoundry.models.serializer import Serializer
+from djangofoundry.models.viewset import ViewSet
```

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/choices.py` & `djangofoundry-0.0.6/src/djangofoundry/models/choices.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/manager.py` & `djangofoundry-0.0.6/src/djangofoundry/models/manager.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/model.py` & `djangofoundry-0.0.6/src/djangofoundry/models/model.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/queryset.py` & `djangofoundry-0.0.6/src/djangofoundry/models/queryset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/serializer.py` & `djangofoundry-0.0.6/src/djangofoundry/models/serializer.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/viewset.py` & `djangofoundry-0.0.6/src/djangofoundry/models/viewset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/exceptions/get.py` & `djangofoundry-0.0.6/src/djangofoundry/models/exceptions/get.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/fields/__init__.py` & `djangofoundry-0.0.6/src/djangofoundry/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/fields/char.py` & `djangofoundry-0.0.6/src/djangofoundry/models/fields/char.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/fields/date.py` & `djangofoundry-0.0.6/src/djangofoundry/models/fields/date.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/fields/number.py` & `djangofoundry-0.0.6/src/djangofoundry/models/fields/number.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/fields/objects.py` & `djangofoundry-0.0.6/src/djangofoundry/models/fields/objects.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/models/fields/relationships.py` & `djangofoundry-0.0.6/src/djangofoundry/models/fields/relationships.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/__init__.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/app.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/app.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/db.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/db.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/lint.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/lint.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 				model = "gpt-4",
 				messages = [
 					{"role": "system", "content": "Your job is to identify bugs in python code and suggest improvements, adhering to modern best " +
 												  "practices, such as DRY. Review the code supplied and list specific changes to the code. If " +
 												  "functionality can be added to the code, suggest them. Use the following format for your " +
 												  "suggestions: 'Change Y to Z'. If there are no changes needed, respond with 'no changes proposed'. " +
 												  "Example response format: In the `calculate` method, change 'area = length * length' to 'area = " +
-												  "length * width'. All code submitted will be from a large django project using python 3.10.4, which " +
+												  "length * width'. All code submitted will be from a large django project using python 3.10 or higher, which " +
 												  "is focused on data analytics and running background automation tasks. The code snippet provided " +
 												  "is not the full file; it excludes all imports and comments in the original. When you are finished, " +
 												  "adding as much functionality as you can and identifying bugs, please write django unit tests for " +
 												  "the code for 100% code coverage"},
 					{"role": "user", "content": f"File: `{file_path}`, Code: \n\n{code}"},
 				]
 			)
```

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/summarize.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/summarize.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/conf/sample-settings.yaml` & `djangofoundry-0.0.6/src/djangofoundry/scripts/conf/sample-settings.yaml`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/__init__.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/action.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/utils/action.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/exceptions.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/settings.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/utils/settings.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/scripts/utils/types.py` & `djangofoundry-0.0.6/src/djangofoundry/scripts/utils/types.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/signals/abstract.py` & `djangofoundry-0.0.6/src/djangofoundry/signals/abstract.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/templates/memory.html` & `djangofoundry-0.0.6/src/djangofoundry/templates/memory.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/templates/angular/base.html` & `djangofoundry-0.0.6/src/djangofoundry/templates/angular/base.html`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/templates/jinja/model.py.jinja` & `djangofoundry-0.0.6/src/djangofoundry/templates/jinja/model.py.jinja`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/src/djangofoundry/templatetags/syntax_highlight.py` & `djangofoundry-0.0.6/src/djangofoundry/templatetags/syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/tests/foundry/test_matching.py` & `djangofoundry-0.0.6/tests/foundry/test_matching.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/tests/foundry/controllers/test_mixins.py` & `djangofoundry-0.0.6/tests/foundry/controllers/test_mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from __future__ import annotations
 
 import re
 # Django imports
 from django.test import TestCase
 from django.views import View
 # Lib imports
-from djangofoundry.controllers.mixins import HasParams
+from djangofoundry.mixins import HasParams
 # App imports
 
 class Sample(HasParams, View):
 	pass
 
 class HasParamsTest(TestCase):
```

### Comparing `djangofoundry-0.0.5/tests/foundry/decorators/test_timeout.py` & `djangofoundry-0.0.6/tests/foundry/decorators/test_timeout.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/tests/foundry/helpers/test_hooks.py` & `djangofoundry-0.0.6/tests/foundry/helpers/test_hooks.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/tests/foundry/helpers/test_queue.py` & `djangofoundry-0.0.6/tests/foundry/helpers/test_queue.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/tests/foundry/models/test_choices.py` & `djangofoundry-0.0.6/tests/foundry/models/test_choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from dateutil.parser import ParserError
 # Django imports
 from django.test import TestCase
 # Lib imports
 from djangofoundry.models.choices import TextChoices
 # App imports
 
-
 class ChoicesTest(TestCase):
 
 	def setUp(self):
 		pass
 
 	def test_choices_valid(self):
 		class Choices(TextChoices):
```

### Comparing `djangofoundry-0.0.5/tests/foundry/models/test_queryset.py` & `djangofoundry-0.0.6/tests/foundry/models/test_queryset.py`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/LICENSE.md` & `djangofoundry-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/README.md` & `djangofoundry-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `djangofoundry-0.0.5/pyproject.toml` & `djangofoundry-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "djangofoundry"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Jess Mann", email="jess.a.mann+df@gmail.com" },
 ]
 description = "A collection of classes built on Django to make it easier to build web applications."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `djangofoundry-0.0.5/PKG-INFO` & `djangofoundry-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangofoundry
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of classes built on Django to make it easier to build web applications.
 Project-URL: Homepage, https://github.com/avranu/Django-Foundry
 Project-URL: Bug Tracker, https://github.com/avranu/Django-Foundry/issues
 Author-email: Jess Mann <jess.a.mann+df@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

