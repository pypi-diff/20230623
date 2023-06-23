# Comparing `tmp/mpyl-1.0.5-py3-none-any.whl.zip` & `tmp/mpyl-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,89 +1,90 @@
-Zip file size: 132278 bytes, number of entries: 87
--rw-r--r--  2.0 unx      766 b- defN 23-Jun-20 14:38 mpyl/__init__.py
--rw-r--r--  2.0 unx      215 b- defN 23-Jun-20 14:38 mpyl/__main__.py
--rw-r--r--  2.0 unx      162 b- defN 23-Jun-20 14:38 mpyl/constants.py
--rw-r--r--  2.0 unx    13469 b- defN 23-Jun-20 14:38 mpyl/project.py
--rw-r--r--  2.0 unx     1708 b- defN 23-Jun-20 14:38 mpyl/validation.py
--rw-r--r--  2.0 unx     2163 b- defN 23-Jun-20 14:38 mpyl/cli/__init__.py
--rw-r--r--  2.0 unx    10555 b- defN 23-Jun-20 14:38 mpyl/cli/build.py
--rw-r--r--  2.0 unx      341 b- defN 23-Jun-20 14:38 mpyl/cli/health.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jun-20 14:38 mpyl/cli/meta_info.py
--rw-r--r--  2.0 unx     3915 b- defN 23-Jun-20 14:38 mpyl/cli/projects.py
--rw-r--r--  2.0 unx       34 b- defN 23-Jun-20 14:38 mpyl/cli/commands/__init__.py
--rw-r--r--  2.0 unx      439 b- defN 23-Jun-20 14:38 mpyl/cli/commands/build/__init__.py
--rw-r--r--  2.0 unx     3822 b- defN 23-Jun-20 14:38 mpyl/cli/commands/build/jenkins.py
--rw-r--r--  2.0 unx     5802 b- defN 23-Jun-20 14:38 mpyl/cli/commands/build/mpyl.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-20 14:38 mpyl/cli/commands/health/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 23-Jun-20 14:38 mpyl/cli/commands/health/checks.py
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-20 14:38 mpyl/cli/commands/projects/__init__.py
--rw-r--r--  2.0 unx     1039 b- defN 23-Jun-20 14:38 mpyl/cli/commands/projects/formatting.py
--rw-r--r--  2.0 unx      620 b- defN 23-Jun-20 14:38 mpyl/projects/__init__.py
--rw-r--r--  2.0 unx     1993 b- defN 23-Jun-20 14:38 mpyl/projects/find.py
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 14:38 mpyl/reporting/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-20 14:38 mpyl/reporting/formatting/__init__.py
--rw-r--r--  2.0 unx     3664 b- defN 23-Jun-20 14:38 mpyl/reporting/formatting/markdown.py
--rw-r--r--  2.0 unx     1413 b- defN 23-Jun-20 14:38 mpyl/reporting/formatting/text.py
--rw-r--r--  2.0 unx     1096 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/__init__.py
--rw-r--r--  2.0 unx     7939 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/github.py
--rw-r--r--  2.0 unx     8965 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/jira.py
--rw-r--r--  2.0 unx     7106 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/slack.py
--rw-r--r--  2.0 unx     8433 b- defN 23-Jun-20 14:38 mpyl/schema/mpyl_config.schema.yml
--rw-r--r--  2.0 unx    25500 b- defN 23-Jun-20 14:38 mpyl/schema/project.schema.yml
--rw-r--r--  2.0 unx     2787 b- defN 23-Jun-20 14:38 mpyl/schema/run_properties.schema.yml
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 14:38 mpyl/stages/__init__.py
--rw-r--r--  2.0 unx     3439 b- defN 23-Jun-20 14:38 mpyl/stages/discovery.py
--rw-r--r--  2.0 unx     6135 b- defN 23-Jun-20 14:38 mpyl/steps/__init__.py
--rw-r--r--  2.0 unx     5977 b- defN 23-Jun-20 14:38 mpyl/steps/models.py
--rw-r--r--  2.0 unx     3429 b- defN 23-Jun-20 14:38 mpyl/steps/run.py
--rw-r--r--  2.0 unx     8978 b- defN 23-Jun-20 14:38 mpyl/steps/steps.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jun-20 14:38 mpyl/steps/build/__init__.py
--rw-r--r--  2.0 unx     2093 b- defN 23-Jun-20 14:38 mpyl/steps/build/docker_after_build.py
--rw-r--r--  2.0 unx     2865 b- defN 23-Jun-20 14:38 mpyl/steps/build/dockerbuild.py
--rw-r--r--  2.0 unx      765 b- defN 23-Jun-20 14:38 mpyl/steps/build/echo.py
--rw-r--r--  2.0 unx     2402 b- defN 23-Jun-20 14:38 mpyl/steps/build/sbt.py
--rw-r--r--  2.0 unx       60 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/__init__.py
--rw-r--r--  2.0 unx     2444 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
--rw-r--r--  2.0 unx     1001 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/echo.py
--rw-r--r--  2.0 unx     1310 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/ephemeral_docker_deploy.py
--rw-r--r--  2.0 unx     2432 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/kubernetes.py
--rw-r--r--  2.0 unx     1111 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/kubernetes_job.py
--rw-r--r--  2.0 unx     1118 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/kubernetes_spark_job.py
--rw-r--r--  2.0 unx     3341 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/__init__.py
--rw-r--r--  2.0 unx    18819 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/chart.py
--rw-r--r--  2.0 unx     2856 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/helm.py
--rw-r--r--  2.0 unx     1579 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/rancher.py
--rw-r--r--  2.0 unx     4467 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/__init__.py
--rw-r--r--  2.0 unx      591 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/sealed_secret.py
--rw-r--r--  2.0 unx     6143 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/spark.py
--rw-r--r--  2.0 unx     1948 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/traefik.py
--rw-r--r--  2.0 unx   168371 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
--rw-r--r--  2.0 unx   151469 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
--rw-r--r--  2.0 unx    11703 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
--rw-r--r--  2.0 unx    42950 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
--rw-r--r--  2.0 unx       64 b- defN 23-Jun-20 14:38 mpyl/steps/postdeploy/__init__.py
--rw-r--r--  2.0 unx     5924 b- defN 23-Jun-20 14:38 mpyl/steps/postdeploy/cypress_test.py
--rw-r--r--  2.0 unx       58 b- defN 23-Jun-20 14:38 mpyl/steps/test/__init__.py
--rw-r--r--  2.0 unx     1428 b- defN 23-Jun-20 14:38 mpyl/steps/test/after_test.py
--rw-r--r--  2.0 unx     2453 b- defN 23-Jun-20 14:38 mpyl/steps/test/before_test.py
--rw-r--r--  2.0 unx     3218 b- defN 23-Jun-20 14:38 mpyl/steps/test/dockertest.py
--rw-r--r--  2.0 unx     1657 b- defN 23-Jun-20 14:38 mpyl/steps/test/echo.py
--rw-r--r--  2.0 unx     4885 b- defN 23-Jun-20 14:38 mpyl/steps/test/sbt.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 14:38 mpyl/utilities/__init__.py
--rw-r--r--  2.0 unx      749 b- defN 23-Jun-20 14:38 mpyl/utilities/cypress/__init__.py
--rw-r--r--  2.0 unx     5583 b- defN 23-Jun-20 14:38 mpyl/utilities/docker/__init__.py
--rw-r--r--  2.0 unx     1739 b- defN 23-Jun-20 14:38 mpyl/utilities/github/__init__.py
--rw-r--r--  2.0 unx     1533 b- defN 23-Jun-20 14:38 mpyl/utilities/jenkins/__init__.py
--rw-r--r--  2.0 unx     7617 b- defN 23-Jun-20 14:38 mpyl/utilities/jenkins/runner.py
--rw-r--r--  2.0 unx     1288 b- defN 23-Jun-20 14:38 mpyl/utilities/junit/__init__.py
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-20 14:38 mpyl/utilities/pyaml_env/__init__.py
--rw-r--r--  2.0 unx     6037 b- defN 23-Jun-20 14:38 mpyl/utilities/repo/__init__.py
--rw-r--r--  2.0 unx     4622 b- defN 23-Jun-20 14:38 mpyl/utilities/s3/__init__.py
--rw-r--r--  2.0 unx     1551 b- defN 23-Jun-20 14:38 mpyl/utilities/sbt/__init__.py
--rw-r--r--  2.0 unx     2110 b- defN 23-Jun-20 14:38 mpyl/utilities/subprocess/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     5945 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7673 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/RECORD
-87 files, 659783 bytes uncompressed, 120048 bytes compressed:  81.8%
+Zip file size: 133968 bytes, number of entries: 88
+-rw-r--r--  2.0 unx      766 b- defN 23-Jun-23 12:50 mpyl/__init__.py
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-23 12:50 mpyl/__main__.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-23 12:50 mpyl/constants.py
+-rw-r--r--  2.0 unx    13526 b- defN 23-Jun-23 12:50 mpyl/project.py
+-rw-r--r--  2.0 unx     1708 b- defN 23-Jun-23 12:50 mpyl/validation.py
+-rw-r--r--  2.0 unx     2163 b- defN 23-Jun-23 12:50 mpyl/cli/__init__.py
+-rw-r--r--  2.0 unx    10619 b- defN 23-Jun-23 12:50 mpyl/cli/build.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-23 12:50 mpyl/cli/health.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jun-23 12:50 mpyl/cli/meta_info.py
+-rw-r--r--  2.0 unx     3915 b- defN 23-Jun-23 12:50 mpyl/cli/projects.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-23 12:50 mpyl/cli/commands/__init__.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Jun-23 12:50 mpyl/cli/commands/build/__init__.py
+-rw-r--r--  2.0 unx     3923 b- defN 23-Jun-23 12:50 mpyl/cli/commands/build/jenkins.py
+-rw-r--r--  2.0 unx     5814 b- defN 23-Jun-23 12:50 mpyl/cli/commands/build/mpyl.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-23 12:50 mpyl/cli/commands/health/__init__.py
+-rw-r--r--  2.0 unx     5200 b- defN 23-Jun-23 12:50 mpyl/cli/commands/health/checks.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-23 12:50 mpyl/cli/commands/projects/__init__.py
+-rw-r--r--  2.0 unx     1039 b- defN 23-Jun-23 12:50 mpyl/cli/commands/projects/formatting.py
+-rw-r--r--  2.0 unx      620 b- defN 23-Jun-23 12:50 mpyl/projects/__init__.py
+-rw-r--r--  2.0 unx     1993 b- defN 23-Jun-23 12:50 mpyl/projects/find.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 12:50 mpyl/reporting/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-23 12:50 mpyl/reporting/formatting/__init__.py
+-rw-r--r--  2.0 unx     4909 b- defN 23-Jun-23 12:50 mpyl/reporting/formatting/markdown.py
+-rw-r--r--  2.0 unx     1413 b- defN 23-Jun-23 12:50 mpyl/reporting/formatting/text.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/__init__.py
+-rw-r--r--  2.0 unx     7939 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/github.py
+-rw-r--r--  2.0 unx     9004 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/jira.py
+-rw-r--r--  2.0 unx     7366 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/slack.py
+-rw-r--r--  2.0 unx     8433 b- defN 23-Jun-23 12:50 mpyl/schema/mpyl_config.schema.yml
+-rw-r--r--  2.0 unx    25500 b- defN 23-Jun-23 12:50 mpyl/schema/project.schema.yml
+-rw-r--r--  2.0 unx     2787 b- defN 23-Jun-23 12:50 mpyl/schema/run_properties.schema.yml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 12:50 mpyl/stages/__init__.py
+-rw-r--r--  2.0 unx     3506 b- defN 23-Jun-23 12:50 mpyl/stages/discovery.py
+-rw-r--r--  2.0 unx     6135 b- defN 23-Jun-23 12:50 mpyl/steps/__init__.py
+-rw-r--r--  2.0 unx     5977 b- defN 23-Jun-23 12:50 mpyl/steps/models.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-Jun-23 12:50 mpyl/steps/run.py
+-rw-r--r--  2.0 unx     8405 b- defN 23-Jun-23 12:50 mpyl/steps/steps.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-23 12:50 mpyl/steps/build/__init__.py
+-rw-r--r--  2.0 unx     2093 b- defN 23-Jun-23 12:50 mpyl/steps/build/docker_after_build.py
+-rw-r--r--  2.0 unx     2865 b- defN 23-Jun-23 12:50 mpyl/steps/build/dockerbuild.py
+-rw-r--r--  2.0 unx      765 b- defN 23-Jun-23 12:50 mpyl/steps/build/echo.py
+-rw-r--r--  2.0 unx     2402 b- defN 23-Jun-23 12:50 mpyl/steps/build/sbt.py
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/__init__.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
+-rw-r--r--  2.0 unx     1001 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/echo.py
+-rw-r--r--  2.0 unx     1310 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/ephemeral_docker_deploy.py
+-rw-r--r--  2.0 unx     3415 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/kubernetes.py
+-rw-r--r--  2.0 unx     1412 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/kubernetes_job.py
+-rw-r--r--  2.0 unx     1380 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/kubernetes_spark_job.py
+-rw-r--r--  2.0 unx     3390 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/__init__.py
+-rw-r--r--  2.0 unx    18819 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/chart.py
+-rw-r--r--  2.0 unx     2856 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/helm.py
+-rw-r--r--  2.0 unx     1685 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/rancher.py
+-rw-r--r--  2.0 unx     4467 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/sealed_secret.py
+-rw-r--r--  2.0 unx     6143 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/spark.py
+-rw-r--r--  2.0 unx     1948 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/traefik.py
+-rw-r--r--  2.0 unx   168371 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
+-rw-r--r--  2.0 unx   151469 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
+-rw-r--r--  2.0 unx    11703 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
+-rw-r--r--  2.0 unx    42950 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-23 12:50 mpyl/steps/postdeploy/__init__.py
+-rw-r--r--  2.0 unx     6004 b- defN 23-Jun-23 12:50 mpyl/steps/postdeploy/cypress_test.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-23 12:50 mpyl/steps/test/__init__.py
+-rw-r--r--  2.0 unx     1428 b- defN 23-Jun-23 12:50 mpyl/steps/test/after_test.py
+-rw-r--r--  2.0 unx     2453 b- defN 23-Jun-23 12:50 mpyl/steps/test/before_test.py
+-rw-r--r--  2.0 unx     3609 b- defN 23-Jun-23 12:50 mpyl/steps/test/dockertest.py
+-rw-r--r--  2.0 unx     1789 b- defN 23-Jun-23 12:50 mpyl/steps/test/echo.py
+-rw-r--r--  2.0 unx     5013 b- defN 23-Jun-23 12:50 mpyl/steps/test/sbt.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 12:50 mpyl/utilities/__init__.py
+-rw-r--r--  2.0 unx      749 b- defN 23-Jun-23 12:50 mpyl/utilities/cypress/__init__.py
+-rw-r--r--  2.0 unx     6470 b- defN 23-Jun-23 12:50 mpyl/utilities/docker/__init__.py
+-rw-r--r--  2.0 unx     1739 b- defN 23-Jun-23 12:50 mpyl/utilities/github/__init__.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-Jun-23 12:50 mpyl/utilities/jenkins/__init__.py
+-rw-r--r--  2.0 unx     7627 b- defN 23-Jun-23 12:50 mpyl/utilities/jenkins/runner.py
+-rw-r--r--  2.0 unx     1382 b- defN 23-Jun-23 12:50 mpyl/utilities/junit/__init__.py
+-rw-r--r--  2.0 unx      254 b- defN 23-Jun-23 12:50 mpyl/utilities/logging/__init__.py
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-23 12:50 mpyl/utilities/pyaml_env/__init__.py
+-rw-r--r--  2.0 unx     6568 b- defN 23-Jun-23 12:50 mpyl/utilities/repo/__init__.py
+-rw-r--r--  2.0 unx     4622 b- defN 23-Jun-23 12:50 mpyl/utilities/s3/__init__.py
+-rw-r--r--  2.0 unx     1551 b- defN 23-Jun-23 12:50 mpyl/utilities/sbt/__init__.py
+-rw-r--r--  2.0 unx     2110 b- defN 23-Jun-23 12:50 mpyl/utilities/subprocess/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5945 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 23-Jun-23 12:51 mpyl-1.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-23 12:51 mpyl-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7763 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/RECORD
+88 files, 665515 bytes uncompressed, 121594 bytes compressed:  81.7%
```

## zipnote {}

```diff
@@ -222,14 +222,17 @@
 
 Filename: mpyl/utilities/jenkins/runner.py
 Comment: 
 
 Filename: mpyl/utilities/junit/__init__.py
 Comment: 
 
