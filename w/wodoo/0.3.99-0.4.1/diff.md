# Comparing `tmp/wodoo-0.3.99.tar.gz` & `tmp/wodoo-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wodoo-0.3.99.tar", last modified: Mon Jan 30 10:10:18 2023, max compression
+gzip compressed data, was "wodoo-0.4.1.tar", last modified: Fri Jun 23 06:05:16 2023, max compression
```

## Comparing `wodoo-0.3.99.tar` & `wodoo-0.4.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-30 10:10:00.000000 wodoo-0.3.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-01-30 10:10:18.253246 wodoo-0.3.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-01-30 10:10:00.000000 wodoo-0.3.99/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-30 10:10:18.253246 wodoo-0.3.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-30 10:10:00.000000 wodoo-0.3.99/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.245247 wodoo-0.3.99/wodoo/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/click_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/click_global_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/config/cicd_network_for_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/config/default_network
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/config/template_onlyloop.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/config/template_withports.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/daddy_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/defaults
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.237247 wodoo-0.3.99/wodoo/extra_install/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.241247 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
--rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
--rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
--rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.241247 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
--rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_clickhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29246 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_control_with_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_db_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_db_snapshots_docker_btrfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_db_snapshots_docker_zfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_db_snapshots_plain_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)    45384 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_src.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/lib_turnintodev.py
--rw-r--r--   0 runner    (1001) docker     (123)    53179 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/module_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/myconfigparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/odoo_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/odoo_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/pudb.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/robo_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/tests/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/tests/gimera.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/tests/module_respartner_dummyfield1/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/tests/module_respartner_dummyfield2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/testzfs.sh
--rw-r--r--   0 runner    (1001) docker     (123)    40552 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 10:10:13.000000 wodoo-0.3.99/wodoo/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo/wait/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/wait/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/wait/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/wait/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-01-30 10:10:00.000000 wodoo-0.3.99/wodoo/wait/tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:10:18.249246 wodoo-0.3.99/wodoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-01-30 10:10:18.000000 wodoo-0.3.99/wodoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-01-30 10:10:18.000000 wodoo-0.3.99/wodoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 10:10:18.000000 wodoo-0.3.99/wodoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-30 10:10:18.000000 wodoo-0.3.99/wodoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-30 10:10:18.000000 wodoo-0.3.99/wodoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 10:10:18.000000 wodoo-0.3.99/wodoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 06:05:01.000000 wodoo-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 06:05:16.665681 wodoo-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-23 06:05:01.000000 wodoo-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 06:05:16.665681 wodoo-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 06:05:01.000000 wodoo-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/click_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/click_global_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/config/cicd_network_for_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/config/default_network
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/config/template_onlyloop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/config/template_withports.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/daddy_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/defaults
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.653681 wodoo-0.4.1/wodoo/extra_install/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.653681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.653681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_clickhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_control_with_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_db_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_db_snapshots_docker_btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_db_snapshots_docker_zfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_db_snapshots_plain_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50013 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_src.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/lib_turnintodev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55120 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/module_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/myconfigparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/odoo_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/odoo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/pudb.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/robo_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/wodoo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/tests/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/tests/gimera.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/wodoo/tests/module_respartner_dummyfield1/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/wodoo/tests/module_respartner_dummyfield2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/testzfs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 06:05:14.000000 wodoo-0.4.1/wodoo/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.665681 wodoo-0.4.1/wodoo/wait/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/wait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/wait/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/wait/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 06:05:01.000000 wodoo-0.4.1/wodoo/wait/tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:05:16.661681 wodoo-0.4.1/wodoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 06:05:16.000000 wodoo-0.4.1/wodoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-23 06:05:16.000000 wodoo-0.4.1/wodoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:05:16.000000 wodoo-0.4.1/wodoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 06:05:16.000000 wodoo-0.4.1/wodoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 06:05:16.000000 wodoo-0.4.1/wodoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 06:05:16.000000 wodoo-0.4.1/wodoo.egg-info/top_level.txt
```

### Comparing `wodoo-0.3.99/LICENSE` & `wodoo-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/PKG-INFO` & `wodoo-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.3.99
+Version: 0.4.1
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -167,15 +167,45 @@
 | ODOO_INSTALL_LIBPOSTAL=1| If set, then the libpostal lib is installed|
 | ODOO_QUEUEJOBS_CRON_IN_ONE_CONTAINER=1 | Runs queuejobs and cronjob in the odoo container where also the web application resides|
 | ODOO_QUEUEJOBS_CHANNELS=root:40,magento2:1 | Configures queues for queuejob module |
 |NAMED_ODOO_POSTGRES_VOLUME| Use a specific external volume; not dropped with down -v command|
 |CRONJOB_DADDY_CLEANUP=0 */1 * * * ${JOB_DADDY_CLEANUP}|Turn on grandfather-principle based backup|
 |RESTART_CONTAINERS=1|Sets "restart unless-stopped" policy|
 
+## Odoo Server Configuration in ~/.odoo/settings/odoo.config and odoo.config.${PROJECT_NAME}
+
+Contents will be appended to [options] section of standard odoo configuration.
+
+Configuration may simple look like:
+
+
+```
+setting1=value1
+```
+
+or like that:
+
+```
+[options]
+setting1=value1
+
+[queue_job]
+settingqj=valueqj
+```
+
+The [options] is prepended automatically if missed.
+
 
 # Pytests
 
 Best executed with:
 
 ```bash
 time sudo -E pytest
 ```
+
+# Performance Check
+
+```python
+pipx runpip wodoo install line_profiler
+~/.local/pipx/venvs/wodoo/bin/python3 -mkernprof -l -v odoo reload
+```
```

### Comparing `wodoo-0.3.99/README.md` & `wodoo-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -155,15 +155,45 @@
 | ODOO_INSTALL_LIBPOSTAL=1| If set, then the libpostal lib is installed|
 | ODOO_QUEUEJOBS_CRON_IN_ONE_CONTAINER=1 | Runs queuejobs and cronjob in the odoo container where also the web application resides|
 | ODOO_QUEUEJOBS_CHANNELS=root:40,magento2:1 | Configures queues for queuejob module |
 |NAMED_ODOO_POSTGRES_VOLUME| Use a specific external volume; not dropped with down -v command|
 |CRONJOB_DADDY_CLEANUP=0 */1 * * * ${JOB_DADDY_CLEANUP}|Turn on grandfather-principle based backup|
 |RESTART_CONTAINERS=1|Sets "restart unless-stopped" policy|
 
+## Odoo Server Configuration in ~/.odoo/settings/odoo.config and odoo.config.${PROJECT_NAME}
+
+Contents will be appended to [options] section of standard odoo configuration.
+
+Configuration may simple look like:
+
+
+```
+setting1=value1
+```
+
+or like that:
+
+```
+[options]
+setting1=value1
+
+[queue_job]
+settingqj=valueqj
+```
+
+The [options] is prepended automatically if missed.
+
 
 # Pytests
 
 Best executed with:
 
 ```bash
 time sudo -E pytest
+```
+
+# Performance Check
+
+```python
+pipx runpip wodoo install line_profiler
+~/.local/pipx/venvs/wodoo/bin/python3 -mkernprof -l -v odoo reload
 ```
