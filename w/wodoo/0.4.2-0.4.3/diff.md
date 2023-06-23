# Comparing `tmp/wodoo-0.4.2.tar.gz` & `tmp/wodoo-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wodoo-0.4.2.tar", last modified: Fri Jun 23 07:27:08 2023, max compression
+gzip compressed data, was "wodoo-0.4.3.tar", last modified: Fri Jun 23 07:47:52 2023, max compression
```

## Comparing `wodoo-0.4.2.tar` & `wodoo-0.4.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.046487 wodoo-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 07:26:34.000000 wodoo-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 07:27:08.046487 wodoo-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-23 07:26:34.000000 wodoo-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 07:27:08.046487 wodoo-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 07:26:34.000000 wodoo-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.034487 wodoo-0.4.2/wodoo/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/click_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/click_global_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.038487 wodoo-0.4.2/wodoo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/config/cicd_network_for_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/config/default_network
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/config/template_onlyloop.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/config/template_withports.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/daddy_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/defaults
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.022487 wodoo-0.4.2/wodoo/extra_install/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.022487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.038487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.038487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.038487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.042487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.042487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.042487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.042487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.042487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
--rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.042487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.042487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.046487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
--rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
--rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.026487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.046487 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_clickhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_control_with_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_db_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_db_snapshots_docker_btrfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_db_snapshots_docker_zfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_db_snapshots_plain_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)    50013 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_src.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/lib_turnintodev.py
--rw-r--r--   0 runner    (1001) docker     (123)    55120 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/module_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/myconfigparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/odoo_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/odoo_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/pudb.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/robo_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.046487 wodoo-0.4.2/wodoo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/tests/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/tests/gimera.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.046487 wodoo-0.4.2/wodoo/tests/module_respartner_dummyfield1/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.046487 wodoo-0.4.2/wodoo/tests/module_respartner_dummyfield2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/testzfs.sh
--rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 07:27:03.000000 wodoo-0.4.2/wodoo/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.046487 wodoo-0.4.2/wodoo/wait/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/wait/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/wait/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/wait/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 07:26:34.000000 wodoo-0.4.2/wodoo/wait/tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:08.034487 wodoo-0.4.2/wodoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 07:27:07.000000 wodoo-0.4.2/wodoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-23 07:27:08.000000 wodoo-0.4.2/wodoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:27:07.000000 wodoo-0.4.2/wodoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 07:27:07.000000 wodoo-0.4.2/wodoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 07:27:08.000000 wodoo-0.4.2/wodoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 07:27:08.000000 wodoo-0.4.2/wodoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.858882 wodoo-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 07:47:23.000000 wodoo-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 07:47:52.858882 wodoo-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-23 07:47:23.000000 wodoo-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 07:47:52.858882 wodoo-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 07:47:23.000000 wodoo-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.850882 wodoo-0.4.3/wodoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/click_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/click_global_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.850882 wodoo-0.4.3/wodoo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/config/cicd_network_for_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/config/default_network
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/config/template_onlyloop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/config/template_withports.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/daddy_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/defaults
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.842882 wodoo-0.4.3/wodoo/extra_install/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.842882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.846882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.854882 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_clickhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_control_with_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_db_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_db_snapshots_docker_btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_db_snapshots_docker_zfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_db_snapshots_plain_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50013 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_src.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/lib_turnintodev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55120 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/module_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/myconfigparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/odoo_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/odoo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/pudb.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/robo_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.858882 wodoo-0.4.3/wodoo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/tests/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/tests/gimera.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.858882 wodoo-0.4.3/wodoo/tests/module_respartner_dummyfield1/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.858882 wodoo-0.4.3/wodoo/tests/module_respartner_dummyfield2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/testzfs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 07:47:49.000000 wodoo-0.4.3/wodoo/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.858882 wodoo-0.4.3/wodoo/wait/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/wait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/wait/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/wait/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 07:47:23.000000 wodoo-0.4.3/wodoo/wait/tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:47:52.850882 wodoo-0.4.3/wodoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 07:47:52.000000 wodoo-0.4.3/wodoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-23 07:47:52.000000 wodoo-0.4.3/wodoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:47:52.000000 wodoo-0.4.3/wodoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 07:47:52.000000 wodoo-0.4.3/wodoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 07:47:52.000000 wodoo-0.4.3/wodoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 07:47:52.000000 wodoo-0.4.3/wodoo.egg-info/top_level.txt
```

### Comparing `wodoo-0.4.2/LICENSE` & `wodoo-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/PKG-INFO` & `wodoo-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.4.2
+Version: 0.4.3
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wodoo-0.4.2/README.md` & `wodoo-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/setup.py` & `wodoo-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/__init__.py` & `wodoo-0.4.3/wodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/cli.py` & `wodoo-0.4.3/wodoo/cli.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/click_config.py` & `wodoo-0.4.3/wodoo/click_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/click_global_commands.py` & `wodoo-0.4.3/wodoo/click_global_commands.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/consts.py` & `wodoo-0.4.3/wodoo/consts.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/daddy_cleanup.py` & `wodoo-0.4.3/wodoo/daddy_cleanup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/defaults` & `wodoo-0.4.3/wodoo/defaults`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings` & `wodoo-0.4.3/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_backup.py` & `wodoo-0.4.3/wodoo/lib_backup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_clickhelpers.py` & `wodoo-0.4.3/wodoo/lib_clickhelpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_composer.py` & `wodoo-0.4.3/wodoo/lib_composer.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_control.py` & `wodoo-0.4.3/wodoo/lib_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 ["docker", "volume", "rm", "-f", vol], encoding="utf8",
                 capture_output=True,
             )
             if rc.returncode:
                 output = rc.stderr
                 for group in re.findall(r"(\[[^\]]*])", output):
                     container_id = group[1:-1]
-                    subprocess.check_call(["docker", "kill", container_id])
+                    subprocess.run(["docker", "kill", container_id])
                     subprocess.check_call(["docker", "rm", "-fv", container_id])
                     output = subprocess.check_output(
                         ["docker", "volume", "rm", "-f", vol], encoding="utf8"
                     )
 
         if dry_run:
             click.secho("Dry Run - didnt do it.")
```