+Filename: mpyl/utilities/logging/__init__.py
+Comment: 
+
 Filename: mpyl/utilities/pyaml_env/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/repo/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/s3/__init__.py
@@ -237,26 +240,26 @@
 
 Filename: mpyl/utilities/sbt/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/subprocess/__init__.py
 Comment: 
 
-Filename: mpyl-1.0.5.dist-info/LICENSE
+Filename: mpyl-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: mpyl-1.0.5.dist-info/METADATA
+Filename: mpyl-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: mpyl-1.0.5.dist-info/WHEEL
+Filename: mpyl-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: mpyl-1.0.5.dist-info/entry_points.txt
+Filename: mpyl-1.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: mpyl-1.0.5.dist-info/top_level.txt
+Filename: mpyl-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mpyl-1.0.5.dist-info/RECORD
+Filename: mpyl-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mpyl/project.py

```diff
@@ -37,14 +37,17 @@
 
 
 @dataclass(frozen=True)
 class Target(Enum):
     def __eq__(self, other):
         return self.value == other.value
 
+    def __str__(self):
+        return str(self.value)
+
     PULL_REQUEST = 'PullRequest'
     PULL_REQUEST_BASE = 'PullRequestBase'
     ACCEPTANCE = 'Acceptance'
     PRODUCTION = 'Production'
 
 
 @dataclass(frozen=True)
@@ -254,22 +257,24 @@
     hosts: list[Host]
 
     @staticmethod
     def from_config(values: dict):
         hosts = values.get('hosts')
         return Traefik(hosts=(list(map(Host.from_config, hosts) if hosts else [])))
 
+
 @dataclass(frozen=True)
 class S3Bucket:
     bucket: TargetProperty[str]
 
     @staticmethod
     def from_config(values: dict):
         return S3Bucket(bucket=TargetProperty.from_config(values.get('bucket', {})))
 
+
 @dataclass(frozen=True)
 class Deployment:
     namespace: Optional[str]
     properties: Properties
     kubernetes: Optional[Kubernetes]
     traefik: Optional[Traefik]
     s3_bucket: Optional[S3Bucket]
```

## mpyl/cli/build.py

```diff
@@ -64,15 +64,16 @@
 )
 @click.pass_obj
 def run(obj: CliContext, ci, all_, tag):  # pylint: disable=invalid-name
     asyncio.run(warn_if_update(obj.console))
     run_properties = RunProperties.from_configuration(obj.run_properties, obj.config) if ci \
         else RunProperties.for_local_run(obj.config, obj.repo.get_sha, obj.repo.get_branch, tag)
 
-    parameters = MpylCliParameters(local=not ci, pull_main=all_, all=all_, verbose=obj.verbose, tag=tag)
+    parameters = MpylCliParameters(local=not ci, pull_main=all_, all=all_, verbose=obj.verbose, tag=tag,
+                                   target=run_properties.target)
     obj.console.log(parameters)
     run_parameters = MpylRunParameters(
         run_config=MpylRunConfig(config=obj.config, run_properties=run_properties),
         parameters=parameters
     )
     run_mpyl(run_parameters, None)
 
@@ -224,15 +225,15 @@
 def jenkins(ctx, user, password, pipeline, test, arguments, background, silent,  # pylint: disable=too-many-arguments
             tag):
     try:
         upgrade_check = asyncio.wait_for(warn_if_update(ctx.obj.console), timeout=5)
         selected_pipeline = pipeline if pipeline else ctx.obj.config['jenkins']['defaultPipeline']
         pipeline_parameters = {'TEST': 'true', 'VERSION': test} if test else {}
         if arguments:
-            pipeline_parameters['PIPENV_PARAMS'] = " ".join(arguments)
+            pipeline_parameters['BUILD_PARAMS'] = " ".join(arguments)
 
         run_argument = JenkinsRunParameters(
             jenkins_user=user, jenkins_password=password, config=ctx.obj.config,
             pipeline=selected_pipeline, pipeline_parameters=pipeline_parameters,
             verbose=not silent or ctx.obj.verbose,
             follow=not background, tag=tag
         )
```

## mpyl/cli/commands/build/jenkins.py

```diff
@@ -47,19 +47,21 @@
     if not branch:
         status.console.log('Could not determine current branch')
         return None
 
     if git_repo.main_branch == branch:
         status.console.log(f'On main branch ({branch}), cannot determine which PR to build')
         return None
-
-    pull = get_pr_for_branch(repo, branch)
-
-    return Pipeline(target=Target.PULL_REQUEST, tag=f'{pull.number}', url=pull.html_url, pipeline=pipeline,
-                    body=pull.body, jenkins_config=JenkinsConfig.from_config(config))
+    try:
+        pull = get_pr_for_branch(repo, branch)
+        return Pipeline(target=Target.PULL_REQUEST, tag=f'{pull.number}', url=pull.html_url, pipeline=pipeline,
+                        body=pull.body, jenkins_config=JenkinsConfig.from_config(config))
+    except ValueError as exc:
+        status.console.log(exc)
+        return None
 
 
 def run_jenkins(run_config: JenkinsRunParameters):
     log_console = Console(log_path=False, log_time=False)
     with log_console.status('Fetching Github info.. [bright_blue]>gh pr view[/bright_blue]') as status:
         config = run_config.config
```

## mpyl/cli/commands/build/mpyl.py