```

### Comparing `wodoo-0.3.99/setup.py` & `wodoo-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/__init__.py` & `wodoo-0.4.1/wodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/cli.py` & `wodoo-0.4.1/wodoo/cli.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/click_config.py` & `wodoo-0.4.1/wodoo/click_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/click_global_commands.py` & `wodoo-0.4.1/wodoo/click_global_commands.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/consts.py` & `wodoo-0.4.1/wodoo/consts.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     'cicd_delegator': '~/.odoo/cicd_delegator',
     'images': '~/.odoo/images',
 }
 
 default_files = {
     'after_reload_script': "/usr/local/bin/after-odoo-reload.sh",
     'after_up_script': "/usr/local/bin/after-odoo-up.sh",
+    'odoo_config_file_additions': "~/.odoo/odoo.config",
+    'odoo_config_file_additions.project': "~/.odoo/odoo.config.${project_name}",
     'project_settings': "~/.odoo/settings.${project_name}",
     'project_docker_compose.home': "~/.odoo/docker-compose.yml",
     'project_docker_compose.home.project': "~/.odoo/docker-compose.${project_name}.yml",
     'project_docker_compose.local': "${working_dir}/.odoo/docker-compose.${project_name}.yml",
     'docker_compose': '${run}/docker-compose.yml',
     'docker_compose_bin': _search_path('docker-compose'),
     'debugging_template_withports': 'config/template_withports.yml',
```

### Comparing `wodoo-0.3.99/wodoo/daddy_cleanup.py` & `wodoo-0.4.1/wodoo/daddy_cleanup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/defaults` & `wodoo-0.4.1/wodoo/defaults`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings` & `wodoo-0.4.1/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_backup.py` & `wodoo-0.4.1/wodoo/lib_backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from codecs import ignore_errors
+from .tools import try_ignore_exceptions
+import psycopg2
 import arrow
 import time
 import sys
 import uuid
 from .tools import abort
 import sys
 import docker
@@ -18,26 +20,29 @@
 import os
 import click
 from pathlib import Path
 from .tools import put_appendix_into_file
 from .tools import _dropdb
 from .tools import remove_webassets
 from .tools import __dc
+from .tools import __dc_out
+from .tools import docker_kill_container
 from .tools import _execute_sql
 from .tools import __rename_db_drop_target
 from .tools import _remove_postgres_connections
 from .tools import _get_dump_files
 from .tools import _binary_zip
 from .tools import autocleanpaper
 from .tools import _shell_complete_file
 from .cli import cli, pass_config, Commands
 from .lib_clickhelpers import AliasedGroup
 from .tools import ensure_project_name
 from .tools import _get_filestore_folder
 from .tools import __try_to_set_owner
+from .tools import docker_list_containers
 
 import inspect
 import os
 from pathlib import Path
 
 current_dir = Path(
     os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
@@ -78,24 +83,24 @@
         filename = Path(config.dumps_path) / filename
     with autocleanpaper(Path(filename.parent) / str(uuid.uuid4())) as tmppath:
         tmppath.mkdir(exist_ok=True, parents=True)
         subprocess.check_output(["chown", str(config.owner_uid), tmppath])
         filepath_db = ctx.invoke(
             backup_db, filename=tmppath / "dump.sql", dumptype="plain"
         )
-        with autocleanpaper(tmppath / filename.name, strict=True) as tmpfile:
+        with autocleanpaper(tmppath / (filename.name + ".zip"), strict=True) as tmpfile:
             folder = _get_filestore_folder(config)
             with autocleanpaper() as fake_filestore:
-                symlink_file = fake_filestore / 'filestore'
+                symlink_file = fake_filestore / "filestore"
                 symlink_file.parent.mkdir(exist_ok=True, parents=True)
                 os.symlink(folder, symlink_file)
 
-                with autocleanpaper(folder / 'zipped.zip', strict=True) as folderzip:
+                with autocleanpaper(folder / "zipped.zip", strict=True) as folderzip:
                     subprocess.check_call(
-                        ["zip", "-r", folderzip, 'filestore'],
+                        ["zip", "-r", folderzip, "filestore"],
                         cwd=fake_filestore,
                     )
                     shutil.move(folderzip, tmpfile)
             subprocess.check_call(
                 [
                     "zip",
                     "-u",
@@ -108,14 +113,15 @@
     __try_to_set_owner(
         int(config.owner_uid),
         filename,
         verbose=True,
     )
     click.secho(f"Created dump-file {filename}", fg="green")
 
+
 @backup.command(name="odoo-db")
 @pass_config
 @click.pass_context
 @click.argument("filename", required=False, default="")
 @click.option("--dbname", required=False)
 @click.option("-T", "--exclude", multiple=True)
 @click.option(
@@ -324,15 +330,15 @@
                 # change owner to OWNER_UID
                 subprocess.check_call(
                     ["chown", str(config.owner_uid), filestore_dest, "-R"]
                 )
             if sqlfile.exists():
                 click.secho(f"Restoring db {sqlfile}")
                 os.chdir(was_dir)
-                params['no_remove_webassets'] = True
+                params["no_remove_webassets"] = True
                 Commands.invoke(ctx, "restore_db", filename=sqlfile, **params)
         finally:
             os.chdir(was_dir)
 
 
 def _after_restore(ctx, conn, config, no_dev_scripts, no_remove_webassets):
     from .lib_turnintodev import __turn_into_devdb
@@ -361,35 +367,37 @@
 )
 @click.option("-v", "--verbose", is_flag=True)
 @click.option(
     "--ignore-errors",
     is_flag=True,
     help="Example if some extensions are missing (replication)",
 )
+@click.option("--dbname")
 @pass_config
 @click.pass_context
 def restore_db(
     ctx,
     config,
     filename,
     no_dev_scripts,
     no_remove_webassets,
     verify,
     workers,
     exclude_tables,
     verbose,
     ignore_errors,
+    dbname,
 ):
     if not filename:
         filename = _inquirer_dump_file(
-            config, "Choose filename to restore", config.dbname
+            config, "Choose filename to restore", (dbname or config.dbname)
         )
     if not filename:
         return
-    if not config.dbname:
+    if not (dbname or config.dbname):
         raise Exception("somehow dbname is missing")
 
     dumps_path = config.dumps_path
     BACKUPDIR = Path(dumps_path)
     filename_absolute = (BACKUPDIR / filename).absolute()
     del filename
 
@@ -400,14 +408,15 @@
         "no_dev_scripts": no_dev_scripts,
         "no_remove_webassets": no_remove_webassets,
         "verify": verify,
         "workers": workers,
         "exclude_tables": exclude_tables,
         "verbose": verbose,
         "ignore_errors": ignore_errors,
+        "dbname": (dbname or config.dbname),
     }
 
     dump_type = _add_cronjob_scripts(config)["postgres"].__get_dump_type(
         filename_absolute
     )
     if dump_type == "odoosh":
         _odoo_sh(ctx, config, filename=filename_absolute, params=params)
@@ -415,15 +424,15 @@
 
     if len(Path(filename_absolute).parts) > 1:
         dumps_path = Path(filename_absolute).parent
         filename = Path(filename_absolute).name
 
     if dump_type.startswith("dump_all"):
         with autocleanpaper() as tmpdir:
-            params['no_remove_webassets'] = True
+            params["no_remove_webassets"] = True
             with _add_cronjob_scripts(config)["postgres"].extract_dumps_all(
                 tmpdir, filename_absolute
             ) as (dbfile, files_file):
                 ctx.invoke(restore_files, filename=files_file)
                 ctx.invoke(
                     restore_db,
                     filename=dbfile,
@@ -436,15 +445,21 @@
             abort("Requires RUN_POSTGRES=1")
 
         _restore_wodoo_bin(ctx, config, filename_absolute, verify)
         conn = config.get_odoo_conn()
         _after_restore(ctx, conn, config, no_dev_scripts, no_remove_webassets)
 
     else:
-        _restore_dump(ctx, config, filename, dumps_path, **params)
+        _restore_dump(
+            ctx,
+            config,
+            filename,
+            dumps_path,
+            **params,
+        )
 
     if config.run_postgres:
         __dc(config, ["up", "-d", "postgres"])
         Commands.invoke(ctx, "wait_for_container_postgres")
         if config.devmode:
             Commands.invoke(ctx, "pghba_conf_wide_open")
 
@@ -457,58 +472,67 @@
     no_dev_scripts,
     no_remove_webassets,
     workers,
     exclude_tables,
     verbose,
     verify,
     ignore_errors,
+    dbname,
 ):
-    DBNAME_RESTORING = config.dbname + "_restoring"
-    if config.run_postgres:
-        postgres_name = f"{config.PROJECT_NAME}_run_postgres"
-        client = docker.from_env()
-        for container in client.containers.list(filters={"name": f"{postgres_name}"}):
-            container.kill()
-            container.remove()
+    DBNAME_RESTORING = (dbname or config.dbname) + "_restoring"
+    if config.run_postgres and config.use_docker:
+        for container_id in docker_list_containers(
+            config.project_name, "postgres", "running"
+        ):
+            docker_kill_container(container_id, remove=True)
+            del container_id
 
-        try:
-            Commands.invoke(ctx, "down")
-        except Exception as ex:
-            pass
+        Commands.invoke(ctx, "remove-volumes")
         Commands.invoke(ctx, "up", machines=["postgres"], daemon=True)
     Commands.invoke(ctx, "wait_for_container_postgres", missing_ok=True)
     conn = config.get_odoo_conn()
     dest_db = conn.dbname
 
     conn = conn.clone(dbname=DBNAME_RESTORING)
-    with config.forced() as config:
-        _dropdb(config, conn)
 
-    _execute_sql(
-        conn.clone(dbname="postgres"),
-        (
-            f"create database {DBNAME_RESTORING} "
-            # "ENCODING 'unicode' "
-            # "LC_COLLATE 'C' "
-            # "TEMPLATE template0 "
-            ";"
-        ),
-        notransaction=True,
+    def dropdb(config):
+        with config.forced() as config:
+            _dropdb(config, conn)
+        try_ignore_exceptions(
+            lambda: dropdb(config), (psycopg2.errors.AdminShutdown, psycopg2.InterfaceError), timeout=30
+        )
+
+    def create_db():
+        _execute_sql(
+            conn.clone(dbname="postgres"),
+            (
+                f"create database {DBNAME_RESTORING} "
+                # "ENCODING 'unicode' "
+                # "LC_COLLATE 'C' "
+                # "TEMPLATE template0 "
+                ";"
+            ),
+            notransaction=True,
+        )
+
+    try_ignore_exceptions(
+        create_db, (psycopg2.errors.AdminShutdown, psycopg2.InterfaceError), timeout=30
     )
+
     effective_host_name = config.DB_HOST
 
     if config.devmode and not no_dev_scripts:
         click.echo("Option devmode is set, so cleanup-scripts are run afterwards")
     try:
         if config.use_docker:
-
             # if postgres docker is used, then make a temporary config to restart docker container
             # with external directory mapped; after that remove config
             if config.run_postgres:
                 __dc(config, ["kill", "postgres"])
+                postgres_name = f"postgres_{uuid.uuid4()}"
                 __dc(
                     config,
                     [
                         "run",
                         "-d",
                         "--name",
                         f"{postgres_name}",
@@ -564,20 +588,20 @@
                 config.DB_USER,
                 config.DB_PWD,
                 Path(config.dumps_path) / filename,
             )
 
         _after_restore(ctx, conn, config, no_dev_scripts, no_remove_webassets)
         __rename_db_drop_target(
-            conn.clone(dbname="postgres"), DBNAME_RESTORING, config.dbname
+            conn.clone(dbname="postgres"), DBNAME_RESTORING, dbname or config.dbname
         )
         _remove_postgres_connections(conn.clone(dbname=dest_db))
 
     finally:
-        if config.run_postgres:
+        if config.run_postgres and config.use_docker:
             # stop the run started postgres container; softly
             subprocess.check_output(["docker", "stop", postgres_name])
             try:
                 subprocess.check_output(["docker", "kill", postgres_name])
             except subprocess.CalledProcessError:
                 # ignore - stopped before
                 pass
```

### Comparing `wodoo-0.3.99/wodoo/lib_clickhelpers.py` & `wodoo-0.4.1/wodoo/lib_clickhelpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_composer.py` & `wodoo-0.4.1/wodoo/lib_composer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import traceback
+from .tools import bash_find
 import arrow
 import threading
 from tabulate import tabulate
 import time
 import collections
 import grp
 import base64
@@ -97,14 +98,17 @@
 @click.option(
     "-c", "--additional_config", help="Base64 encoded configuration like in settings"
 )
 @click.option("-cR", "--additional_config_raw", help="like ODOO_DEMO=1;RUN_PROXY=0")
 @click.option("--images-url", help="default: https://github.com/marcwimmer/odoo")
 @click.option("-I", "--no-update-images", is_flag=True)
 @click.option("-A", "--no-auto-repo", is_flag=True)
+@click.option(
+    "--docker-compose", help="additional docker-compose files, separated by colon :"
+)
 @pass_config
 @click.pass_context
 def do_reload(
     ctx,
     config,
     db,
     demo,
@@ -113,14 +117,15 @@
     headless,
     devmode,
     additional_config,
     additional_config_raw,
     images_url,
     no_update_images,
     no_auto_repo,
+    docker_compose,
 ):
     from .myconfigparser import MyConfigParser
 
     if headless and proxy_port:
         click.secho(("Proxy Port and headless together not compatible."), fg="red")
         sys.exit(-1)
 
@@ -158,25 +163,29 @@
             )
         ) + "\n"
         if additional_config:
             # conflicts with demo flag
             if "ODOO_DEMO=1\n" in additional_config:
                 demo = True
 
+        if docker_compose:
+            docker_compose = docker_compose.split(":")
+
         internal_reload(
             ctx,
             config,
             db,
             demo,
             devmode,
             headless,
             proxy_port,
             mailclient_gui_port,
             additional_config,
             apply_auto_repo=not no_auto_repo,
+            additional_docker_configuration_files=docker_compose,
         )
 
     finally:
         if additional_config_file and additional_config_file.exists():
             additional_config_file.unlink()
 
 
@@ -192,16 +201,18 @@
     devmode,
     headless,
     local,
     proxy_port,
     mailclient_gui_port,
     additional_config=None,
     apply_auto_repo=True,
+    additional_docker_configuration_files=None,
 ):
     ensure_project_name(config)
+    additional_docker_configuration_files = additional_docker_configuration_files or []
     defaults = {
         "config": config,
         "db": db,
         "demo": demo,
         "LOCAL_SETTINGS": "1" if local else "0",
         "CUSTOMS_DIR": config.WORKING_DIR,
         "WODOO_VERSION": _get_version(),
@@ -231,15 +242,18 @@
 
         click.secho("Additional config: {defaults}")
 
     if apply_auto_repo:
         _apply_autorepo(ctx=ctx, config=config)
 
     # assuming we are in the odoo directory
-    _do_compose(**defaults)
+    _do_compose(
+        **defaults,
+        additional_docker_configuration_files=additional_docker_configuration_files,
+    )
 
     _execute_after_reload(config)
 
 
 def _execute_after_reload(config):
     execute_script(
         config,
@@ -250,15 +264,21 @@
 
 def _set_defaults(config, defaults):
     defaults["HOST_RUN_DIR"] = config.HOST_RUN_DIR
     defaults["NETWORK_NAME"] = config.project_name
     defaults["project_name"] = config.project_name
 
 
-def _do_compose(config, db="", demo=False, **forced_values):
+def _do_compose(
+    config,
+    db="",
+    demo=False,
+    additional_docker_configuration_files=None,
+    **forced_values,
+):
     """
     builds docker compose, proxy settings, setups odoo instances
     """
     from .myconfigparser import MyConfigParser
     from .settings import _export_settings
 
     rows = []
@@ -278,15 +298,17 @@
     defaults = {}
     _set_defaults(config, defaults)
     setup_settings_file(config, db, demo, **defaults)
     _export_settings(config, forced_values)
     _prepare_filesystem(config)
     _execute_after_settings(config)
 
-    _prepare_yml_files_from_template_files(config)
+    _prepare_yml_files_from_template_files(
+        config, additional_docker_configuration_files
+    )
 
     click.echo("Built the docker-compose file.")
 
 
 def _download_images(config, images_url):
     from . import consts
 
@@ -317,15 +339,14 @@
     ).strip()
     if config.ODOO_IMAGES_BRANCH and config.ODOO_IMAGES_BRANCH != current_branch:
         subprocess.check_call(["git", "checkout", config.ODOO_IMAGES_BRANCH])
 
     if subprocess.check_output(
         ["git", "remote"], encoding="utf8", cwd=config.dirs["images"]
     ).strip():
-
         trycount = 0
         for i in range(10):
             trycount += 1
             try:
                 subprocess.check_call(["git", "pull"], cwd=config.dirs["images"])
             except Exception as ex:
                 if trycount < 5:
@@ -465,15 +486,17 @@
         )
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         module.after_settings(settings)
         settings.write()
 
 
-def _prepare_yml_files_from_template_files(config):
+def _prepare_yml_files_from_template_files(
+    config, additional_docker_configuration_files=None
+):
     # replace params in configuration file
     # replace variables in docker-compose;
     from . import odoo_config
 
     # python: find all configuration files from machines folder; extract sort
     # by manage-sort flag and put file into run directory
     # only if RUN_parentpath like RUN_ODOO is <> 0 include the machine
@@ -487,15 +510,16 @@
         Path("/etc/odoo/"),
     ]:
         if not dir.exists():
             continue
         if dir.is_file():
             _files += [dir]
         else:
-            [_files.append(x) for x in dir.glob("**/docker-compose*.yml")]
+            for file in bash_find(dir, "docker-compose*.yml"):
+                _files.append(file)
 
     if config.restrict and config.restrict.get("docker-compose"):
         _files += config.restrict["docker-compose"]
     else:
         for d in [
             config.files["project_docker_compose.local"],
             config.files["project_docker_compose.home"],
@@ -510,14 +534,22 @@
             if d.is_file():
                 _files.append(d)
             else:
                 [
                     _files.append(x) for x in d.glob("docker-compose*.yml")
                 ]  # not recursive
 
+    if additional_docker_configuration_files:
+        for file in additional_docker_configuration_files:
+            file = Path(os.path.expanduser(file))
+            if not file.exists():
+                raise Exception(f"File {file} does not exist")
+            file = file.absolute()
+            _files += [file]
+
     _files2 = []
     for x in _files:
         if x in _files2:
             continue
         _files2.append(x)
     _files = _files2
     del _files2
@@ -561,15 +593,15 @@
         contents.append((order, yaml.safe_load(content), path))
 
     contents = list(map(lambda x: x[1], sorted(contents, key=lambda x: x[0])))
     return contents
 
 
 def __set_environment_in_services(content):
-    for service in content.get("services", []):
+    for service in (content.get("services", []) or []):
         service = content["services"][service]
         service.setdefault("env_file", [])
         if isinstance(service["env_file"], str):
             service["env_file"] = [service["env_file"]]
 
         file = "$HOST_RUN_DIR/settings"
         if not [x for x in service["env_file"] if x == file]:
@@ -659,16 +691,14 @@
         except KeyError:
             d["DOCKER_GROUP_ID"] = "0"
 
         conf = subprocess.check_output(cmdline, cwd=temp_path, env=d)
         conf = yaml.safe_load(conf)
         return conf
 
-    except Exception:
-        raise
     finally:
         if temp_path.exists():
             shutil.rmtree(temp_path)
 
 
 def dict_merge(dct, merge_dct):
     """Recursive dict merge. Inspired by :meth:``dict.update()``, instead of
@@ -709,26 +739,25 @@
         if (
             k in dct
             and isinstance(dct[k], dict)
             and isinstance(merge_dct[k], collections.abc.Mapping)
         ):
             dict_merge(dct[k], merge_dct[k])
         else:
-
             # merging lists of tuples and lists
             if k in dct:
                 _make_dict_if_possible(dct, k)
 
             if k not in dct:
                 dct[k] = merge_dct[k]
 
 
 def _prepare_docker_compose_files(config, dest_file, paths):
     from .myconfigparser import MyConfigParser
-    from .tools import abort
+    from .tools import abort, atomic_write
     import yaml
 
     if not dest_file:
         raise Exception("require destination path")
 
     myconfig = MyConfigParser(config.files["settings"])
     env = dict(map(lambda k: (k, myconfig.get(k)), myconfig.keys()))
@@ -745,20 +774,21 @@
     _explode_referenced_machines(contents)
     _fix_contents(contents)
 
     # call docker compose config to get the complete config
     content = __run_docker_compose_config(config, contents, env)
     content = post_process_complete_yaml_config(config, content)
     content = _execute_after_compose(config, content)
-    dest_file.write_text(yaml.dump(content, default_flow_style=False))
+    with atomic_write(dest_file) as file:
+        file.write_text(yaml.dump(content, default_flow_style=False))
 
 
 def _fix_contents(contents):
     for content in contents:
-        services = content.get("services")
+        services = content.get("services", []) or []
         for service in services:
             service = services[service]
             # turn {"env_file": {"FILE1": null} --> ["FILE1"]
             if "env_file" in service:
                 if isinstance(service["env_file"], dict):
                     service["env_file"] = list(service["env_file"].keys())
 
@@ -775,24 +805,24 @@
     name in docker compose config
     """
     import yaml
 
     needs_explosion = {}
 
     for content in contents:
-        for service in content.get("services"):
+        for service in (content.get("services", []) or []):
             labels = content["services"][service].get("labels")
             if labels:
                 if labels.get("compose.merge"):
                     needs_explosion.setdefault(labels["compose.merge"], set())
                     needs_explosion[labels["compose.merge"]].add(service)
 
     for content in contents:
         for explode, to_explode in needs_explosion.items():
-            if explode in content.get("services", []):
+            if explode in (content.get("services", []) or []):
                 for to_explode in to_explode:
                     if to_explode in content["services"]:
                         src = deepcopy(content["services"][explode])
                         dict_merge(src, content["services"][to_explode])
                     else:
                         src = content["services"][explode]
                     content["services"][to_explode] = src
```

### Comparing `wodoo-0.3.99/wodoo/lib_control.py` & `wodoo-0.4.1/wodoo/lib_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,39 @@
     if config.use_docker:
         from .lib_control_with_docker import do_kill as lib_do_kill
 
         lib_do_kill(ctx, config, machines, brutal=False)
 
 
 @docker.command()
+@click.option("-d", "--dry-run", is_flag=True)
+@pass_config
+@click.pass_context
+def remove_volumes(ctx, config, dry_run):
+    """
+    Experience: docker-compose down -v lets leftovers since june/2023
+    At restore everything must be cleaned up.
+    """
+    ensure_project_name(config)
+    if not config.devmode:
+        if not config.force:
+            abort("Please provide force option on non live systems")
+    if not config.use_docker:
+        return
+    subprocess.check_call(["sync"])
+    volumes = _get_project_volumes(config)
+    for vol in volumes:
+        click.secho(f"Removing: {vol}", fg='red')
+        if not dry_run:
+            subprocess.check_call(["docker", "volume", "rm", "-f", vol])
+        if dry_run:
+            click.secho("Dry Run - didnt do it.")
+
+
+@docker.command()
 @pass_config
 @click.pass_context
 def force_kill(ctx, config, machine):
     if config.use_docker:
         from .lib_control_with_docker import force_kill as lib_force_kill
     lib_force_kill(ctx, config, machine)
 
@@ -303,41 +328,51 @@
 #         from .lib_control_with_docker import shell as lib_shell
 #     command = (
 #         f"env['queue.job'].browse({id}).run_now()"
 #     )
 #     lib_shell(command, queuejobs)
 
 
+def _get_project_volumes(config):
+    ensure_project_name(config)
+    import yaml
+    compose = yaml.safe_load(config.files["docker_compose"].read_text())
+    full_volume_names = []
+    for volume in compose["volumes"]:
+        full_volume_names.append(f"{config.project_name}_{volume}")
+    system_volumes = subprocess.check_output(
+        ["docker", "volume", "ls"], encoding="utf8"
+    ).splitlines()[1:]
+    system_volumes = [x.split(" ")[-1] for x in system_volumes]
+    system_volumes = [x for x in system_volumes if "_" in x]  # named volumes
+    system_volumes = [
+        x for x in system_volumes if x.startswith(config.project_name + "_")
+    ]
+
+    full_volume_names = list(filter(lambda x: x in system_volumes, full_volume_names))
+    return full_volume_names
+
+
 @docker.command()
 @click.option("-f", "--filter")
 @pass_config
 def show_volumes(config, filter):
     import yaml
     from tabulate import tabulate
     from .lib_control_with_docker import _get_volume_size
 
-    volumes = (
-        subprocess.check_output(["docker", "volume", "ls"])
-        .decode("utf-8")
-        .split("\n")[1:]
-    )
-    volumes = [x.split(" ")[-1] for x in volumes]
-    volumes = [[x] for x in volumes if "_" in x]  # named volumes
-    volumes = [x for x in volumes if config.project_name in x[0]]
+    volumes = _get_project_volumes(config)
     if filter:
         volumes = [x for x in volumes if filter in x]
+    recs = []
     for volume in volumes:
-        size = _get_volume_size(volume[0])
-        volume.append(size)
-    click.echo(tabulate(volumes, ["Volume", "Size"]))
+        size = _get_volume_size(volume)
+        recs.append((volume, size))
+    click.echo(tabulate(recs, ["Volume", "Size"]))
 
-    click.secho("\ndocker-compose file:", bold=True)
-    compose = yaml.safe_load(config.files["docker_compose"].read_text())
-    for volume in compose["volumes"]:
-        click.secho(f"docker-compose volume: {volume}")
 
 
 @docker.command()
 @click.option("-a", "--show-all", is_flag=True)
 @click.option("-f", "--filter")
 @click.option("-B", "--no-backup", is_flag=True)
 @pass_config
@@ -453,7 +488,8 @@
 Commands.register(rm)
 Commands.register(recreate)
 Commands.register(debug)
 Commands.register(restart)
 Commands.register(shell, "odoo-shell")
 Commands.register(down)
 Commands.register(stop)
+Commands.register(remove_volumes, "remove-volumes")
```

### Comparing `wodoo-0.3.99/wodoo/lib_control_with_docker.py` & `wodoo-0.4.1/wodoo/lib_control_with_docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,17 @@
     # '--remove-orphans', # lost data with that; postgres volume suddenly new after rm?
     if volumes:
         options += ["--volumes"]
     if remove_orphans:
         options += ["--remove-orphans"]
     __dc(config, ["down"] + options + machines)
 
+    if volumes:
+        Commands.invoke(ctx, "remove-volumes")
+
 
 def stop(ctx, config, machines=[]):
     do_kill(ctx, config, machines=machines)
 
 
 def rebuild(ctx, config, machines=[]):
     Commands.invoke(ctx, "compose", customs=config.customs)
@@ -249,15 +252,16 @@
         options += ["--no-cache"]
         if "--pull" not in options:
             options += ["--pull"]
 
     if config.verbose:
         os.environ["BUILDKIT_PROGRESS"] = "plain"
 
-    __dc(config, 
+    __dc(
+        config,
         ["build"] + options + list(machines),
         env={
             "ODOO_VERSION": config.odoo_version,  # at you developer: do not mismatch with build args
         },
     )
```

### Comparing `wodoo-0.3.99/wodoo/lib_db.py` & `wodoo-0.4.1/wodoo/lib_db.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_db_snapshots.py` & `wodoo-0.4.1/wodoo/lib_db_snapshots.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,19 +108,21 @@
 
 @snapshot.command(name="clear", help="Removes all snapshots")
 @pass_config
 @click.pass_context
 def snapshot_clear_all(ctx, config):
     config.snapshot_manager.assert_environment(config)
 
-    snapshots = config.snapshot_manager.__get_snapshots(config)
-    if snapshots:
-        for snap in snapshots:
-            config.snapshot_manager.remove(config, snap)
-    config.snapshot_manager.clear_all(config)
+    if hasattr(config.snapshot_manager, 'clear_all'):
+        config.snapshot_manager.clear_all(config)
+    else:
+        snapshots = config.snapshot_manager.__get_snapshots(config)
+        if snapshots:
+            for snap in snapshots:
+                config.snapshot_manager.remove(config, snap)
     ctx.invoke(do_list)
 
 
 @snapshot.command(
     name="purge-inactive-subvolumes",
     help=(
         "Compares subvolumes to docker volumes. If the "
```

### Comparing `wodoo-0.3.99/wodoo/lib_db_snapshots_docker_btrfs.py` & `wodoo-0.4.1/wodoo/lib_db_snapshots_docker_btrfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_db_snapshots_docker_zfs.py` & `wodoo-0.4.1/wodoo/lib_db_snapshots_docker_zfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_db_snapshots_plain_postgres.py` & `wodoo-0.4.1/wodoo/lib_db_snapshots_plain_postgres.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_docker_registry.py` & `wodoo-0.4.1/wodoo/lib_docker_registry.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_lang.py` & `wodoo-0.4.1/wodoo/lib_lang.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_module.py` & `wodoo-0.4.1/wodoo/lib_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,41 +5,45 @@
 import uuid
 import arrow
 import threading
 import json
 import base64
 import subprocess
 import inquirer
-from git import Repo
 import traceback
 from datetime import datetime
 import shutil
 import os
 import tempfile
 import click
 
 from wodoo.robo_helpers import _get_required_odoo_modules_from_robot_file
 from .tools import is_git_clean
+from gimera.repo import Repo
 from .tools import get_hash
 from .tools import get_directory_hash
 from .tools import sync_folder
 from .tools import __dcrun
 from .tools import __cmd_interactive
 from .tools import __get_installed_modules
 from .tools import __concurrent_safe_write_file
 from .cli import cli, pass_config, Commands
 from .lib_clickhelpers import AliasedGroup
 from .tools import _execute_sql
 from .tools import get_services
 from .tools import __try_to_set_owner
 from .tools import measure_time, abort
+from .tools import _update_setting
+from .tools import _get_setting
+from .tools import get_git_hash
 from .module_tools import _determine_affected_modules_for_ir_field_and_related
 from pathlib import Path
 
 DTF = "%Y-%m-%d %H:%M:%S"
+KEY_SHA_REVISION = "sha.revision"
 
 
 class UpdateException(Exception):
     pass
 
 
 class RepeatUpdate(Exception):
@@ -211,26 +215,27 @@
     Gets dependency tree of modules and copmares version in manifest with
     version in database. If db is newer then update is required.
 
     This usually habens after an update of odoo core.
 
     """
     from .module_tools import Modules, DBModules, Module
+    from .module_tools import NotInAddonsPath
     from .odoo_config import MANIFEST
 
     mods = Modules()
     cache_db_modules = {}
 
     for module in sorted(modules):
         if module == "base":
             continue
 
         try:
             mod = Module.get_by_name(module)
-        except KeyError:
+        except (KeyError, NotInAddonsPath):
             click.secho(
                 f"Warning module not found: {module}",
                 fg="yellow",
             )
             continue
         for dep in mods.get_module_flat_dependency_tree(mod):
             if dep.name not in cache_db_modules:
@@ -253,20 +258,26 @@
                 continue
             new_version = tuple([int(x) for x in new_version.split(".")])
             if len(new_version) == 2:
                 # add odoo version in front
                 odoo_version = str(MANIFEST()["version"]).split(".")
                 assert (
                     len(odoo_version) == 2
-                ), "Version in manifest should be like 16.0 not '{odoo_version}'"
+                ), f"Version in manifest should be like 16.0 not '{odoo_version}' as it is in {MANIFEST().path}"
                 new_version = tuple(list(map(int, odoo_version)) + list(new_version))
                 del odoo_version
 
             if new_version > version:
-                yield dep
+                # seen: if version in manifest is 14.0.1.0 and installed in
+                # 13.0 odoo then version becomes inside odoo: 13.0.14.0.10
+                # so try to match including current version:
+                odoo_version = list(map(int, str(MANIFEST()['version']).split(".")))
+                new_version = tuple(odoo_version + list(new_version))
+                if new_version != version:
+                    yield dep
 
 
 def _get_available_modules(ctx, param, incomplete):
     from .odoo_config import MANIFEST
 
     try:
         manifest = MANIFEST()
@@ -276,26 +287,50 @@
         return []
     modules = manifest["install"]
     if incomplete:
         modules = [x for x in modules if incomplete in x]
     return sorted(modules)
 
 
+@odoo_module.command(name="UPDATE")
+@click.option(
+    "--no-dangling-check",
+    default=False,
+    is_flag=True,
+    help="Not checking for dangling modules",
+)
+@click.option("--non-interactive", "-I", is_flag=True, help="Not interactive")
+@click.option(
+    "--recover-view-error",
+    is_flag=True,
+    help="Can happen if per update fields are removed and views still referencing this field.",
+)
+@click.option("--i18n", default=False, is_flag=True, help="Overwrite Translations")
+@pass_config
+@click.pass_context
+def update2(ctx, config, no_dangling_check, non_interactive, recover_view_error, i18n):
+    conn = config.get_odoo_conn()
+    revision = _get_setting(conn, KEY_SHA_REVISION)
+    Commands.invoke(
+        ctx,
+        "update",
+        no_outdated_modules=True,
+        since_git_sha=revision,
+        no_dangling_check=no_dangling_check,
+        non_interactive=non_interactive,
+        recover_view_error=recover_view_error,
+        i18n=i18n,
+    )
+
+
 @odoo_module.command()
 @click.argument(
     "module", nargs=-1, required=False, shell_complete=_get_available_modules
 )
 @click.option(
-    "--since-git-sha",
-    "-i",
-    default=None,
-    is_flag=False,
-    help="Extracts modules changed since this git sha and updates them",
-)
-@click.option(
     "--installed-modules",
     "-i",
     default=False,
     is_flag=True,
     help="Updates only installed modules",
 )
 @click.option(
@@ -350,15 +385,15 @@
     "--test-tags",
     help="e.g. at_install/account_accountant,post_install/account_accountant",
 )
 @click.option(
     "-l",
     "--log",
     default="info",
-    type=click.Choice(["info", "debug", "error"]),
+    type=click.Choice(["test", "info", "debug", "error"]),
     help="display logs with given level",
 )
 @click.option(
     "-dt",
     "--default-test-tags",
     is_flag=True,
     help="Adds at_install/{module},post_install/{module},standard/{module}",
@@ -370,14 +405,21 @@
 )
 @click.option(
     "-O",
     "--no-outdated-modules",
     is_flag=True,
     help="dont check for outdated modules (for migrations suitable)",
 )
+@click.option(
+    "--since-git-sha",
+    "-G",
+    default=None,
+    is_flag=False,
+    help="Extracts modules changed since this git sha and updates them",
+)
 @pass_config
 @click.pass_context
 def update(
     ctx,
     config,
     module,
     since_git_sha,
@@ -453,26 +495,15 @@
         Commands.invoke(ctx, "up", machines=["postgres"], daemon=True)
         Commands.invoke(ctx, "wait_for_container_postgres", missing_ok=True)
 
     def _perform_install(module):
         if since_git_sha and module:
             raise Exception("Conflict: since-git-sha and modules")
         if since_git_sha:
-            module = list(_get_changed_modules(since_git_sha))
-
-            # filter modules to defined ones in MANIFEST
-            click.secho(f"Following modules change since last sha: {' '.join(module)}")
-
-            module = list(filter(lambda x: x in MANIFEST()["install"], module))
-            click.secho(
-                (
-                    "Following modules changed since last sha "
-                    f"(filtered to manifest): {' '.join(module)}"
-                )
-            )
+            module = _get_modules_since_git_sha(since_git_sha)
 
             if not module:
                 click.secho("No module update required - exiting.")
                 return
         else:
             module = _parse_modules(module)
 
@@ -559,14 +590,16 @@
                     if recover_view_error:
                         try:
                             _try_to_recover_view_error(config, output)
                         except RepeatUpdate as ex:
                             _technically_update(ex.affected_modules)
                         except Exception as ex:
                             raise UpdateException(module) from ex
+                        else:
+                            raise Exception(f"Error at update - please check logs")
                     else:
                         raise UpdateException(module)
 
             except UpdateException:
                 raise
             except RepeatUpdate:
                 raise
@@ -627,14 +660,26 @@
     # check danglings
     if not no_dangling_check and all_modules:
         ctx.invoke(show_install_state, suppress_error=False)
 
     if check_install_state:
         _do_check_install_state(ctx, config, module, all_modules, no_dangling_check)
 
+    _set_sha(config)
+
+
+def _set_sha(config):
+    conn = config.get_odoo_conn()
+    try:
+        sha = get_git_hash()
+    except:
+        pass
+    else:
+        _update_setting(conn, KEY_SHA_REVISION, sha)
+
 
 def _try_to_recover_view_error(config, output):
     """
     If a field is removed it can be that views still reference it, so
     remove the item from the view.
 
     Field "product_not_show_ax_code" does not exist in model "res.company"
@@ -719,15 +764,15 @@
                 config.get_odoo_conn(),
                 (
                     "update ir_module_module set state = "
                     "'uninstalled' where state = 'uninstallable';"
                 ),
             )
     if DBModules.get_dangling_modules() and not dangling_modules:
-        if show_dangling():
+        if show_dangling() and not non_interactive:
             input("Abort old upgrade and continue? (Ctrl+c to break)")
             ctx.invoke(abort_upgrade)
 
 
 def _parse_modules(modules):
     if isinstance(modules, (str, bytes)):
         modules = modules.split(",")
@@ -1242,60 +1287,55 @@
     filepaths = git_diff_files(cwd, git_sha, "HEAD")
     repo = Repo(cwd)
 
     # check if there are submodules:
     filepaths2 = []
     cwd = Path(os.getcwd())
     for filepath in filepaths:
+        filepath = repo.path / filepath
         os.chdir(cwd)
-        submodule = [x for x in repo.submodules if x.path == filepath]
+
+        def get_submodule(filepath):
+            for submodule in repo.get_submodules():
+                try:
+                    filepath.relative_to(submodule.path)
+                    return submodule
+                except ValueError:
+                    continue
+
+        submodule = get_submodule(filepath)
+
         if submodule:
-            current_commit = str(repo.active_branch.commit)
+            current_commit = str(repo.hex)
+            relpath = filepath.relative_to(repo.path)
             old_commit = (
-                subprocess.check_output(["git", "rev-parse", f"{git_sha}:./{filepath}"])
-                .decode("utf-8")
+                subprocess.check_output(
+                    [
+                        "git",
+                        "rev-parse",
+                        f"{git_sha}:./{relpath}",
+                    ], encoding='utf8'
+                )
                 .strip()
             )
             new_commit = (
                 subprocess.check_output(
-                    ["git", "rev-parse", f"{current_commit}:./{filepath}"]
+                    ["git", "rev-parse", f"{current_commit}:./{relpath}"], encoding='utf8',
                 )
-                .decode("utf-8")
                 .strip()
             )
             # now diff the submodule
-            submodule_path = cwd / filepath
-            submodule_relative_path = filepath
-            for filepath2 in git_diff_files(submodule_path, old_commit, new_commit):
-                filepaths2.append(submodule_relative_path + "/" + filepath2)
+            for filepath2 in git_diff_files(filepath, old_commit, new_commit):
+                filepaths2.append(str(relpath / filepath2))
         else:
-            filepaths2.append(filepath)
+            filepaths2.append(str(filepath.relative_to(repo.path)))
 
     return filepaths2
 
 
-def _get_changed_modules(git_sha):
-    from .module_tools import Module
-
-    filepaths = _get_changed_files(git_sha)
-    modules = []
-    root = Path(os.getcwd())
-    for filepath in filepaths:
-
-        filepath = root / filepath
-
-        try:
-            module = Module(filepath)
-        except Module.IsNot:
-            pass
-        else:
-            modules.append(module.name)
-    return list(sorted(set(modules)))
-
-
 @odoo_module.command(name="list-changed-modules")
 @click.option("-s", "--start")
 @click.pass_context
 @pass_config
 def list_changed_modules(ctx, config, start):
     modules = _get_changed_modules(start)
 
@@ -1377,18 +1417,18 @@
         module = [Module.get_by_name(x) for x in modules.modules]
     else:
         do_all = False
         module = [Module.get_by_name(module)]
 
     result = {}
     for module in module:
-
         data = {"modules": []}
         data["modules"] = sorted(
-            map(lambda x: x.name, modules.get_module_flat_dependency_tree(module))
+            list(map(lambda x: x.name, modules.get_module_flat_dependency_tree(module)))
+            + [module.name]
         )
 
         data["auto_install"] = sorted(
             map(
                 lambda x: x.name,
                 modules.get_filtered_auto_install_modules_based_on_module_list(
                     data["modules"]
@@ -1475,9 +1515,114 @@
     mods = Modules()
     modules = list(sorted(mods.get_all_modules_installed_by_manifest()))
     print("---")
     for m in modules:
         print(m)
 
 
+@odoo_module.command()
+@pass_config
+@click.pass_context
+def list_outdated_modules(ctx, config):
+    modules = _get_default_modules_to_update()
+
+    def _get_outdated_modules(module):
+        return list(
+            map(
+                lambda x: x.name,
+                set(_get_outdated_versioned_modules_of_deptree(module)),
+            )
+        )
+
+    print("---")
+    for mod2 in _get_outdated_modules(modules):
+        print(mod2)
+
+
+def _get_modules_since_git_sha(sha):
+    from .odoo_config import MANIFEST
+
+    module = list(_get_changed_modules(sha))
+
+    # filter modules to defined ones in MANIFEST
+    click.secho(f"Following modules change since last sha: {' '.join(module)}")
+
+    module = list(filter(lambda x: x in MANIFEST()["install"], module))
+    click.secho(
+        (
+            "Following modules changed since last sha "
+            f"(filtered to manifest): {' '.join(module)}"
+        )
+    )
+    return module
+
+
+def _get_changed_modules(git_sha):
+    from .module_tools import Module
+
+    filepaths = _get_changed_files(git_sha)
+    modules = []
+    root = Path(os.getcwd())
+    for filepath in filepaths:
+        filepath = root / filepath
+
+        try:
+            module = Module(filepath)
+        except Module.IsNot:
+            pass
+        else:
+            modules.append(module.name)
+    return list(sorted(set(modules)))
+
+
+@odoo_module.command
+@click.option("-f", "--fix-not-in-manifest", is_flag=True)
+@click.option("--only-customs", is_flag=True)
+@pass_config
+def list_installed_modules(config, fix_not_in_manifest, only_customs):
+    from .module_tools import DBModules, Module
+    from .module_tools import NotInAddonsPath
+    from .odoo_config import customs_dir
+    from .odoo_config import MANIFEST
+
+    collected = []
+    not_in_manifest = []
+    manifest = MANIFEST()
+    setinstall = manifest.get("install", [])
+
+    for module in sorted(DBModules.get_all_installed_modules()):
+        try:
+            mod = Module.get_by_name(module)
+        except (Module.IsNot, NotInAddonsPath):
+            click.secho(f"Ignoring {module} - not found in source", fg="yellow")
+            continue
+        if only_customs:
+            try:
+                parts = mod.path.parts
+            except Module.IsNot:
+                click.secho(f"Ignoring {module} - not found in source", fg="yellow")
+                continue
+            if any(x in parts for x in ["odoo", "enterprise", "themes"]):
+                continue
+        try:
+            click.secho(f"{module}: {mod.path}", fg="green")
+            if not [x for x in setinstall if x == module]:
+                not_in_manifest.append(module)
+        except KeyError:
+            collected.append(module)
+
+    for module in not_in_manifest:
+        if fix_not_in_manifest:
+            setinstall += [module]
+            click.secho(f"Added to manifest: {module}", fg="green")
+        else:
+            click.secho(f"Not in MANIFEST: {module}", fg="yellow")
+    for module in collected:
+        click.secho(f"Not in filesystem: {module}", fg="red")
+
+    if fix_not_in_manifest:
+        manifest["install"] = setinstall
+        manifest.rewrite()
+
+
 Commands.register(update)
 Commands.register(show_install_state)
```

### Comparing `wodoo-0.3.99/wodoo/lib_setup.py` & `wodoo-0.4.1/wodoo/lib_setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/lib_src.py` & `wodoo-0.4.1/wodoo/lib_src.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,60 +7,57 @@
 import inquirer
 import sys
 from datetime import datetime
 import os
 import click
 from .odoo_config import current_version
 from .odoo_config import MANIFEST
-from .tools import _is_dirty
 from .odoo_config import customs_dir
 from .cli import cli, pass_config, Commands
 from .lib_clickhelpers import AliasedGroup
 from .tools import split_hub_url
 from .tools import autocleanpaper
 from .tools import copy_dir_contents, rsync
 from .tools import abort
 from .tools import __assure_gitignore
 from .tools import _write_file
 from .tools import bashfind
+from .tools import cwd
 
 ADDONS_OCA = "addons_OCA"
 
 
 @cli.group(cls=AliasedGroup)
 @pass_config
 def src(config):
     pass
 
 
 @click.command()
 @click.pass_context
 @pass_config
 def ensure_odoosh_repo(config, ctx):
-    _ensure_odoosh_repo()
+    _ensure_odoosh_repo(ctx)
 
 
-def _ensure_odoosh_repo():
+def _ensure_odoosh_repo(ctx):
+    from gimera.gimera import apply as gimera_apply
+
     odoosh_path = Path(os.environ["ODOOSH_REPO"] or "../odoo.sh").resolve().absolute()
     if not odoosh_path.exists():
         subprocess.check_call(
             [
                 "git",
                 "clone",
                 "https://github.com/Odoo-Ninjas/odoo.sh.git",
                 odoosh_path,
             ]
         )
-        subprocess.check_call(
-            [
-                "gimera",
-                "apply",
-            ],
-            cwd=odoosh_path.absolute(),
-        )
+        with cwd(odoosh_path.absolute()):
+            ctx.invoke(gimera_apply)
     return odoosh_path
 
 
 def _build_gimera(path):
     gimera_file = path / "gimera.yml"
     if gimera_file.exists():
         content = yaml.safe_load(gimera_file.read_text())
@@ -96,16 +93,15 @@
     if current_content != new_content:
         gimera_file.write_text(new_content)
         content_changed = True
     return content_changed
 
 
 def _turn_into_odoosh(ctx, path):
-
-    _ensure_odoosh_repo()
+    _ensure_odoosh_repo(ctx)
     content_changed = _build_gimera(path)
 
     repos = yaml.safe_load((path / "gimera.yml").read_text())
     _apply_gimera_if_required(ctx, path, repos, force_do=content_changed)
     _find_duplicate_modules()
 
 
@@ -114,46 +110,47 @@
 
     modules = Modules()
     all_modules = modules.get_all_modules_installed_by_manifest()
     _identify_duplicate_modules(all_modules)
 
 
 def _apply_gimera_if_required(ctx, path, content, force_do=False):
+    from gimera.gimera import apply as gimera
+
     def needs_apply():
         for repo in content["repos"]:
             repo_path = path / repo["path"]
             if not repo_path.exists():
                 return True
         return False
 
     if force_do or needs_apply():
-        subprocess.check_call(
-            [
-                "gimera",
-                "apply",
-            ],
-            cwd=customs_dir(),
-        )
-
-        click.secho("Restarting reloading because gimera apply was done", fg="yellow")
-        Commands.invoke(ctx, "reload", no_auto_repo=True)
+        with cwd(path):
+            ctx.invoke(gimera, recursive=True)
+            click.secho(
+                "Restarting reloading because gimera apply was done", fg="yellow"
+            )
+            Commands.invoke(ctx, "reload", no_auto_repo=True)
 
-        from .module_tools import Modules
+            from .module_tools import Modules
 
-        modules = Modules()
-        all_modules = modules.get_all_modules_installed_by_manifest()
+            modules = Modules()
+            all_modules = modules.get_all_modules_installed_by_manifest()
 
 
 @src.command()
 @click.pass_context
 def apply_gimera_if_required(ctx):
     path = customs_dir()
     gimera_file = path / "gimera.yml"
     if not gimera_file.exists():
-        _build_gimera(path)
+        if MANIFEST().get("auto_repo", False):
+            _build_gimera(path)
+        else:
+            return
     repos = yaml.safe_load(gimera_file.read_text())
     _apply_gimera_if_required(ctx, path, repos)
 
 
 @src.command()
 @click.pass_context
 @pass_config
@@ -168,15 +165,15 @@
 @pass_config
 def init(config, ctx, path, odoosh):
     from .module_tools import make_customs
 
     path = Path(path)
     if not path.exists():
         path.mkdir(parents=True)
-    make_customs(path)
+    make_customs(ctx, path)
 
     odoosh and _turn_into_odoosh(ctx, Path(os.getcwd()))
 
 
 @src.command(help="Makes odoo and enterprise code available from common code")
 @click.pass_context
 @pass_config
@@ -468,49 +465,33 @@
                         "Found duplicate module, which is a problem for odoo.sh deployment.\n"
                         "Not clear which module gets installed: \n"
                         f"{module.path}\n"
                         f"{y}"
                     )
 
 
-@src.command
-@click.option("-f", "--fix-not-in-manifest", is_flag=True)
-@pass_config
-def show_installed_modules(config, fix_not_in_manifest):
-    from .module_tools import DBModules, Module
-    from .odoo_config import customs_dir
-
-    path = customs_dir()
-    collected = []
-    not_in_manifest = []
-    manifest = MANIFEST()
-    setinstall = manifest.get("install", [])
-
-    for module in sorted(DBModules.get_all_installed_modules()):
-        try:
-            mod = Module.get_by_name(module)
-            click.secho(f"{module}: {mod.path}", fg="green")
-            if not [x for x in setinstall if x == module]:
-                not_in_manifest.append(module)
-        except KeyError:
-            collected.append(module)
-
-    for module in not_in_manifest:
-        if fix_not_in_manifest:
-            setinstall += [module]
-            click.secho(f"Added to manifest: {module}", fg="green")
-        else:
-            click.secho(f"Not in MANIFEST: {module}", fg="yellow")
-    for module in collected:
-        click.secho(f"Not in filesystem: {module}", fg="red")
-
-    if fix_not_in_manifest:
-        manifest["install"] = setinstall
-        manifest.rewrite()
-
 
 @src.command(name="pretty-print-manifest")
 def pretty_print_manifest():
     from .odoo_config import MANIFEST
 
     MANIFEST().rewrite()
 
+
+@src.command()
+@pass_config
+@click.argument("module")
+def security(config, module, model):
+    from .module_tools import Modules, Module
+
+    modules = Modules()
+    module = modules.get_by_name(module)
+
+    def ensure_secfile():
+        header = "model_id:id,group_id:id,id,name,perm_read,perm_write,perm_create,perm_unlink"
+        filepath = module.path / "security" / "ir.model.access.csv"
+        filepath.parent.mkdir(exist_ok=True)
+        if not filepath.read_text():
+            filepath.write_text(header + "\n")
+
+    # give rights to choose
+    # TODO ...
```

### Comparing `wodoo-0.3.99/wodoo/lib_turnintodev.py` & `wodoo-0.4.1/wodoo/lib_turnintodev.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 from .tools import remove_webassets
 from .tools import _execute_sql
 from .cli import cli, pass_config, Commands
 from .lib_clickhelpers import AliasedGroup
 from .tools import __hash_odoo_password
 from .tools import __replace_all_envs_in_str
+from .tools import _update_setting
 
 
 @cli.group(cls=AliasedGroup, name="dev-env")
 @pass_config
 def turn_into_dev(config):
     pass
 
@@ -187,18 +188,7 @@
 @click.argument("key", required=True)
 @click.argument("value", required=True)
 @pass_config
 def update_setting(config, key, value):
     conn = config.get_odoo_conn()
     _update_setting(conn, key, value)
 
-
-def _update_setting(conn, key, value):
-    _execute_sql(
-        conn,
-        """
-        DELETE FROM ir_config_parameter WHERE key = '{key}';
-        INSERT INTO ir_config_parameter(key, value) values('{key}', '{value}');
-    """.format(
-            key=key, value=value
-        ),
-    )
```

### Comparing `wodoo-0.3.99/wodoo/module_tools.py` & `wodoo-0.4.1/wodoo/module_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import iscompatible
 from pathlib import Path
 from copy import deepcopy
 import pickle
 import os
 import shutil
 import uuid
+from gimera.repo import Repo
 from .tools import get_hash, get_git_hash
 from .tools import __try_to_set_owner as try_to_set_owner
 from .tools import measure_time
 from .tools import is_git_clean
 from .tools import whoami
 from .tools import __rmtree as rmtree
 
@@ -80,15 +81,14 @@
 
     uid = login(username, pwd)
     socket_obj = xmlrpclib.ServerProxy("%s/xmlrpc/object" % (host))
     return socket_obj.execute(config["DBNAME"], uid, pwd, *params)
 
 
 def delete_qweb(config, modules):
-
     with get_conn_autoclose(config) as cr:
         if modules != "all":
             cr.execute("select name from ir_module_module where name = %s", (modules,))
         else:
             cr.execute("select name from ir_module_module; ")
 
         def erase_view(view_id):
@@ -321,25 +321,25 @@
             )
             state = cr.fetchone()
             if not state:
                 return False
             return state[1] in ["installed", "to upgrade"]
 
 
-def make_customs(path):
+def make_customs(ctx, path):
+    from gimera.gimera import apply as gimera
     from .tools import abort
     import click
 
     if not path.exists():
         abort("Path does not exist: {}".format(path))
     elif list(path.glob("*")):
         abort("Path is not empty: {}".format(path))
 
     import inquirer
-    from git import Repo
     from .tools import copy_dir_contents
 
     dir = get_template_dir()
     src_dir = dir / "customs_template"
 
     def _floatify(x):
         try:
@@ -355,34 +355,34 @@
     ]
     del versions
 
     copy_dir_contents(src_dir / version, path)
 
     manifest_file = path / "MANIFEST"
     manifest = eval(manifest_file.read_text())
+    raise Exception("Rewrite to use gimera")
 
     click.echo("Checking for odoo repo at env variable 'ODOO_REPO'")
     if os.getenv("ODOO_REPO", ""):
         odoo_path = path / "odoo"
         repo_path = Path(os.environ["ODOO_REPO"])
         repo = Repo(repo_path)
-        repo.git.checkout(str(version))
+        repo.X("git", "checkout", str(version))
         odoo_path.mkdir()
-        sha = repo.head.object.hexsha
-        sha = repo.git.rev_parse(sha)
+        sha = repo.hex
         click.echo("Copying odoo with sha to local directory [{}]".format(sha))
         copy_dir_contents(repo_path, odoo_path, exclude=[".git"])
         manifest["odoo_commit"] = sha
 
     manifest_file.write_text(json.dumps(manifest, indent=4))
 
     subprocess.call(["git", "init"], cwd=path)
     subprocess.call(["git", "add", "."], cwd=path)
     subprocess.call(["git", "commit", "-am", "init"], cwd=path)
-    subprocess.call(["gimera", "apply", "--update", "--recursive"], cwd=path)
+    ctx.invoke(gimera, recursive=True, update=True)
     try_to_set_owner(whoami(), path)
 
     click.secho("Initialized - please call following now.", fg="green")
     click.secho("odoo db reset", fg="green")
     sys.exit(0)
 
 
@@ -638,35 +638,41 @@
     def modules(self):
         if "modules" not in Modules_Cache:
             modules = self._get_modules()
             Modules_Cache["modules"] = modules
         return Modules_Cache["modules"]
 
     @classmethod
-    @measure_time
+    # @profile
     def _get_modules(self, no_deptree=False):
         modnames = set()
         from .odoo_config import get_odoo_addons_paths
 
         @measure_time
         def get_all_manifests():
             """
             Returns a list of full paths of all manifests
             """
             for path in reversed(get_odoo_addons_paths()):
-                for file in sorted(path.glob("*/" + manifest_file_names())):
+                mans = subprocess.check_output(
+                    ["find", ".", "-maxdepth", "2", "-name", manifest_file_names()],
+                    cwd=path,
+                    encoding="utf8",
+                ).splitlines()
+                for file in sorted(mans):
+                    file = path / file
                     modname = file.parent.name
                     if modname in modnames:
                         continue
                     modnames.add(file.absolute())
                     yield file.absolute()
 
         modules = {}
         all_manifests = get_all_manifests()
-        for m in all_manifests:
+        for m in list(all_manifests):
             module = Module(m)
             module.manifest_dict.get("just read manifest")
             modules[m.parent.name] = module
 
         if not no_deptree:
             for module in sorted(set(modules.values())):
                 self.get_module_flat_dependency_tree(module=module)
@@ -694,14 +700,15 @@
             try:
                 module = Module(filepath)
             except Module.IsNot:
                 pass
             else:
                 modules.append(module.name)
 
+    # @profile
     def get_customs_modules(self, mode=None):
         """
         Called by odoo update
 
         - fetches to be installed modules from install-file
         - selects all installed, to_be_installed, to_upgrade modules from db and checks wether
             they are from "us" or OCA
@@ -811,23 +818,24 @@
                 module = Module.get_by_name(module)
             except NotInAddonsPath:
                 continue
             if module.manifest_dict.get("auto_install", False):
                 auto_install_modules.append(module)
         return list(sorted(set(auto_install_modules)))
 
-    @measure_time
+    # @profile
     def get_filtered_auto_install_modules_based_on_module_list(self, module_list):
         def _transform_modulelist(module_list):
             for mod in module_list:
                 try:
                     objmod = Module.get_by_name(mod)
                     yield objmod
                 except NotInAddonsPath:
                     pass
+
         module_list = list(_transform_modulelist(module_list))
 
         complete_modules = set()
         for mod in module_list:
             complete_modules |= set(list(self.get_module_flat_dependency_tree(mod)))
 
         def _get(all_modules):
@@ -854,14 +862,15 @@
             before = list(sorted(set(map(lambda x: x.name, modules))))
             modules = list(_get(modules))
             after = list(sorted(set(map(lambda x: x.name, modules))))
             if after == before:
                 break
         return list(sorted(set(modules)))
 
+    # @profile
     def get_all_used_modules(self):
         """
         Returns all modules that are directly or indirectly
         (auto install, depends) installed.
         """
         result = set()
         modules = self.get_customs_modules()
@@ -875,43 +884,41 @@
             dependencies = self.get_module_flat_dependency_tree(module)
             for dep in dependencies:
                 result.add(dep)
 
         return list(result)
 
     def get_all_external_dependencies(self, modules):
-        pydeps = []
-        deb_deps = []
-        for module in modules:
-            module = Module.get_by_name(module)
+        global_data = {"pip": []}
+        for module_name in modules:
+            module = Module.get_by_name(module_name)
+            if module.path is None:
+                raise Exception(f"Module has no path: {module_name}")
             file = module.path / "external_dependencies.txt"
             new_deps = []
+
+            def extract_deps(data):
+                global_data["pip"].extend(data.get("pip", data.get("python", [])))
+                for k, v in data.items():
+                    if k not in ["pip", "python"]:
+                        global_data.setdefault(k, []).extend(v)
+
             if file.exists():
                 try:
                     content = json.loads(file.read_text())
                 except Exception as e:
-                    click.secho(
-                        "Error parsing json in\n{}:\n{}".format(file, e), fg="red"
-                    )
+                    click.secho("Error parsing json in\n{file}:\n{e}", fg="red")
                     click.secho(file.read_text(), fg="red")
                     sys.exit(1)
-                new_deps = content.get("pip", [])
-                pydeps += new_deps
-                deb_deps += content.get("deb", [])
+                extract_deps(content)
             else:
-                new_deps = module.manifest_dict.get("external_dependencies", {}).get(
-                    "python", []
-                )
-                pydeps += new_deps
+                extract_deps(module.manifest_dict.get("external_dependencies", {}))
 
-            # if new_deps:
-            #    click.secho(f"Adding python dependencies {','.join(new_deps)} from {module.name}", fg='yellow')
-
-        pydeps = self.resolve_pydeps(pydeps)
-        return {"pip": pydeps, "deb": deb_deps}
+        global_data["pip"] = self.resolve_pydeps(set(global_data["pip"]))
+        return global_data
 
     def resolve_pydeps(self, pydeps):
         pydeps = list(set(pydeps))
         libnames = [_extract_python_libname(x) for x in pydeps]
         result = set()
 
         # keep highest version and or leaveout loosers
@@ -1017,61 +1024,67 @@
 
     def __eq__(self, other):
         if isinstance(other, str):
             return self.name == other
         return self.name == other.name and self.path == other.path
 
     def __hash__(self):
-        return hash(f"Module_{self.path}_{self.name}")
+        try:
+            path = self.path
+            name = self.name
+            return hash(f"Module_{path}_{name}")
+        except RecursionError:
+            raise Exception(f"Recursion at {self.name}")
 
     def __init__(self, path, force_name=None):
         self.version = float(current_version())
         self._manifest_dict = None
         self._manifest_path = None
         self._dep_tree = None
         if path:
-            self.__init_path(path)
+            self.__init_path(path, manifest_file_names())
             self.path = self._manifest_path.parent
         else:
             self.path = None
 
         if force_name:
             self.name = force_name
         else:
             self.name = self._manifest_path.parent.name
 
     @property
     def exists(self):
         return bool(self.path)
 
-    def __init_path(self, path):
+    def __init_path(self, path, manifest_filename):
         path = Path(path)
+        _customs_dir = customs_dir()
 
         remember_cwd = os.getcwd()
         try:
-            cwd = Path(os.getcwd())
+            cwd = Path(remember_cwd)
             if str(path).startswith("/"):
                 try:
-                    path = path.relative_to(customs_dir())
-                    os.chdir(customs_dir())
-                except:
+                    path = path.relative_to(_customs_dir)
+                    os.chdir(_customs_dir)
+                except Exception:
                     try:
                         path = path.relative_to(cwd)
                     except ValueError:
-                        path = path.relative_to(customs_dir())
+                        path = path.relative_to(_customs_dir)
                         os.chdir(
-                            customs_dir()
+                            _customs_dir
                         )  # reset later; required that parents works
             p = path if path.is_dir() else path.parent
 
             for p in [p] + list(p.parents):
-                if (p / manifest_file_names()).exists():
+                if (p / manifest_filename).exists():
                     if ".git" in p.parts:
                         continue
-                    self._manifest_path = p / manifest_file_names()
+                    self._manifest_path = p / manifest_filename
                     break
             if not getattr(self, "_manifest_path", ""):
                 raise Module.IsNot((f"no module found for {path}"))
         finally:
             os.chdir(remember_cwd)
 
     @property
@@ -1087,17 +1100,19 @@
                 content = "\n".join(
                     filter(
                         lambda x: not x.strip().startswith("#"), content.splitlines()
                     )
                 )
                 self._manifest_dict = eval(content)  # TODO safe
 
-            except (SyntaxError, Exception):
-                click.secho((f"error at file: {self.manifest_path}"), fg="red")
-                raise
+            except (SyntaxError, Exception) as e:
+                click.secho(
+                    (f"error at file: {self.manifest_path}:\n{str(e)}"), fg="red"
+                )
+                sys.exit(-1)
         return self._manifest_dict
 
     def __make_path_relative(self, path):
         path = path.resolve().absolute()
         path = path.relative_to(self.path)
         if not path:
             raise Exception("not part of module")
@@ -1135,19 +1150,14 @@
         mod = cls.__get_by_name_cached(name, nocache=nocache, no_deptree=no_deptree)
         return mod
 
     @classmethod
     def _get_by_name(cls, name, nocache=False, no_deptree=False):
         from .odoo_config import get_odoo_addons_paths
 
-        if not name:
-            import pudb
-
-            pudb.set_trace()
-
         if isinstance(name, Module):
             name = name.name
         path = None
         for addon_path in get_odoo_addons_paths():
             dir = addon_path / name
             if dir.exists():
                 path = dir
@@ -1305,15 +1315,15 @@
                 )
             doc.xpath("/odoo/data")[0].append(parent)
 
         # remove empty assets and the first template template
         for to_remove in doc.xpath("//template[1] | //template[xpath[not(*)]]"):
             to_remove.getparent().remove(to_remove)
 
-        if current_version() >= 15.0:
+        if current_version() > 14.0:
             manifest = self.path / "__manifest__.py"
             jsoncontent = eval(manifest.read_text())
             jsoncontent.setdefault("assets", {})
             existing_files = []
             for asset_file in jsoncontent.get("assets", []):
                 for file in jsoncontent["assets"][asset_file]:
                     existing_files.append(file)
@@ -1349,23 +1359,26 @@
 
     def update_init_imports(self):
         def _remove_all_instruction(content):
             if "__all__ =" not in content:
                 return content
             content = content.replace("import os", "")
             content = content.replace("import glob", "")
-            content = "\n".join(
-                filter(lambda x: "__all__ =" not in x, content.splitlines())
-            ).strip() + "\n"
+            content = (
+                "\n".join(
+                    filter(lambda x: "__all__ =" not in x, content.splitlines())
+                ).strip()
+                + "\n"
+            )
             return content
 
         for path in self.path.glob("*"):
             if not path.is_dir():
                 continue
-            if not path.name in ["models", "tests", "controller", "controllers"]:
+            if path.name not in ["models", "tests", "controller", "controllers"]:
                 continue
             init_file = path / "__init__.py"
             if not init_file.exists():
                 continue
             content = _remove_all_instruction(init_file.read_text()).splitlines()
 
             for file in path.glob("*"):
@@ -1376,66 +1389,83 @@
 
             # remove if py does not exist anymore:
             for line in list(content):
                 if line.startswith("from . import "):
                     if not (path / (line.split(" ")[-1] + ".py")).exists():
                         content.remove(line)
 
-            init_file.write_text('\n'.join(content))
+            init_file.write_text("\n".join(content))
 
     def update_module_file(self):
-        # updates __openerp__.py the update-section to point to all xml files in the module;
-        # except if there is a directory test; those files are ignored;
+        # updates __openerp__.py the update-section to point to all xml files
+        # in the module; # except if there is a directory test; those files are ignored;
         self.update_assets_file()
         self.update_init_imports()
         mod = self.manifest_dict
 
         all_files = list(self.get_all_files_of_module())
         # first collect all xml files and ignore test and static
         DATA_NAME = "data"
         if current_version() <= 7.0:
             DATA_NAME = "update_xml"
 
         mod[DATA_NAME] = []
         mod["demo"] = []
-        if current_version() <= 13.0:
+        mod["qweb"] = []
+        if current_version() < 14.0:
             mod["css"] = []
-            mod["qweb"] = []
         is_web = False
 
         for local_path in all_files:
             if "test" in local_path.parts:
                 continue
             if local_path.suffix in [".xml", ".csv", ".yml"]:
                 if "demo" in local_path.parts:
                     mod["demo"].append(str(local_path))
                 elif "static" in local_path.parts:
                     # contains qweb file
                     is_web = True
                     if local_path.suffix == ".xml":
                         if "qweb" in mod:
-                            mod["qweb"].append(str(local_path))
+                            if str(local_path) not in mod["qweb"]:
+                                if current_version() <= 14.0:
+                                    mod["qweb"].append(str(local_path))
+                                else:
+                                    mod["qweb"].append(
+                                        self.name + "/" + str(local_path)
+                                    )
                 else:
-                    mod[DATA_NAME].append(str(local_path))
+                    if local_path.name not in ["gimera.yml"]:
+                        mod[DATA_NAME].append(str(local_path))
             elif local_path.suffix == ".js":
                 pass
             elif local_path.suffix in [".css", ".less", ".scss"]:
                 if "css" in mod:
-                    mod["css"].append(str(local_path))
+                    mod["css"] = list(set(mod["css"] + [str(local_path)]))
 
-        # keep test empty: use concrete call to test-file instead of testing on every module update
+        # keep test empty: use concrete call to test-file instead of testing
+        # on every module update
         mod["test"] = []
 
         # sort
         mod[DATA_NAME].sort()
         if mod.get("css"):
             mod["css"].sort()
         if "depends" in mod:
             mod["depends"].sort()
 
+        if current_version() > 14.0:
+            if "qweb" in mod:
+                mod.setdefault("assets", {})
+                mod["assets"].setdefault("web.assets_qweb", [])
+                mod["assets"]["web.assets_qweb"] += mod.pop("qweb")
+                mod["assets"]["web.assets_qweb"] = list(
+                    sorted(set(mod["assets"]["web.assets_qweb"]))
+                )
+
         # now sort again by inspecting file content - if __openerp__.sequence NUMBER is found, then
         # set this index; reason: some times there are wizards that reference forms and vice versa
         # but cannot find action ids
         # 06.05.2014: put the ir.model.acces.csv always at the end, because it references others, but security/groups always in front
         sorted_by_index = []  # contains tuples (index, filename)
         for filename in mod[DATA_NAME]:
             filename_xml = filename
@@ -1458,26 +1488,41 @@
                 elif filename.name == "ir.model.access.csv":
                     sequence = 999999
             sorted_by_index.append((sequence, filename_xml))
 
         sorted_by_index = sorted(sorted_by_index, key=lambda x: x[0])
         mod[DATA_NAME] = [x[1] for x in sorted_by_index]
 
+        # remove assets.xml for newer versions
+        if current_version() > 14.0:
+            mod[DATA_NAME] = list(filter(lambda x: not x.endswith("/assets.xml"), mod[DATA_NAME]))
+
         if is_web:
             mod["web"] = True
         if "application" not in mod:
             mod["application"] = False
 
         self.write_manifest(mod)
 
     def write_manifest(self, data):
         with self.manifest_path.open("w") as file:
             pp = pprint.PrettyPrinter(indent=4, stream=file)
             pp.pprint(data)
 
+    def calc_complexity(self):
+        """
+        Calculates the complexity of the module
+        """
+        res = {"loc": 0}
+        for file in self.get_all_files_of_module():
+            if file.suffix in [".py", ".csv", ".xml"]:
+                file = self.path / file
+                res["loc"] += len(file.read_text().splitlines())
+        return res
+
 
 def write_debug_instruction(instruction):
     (customs_dir() / ".debug").write_text(instruction)
 
 
 def _resolve_path_mapping(conn, path, model):
     """
```

### Comparing `wodoo-0.3.99/wodoo/myconfigparser.py` & `wodoo-0.4.1/wodoo/myconfigparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # used to read and write to settings
+import uuid
 import sys
 from pathlib import Path
+from .tools import atomic_write
+
 
 def _get_ignore_case_item(d, k):
     try:
         return d[k]
     except KeyError:
         if isinstance(k, str):
             for i in d.keys():
@@ -13,15 +16,14 @@
             else:
                 raise
         else:
             raise
 
 
 class MyConfigParser:
-
     def __init__(self, fileName, debug=False):
         if isinstance(fileName, dict):
             self.fileName = None
             self.configOptions = fileName
         else:
             self.fileName = Path(fileName)
             self.configOptions = {}
@@ -46,82 +48,83 @@
     def _open(self):
         if not self.fileName or not self.fileName.exists():
             return
         content = self.fileName.read_text().strip()
         for line in content.split("\n"):
             # If it isn't a comment get the variable and value and put it on a dict
             if not line.startswith("#") and len(line) > 1:
-                if '=' not in line:
+                if "=" not in line:
                     import click
-                    click.secho(f"Invalid configuration option '{line}' ignored.", fg='red')
+
+                    click.secho(
+                        f"Invalid configuration option '{line}' ignored.", fg="red"
+                    )
                     continue
-                (key, val) = line.rstrip('\n').split('=', 1)
+                (key, val) = line.rstrip("\n").split("=", 1)
                 val = val.strip()
-                val = val.strip('\"')
-                val = val.strip('\'')
+                val = val.strip('"')
+                val = val.strip("'")
                 self.configOptions[key.strip()] = val
 
     def write(self):
         handled_keys = set()
         if not self.fileName:
             return
-        try:
-            # Write the file contents
-            if not self.fileName.is_file():
-                self.fileName.parent.mkdir(exist_ok=True, parents=True)
-                self.fileName.write_text("")
-            with self.fileName.open("r+") as file:
-                lines = file.readlines()
-                # Truncate file so we don't need to close it and open it again
-                # for writing
-                file.seek(0)
-                file.truncate()
-
-                def write_line(key, val):
-                    if val is None:
-                        raise Exception("None value not allowed for: {}".format(key))
-                    return key + "=" + str(val)
-
-                # Loop through the file to change with new values in dict
-                for line in lines:
-                    if not line.startswith("#") and len(line) > 1:
-                        (key, val) = line.rstrip('\n').split('=', 1)
-                        key = key.strip()
-                        if key in self.configOptions:
-                            newVal = self.configOptions[key]
-
-                            # Only update if the variable value has changed
-                            if val != newVal:
-                                line = write_line(key, newVal)
-                        handled_keys.add(key)
-                    file.write(line.strip() + "\n")
-                for key in self.configOptions.keys():
-                    if key not in handled_keys:
-                        file.write(write_line(key, self.configOptions[key]).strip() + "\n")
-        except IOError as e:
-            print("ERROR opening file " + self.fileName + ": " + e.strerror + "\n")
+        # Write the file contents
+        if not self.fileName.is_file():
+            self.fileName.parent.mkdir(exist_ok=True, parents=True)
+
+        lines = []
+        if self.fileName.exists():
+            lines = self.fileName.read_text().splitlines()
+
+        def format_line(key, val):
+            if val is None:
+                raise Exception("None value not allowed for: {}".format(key))
+            return key + "=" + str(val)
+
+        # Loop through the file to change with new values in dict
+        def _update_lines():
+            for line in lines:
+                if line.startswith("#") or len(line) <= 1:
+                    yield line
+                    continue
+                (key, val) = line.rstrip("\n").split("=", 1)
+                key = key.strip()
+                if key in self.configOptions:
+                    newVal = self.configOptions[key]
+
+                    # Only update if the variable value has changed
+                line = format_line(key, newVal)
+                yield line
+                handled_keys.add(key)
+
+            for key in self.configOptions.keys():
+                if key not in handled_keys:
+                    yield format_line(key, self.configOptions[key])
 
-    # Redefinition of __getitem__ and __setitem__
+        with atomic_write(self.fileName) as file:
+            file.write_text("\n".join(_update_lines()) + "\n")
 
     def __getitem__(self, key):
         try:
             return _get_ignore_case_item(self.configOptions, key)
         except KeyError:
             if isinstance(key, int):
                 keys = self.configOptions.keys()
                 return _get_ignore_case_item(self.configOptions[keys[key]])
             else:
                 raise KeyError(f"Key {key} doesn't exist in {self.fileName}")
 
     def __setitem__(self, key, value):
         if isinstance(value, list):
-            value_list = '('
+            value_list = "("
             for item in value:
-                value_list += ' \"' + item + '\"'
-            value_list += ' )'
+                value_list += ' "' + item + '"'
+            value_list += " )"
             self.configOptions[key] = value_list
         else:
             self.configOptions[key] = value
 
     def get(self, key, default_value=""):
         try:
             return self[key]
```

### Comparing `wodoo-0.3.99/wodoo/odoo_config.py` & `wodoo-0.4.1/wodoo/odoo_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,27 +133,32 @@
     def _update(self, d):
         d["install"] = list(sorted(set(d["install"])))
         s = json.dumps(d, indent=4)
         tfile = Path(tempfile.mktemp(suffix=".MANIFEST"))
         tfile.write_text(s)
         shutil.move(tfile, MANIFEST_FILE())
 
-        if len(set(d['addons_paths'])) != len(d['addons_paths']):
+        if len(set(d["addons_paths"])) != len(d["addons_paths"]):
             abort("Addons Paths contains duplicate entries!")
 
     def rewrite(self):
         self._update(self._get_data())
 
 
 def MANIFEST():
     return MANIFEST_CLASS()
 
 
+cache_version = {}
+
+
 def current_version():
-    return float(MANIFEST()["version"])
+    if cache_version.get("value") is None:
+        cache_version["value"] = float(MANIFEST()["version"])
+    return cache_version["value"]
 
 
 def get_postgres_connection_params(inside_container=None):
     config = get_settings()
     if (
         not inside_container
         and os.getenv("DOCKER_MACHINE") != "1"
```

### Comparing `wodoo-0.3.99/wodoo/odoo_parser.py` & `wodoo-0.4.1/wodoo/odoo_parser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/robo_helpers.py` & `wodoo-0.4.1/wodoo/robo_helpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/settings.py` & `wodoo-0.4.1/wodoo/settings.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/testzfs.sh` & `wodoo-0.4.1/wodoo/testzfs.sh`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/tools.py` & `wodoo-0.4.1/wodoo/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import platform
+import uuid
+import time
 from subprocess import PIPE, STDOUT
 import hashlib
 import requests
 import stat
 from contextlib import contextmanager
 import re
 import inquirer
+import cProfile
+import functools
 
 try:
     import arrow
 except ImportError:
     pass
 from pathlib import Path
 import io
@@ -61,22 +64,30 @@
         if dbname:
             result.dbname = dbname
         return result
 
     def get_psyco_connection(self, db=None):
         import psycopg2
 
-        conn = psycopg2.connect(
-            dbname=db or self.dbname,
-            user=self.user,
-            password=self.pwd,
-            host=self.host,
-            port=self.port or None,
-            connect_timeout=int(os.getenv("PSYCOPG_TIMEOUT", "3")),
-        )
+        while True:
+            try:
+                conn = psycopg2.connect(
+                    dbname=db or self.dbname,
+                    user=self.user,
+                    password=self.pwd,
+                    host=self.host,
+                    port=self.port or None,
+                    connect_timeout=int(os.getenv("PSYCOPG_TIMEOUT", "3")),
+                )
+                break
+            except psycopg2.OperationalError as ex:
+                if "database system is starting up" in str(ex):
+                    time.sleep(2)
+                else:
+                    raise
         return conn
 
     @contextmanager
     def connect(self, db=None):
         conn = self.get_psyco_connection(db=db)
         cr = conn.cursor()
         try:
@@ -227,14 +238,30 @@
             ")"
         ),
         fetchone=True,
     )
     return record[0]
 
 
+def docker_list_containers(project_name, service_name, status_filter=None):
+    cmd = [
+        "docker",
+        "ps",
+        "-a",
+        "-q",
+        "--no-trunc",
+        "--filter",
+        f"name=^/{project_name}_{service_name}$",
+    ]
+    if status_filter:
+        cmd += ["--filter", f"status={status_filter}"]
+    container_ids = subprocess.check_output(cmd, encoding="utf8").strip().splitlines()
+    return container_ids
+
+
 def _wait_postgres(config, timeout=600):
     started = arrow.get()
     if config.run_postgres:
         conn = config.get_odoo_conn().clone(dbname="postgres")
         container_ids = (
             subprocess.check_output(
                 [
@@ -255,20 +282,17 @@
         import docker
 
         client = docker.from_env()
         postgres_containers = []
         for container_id in container_ids:
             if not container_id:
                 continue
-            container = client.containers.get(container_id)
-            if not container:
-                continue
-            if not container.attrs["State"]["Running"]:
-                continue
-            postgres_containers += [container]
+            state = _docker_id_state(container_id)
+            if state == "running":
+                postgres_containers += [container_id]
 
         deadline = arrow.get().shift(seconds=timeout)
         last_ex = None
         while True:
             if arrow.get() > deadline:
                 # if running containers wait for health state:
                 if not postgres_containers:
@@ -279,50 +303,64 @@
                             "'odoo up -d postgres' first?"
                         )
                     )
 
                 raise Exception(f"Timeout waiting postgres reached: {timeout}seconds")
             try:
                 _execute_sql(
-                    conn,
-                    sql="""
-                SELECT table_schema,table_name
-                FROM information_schema.tables
-                ORDER BY table_schema,table_name
-                LIMIT 1;
-                """,
+                    conn.clone(dbname="postgres"),
+                    sql=(
+                        " SELECT table_schema,table_name "
+                        " FROM information_schema.tables "
+                        " ORDER BY table_schema,table_name "
+                        " LIMIT 1; "
+                    ),
                 )
                 break
 
             except Exception as ex:
                 seconds = (arrow.get() - started).total_seconds()
-                if seconds > 5:
+                if seconds > 10:
                     if str(ex) != str(last_ex):
                         click.secho(
                             f"Waiting again for postgres. Last error is: {str(ex)}"
                         )
                     last_ex = ex
                 time.sleep(1)
         click.secho("Postgres now available.", fg="green")
 
 
-def _is_container_running(config, machine_name):
-    import docker
+def _docker_id_state(container_id):
+    status = subprocess.check_output(
+        [
+            "docker",
+            "container",
+            "ls",
+            "--format",
+            "{{.State}}",
+            "--filter",
+            f"id={container_id}",
+        ],
+        encoding="utf8",
+    ).strip()
+    return status
+
+
+def docker_kill_container(container_id, remove=False):
+    subprocess.check_call(["docker", "kill", container_id])
+    if remove:
+        subprocess.check_call(["docker", "rm", container_id])
 
+
+def _is_container_running(config, machine_name):
     container_id = __dc_out(config, ["ps", "-q", machine_name]).strip()
     if container_id:
-        container = list(
-            filter(
-                lambda container: container.id == container_id,
-                docker.from_env().containers.list(),
-            )
-        )
-        if container:
-            container = container[0]
-            return container.status == "running"
+        status = _docker_id_state(container_id)
+        if status:
+            return status == "running"
     return False
 
 
 def is_up(config, *machine_name):
     assert len(machine_name) == 1
     click.echo(
         "Running" if _is_container_running(config, machine_name[0]) else "Not Running",
@@ -813,14 +851,15 @@
         f"delete from ir_attachment where res_model = 'ir.ui.view' and name ilike '%.scss%' {ignore_url_str};",
         f"delete from ir_attachment where name ilike '/web/%web%asset%' {ignore_url_str}",
         f"delete from ir_attachment where name ilike 'import_bootstrap.less' {ignore_url_str}",
         f"delete from ir_attachment where name ilike '%.less' {ignore_url_str}",
         f"delete from ir_attachment where name ilike '%.scss' {ignore_url_str}",
         f"delete from ir_attachment where name ilike 'web_icon_data' {ignore_url_str}",
         f"delete from ir_attachment where name ilike 'web_editor.summernote.%' {ignore_url_str}",
+        f"delete from ir_attachment where name ilike 'web.assets_backend_prod_only.js'",
     ]
     try:
         for query in queries:
             try:
                 click.secho(query, fg="grey")
                 cr.execute(query)
                 conn.commit()
@@ -886,21 +925,22 @@
         raise E
 
 
 def __hash_odoo_password(pwd):
     from .odoo_config import current_version
 
     if current_version() in [
+        9.0,
+        10.0,
         11.0,
         12.0,
         13.0,
         14.0,
         15.0,
-        10.0,
-        9.0,
+        16.0,
     ]:
         setpw = CryptContext(schemes=["pbkdf2_sha512", "md5_crypt"])
         return setpw.encrypt(pwd)
     else:
         raise NotImplementedError()
 
 
@@ -953,51 +993,14 @@
 def _get_host_ip():
     conn = os.getenv("SSH_CONNECTION", "")
     if conn:
         conn = [x for x in conn.split(" ") if x]
         return conn[2]
 
 
-def _is_dirty(repo, check_submodule, assert_clean=False):
-    from git import Repo
-    from git import InvalidGitRepositoryError
-    from git import NoSuchPathError
-
-    def raise_error():
-        if assert_clean:
-            click.secho(
-                ("Dirty directory - please cleanup: {repo.working_dir}"),
-                bold=True,
-                fg="red",
-            )
-            sys.exit(42)
-
-    if repo.is_dirty() or repo.untracked_files:
-        raise_error()
-        return True
-    if check_submodule:
-        try:
-            repo.submodules
-        except AttributeError:
-            pass
-        else:
-            for submodule in repo.submodules:
-                try:
-                    sub_repo = Repo(submodule.path)
-                except InvalidGitRepositoryError:
-                    click.secho(f"Invalid Repo: {submodule}", bold=True, fg="red")
-                except NoSuchPathError:
-                    click.secho(f"Invalid Repo: {submodule}", bold=True, fg="red")
-                else:
-                    if _is_dirty(sub_repo, True, assert_clean=assert_clean):
-                        raise_error()
-                        return True
-    return False
-
-
 def __assure_gitignore(gitignore_file, content):
     p = Path(gitignore_file)
     if not p.exists():
         p.write_text(content + "\n")
         return
     exists = [
         l for l in gitignore_file.read_text().splitlines() if l.strip() == content
@@ -1145,22 +1148,25 @@
         .split(" ")[0]
         .strip()
     )
     return hex
 
 
 def git_diff_files(path, commit1, commit2):
+    params = [
+        "git",
+        "diff",
+        "--name-only",
+    ]
+    if commit1:
+        params += [commit1]
+    if commit2:
+        params += [commit2]
     output = subprocess.check_output(
-        [
-            "git",
-            "diff",
-            "--name-only",
-            commit1,
-            commit2,
-        ],
+        params,
         encoding="utf8",
         cwd=path,
     )
     filepaths = list(filter(bool, output.splitlines()))
     return filepaths
 
 
@@ -1169,14 +1175,30 @@
     if not Path(folder).exists():
         raise Exception(f"Could not zip folder: {folder}")
     os.system((f"cd '{folder}' && tar c . | pv | pigz > '{destpath}'"))
     if not destpath.exists():
         raise Exception(f"file {destpath} not generated")
 
 
+def try_ignore_exceptions(execute, exceptions, timeout=10):
+    started = arrow.get()
+    while True:
+        try:
+            execute()
+        except exceptions:
+            if (arrow.get() - started).total_seconds() > timeout:
+                raise
+            else:
+                time.sleep(0.5)
+        except Exception:
+            raise
+        else:
+            break
+
+
 @contextmanager
 def autocleanpaper(filepath=None, strict=False):
     if strict:
         assert filepath
     else:
         filepath = Path(filepath or tempfile._get_default_tempdir()) / next(
             tempfile._get_candidate_names()
@@ -1217,15 +1239,17 @@
     )
     fstype = list(filter(bool, lines[1].replace("\t", " ").split(" ")))[1]
     return fstype
 
 
 def get_git_hash(path=None):
     return subprocess.check_output(
-        ["git", "log", "-n", "1", "--format=%H"], cwd=path or os.getcwd()
+        ["git", "log", "-n", "1", "--format=%H"],
+        cwd=path or os.getcwd(),
+        encoding="utf8",
     ).strip()
 
 
 def is_git_clean(path=None, ignore_files=None):
     ignore_files = ignore_files or []
     path = path or Path(os.getcwd())
     if not (path / ".git").exists():
@@ -1382,38 +1406,31 @@
 
 
 def _make_sure_module_is_installed(ctx, config, modulename, repo_url):
     from .module_tools import DBModules
     from .odoo_config import MANIFEST
     from .odoo_config import current_version
     from .cli import cli, pass_config, Commands
+    from gimera.gimera import add as gimera_add
+    from gimera.gimera import apply as gimera_apply
 
     state = DBModules.get_meta_data(modulename)
     if state["state"] == "installed":
         return
 
     path = Path("addons_wodoo") / modulename
     if not path.exists():
-        subprocess.check_call(
-            [
-                "gimera",
-                "add",
-                "-u",
-                repo_url,
-                "--path",
-                path,
-                "--branch",
-                str(current_version()),
-                "--type", 
-                "integrated",
-            ]
+        ctx.invoke(
+            gimera_add,
+            url=repo_url,
+            path=str(path),
+            branch=str(current_version()),
+            type="integrated",
         )
-        subprocess.check_call([
-            "gimera", "apply", path,
-        ])
+        ctx.invoke(gimera_apply, repos=str(path))
 
     # if not yet there, then pack into "addons_framework"
     manifest = MANIFEST()
     addons_paths = manifest.get("addons_paths", [])
     install = manifest.get("install", [])
     if modulename not in install:
         install += [modulename]
@@ -1423,15 +1440,15 @@
         addons_paths += [str(path)]
         manifest["addons_paths"] = addons_paths
 
     manifest.rewrite()
 
     Commands.invoke(
         ctx,
-        'update',
+        "update",
         module=[modulename],
         no_restart=False,
         no_dangling_check=True,
         no_update_module_list=False,
         non_interactive=True,
     )
 
@@ -1442,18 +1459,76 @@
     ]
     if type:
         cmd += [
             "-type",
             type,
         ]
     if wholename:
-        cmd += [
-            "-wholename",
-            wholename
-        ]
+        cmd += ["-wholename", wholename]
     if name:
+        cmd += ["-name", name]
+    files = subprocess.check_output(cmd, cwd=path, encoding="utf8").splitlines()
+    return map(lambda x: Path(path) / x, files)
+
+
+def _update_setting(conn, key, value):
+    value = str(value)
+    _execute_sql(
+        conn,
+        f"DELETE FROM ir_config_parameter WHERE key = '{key}'; "
+        f"INSERT INTO ir_config_parameter(key, value, create_date, write_date) values('{key}', '{value}', now(), now());",
+    )
+
+
+def _get_setting(conn, key):
+    rec = _execute_sql(
+        conn,
+        f"SELECT value FROM ir_config_parameter WHERE key = '{key}'",
+        fetchone=True,
+    )
+    if rec:
+        return rec[0]
+
+
+@contextmanager
+def cwd(path):
+    remember = os.getcwd()
+    os.chdir(path)
+    try:
+        yield
+    finally:
+        os.chdir(remember)
+
+
+@contextmanager
+def atomic_write(file):
+    tempfile = file.parent / f"{file.name}.{uuid.uuid4()}"
+    try:
+        yield tempfile
+
+        if file.exists():
+            file.unlink()
+        tempfile.rename(file)
+
+    except Exception:
+        if tempfile.exists():
+            try:
+                tempfile.unlink()
+            except Exception:
+                pass
+
+
+def bash_find(path, name=None, wholename=None, type=None):
+    cmd = [
+        "find",
+    ]
+    if type:
         cmd += [
-            "-name",
-            name
+            "-type",
+            type,
         ]
+    if wholename:
+        cmd += ["-wholename", wholename]
+    if name:
+        cmd += ["-name", name]
     files = subprocess.check_output(cmd, cwd=path, encoding="utf8").splitlines()
-    return map(lambda x: Path(path) / x, files)
+    return list(map(lambda x: Path(path) / x, files))
```

### Comparing `wodoo-0.3.99/wodoo/wait/decorator.py` & `wodoo-0.4.1/wodoo/wait/decorator.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/wait/log.py` & `wodoo-0.4.1/wodoo/wait/log.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo/wait/tcp.py` & `wodoo-0.4.1/wodoo/wait/tcp.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.3.99/wodoo.egg-info/PKG-INFO` & `wodoo-0.4.1/wodoo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.3.99
+Version: 0.4.1
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -167,15 +167,45 @@
 | ODOO_INSTALL_LIBPOSTAL=1| If set, then the libpostal lib is installed|
 | ODOO_QUEUEJOBS_CRON_IN_ONE_CONTAINER=1 | Runs queuejobs and cronjob in the odoo container where also the web application resides|
 | ODOO_QUEUEJOBS_CHANNELS=root:40,magento2:1 | Configures queues for queuejob module |
 |NAMED_ODOO_POSTGRES_VOLUME| Use a specific external volume; not dropped with down -v command|
 |CRONJOB_DADDY_CLEANUP=0 */1 * * * ${JOB_DADDY_CLEANUP}|Turn on grandfather-principle based backup|
 |RESTART_CONTAINERS=1|Sets "restart unless-stopped" policy|
 
+## Odoo Server Configuration in ~/.odoo/settings/odoo.config and odoo.config.${PROJECT_NAME}
+
+Contents will be appended to [options] section of standard odoo configuration.
+
+Configuration may simple look like:
+
+
+```
+setting1=value1
+```
+
+or like that:
+
+```
+[options]
+setting1=value1
+
+[queue_job]
+settingqj=valueqj
+```
+
+The [options] is prepended automatically if missed.
+
 
 # Pytests
 
 Best executed with:
 
 ```bash
 time sudo -E pytest
 ```
+
+# Performance Check
+
+```python
+pipx runpip wodoo install line_profiler
+~/.local/pipx/venvs/wodoo/bin/python3 -mkernprof -l -v odoo reload
+```
```

### Comparing `wodoo-0.3.99/wodoo.egg-info/SOURCES.txt` & `wodoo-0.4.1/wodoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