### Comparing `wodoo-0.4.2/wodoo/lib_control_with_docker.py` & `wodoo-0.4.3/wodoo/lib_control_with_docker.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_db.py` & `wodoo-0.4.3/wodoo/lib_db.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_db_snapshots.py` & `wodoo-0.4.3/wodoo/lib_db_snapshots.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_db_snapshots_docker_btrfs.py` & `wodoo-0.4.3/wodoo/lib_db_snapshots_docker_btrfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_db_snapshots_docker_zfs.py` & `wodoo-0.4.3/wodoo/lib_db_snapshots_docker_zfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_db_snapshots_plain_postgres.py` & `wodoo-0.4.3/wodoo/lib_db_snapshots_plain_postgres.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_docker_registry.py` & `wodoo-0.4.3/wodoo/lib_docker_registry.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_lang.py` & `wodoo-0.4.3/wodoo/lib_lang.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_module.py` & `wodoo-0.4.3/wodoo/lib_module.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_setup.py` & `wodoo-0.4.3/wodoo/lib_setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_src.py` & `wodoo-0.4.3/wodoo/lib_src.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_talk.py` & `wodoo-0.4.3/wodoo/lib_talk.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/lib_turnintodev.py` & `wodoo-0.4.3/wodoo/lib_turnintodev.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/module_tools.py` & `wodoo-0.4.3/wodoo/module_tools.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/myconfigparser.py` & `wodoo-0.4.3/wodoo/myconfigparser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/odoo_config.py` & `wodoo-0.4.3/wodoo/odoo_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/odoo_parser.py` & `wodoo-0.4.3/wodoo/odoo_parser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/robo_helpers.py` & `wodoo-0.4.3/wodoo/robo_helpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/settings.py` & `wodoo-0.4.3/wodoo/settings.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/testzfs.sh` & `wodoo-0.4.3/wodoo/testzfs.sh`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/tools.py` & `wodoo-0.4.3/wodoo/tools.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/wait/decorator.py` & `wodoo-0.4.3/wodoo/wait/decorator.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/wait/log.py` & `wodoo-0.4.3/wodoo/wait/log.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo/wait/tcp.py` & `wodoo-0.4.3/wodoo/wait/tcp.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.2/wodoo.egg-info/PKG-INFO` & `wodoo-0.4.3/wodoo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.4.2
+Version: 0.4.3
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wodoo-0.4.2/wodoo.egg-info/SOURCES.txt` & `wodoo-0.4.3/wodoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