```diff
@@ -25,14 +25,15 @@
     config: dict
     run_properties: RunProperties
 
 
 @dataclass(frozen=True)
 class MpylCliParameters:
     local: bool
+    target: str
     tag: Optional[str] = None
     pull_main: bool = False
     verbose: bool = False
     all: bool = False
 
 
 @dataclass(frozen=True)
@@ -43,15 +44,15 @@
 
 FORMAT = "%(name)s  %(message)s"
 
 
 def get_build_plan(logger: logging.Logger, repo: Repository, mpyl_run_parameters: MpylRunParameters) -> RunResult:
     params = mpyl_run_parameters.parameters
     branch = repo.get_branch or mpyl_run_parameters.run_config.run_properties.versioning.branch
-    logger.info(f"Running with {params} on {branch}")
+    logger.info(f"Running with {params}")
     if branch:
         if repo.main_branch_pulled:
             logger.info(f'Branch `{repo.main_branch}` already present locally. Skipping pull.')
         else:
             logger.info(f'Pulling `{repo.main_branch}` from {repo.get_remote_url}')
             pull_result = repo.pull_main_branch()
             logger.info(f'Pulled `{pull_result[0].remote_ref_path.strip()}` to local')
@@ -63,21 +64,21 @@
     projects_per_stage: dict[Stage, set[Project]] = find_build_set(repo, changes, params.all)
     return RunResult(run_properties=mpyl_run_parameters.run_config.run_properties, run_plan=projects_per_stage)
 
 
 def run_mpyl(mpyl_run_parameters: MpylRunParameters, reporter: Optional[Reporter]) -> RunResult:
     params = mpyl_run_parameters.parameters
     console_properties = mpyl_run_parameters.run_config.run_properties.console
-    console = Console(markup=True, width=None if params.local else console_properties.width, no_color=False,
+    console = Console(markup=False, width=None if params.local else console_properties.width, no_color=False,
                       log_path=False, color_system='256')
     print(f"Logging properties: {console_properties}, console: {console}")
+    logging.raiseExceptions = False
     logging.basicConfig(
         level="DEBUG" if params.verbose else console_properties.log_level, format=FORMAT, datefmt="[%X]",
-        handlers=[RichHandler(markup=True,
-                              console=console, show_path=params.local)]
+        handlers=[RichHandler(markup=False, console=console, show_path=params.local)]
     )
     logger = logging.getLogger('mpyl')
     try:
         with Repository(RepoConfig.from_config(mpyl_run_parameters.run_config.config)) as repo:
 
             run_plan = get_build_plan(logger, repo, mpyl_run_parameters)
```

## mpyl/cli/commands/health/checks.py

```diff
@@ -119,11 +119,13 @@
         parsed = parse_config(path)
         schema_dict = pkgutil.get_data(__name__, schema_path)
         if schema_dict:
             try:
                 validate(parsed, schema_dict.decode('utf-8'))
                 console.check(f'{name.capitalize()} is valid', success=True)
             except jsonschema.exceptions.ValidationError as exc:
-                console.check(f"{name.capitalize()} is invalid: {exc.message} at '{'.'.join(exc.path)}'",
-                              success=False)
+                console.check(
+                    f"{name.capitalize()} is invalid: {exc.message} at '{'.'.join(exc.path)}'. 🤔Did you rebase"
+                    f" your branch onto {parsed['cvs']['git']['mainBranch']}?",
+                    success=False)
     else:
         console.check(f"Could not find {location}. Location can be specified with env var '{env_var}'", success=False)
```

## mpyl/reporting/formatting/markdown.py

```diff
@@ -1,19 +1,22 @@
 """
 Markdown run result formatters
 """
 import operator
+import itertools
 
 from junitparser import TestSuite
 
 from ...project import Stage, Project
 from ...steps import Output, ArtifactType
+from ...steps.models import Artifact
 from ...steps.run import RunResult
-from ...steps.steps import StepResult, collect_test_results, collect_test_artifacts
-from ...utilities.junit import TestRunSummary, sum_suites
+from ...steps.steps import StepResult
+from ...utilities.junit import TestRunSummary, sum_suites, TEST_RESULTS_URL_KEY, TEST_RESULTS_URL_NAME_KEY, \
+    to_test_suites
 
 
 def summary_to_markdown(summary: TestRunSummary):
     return f"🧪 {summary.tests} ❌ {summary.failures} " \
            f"💔 {summary.errors} 🙈 {summary.skipped}"
 
 
@@ -63,46 +66,71 @@
 
 def markdown_for_stage(run_result: RunResult, stage: Stage):
     step_results: list[StepResult] = run_result.results_for_stage(stage)
     plan: set[Project] = run_result.plan_for_stage(stage)
     if not step_results and not plan:
         return ''
 
-    result = f"{stage_to_icon(stage)}  {__to_oneliner(step_results, plan)}  \n"
-    test_artifacts = collect_test_artifacts(step_results)
-    test_results = collect_test_results(test_artifacts)
+    result = f"{stage_to_icon(stage)} {__to_oneliner(step_results, plan)}  \n"
+    test_artifacts = _collect_test_artifacts(step_results)
+    test_results = _collect_test_results(test_artifacts)
 
     if test_results:
         result += to_markdown_test_report(test_results)
+        unique_artifacts = _collect_unique_test_artifacts_with_url(test_artifacts)
 
-        if stage == Stage.POST_DEPLOY:
-            test_results_url = next((artifact.spec['cypress_results_url'] for artifact in test_artifacts
-                                    if artifact.spec['cypress_results_url']), '')
-        else:
-            test_results_url = run_result.run_properties.details.tests_url
+        for unique_artifact in unique_artifacts:
+            result += f' [{unique_artifact.spec[TEST_RESULTS_URL_NAME_KEY]}]' \
+                      f'({unique_artifact.spec[TEST_RESULTS_URL_KEY]})'
 
-        if test_results_url:
-            result += f' [link]({test_results_url}) \n'
+        result += '  \n'
 
     return result
 
 
 def run_result_to_markdown(run_result: RunResult) -> str:
     result: str = f'{run_result.status_line}  \n'
     exception = run_result.exception
     if exception:
         result += f"For _{exception.executor}_ on _{exception.project_name}_ at _{exception.stage}_ \n"
-        result += f"\n```\n{exception}\n```\n"
+        result += f"\n\n{exception}\n\n"
     elif run_result.failed_result:
         failed = run_result.failed_result
         result += f"For _{failed.project.name}_ at _{failed.stage}_ \n"
-        result += f"\n```\n{run_result.failed_result.output.message}\n```\n"
+        result += f"\n\n{run_result.failed_result.output.message}\n\n"
 
     for stage in Stage:
         result += markdown_for_stage(run_result, stage)
 
     return result
 
 
 def to_markdown_test_report(suites: list[TestSuite]):
     total_tests = sum_suites(suites)
     return f"{summary_to_markdown(total_tests)}"
+
+
+def _collect_test_artifacts(step_results: list[StepResult]) -> list[Artifact]:
+    return [res.output.produced_artifact for res in step_results if
+            (res.output.produced_artifact and
+             res.output.produced_artifact.artifact_type == ArtifactType.JUNIT_TESTS)]
+
+
+def _collect_test_results(test_artifacts: list[Artifact]) -> list[TestSuite]:
+    suites: list[list[TestSuite]] = list(map(to_test_suites, test_artifacts))
+
+    return list(itertools.chain(*suites))
+
+
+def _collect_unique_test_artifacts_with_url(test_artifacts: list[Artifact]) -> list[Artifact]:
+    unique_artifacts: list[Artifact] = []
+    for test_artifact in test_artifacts:
+        if TEST_RESULTS_URL_KEY in test_artifact.spec and test_artifact.spec[TEST_RESULTS_URL_KEY] != '':
+            duplicate_artifact = next((x for x in unique_artifacts if
+                                       x.spec[TEST_RESULTS_URL_KEY] == test_artifact.spec[TEST_RESULTS_URL_KEY]), None)
+            if not duplicate_artifact:
+                test_artifact.spec[TEST_RESULTS_URL_NAME_KEY] = test_artifact.producing_step
+                unique_artifacts.append(test_artifact)
+            else:
+                duplicate_artifact.spec[TEST_RESULTS_URL_NAME_KEY] = 'link'
+
+    return unique_artifacts
```

## mpyl/reporting/targets/jira.py

```diff
@@ -140,15 +140,15 @@
         description_markdown = "\n".join(lines[:max_message_length]) + "\n..."
 
     details = run_result.run_properties.details
 
     build_status = f"🏗️ Build [{details.build_id}]({details.run_url}) {run_result.status_line}, " \
                    f"started by _{details.user}_  \n{markdown_for_stage(run_result, Stage.DEPLOY)}"
     return f"📕 [{ticket.ticket_id}]({ticket.ticket_url}) {ticket.summary} " \
-           f"![{ticket.user_email}]({ticket.user_avatar}) \n" \
+           f'<img src="{ticket.user_avatar}" width="24" height="24" alt="{ticket.user_email}" /> \n' \
            f"{description_markdown}\n\n" \
            f"{build_status}"
 
 
 def compose_build_status(result: RunResult, config: dict) -> str:
     jira_config = JiraConfig.from_config(config=config)
     jira_client = create_jira_for_config(jira_config)
```

## mpyl/reporting/targets/slack.py

```diff
@@ -31,15 +31,15 @@
 ```
 """
 import re
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from slack_sdk import WebClient
-from slack_sdk.errors import SlackClientError
+from slack_sdk.errors import SlackClientError, SlackApiError
 from slack_sdk.models.blocks import HeaderBlock, SectionBlock, MarkdownTextObject, ContextBlock, ImageElement, Block
 
 from . import Reporter, ReportOutcome
 from ..formatting.markdown import run_result_to_markdown
 from ...steps.models import RunProperties
 from ...steps.run import RunResult
 
@@ -84,22 +84,27 @@
     pass
 
 
 class SlackReporter(Reporter):
     _icons: SlackIcons
     _message_identifier: Optional[MessageIdentifier]
 
-    def __init__(self, config: Dict, channel: Optional[str], title: str,
+    def __init__(self,
+                 config: Dict,
+                 channel: Optional[str],
+                 versioning_identifier: str,
+                 target: str,
                  message_identifier: Optional[MessageIdentifier] = None):
+
         slack_config = config.get('slack')
         if not slack_config:
             raise ValueError('slack config not set')
         self._client = WebClient(token=slack_config['botToken'])
         self._channel = channel
-        self._title = title
+        self._title = f'MPyL run for {versioning_identifier} on {target}'
         icons = slack_config['icons']
         self._icons = SlackIcons(success=icons['success'], failure=icons['failure'], building=icons['building'])
         self._message_identifier = message_identifier
 
     def send_report(self, results: RunResult, text: Optional[str] = None) -> ReportOutcome:
         try:
             user_info = self.__get_user_info(results.run_properties.details.user_email)
@@ -140,18 +145,21 @@
         opened_channel = self._client.conversations_open(users=[user_id])
         return opened_channel['channel']['id']
 
     def __get_user_info(self, user_email: Optional[str]):
         profile_data: dict[str, str] = {}
         user_id = None
         if user_email:
-            user = self._client.users_lookupByEmail(email=user_email)
-            user_id = user['user']['id']
-            resp = self._client.users_profile_get(user=user_id)
-            profile_data = resp.get('profile', {})
+            try:
+                user = self._client.users_lookupByEmail(email=user_email)
+                user_id = user['user']['id']
+                resp = self._client.users_profile_get(user=user_id)
+                profile_data = resp.get('profile', {})
+            except SlackApiError:
+                profile_data = {}
 
         return UserInfo(user_name=profile_data.get('real_name_normalized', 'Anonymous'),
                         profile_image=profile_data.get('image_24',
                                                        'https://avatars.githubusercontent.com/u/18010732'),
                         initiator=user_id)
 
     def __get_icon(self, results: RunResult):
```

## mpyl/stages/discovery.py

```diff
@@ -62,17 +62,17 @@
 
 
 def find_invalidated_projects_for_stage(all_projects: set[Project], stage: Stage,
                                         change_history: list[Revision]) -> set[Project]:
     return set(filter(lambda p: are_invalidated(p, stage, change_history), all_projects))
 
 
-def find_deploy_set(repo_config: RepoConfig) -> DeploySet:
+def find_deploy_set(repo_config: RepoConfig, tag: Optional[str]) -> DeploySet:
     with Repository(repo_config) as repo:
-        changes_in_branch = repo.changes_in_branch_including_local()
+        changes_in_branch = repo.changes_in_tagged_commit(tag) if tag else repo.changes_in_branch_including_local()
         project_paths = repo.find_projects()
         all_projects = set(map(lambda p: load_project(Path(""), Path(p), False), project_paths))
         return DeploySet(all_projects,
                          find_invalidated_projects_for_stage(all_projects, Stage.DEPLOY, changes_in_branch))
 
 
 def find_invalidated_projects_per_stage(all_projects: set[Project], change_history: list[Revision]) \
```

## mpyl/steps/models.py

```diff
@@ -22,17 +22,16 @@
     tag: Optional[str]
 
     def __post_init__(self):
         if not self.pr_number and not self.tag:
             raise ValueError('Either pr_number or tag need to be set')
 
     @property
-    def identifier(self):
-        return f'pr-{self.pr_number}' if self.pr_number else self.tag
-
+    def identifier(self) -> str:
+        return self.tag if self.tag else f'pr-{self.pr_number}'
 
 
 @dataclass(frozen=True)
 class RunContext:
     build_id: str
     """Uniquely identifies the run. Typically a monotonically increasing number"""
     run_url: str
```

## mpyl/steps/steps.py

```diff
@@ -1,17 +1,15 @@
 """ Entry point of MPyL. Loads all available Step implementations and triggers their execution based on the specified
 Project and Stage.
 """
-import itertools
 import pkgutil
 from dataclasses import dataclass
 from datetime import datetime
 from logging import Logger
 from typing import Optional
-from unittest import TestSuite
 
 from ruamel.yaml import YAML  # type: ignore
 
 from . import Step
 from .build.dockerbuild import BuildDocker
 from .build.echo import BuildEcho
 from .build.sbt import BuildSbt
@@ -24,15 +22,14 @@
 from .models import Output, Input, RunProperties, ArtifactType, Artifact
 from .postdeploy.cypress_test import CypressTest
 from .test.dockertest import TestDocker
 from .test.echo import TestEcho
 from .test.sbt import TestSbt
 from ..project import Project
 from ..project import Stage
-from ..utilities.junit import to_test_suites
 from ..validation import validate
 
 yaml = YAML()
 
 
 class ExecutionException(Exception):
     """ Exception thrown when a step execution fails. """
@@ -49,26 +46,14 @@
 class StepResult:
     stage: Stage
     project: Project
     output: Output
     timestamp: datetime = datetime.now()
 
 
-def collect_test_artifacts(step_results: list[StepResult]) -> list[Artifact]:
-    return [res.output.produced_artifact for res in step_results if
-            (res.output.produced_artifact and
-             res.output.produced_artifact.artifact_type == ArtifactType.JUNIT_TESTS)]
-
-
-def collect_test_results(test_artifacts: list[Artifact]) -> list[TestSuite]:
-    suites: list[list[TestSuite]] = list(map(to_test_suites, test_artifacts))
-
-    return list(itertools.chain(*suites))
-
-
 class Steps:
     """ Executor of individual steps within a pipeline. """
     _step_executors: dict[Stage, set[Step]]
     _logger: Logger
     _properties: RunProperties
 
     def __init__(self, logger: Logger, properties: RunProperties) -> None:
```

## mpyl/steps/deploy/cloudfront_kubernetes_deploy.py

```diff
@@ -3,15 +3,15 @@
 from logging import Logger
 import tempfile
 
 from .kubernetes import DeployKubernetes
 from .. import Step, Meta
 from ...project import Stage
 from ..models import Input, Output, ArtifactType
-from ...utilities.docker import docker_image_tag, docker_copy
+from ...utilities.docker import docker_image_tag, docker_copy, create_container
 from ...utilities.s3 import S3Client, S3ClientConfig
 
 STATIC_FOLDER = 'static'
 
 
 class CloudFrontKubernetesDeploy(Step):
 
@@ -35,17 +35,16 @@
     @staticmethod
     def __copy_docker_assets(logger: Logger, step_input: Input, tmp_folder: str):
         """
         Copies the static assets from the docker image to a temp folder
         """
         image_name = docker_image_tag(step_input)
         container_path = f'{step_input.project.name}/{STATIC_FOLDER}'
-
-        docker_copy(logger=logger, container_path=container_path, dst_path=tmp_folder,
-                    image_name=image_name)
+        container = create_container(logger, image_name)
+        docker_copy(logger=logger, container_path=container_path, dst_path=tmp_folder, container=container)
 
     @staticmethod
     def __upload_to_s3(logger: Logger, step_input: Input, tmp_folder: str):
         """
         Creates an S3 client and uploads the static assets stored in the temp folder
         """
         logger.info("Creating S3 client")
```

## mpyl/steps/deploy/kubernetes.py

```diff
@@ -1,17 +1,17 @@
 """ Step that deploys the docker image produced in the build stage to Kubernetes, using HELM. """
 import re
 from logging import Logger
 from typing import Optional
 
-from .k8s import deploy_helm_chart, CustomResourceDefinition
+from .k8s import deploy_helm_chart, CustomResourceDefinition, cluster_config
 from .k8s.chart import ChartBuilder, to_service_chart
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact
-from ...project import Stage
+from ...project import Stage, Target
 from ...stages.discovery import find_deploy_set
 from ...utilities.repo import RepoConfig
 
 DEPLOYED_SERVICE_KEY = 'url'
 
 
 class DeployKubernetes(Step):
@@ -35,24 +35,37 @@
             routes = ingress.spec.get('routes', {})
             if routes:
                 match = routes[0].get('match')
                 return DeployKubernetes.match_to_url(match)
         return None
 
     def execute(self, step_input: Input) -> Output:
-        builder = ChartBuilder(step_input, find_deploy_set(RepoConfig.from_config(step_input.run_properties.config)))
+        properties = step_input.run_properties
+        builder = ChartBuilder(step_input, find_deploy_set(repo_config=RepoConfig.from_config(properties.config),
+                                                           tag=step_input.run_properties.versioning.tag))
         chart = to_service_chart(builder)
 
-        deploy_result = deploy_helm_chart(self._logger, chart, step_input, builder.release_name)
+        target_cluster = cluster_config(properties.target, properties)
+        deploy_result = deploy_helm_chart(self._logger, chart, step_input, target_cluster, builder.release_name)
         if deploy_result.success:
             hostname = self.try_extract_hostname(chart)
             spec = {}
             if hostname:
                 has_specific_routes_configured: bool = bool(builder.deployment.traefik is not None)
                 self._logger.info(f"Service {step_input.project.name} reachable at: {hostname}")
 
                 endpoint = '/' if has_specific_routes_configured else '/swagger/index.html'
                 spec[DEPLOYED_SERVICE_KEY] = f'{hostname}{endpoint}'
             artifact = input_to_artifact(ArtifactType.DEPLOYED_HELM_APP, step_input, spec=spec)
+            if properties.target == Target.PRODUCTION:
+                self._logger.info(
+                    f"Release to production successful, updating base images in {Target.PULL_REQUEST_BASE} "
+                    f"to make sure the Test environment is in sync with production")
+                target_cluster = cluster_config(Target.PRODUCTION, properties)
+                deploy_to_prod_result = deploy_helm_chart(self._logger, chart, step_input, target_cluster,
+                                                          builder.release_name)
+                return Output(success=True, message=deploy_result.message + '\n' + deploy_to_prod_result.message,
+                              produced_artifact=artifact)
+
             return Output(success=True, message=deploy_result.message, produced_artifact=artifact)
 
         return deploy_result
```

## mpyl/steps/deploy/kubernetes_job.py

```diff
@@ -1,12 +1,12 @@
 """ A step to deploy a job to kubernetes. """
 
 from logging import Logger
 
-from .k8s import deploy_helm_chart
+from .k8s import deploy_helm_chart, cluster_config
 from .k8s.chart import ChartBuilder, to_cron_job_chart, to_job_chart
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
 from ...stages.discovery import find_deploy_set
 from ...utilities.repo import RepoConfig
 
@@ -18,10 +18,14 @@
             name='Kubernetes Job Deploy',
             description='Deploy a job to k8s',
             version='0.0.1',
             stage=Stage.DEPLOY
         ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
 
     def execute(self, step_input: Input) -> Output:
-        builder = ChartBuilder(step_input, find_deploy_set(RepoConfig.from_config(step_input.run_properties.config)))
+        run_properties = step_input.run_properties
+        builder = ChartBuilder(step_input, find_deploy_set(repo_config=RepoConfig.from_config(run_properties.config),
+                                                           tag=step_input.run_properties.versioning.tag))
         chart = to_cron_job_chart(builder) if builder.is_cron_job else to_job_chart(builder)
-        return deploy_helm_chart(self._logger, chart, step_input, builder.release_name, delete_existing=True)
+        target_cluster = cluster_config(run_properties.target, run_properties)
+        return deploy_helm_chart(self._logger, chart, step_input, target_cluster, builder.release_name,
+                                 delete_existing=True)
```

## mpyl/steps/deploy/kubernetes_spark_job.py

```diff
@@ -1,12 +1,12 @@
 """ A step to deploy a job to kubernetes. """
 
 from logging import Logger
 
-from .k8s import deploy_helm_chart
+from .k8s import deploy_helm_chart, cluster_config
 from .k8s.chart import ChartBuilder, to_spark_job_chart
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
 from ...stages.discovery import find_deploy_set
 from ...utilities.repo import RepoConfig
 
@@ -18,11 +18,14 @@
             name='Kubernetes Spark Job Deploy',
             description='Deploy a Spark Job to the Spark Operator',
             version='0.0.1',
             stage=Stage.DEPLOY
         ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
 
     def execute(self, step_input: Input) -> Output:
+        run_properties = step_input.run_properties
         chart = to_spark_job_chart(
-            ChartBuilder(step_input, find_deploy_set(RepoConfig.from_config(step_input.run_properties.config))))
-        return deploy_helm_chart(self._logger, chart, step_input, ChartBuilder(step_input).release_name,
+            ChartBuilder(step_input, find_deploy_set(repo_config=RepoConfig.from_config(run_properties.config),
+                                                     tag=step_input.run_properties.versioning.tag)))
+        target_cluster = cluster_config(run_properties.target, run_properties)
+        return deploy_helm_chart(self._logger, chart, step_input, target_cluster, ChartBuilder(step_input).release_name,
                                  delete_existing=True)
```

## mpyl/steps/deploy/k8s/__init__.py

```diff
@@ -5,15 +5,15 @@
 from kubernetes import config, client
 
 from ...deploy.k8s.resources import CustomResourceDefinition
 from ...models import RunProperties
 from ....project import Project, Target, ProjectName
 from ....steps import Input, Output
 from ....steps.deploy.k8s import helm
-from ....steps.deploy.k8s.rancher import cluster_config, rancher_namespace_metadata
+from ....steps.deploy.k8s.rancher import cluster_config, rancher_namespace_metadata, ClusterConfig
 
 
 def get_namespace(run_properties: RunProperties, project: Project) -> Optional[str]:
     if run_properties.target == Target.PULL_REQUEST:
         return run_properties.versioning.identifier
 
     return get_namespace_from_project(project)
@@ -42,19 +42,19 @@
     else:
         logger.info(f"Found namespace {namespace}")
 
     return namespace
 
 
 def deploy_helm_chart(logger: Logger, chart: dict[str, CustomResourceDefinition], step_input: Input,
+                      target_cluster: ClusterConfig,
                       release_name: str, delete_existing: bool = False) -> Output:
-    context = cluster_config(step_input).context
-    namespace = upsert_namespace(logger, step_input, context)
+    namespace = upsert_namespace(logger, step_input, target_cluster.context)
 
-    return helm.install(logger, chart, step_input, release_name, namespace, context, delete_existing)
+    return helm.install(logger, chart, step_input, release_name, namespace, target_cluster.context, delete_existing)
 
 
 def substitute_namespaces(env_vars: dict[str, str], all_projects: set[ProjectName],
                           projects_to_deploy: set[ProjectName],
                           pr_identifier: Optional[int]) -> dict[str, str]:
     env = env_vars.copy()
```

## mpyl/steps/deploy/k8s/rancher.py

```diff
@@ -1,13 +1,14 @@
 """ Utilities for creating rancher compatible helm charts. """
 
 from dataclasses import dataclass
 
-from ....steps import Input
+from ...models import RunProperties
 from ....project import Target
+from ....steps import Input
 
 
 @dataclass(frozen=True)
 class ClusterConfig:
     project_id: str
     cluster_id: str
     cluster_env: str
@@ -15,29 +16,28 @@
 
     @staticmethod
     def from_config(config: dict):
         return ClusterConfig(project_id=config['clusterId'], cluster_id=config['clusterId'],
                              cluster_env=config['clusterEnv'], context=config['context'])
 
 
-def cluster_config(step_input: Input):
-    target = step_input.run_properties.target
-    cluster_configs = step_input.run_properties.config['kubernetes']['rancher']['cluster']
+def cluster_config(target: Target, run_properties: RunProperties) -> ClusterConfig:
+    cluster_configs = run_properties.config['kubernetes']['rancher']['cluster']
 
     if target in {Target.PULL_REQUEST, Target.PULL_REQUEST_BASE}:
         return ClusterConfig.from_config(cluster_configs['test'])
     if target == Target.ACCEPTANCE:
         return ClusterConfig.from_config(cluster_configs['acceptance'])
     if target == Target.PRODUCTION:
         return ClusterConfig.from_config(cluster_configs['production'])
-    return None
+    raise ValueError(f"Unknown target {target}")
 
 
 def rancher_namespace_metadata(namespace: str, step_input: Input):
-    rancher_config = cluster_config(step_input)
+    rancher_config = cluster_config(step_input.run_properties.target, step_input.run_properties)
 
     return {
         'annotations': {
             'field.cattle.io/projectId': f'{rancher_config.cluster_id}:{rancher_config.project_id}',
             'lifecycle.cattle.io/create.namespace-auth': 'true'
         },
         'labels': {
```

## mpyl/steps/postdeploy/cypress_test.py

```diff
@@ -7,15 +7,15 @@
 from python_on_whales import docker, Container, DockerException
 
 from .. import Step, Meta
 from ..models import ArtifactType, Input, Output, input_to_artifact
 from ...project import Stage, Target
 from ...utilities.cypress import CypressConfig
 from ...utilities.docker import execute_with_stream
-from ...utilities.junit import TEST_OUTPUT_PATH_KEY
+from ...utilities.junit import TEST_OUTPUT_PATH_KEY, TEST_RESULTS_URL_KEY
 
 
 class CypressTest(Step):
     def __init__(self, logger: Logger) -> None:
         super().__init__(logger, Meta(
             name='Cypress Test',
             description='Step to run cypress tests',
@@ -32,26 +32,30 @@
         volume_path = os.path.join(os.getcwd(), cypress_config.cypress_source_code_path)
 
         if step_input.project.dependencies and step_input.project.dependencies.postdeploy:
             specs_string = ', '.join(step_input.project.dependencies.postdeploy)
         else:
             raise ValueError("No cypress specs are defined in the project dependencies")
 
-        cypress_results_url = ''
         custom_image_tag = "mpyl/cypress"
         docker.build(context_path=volume_path, tags=[custom_image_tag], file=f"{volume_path}/Dockerfile-mpyl")
         docker_container = docker.run(image=custom_image_tag, interactive=True, detach=True,
                                       volumes=[
                                           (volume_path, "/cypress"),
                                           (os.path.expanduser(cypress_config.kubectl_config_path), "/root/.kube/config")
                                       ],
                                       workdir="/cypress")
         if not isinstance(docker_container, Container):
             raise TypeError("Docker run command should return a container")
 
+        reports_folder = f"reports/{step_input.project.name}"
+        artifact = input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
+                                     spec={TEST_OUTPUT_PATH_KEY: f"{volume_path}/{reports_folder}",
+                                           TEST_RESULTS_URL_KEY: ''})
+
         try:
             execute_with_stream(logger=self._logger, container=docker_container,
                                 command='bash -c "cp cypress.env.json.example cypress.env.json && '
                                         f"sed -i 's/acceptance/"
                                         f"{CypressTest._target_to_test_target(step_input.run_properties.target)}"
                                         f"/' cypress.env.json && "
                                         f"sed -i 's/{{PR_NUMBER}}/{step_input.run_properties.versioning.pr_number}/' "
@@ -61,43 +65,42 @@
                                 task_name="Running yarn install")
             execute_with_stream(logger=self._logger, container=docker_container, command="yarn cypress install",
                                 task_name="Installing cypress")
             execute_with_stream(logger=self._logger, container=docker_container, command="yarn cypress verify",
                                 task_name="Verifying cypress")
             execute_with_stream(logger=self._logger, container=docker_container, command="yarn tsc",
                                 task_name="Compiling typescript")
+            execute_with_stream(logger=self._logger, container=docker_container, command=f"rm -rf {reports_folder}",
+                                task_name="Remove old report files")
 
-            run_command = f'bash -c "yarn cypress run --spec {specs_string} || true"'
+            run_command = f'bash -c "yarn cypress run --spec {specs_string} --reporter-options mochaFile=' \
+                          f'"{reports_folder}/[hash].xml" || true"'
             record_key = cypress_config.record_key
             if record_key:
-                run_command = f'bash -c "yarn cypress run --spec {specs_string} --record --key ' \
+                run_command = f'bash -c "yarn cypress run --spec {specs_string} --reporter-options ' \
+                              f'"mochaFile={reports_folder}/[hash].xml" --record --key ' \
                               f'b6a2aab1-0b80-4ca0-a56c-1c8d98a8189c || true "'
             result = execute_with_stream(logger=self._logger, container=docker_container, command=run_command,
                                          task_name="Running cypress tests")
 
             for stdout in result:
                 if record_key and "Recorded Run" in stdout:
-                    cypress_results_url = stdout.rstrip().rsplit('Recorded Run: ', 1)[1]
+                    artifact.spec[TEST_RESULTS_URL_KEY] = stdout.rstrip().rsplit('Recorded Run: ', 1)[1]
                 if "error Command failed with exit code" in stdout:
                     raise DockerException(command_launched=[run_command], return_code=1)
         except DockerException:
             return Output(success=False,
                           message=f"Cypress tests for project {step_input.project.name} have one or more failures",
-                          produced_artifact=input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS,
-                                                              step_input=step_input,
-                                                              spec={TEST_OUTPUT_PATH_KEY: volume_path,
-                                                                    "cypress_results_url": cypress_results_url}))
+                          produced_artifact=artifact)
         finally:
             docker_container.stop()
             docker_container.remove()
 
         return Output(success=True, message=f"Cypress tests for project {step_input.project.name} passed",
-                      produced_artifact=input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                                          spec={TEST_OUTPUT_PATH_KEY: volume_path,
-                                                                "cypress_results_url": cypress_results_url}))
+                      produced_artifact=artifact)
 
     @staticmethod
     def _target_to_test_target(target: Target) -> str:
         if target == Target.PULL_REQUEST_BASE:
             return 'test'
         if target == Target.ACCEPTANCE:
             return 'acceptance'
```

## mpyl/steps/test/dockertest.py

```diff
@@ -10,21 +10,24 @@
 The test results need to be writted  written to a folder named `$WORKDIR/target/test-reports/` for
 `TestDocker.extract_test_results` to find and extract them.
 
 
 """
 from logging import Logger
 
+from python_on_whales import Container
+
 from .after_test import IntegrationTestAfter
 from .before_test import IntegrationTestBefore
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact, Artifact
 from ...project import Stage, Project
-from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path, docker_copy
-from ...utilities.junit import to_test_suites, sum_suites, TEST_OUTPUT_PATH_KEY
+from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path, docker_copy, \
+    remove_container, create_container
+from ...utilities.junit import to_test_suites, sum_suites, TEST_OUTPUT_PATH_KEY, TEST_RESULTS_URL_KEY
 
 
 class TestDocker(Step):
     def __init__(self, logger: Logger) -> None:
         meta = Meta(name='Docker Test', description='Test docker image', version='0.0.1', stage=Stage.TEST)
         super().__init__(
             logger=logger, meta=meta,
@@ -39,32 +42,38 @@
         test_target = docker_config.test_target
         if not test_target:
             raise ValueError('docker.testTarget must be specified')
 
         tag = docker_image_tag(step_input) + '-test'
         project = step_input.project
         dockerfile = docker_file_path(project=project, docker_config=docker_config)
-
         success = build(logger=self._logger, root_path=docker_config.root_folder,
                         file_path=dockerfile, image_tag=tag, target=test_target)
+        container = create_container(self._logger, tag)
 
         if success:
-            artifact = self.extract_test_results(self._logger, project, tag, step_input)
+            artifact = self.extract_test_results(self._logger, project, container, step_input)
 
             suite = to_test_suites(artifact)
             summary = sum_suites(suite)
 
-            return Output(success=summary.is_success, message=f"Tests results produced for {project.name} ({summary})",
-                          produced_artifact=artifact)
+            output = Output(success=summary.is_success,
+                            message=f"Tests results produced for {project.name} ({summary})",
+                            produced_artifact=artifact)
+        else:
+            output = Output(success=False,
+                            message=f"Tests failed to run for {project.name}. No test results have been recorded.",
+                            produced_artifact=None)
+
+        remove_container(self._logger, container)
 
-        return Output(success=False,
-                      message=f"Tests failed to run for {project.name}. No test results have been recorded.",
-                      produced_artifact=None)
+        return output
 
     @staticmethod
-    def extract_test_results(logger: Logger, project: Project, tag: str, step_input: Input) -> Artifact:
-        test_result_path = f'{project.target_path}/test_results'
-        path_in_container = f'/{project.test_report_path}/'
-        docker_copy(logger=logger, container_path=path_in_container, dst_path=test_result_path, image_name=tag)
+    def extract_test_results(logger: Logger, project: Project, container: Container, step_input: Input) -> Artifact:
+        path_in_container = f'{project.test_report_path}/.'
+        docker_copy(logger=logger, container_path=path_in_container, dst_path=project.test_report_path,
+                    container=container)
 
         return input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                 spec={TEST_OUTPUT_PATH_KEY: f'{test_result_path}'})
+                                 spec={TEST_OUTPUT_PATH_KEY: project.test_report_path,
+                                       TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url})
```

## mpyl/steps/test/echo.py

```diff
@@ -2,15 +2,15 @@
 
 from logging import Logger
 from pathlib import Path
 
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...project import Stage
-from ...utilities.junit import TEST_OUTPUT_PATH_KEY
+from ...utilities.junit import TEST_OUTPUT_PATH_KEY, TEST_RESULTS_URL_KEY
 
 SAMPLE_JUNIT_RESULT = """
 <?xml version="1.0" encoding="UTF-8"?>
 <testsuites name="jest tests" tests="1" failures="0" errors="0" time="0.486">
   <testsuite name="undefined" errors="0" failures="0" skipped="0" timestamp="2023-03-29T02:51:00" time="0.244" tests="1">
     <testcase classname="Test Echo" name=" fake test case from TestEcho step" time="0.002">
     </testcase>
@@ -32,9 +32,10 @@
     def execute(self, step_input: Input) -> Output:
         self._logger.info(f"Testing project {step_input.project.name}")
         path = Path(step_input.project.target_path, "test_results")
         path.mkdir(parents=True, exist_ok=True)
         Path(path, "test.xml").write_text(SAMPLE_JUNIT_RESULT, encoding='utf-8')
 
         artifact = input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                     spec={TEST_OUTPUT_PATH_KEY: str(path)})
+                                     spec={TEST_OUTPUT_PATH_KEY: str(path),
+                                           TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url})
         return Output(success=True, message=f"Tested {step_input.project.name}", produced_artifact=artifact)
```

## mpyl/steps/test/sbt.py

```diff
@@ -4,15 +4,15 @@
 
 from .after_test import IntegrationTestAfter
 from .before_test import IntegrationTestBefore
 from .. import Input, Output, Step
 from ..models import Artifact, input_to_artifact
 from ...project import Stage, Project
 from ...steps import Meta, ArtifactType
-from ...utilities.junit import TEST_OUTPUT_PATH_KEY, to_test_suites, sum_suites
+from ...utilities.junit import TEST_OUTPUT_PATH_KEY, to_test_suites, sum_suites, TEST_RESULTS_URL_KEY
 from ...utilities.sbt import SbtConfig
 from ...utilities.subprocess import custom_check_output
 
 
 class TestSbt(Step):
     def __init__(self, logger: Logger) -> None:
         meta = Meta(name='Sbt Test', description='Run sbt tests', version='0.0.1', stage=Stage.TEST)
@@ -94,8 +94,9 @@
     @staticmethod
     def _construct_sbt_command(step_input: Input, config: SbtConfig, commands_fn: Callable[[Input], list[str]]):
         return config.to_command(config.test_with_client, commands_fn(step_input))
 
     @staticmethod
     def _extract_test_report(project: Project, step_input: Input) -> Artifact:
         return input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                 spec={TEST_OUTPUT_PATH_KEY: f'{project.test_report_path}'})
+                                 spec={TEST_OUTPUT_PATH_KEY: f'{project.test_report_path}',
+                                       TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url})
```

## mpyl/utilities/docker/__init__.py

```diff
@@ -1,21 +1,23 @@
 """Docker related utility methods"""
 import logging
 import shlex
 
 from dataclasses import dataclass
 from itertools import tee
 from logging import Logger
+from traceback import print_exc
 from typing import Dict, Optional, Iterator, cast, Union
 import shutil
 from pathlib import Path
-from python_on_whales import docker, Image, Container
+from python_on_whales import docker, Image, Container, DockerException
 from python_on_whales.exceptions import NoSuchContainer
 from rich.text import Text
 
+from ..logging import try_parse_ansi
 from ...project import Project
 from ...steps.models import Input
 
 
 @dataclass(frozen=True)
 class DockerComposeConfig:
     period_seconds: int
@@ -74,75 +76,97 @@
     copied_logs = []
 
     while True:
         try:
             next_item = next(generator)
             log_line = next_item[1].decode(errors="replace") if isinstance(next_item, tuple) else next_item
             copied_logs.append(log_line)
-            logger.log(level, Text.from_ansi(log_line))
+            logger.log(level, try_parse_ansi(log_line))
         except StopIteration:
             logger.info(f'{task_name} complete.')
             return copied_logs
 
 
 def docker_image_tag(step_input: Input):
     git = step_input.run_properties.versioning
-    tag = f"pr-{git.pr_number}" if git.pr_number else git.tag
+    tag = git.tag if git.tag else f"pr-{git.pr_number}"
     return f"{step_input.project.name.lower()}:{tag}".replace('/', '_')
 
 
 def docker_file_path(project: Project, docker_config: DockerConfig):
     return f'{project.deployment_path}/{docker_config.docker_file_name}'
 
 
-def docker_copy(logger: Logger, container_path: str, dst_path: str, image_name: str):
+def docker_copy(logger: Logger, container_path: str, dst_path: str, container: Container):
     """
     Copies the contents of the specified path within the container to a locally created destination
 
     :param logger: the logger
     :param container_path: the path of the directory in the container to copy
     :param dst_path: the path to copy the container content to
-    :param image_name: the name of the docker image which a container is created from
+    :param container: the container to copy from
     """
     shutil.rmtree(dst_path, ignore_errors=True)
     Path(dst_path).mkdir(parents=True, exist_ok=True)
 
-    container = docker.create(image_name)
-
     if not docker.container.exists(container.id):
         raise ValueError(f'Container {container.id} does not exist')
 
     logger.info(
         f"Copying contents from container {container.id} at "
         f"path {container_path} to host at {dst_path}"
     )
     try:
         docker.copy(f'{container.id}:{container_path}', dst_path)
     except NoSuchContainer as exc:
-        logger.warning(f'Could not find data in container {image_name} at expected location {container_path}')
+        logger.warning(f'Could not find data in container {container.name} at expected location {container_path}')
         raise exc
 
 
 def build(logger: Logger, root_path: str, file_path: str, image_tag: str, target: str) -> bool:
     """
     :param logger: the logger
     :param root_path: the root path to which `docker_file_path` is relative
     :param file_path: path to the docker file to be built
     :param image_tag: the tag of the image
     :param target: the 'target' within the multi-stage docker image
     :return: True if success, False if failure
     """
     logger.info(f"Building docker image with {file_path} and target {target}")
 
-    logs = docker.buildx.build(context_path=root_path, file=file_path, tags=[image_tag], target=target,
-                               stream_logs=True)
-    if logs is not None and not isinstance(logs, Image):
-        stream_docker_logging(logger=logger, generator=logs, task_name=f'Build {file_path}:{target}')
-    logger.debug(logs)
-    return True
+    try:
+        logs = docker.buildx.build(context_path=root_path, file=file_path, tags=[image_tag], target=target,
+                                   stream_logs=True)
+        if logs is not None and not isinstance(logs, Image):
+            stream_docker_logging(logger=logger, generator=logs, task_name=f'Build {file_path}:{target}')
+        logger.debug(logs)
+        return True
+
+    except DockerException as exc:
+        command = " ".join(exc.docker_command)
+        logger.warning(f"Docker build failed with command {command} and exit code {exc.return_code}")
+        return False
+    except Exception as exc:  # pylint: disable=broad-exception-caught
+        print(f"Docker build failed with {exc.__class__.__name__}")
+        print_exc()
+        return False
 
 
 def login(logger: Logger, docker_config: DockerConfig) -> None:
     logger.info(f"Logging in with user '{docker_config.user_name}'")
     docker.login(server=f'https://{docker_config.host_name}', username=docker_config.user_name,
                  password=docker_config.password)
     logger.debug(f"Logged in as '{docker_config.user_name}'")
+
+
+def create_container(logger: Logger, image_name: str) -> Container:
+    logger.info(f"Creating container from image {image_name}")
+    container = docker.create(image_name)
+    logger.info(f"Created container {container.id}")
+
+    return container
+
+
+def remove_container(logger: Logger, container: Container) -> None:
+    logger.info(f"Removing container {container.id}")
+    docker.remove(container.id)
+    logger.info(f"Removed container {container.id}")
```

## mpyl/utilities/jenkins/runner.py

```diff
@@ -15,18 +15,18 @@
 from rich.errors import MarkupError
 from rich.live import Live
 from rich.progress import Progress, TimeElapsedColumn, TextColumn, BarColumn, TaskProgressColumn, \
     TimeRemainingColumn
 from rich.prompt import Confirm
 from rich.status import Status
 from rich.table import Column
-from rich.text import Text
 
 from . import Pipeline
 from ...cli.commands.build import play_sound, Sound
+from ..logging import try_parse_ansi
 
 
 def stream_utf_8_logs(self, interval=0):
     """
     Return generator which streams parts of text console.
     Workaround for https://github.com/pycontribs/jenkinsapi/pull/843
     """
@@ -146,15 +146,15 @@
             for line in build_to_follow.stream_utf_8_logs():
                 elapsed_time = time.time() - start_time
                 lines = line.rstrip().split('\n')
 
                 try:
                     text = "".join(lines)
                     if verbose:
-                        progress.log(Text.from_ansi(text))
+                        progress.log(try_parse_ansi(text))
                     else:
                         log_line.update(label_task_id, description=text)
                 except MarkupError:
                     progress.log("Could not render log line")
                 progress.update(build_task_id, completed=elapsed_time)
             progress.update(build_task_id, completed=duration_estimation)
```

## mpyl/utilities/junit/__init__.py

```diff
@@ -4,14 +4,16 @@
 from pathlib import Path
 
 from junitparser import JUnitXml, TestSuite
 
 from ...steps.models import Artifact, ArtifactType
 
 TEST_OUTPUT_PATH_KEY = 'test_output_path'
+TEST_RESULTS_URL_KEY = 'test_results_url'
+TEST_RESULTS_URL_NAME_KEY = 'test_results_url_name'
 
 
 @dataclass(frozen=True)
 class TestRunSummary:
     tests: int
     failures: int
     errors: int
```

## mpyl/utilities/repo/__init__.py

```diff
@@ -6,14 +6,15 @@
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Optional
 from urllib.parse import urlparse
 
 from git import Git, Repo, Remote
+from git.objects import Commit
 
 from ...project import Project
 
 
 @dataclass(frozen=True)
 class Revision:
     ord: int
@@ -106,20 +107,26 @@
     def __get_filter_patterns(self):
         return ["--"] + [f":!{pattern}" for pattern in self._config.ignore_patterns]
 
     @property
     def latest_tag(self) -> str:
         return str(sorted(self._repo.tags, key=lambda t: t.commit.committed_datetime)[-1])
 
+    def __to_revision(self, count: int, revision: Commit, files_touched_in_branch: set[str]) -> Revision:
+        files_in_revision = set(
+            self._repo.git.diff_tree(self.__get_filter_patterns(), no_commit_id=True, name_only=True,
+                                     r=str(revision)).splitlines())
+        intersection = files_in_revision.intersection(files_touched_in_branch)
+        return Revision(count, str(revision), intersection)
+
     def changes_in_branch(self) -> list[Revision]:
-        revisions = reversed(list(self._repo.iter_commits(f"{self._config.main_branch}..HEAD")))
-        return [Revision(count, str(rev),
-                         self._repo.git.diff_tree(self.__get_filter_patterns(), no_commit_id=True, name_only=True,
-                                                  r=str(rev), ).splitlines()) for
-                count, rev in enumerate(revisions)]
+        revisions = list(reversed(list(self._repo.iter_commits(f"{self._config.main_branch}..HEAD"))))
+        files_touched_in_branch = set(
+            self._repo.git.diff(f'{revisions[0].hexsha}..{revisions[-1].hexsha}', name_only=True).splitlines())
+        return [self.__to_revision(count, rev, files_touched_in_branch) for count, rev in enumerate(revisions)]
 
     def changes_in_commit(self) -> set[str]:
         changed: set[str] = set(self._repo.git.diff(self.__get_filter_patterns(), None, name_only=True).splitlines())
         return changed.union(self._repo.untracked_files)
 
     def changes_in_branch_including_local(self) -> list[Revision]:
         in_branch = self.changes_in_branch()
@@ -137,20 +144,22 @@
 
     def changes_in_merge_commit(self):
         parent_revs = self._repo.head.commit.parents
         if not parent_revs:
             logging.error("HEAD is not at merge commit, cannot determine changed files.")
             return []
         logging.debug(f"Parent revisions: {parent_revs}")
-        files_changed = self._repo.git.diff(f"{str(parent_revs[0])}..{str(parent_revs[1])}",
+        files_changed = self._repo.git.diff(f"{str(self._repo.head.commit)}..{str(parent_revs[0])}",
                                             name_only=True).splitlines()
         return [Revision(ord=0, hash=str(self.get_sha), files_touched=files_changed)]
 
     @property
     def main_branch_pulled(self) -> bool:
+        if self._repo.head.is_detached:
+            return False
         branch_names = list(map(lambda n: n.name, self._repo.references))
         return f'{self._config.main_branch}' in branch_names
 
     def __get_remote(self) -> Remote:
         default_remote = self._repo.remote('origin')
         if 'https:' not in default_remote.url or self._config.repo_credentials is None:
             return default_remote
```

## Comparing `mpyl-1.0.5.dist-info/LICENSE` & `mpyl-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mpyl-1.0.5.dist-info/METADATA` & `mpyl-1.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpyl
-Version: 1.0.5
+Version: 1.0.6
 Summary: Modular Pipeline Library
 Home-page: https://vandebron.github.io/mpyl
 Author: Vandebron Energie BV
 Project-URL: Documentation, https://vandebron.github.io/mpyl
 Project-URL: Source, https://github.com/Vandebron/mpyl
 Project-URL: Tracker, https://github.com/Vandebron/mpyl/issues
 Classifier: Topic :: Software Development :: Build Tools
```

## Comparing `mpyl-1.0.5.dist-info/RECORD` & `mpyl-1.0.6.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 mpyl/__init__.py,sha256=sLR4OPN49X7SpQiYro_GrizAvJo_CI7nXiZh662D7OE,766
 mpyl/__main__.py,sha256=S7WS_61OT3kRc5RJq3vz4AI6N4YRU5h2KG1kBeQKK6I,215
 mpyl/constants.py,sha256=mr9QfGfl56MCHthSyWkFQfDTHrxMuxLW-1xy6TtHKKQ,162
-mpyl/project.py,sha256=VHpyOsWYbi0nQ9EcJ7A8CZ84gr0jlyG1JGnQVTYJo9o,13469
+mpyl/project.py,sha256=91aqusKKQUnB29kem8cxs7GVuqyCgEAAC2YkSLqLYW4,13526
 mpyl/validation.py,sha256=EMbkceP3w805916gdoKqGeD1SPONu3FEb2cJld5V05E,1708
 mpyl/cli/__init__.py,sha256=3sN-_zD8pS3JdHh49qC77aFdwIGTXEV2nGxZbc5Ijx8,2163
-mpyl/cli/build.py,sha256=GKLgpW9-dM7Yh1Fzqyr3SYxf0J4YUmjYp8XaC4vRGfg,10555
+mpyl/cli/build.py,sha256=UWttK-sNbY3tU7HYl763005yTMjcd_mN_FhvlhRT_1Q,10619
 mpyl/cli/health.py,sha256=ny37_DVoqXp8IxGQt9KeBZdrbvtd2WGxXtANXPDiENo,341
 mpyl/cli/meta_info.py,sha256=MJhWR8GxSL1Anx7Cs_6c0QU6_tYP_pNxaazGV8JoO60,2170
 mpyl/cli/projects.py,sha256=m6AYs8cn-TGTgobktzKd2MW7xj9D8Sm5GEkMXYVj1vA,3915
 mpyl/cli/commands/__init__.py,sha256=DaL5q4ibFJT7EMlgcQBSpAaaQNiBqnSJZ2WIKtPzLJk,34
 mpyl/cli/commands/build/__init__.py,sha256=Ox0F68re6bNGLBC4KEBLmXXSRf5OIJZ8N2Vens3rgEk,439
-mpyl/cli/commands/build/jenkins.py,sha256=ao1oRp-Hi26roh1EmHLOuqTuvrRncI0H5MT590wKlTg,3822
-mpyl/cli/commands/build/mpyl.py,sha256=6D2d-MrhH2cjP9lTEGESoSnbzJejDd0mYktBvKat82U,5802
+mpyl/cli/commands/build/jenkins.py,sha256=GYXj4N0GLIm23Lx8hTIEhlGTxgUhyhYVnnhLD1LCfXQ,3923
+mpyl/cli/commands/build/mpyl.py,sha256=S03ZF4XamZAIgxm81xYXu7Pwwnhk7-ManCaa_bizTVc,5814
 mpyl/cli/commands/health/__init__.py,sha256=Bx6QcWIN-EadbpSe1XAXs1aYCD7Ad8_t3lWRlGDsIr0,38
-mpyl/cli/commands/health/checks.py,sha256=XEBcsrey-UsQBZJtPWn9wxOvJsEGZdVJalxYnczn3Mg,5090
+mpyl/cli/commands/health/checks.py,sha256=-GEUCE8Jrj-rhOv5hKEPQsNtB_TGqmsKVA59ysw8CqQ,5200
 mpyl/cli/commands/projects/__init__.py,sha256=YoVobAUCYwqc23p-iAuQnpJQYpdri5ljtj8l_XKYOr0,46
 mpyl/cli/commands/projects/formatting.py,sha256=bhoLOUunClIPmSM6eZzJqHgTsdy6fidtz455IlV4xEU,1039
 mpyl/projects/__init__.py,sha256=31HPF5jDZK5UkQT8Zw0V0QSJLqzp8f2zFiWd-QkDjRE,620
 mpyl/projects/find.py,sha256=iUA1_8Tz3tZs-GvEQyvru3g9o3erSt5yxCHXLm96h4k,1993
 mpyl/reporting/__init__.py,sha256=vRvt_67opWXCfe_zYZChT-YhjoPOahAjLagoaVzOcFM,92
 mpyl/reporting/formatting/__init__.py,sha256=GAvYJpHT2SMQxjiLCSqFy57PNWsGI_Ow2bFnA8cX08k,76
-mpyl/reporting/formatting/markdown.py,sha256=n1KesnX2SzNan2L_tN0wPuaxOWDAaXceVeXDAbPsmHI,3664
+mpyl/reporting/formatting/markdown.py,sha256=PGPbgYMcr9xEmKQZWc_QUbNjl_lQ1yaRydSLbr2-3FE,4909
 mpyl/reporting/formatting/text.py,sha256=zgRnXSvnwi69mCbAsmcJgiU0PITe9uD8cBgPat4l6t8,1413
 mpyl/reporting/targets/__init__.py,sha256=ePSvaZMALkukb0ovhKRGkyIcwavI_VZi7GUeRuLMeEo,1096
 mpyl/reporting/targets/github.py,sha256=en1ph8y_cVh4jaDeoZLsTPngZW6oxWu4DM6v2Md3p3g,7939
-mpyl/reporting/targets/jira.py,sha256=XLHi99E2liSnHSxu1mk_DUJ8fsWH92WZupFqphl7WH4,8965
-mpyl/reporting/targets/slack.py,sha256=mfyHI447djo6hHxUoVniETjPlHCe3B8SHWbmGiKiy2U,7106
+mpyl/reporting/targets/jira.py,sha256=cc6ndmj3F1w7Y9wZTycMrlz_nCZXurq9aT7u5bCeCMU,9004
+mpyl/reporting/targets/slack.py,sha256=vzMlhHCN1Ldbv6Ssg6SZt2cF5s14H4NNeKkyZZadrqg,7366
 mpyl/schema/mpyl_config.schema.yml,sha256=f7j-04KI0Im1CoOZZ-Dale-Sw4RSnX0fdzsJ72FGKU8,8433
 mpyl/schema/project.schema.yml,sha256=Pn31oWBvupNXOVuUwykJv-P7C28eoELz5YwCJcKnntI,25500
 mpyl/schema/run_properties.schema.yml,sha256=A5T0m0_6JQ2D6yPHA6GyNNOggID9iWSnwWcfWCG6Fwk,2787
 mpyl/stages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mpyl/stages/discovery.py,sha256=Kv7zsV73jCPOelPiwXYNnMuomt2HDWh12xuzfvEpdfM,3439
+mpyl/stages/discovery.py,sha256=5u0QHC9RNjcu855Y0DqGKq2XP_1n42_H4sV-v0MDaqU,3506
 mpyl/steps/__init__.py,sha256=jpcKUPNLQm_8LngC7mbwYUzaoiisgyJy4R8u0qOkmAU,6135
-mpyl/steps/models.py,sha256=_TwBqCuMmQv4VBSuDVVpjXdk63-wTZ8KTcHyEx5hQKY,5977
+mpyl/steps/models.py,sha256=5IVLMwPf5AjRgod6W6ATWjMpNcSNACqtq-g92LnBs7k,5977
 mpyl/steps/run.py,sha256=ZzyljvUxkD6Qrwd9QXAFqXLxVFwyf7ZKUcZECkvbB6U,3429
-mpyl/steps/steps.py,sha256=4oIt_ePY9hY6oJEaoaYqer8ujJsf0dsX6IrjQb8bH_E,8978
+mpyl/steps/steps.py,sha256=QkT8S600vhPf9QQ_N2vq-iYjBE3__I55cckS1kZl6I4,8405
 mpyl/steps/build/__init__.py,sha256=EyPUNNDMQfJK-RVjYM9WvPhEDITbu2n4fx9mxhGLlDs,59
 mpyl/steps/build/docker_after_build.py,sha256=nok2HRrH66e9FBvfwEKnalJhX3io__PQZaq_fR0S8BI,2093
 mpyl/steps/build/dockerbuild.py,sha256=6lqVqiuGYk8ISuzTterTFdcIWqUkvSOUCOCDmjHkM2s,2865
 mpyl/steps/build/echo.py,sha256=on6n-zYs55z6_CouMrSTRIV_JDSTVdQ53raTt3im1qU,765
 mpyl/steps/build/sbt.py,sha256=rvJzIVgsx6KrX5HW_jqEhu6yV2QAttEXQRJ3A7XJJ-k,2402
 mpyl/steps/deploy/__init__.py,sha256=14PYgOvt7YEO2Zw4kEeZxWUNBR7Lz91nSoJZpvJHqzE,60
-mpyl/steps/deploy/cloudfront_kubernetes_deploy.py,sha256=fPbV0TGVO8pReO9EunVpnGC-IZ6jAM22wWfD0q8vj3o,2444
+mpyl/steps/deploy/cloudfront_kubernetes_deploy.py,sha256=4rE6n_Vh3QAl8QyA3Gv1elMcP3amrOUMkGbhVYfGCsU,2496
 mpyl/steps/deploy/echo.py,sha256=f43TQmiY96Da_OLZcjkQx-RjCvlo09Dclpezv9RoMlo,1001
 mpyl/steps/deploy/ephemeral_docker_deploy.py,sha256=NySUtyGl7xOjsgDK48AxorVik_iljcifWcRhJZADFs8,1310
-mpyl/steps/deploy/kubernetes.py,sha256=snsHFF04Ns_5kJ8utwXEGmY2sJN4k_Dvw70pmEN1tOE,2432
-mpyl/steps/deploy/kubernetes_job.py,sha256=8b2F-ew51ld1L1Az7Gr4_qYSQ2OngZBrQdVuoitMa_E,1111
-mpyl/steps/deploy/kubernetes_spark_job.py,sha256=bM4vKv7HylmcztAhuUpX5Vsnq-Hul3L8B0B0c37KzPE,1118
-mpyl/steps/deploy/k8s/__init__.py,sha256=OhApd2MdkCm0P7MAvs35qRBdSIbyPKOQBZMr3tivE88,3341
+mpyl/steps/deploy/kubernetes.py,sha256=UAUqQ9EcsT87RNH014TBnx7shcgqsvxP3e__RitC8eA,3415
+mpyl/steps/deploy/kubernetes_job.py,sha256=ME3O5PEnNGDdJHDp-iIWp5i1nFxgOyo7QMn2Axjec1U,1412
+mpyl/steps/deploy/kubernetes_spark_job.py,sha256=XHE_PrEMHGfualvdApAZJr7h0qwPDV9e5Lq2UCZSVDA,1380
+mpyl/steps/deploy/k8s/__init__.py,sha256=JcPfCITgl6JrHb-Enxe2dR1bk8mQ-SD2pIrKsjD80a8,3390
 mpyl/steps/deploy/k8s/chart.py,sha256=uTklf6xJRS1NCSlF_Z6uq2csw3fLlWWSCND07fKpV0Y,18819
 mpyl/steps/deploy/k8s/helm.py,sha256=0ZAMhuTMYyPDHfaUVNJDci3pZtGc3jyOXCaauznJf5U,2856
-mpyl/steps/deploy/k8s/rancher.py,sha256=9ZSBf3CQ-BRtkYJmQBleVLUaqQLkOA7QvYlr2N1Kous,1579
+mpyl/steps/deploy/k8s/rancher.py,sha256=TNxEcniLqvNif0ymqW2QvY1XPBiKXeh5o12EMNxTx-Y,1685
 mpyl/steps/deploy/k8s/resources/__init__.py,sha256=eSHp1ERR8FPPujHDiyLp8SchAza6TicPgx96zvSq4uQ,4467
 mpyl/steps/deploy/k8s/resources/sealed_secret.py,sha256=4q1POq2Z35putRlQ6cNWDBoTtRbFDDI2rr7JElCIzbM,591
 mpyl/steps/deploy/k8s/resources/spark.py,sha256=GT2lb66Xejb9uSdGE77ItaFBHh1K0IpJDX95RVHUxKQ,6143
 mpyl/steps/deploy/k8s/resources/traefik.py,sha256=uI8xE1KjywZ84OktNMPAB58JIu7tN4OT2V3iZO8tI7o,1948
 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml,sha256=jTo3LZklRCZ1L7JZbUdcmhDWhk3VDJhrDz_OTHNUm58,168371
 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml,sha256=s1rMobinpB3aXI1ONcuTMGLMIRRQ_qZrZtQTYZHcDFU,151469
 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml,sha256=3Oc1awM23acMS36kqpbfqwx6D8Sft4FnL8abNLgcwBI,11703
 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml,sha256=6QCi1F9LJ3cgmwaPBV8dWFvbXb2B5huKvfp4Pa1hoBw,42950
 mpyl/steps/postdeploy/__init__.py,sha256=cUDlHPzcW5zGGPxr9T77pATS5lwKnP9Ge8JroAGSvBg,64
-mpyl/steps/postdeploy/cypress_test.py,sha256=NyltDXfYkOLZ8QVH_di2pEqrREJZowhdhCN0VcCriCw,5924
+mpyl/steps/postdeploy/cypress_test.py,sha256=qVTaWKfUiL7ui3WLGa1hngD701mDXfEUMKTdMV8m4wU,6004
 mpyl/steps/test/__init__.py,sha256=XL1gSbIMJYSFcy4Vf8YRbZM9yAs3Fzvq2tfX9xTDZX8,58
 mpyl/steps/test/after_test.py,sha256=bKTBVFm88s4Kzr6JypxLAbKTlbRsha7gff3RjSr3ip0,1428
 mpyl/steps/test/before_test.py,sha256=IOUvAa3lKox8IKS28aGmmWJMNWcQWv9yGnTydVBvM14,2453
-mpyl/steps/test/dockertest.py,sha256=EhSZzjWti2wlKtx2xZiOZkBzjlmZZULsdkbOJAgtLMY,3218
-mpyl/steps/test/echo.py,sha256=Jm4oKYhauVbfBZ4D3m6hRY9FM5CikBNP07qcg6NhxmM,1657
-mpyl/steps/test/sbt.py,sha256=3igitohnF_B2qujC1XN1rbUaPxCOBiDMt0ypS8ngM7g,4885
+mpyl/steps/test/dockertest.py,sha256=upna6Q5tHkyZUpclaeYe7H7Y02JlMVvo2xxWWPlrdMg,3609
+mpyl/steps/test/echo.py,sha256=ShYQNzlCrhU10UKQSbmWm-GPZ9hEt6wE31bDfgxsBRU,1789
+mpyl/steps/test/sbt.py,sha256=4_tZrgyzBoCNWm6sV6XPM7qbUrlx50vVT-qv9UJP-ac,5013
 mpyl/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mpyl/utilities/cypress/__init__.py,sha256=cKSYzS1CfQgIClUX7Sj8EF5YlJ-34uck6rjyMJsBkFc,749
-mpyl/utilities/docker/__init__.py,sha256=ti4tDTEiuXT8MiiuhA06GafSR-N9Ye7RFXbORaVNobY,5583
+mpyl/utilities/docker/__init__.py,sha256=djMUvAeU2AUV6bRj13yLsuChoKW4L2DnAULzAfotO5o,6470
 mpyl/utilities/github/__init__.py,sha256=EnkcxQ5UQ08ZZOfShr3LFodu4pmzED9wMoHakIRbYO4,1739
 mpyl/utilities/jenkins/__init__.py,sha256=sX-ZO6NnG0i0LOo_0AMdVMmOluG1zUFxwuHip31TDLE,1533
-mpyl/utilities/jenkins/runner.py,sha256=QNW71misEkmYcPKUB0RTLor-teaHZvo-5J2LWEmuy44,7617
-mpyl/utilities/junit/__init__.py,sha256=kdNbSYHvm5BaFcES_Cked-J5SlqZ_4GByzpg5pVVueY,1288
+mpyl/utilities/jenkins/runner.py,sha256=BnndcXKTlwLXFja3nGa_81Jx5frbnMenr0aBVoNdLgU,7627
+mpyl/utilities/junit/__init__.py,sha256=zxWSjvglZJPQPxCSB9TtX-Gaw5i8M0f-IzM3DQQczRY,1382
+mpyl/utilities/logging/__init__.py,sha256=dlVErHdOt6YQ9LV91_7e1-XMTa4fagC-xl-GROppD5c,254
 mpyl/utilities/pyaml_env/__init__.py,sha256=vrWacRoipXG4SEVOG6ECvp1JwaukhHJhL3xKxVc1mKg,847
-mpyl/utilities/repo/__init__.py,sha256=OVM3es2dvOM-JH9fyet_04J9EMAoq7G1QazK22kUrjo,6037
+mpyl/utilities/repo/__init__.py,sha256=YGPBcXNARtRWdwG2U01x2lfhlEalTHStpTvcB4OGFVM,6568
 mpyl/utilities/s3/__init__.py,sha256=u7NBYcHgXBeSSsqGSFVQs3FLvK-3M4wPC2-Vsc0AQz8,4622
 mpyl/utilities/sbt/__init__.py,sha256=FQOMPPgmiU7HMgMoioM5T0fSk0LwGti-k8l3f75Cuqw,1551
 mpyl/utilities/subprocess/__init__.py,sha256=_NehZ65pzu_qxsQQ_Q9t_-zX-FBGeiiaNsjuuPJsgVc,2110
-mpyl-1.0.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mpyl-1.0.5.dist-info/METADATA,sha256=OLmFQ9ruW2IbA2B5kKfnmoM81zmoYLf1Iit3RoccT1c,5945
-mpyl-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mpyl-1.0.5.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
-mpyl-1.0.5.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
-mpyl-1.0.5.dist-info/RECORD,,
+mpyl-1.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mpyl-1.0.6.dist-info/METADATA,sha256=9emFgyRk_z3arF92XB4tMroDze6YErwk6_nGNWS4mtA,5945
+mpyl-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mpyl-1.0.6.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
+mpyl-1.0.6.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
+mpyl-1.0.6.dist-info/RECORD,,
```

