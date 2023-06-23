# Comparing `tmp/erpbrasil.edoc-2.3.1.tar.gz` & `tmp/erpbrasil.edoc-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erpbrasil.edoc-2.3.1.tar", last modified: Wed Mar 22 14:50:39 2023, max compression
+gzip compressed data, was "erpbrasil.edoc-2.4.0.tar", last modified: Fri Jun 23 13:58:03 2023, max compression
```

## Comparing `erpbrasil.edoc-2.3.1.tar` & `erpbrasil.edoc-2.4.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.869213 erpbrasil.edoc-2.3.1/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1424 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/.appveyor.yml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      511 2023-03-22 14:50:17.000000 erpbrasil.edoc-2.3.1/.bumpversion.cfg
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     2893 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/.cookiecutterrc
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      182 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/.coveragerc
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      215 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/.editorconfig
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      915 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/.travis.yml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       64 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/AUTHORS.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1181 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/CHANGELOG.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     2753 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1105 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/LICENSE
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      359 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/MANIFEST.in
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     4556 2023-03-22 14:50:39.869213 erpbrasil.edoc-2.3.1/PKG-INFO
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     3582 2023-03-22 14:50:17.000000 erpbrasil.edoc-2.3.1/README.rst
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.861213 erpbrasil.edoc-2.3.1/ci/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     3995 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/appveyor-bootstrap.py
--rwxrwxr-x   0 mileo     (1000) mileo     (1000)     3827 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/appveyor-download.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      763 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/appveyor-with-compiler.cmd
--rwxrwxr-x   0 mileo     (1000) mileo     (1000)     2097 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/bootstrap.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       50 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/requirements.txt
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.861213 erpbrasil.edoc-2.3.1/ci/templates/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1756 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/templates/.appveyor.yml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      956 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/templates/.travis.yml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1816 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/ci/templates/appveyor.yml
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.861213 erpbrasil.edoc-2.3.1/docs/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       28 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/authors.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       30 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/changelog.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1382 2023-03-22 14:50:17.000000 erpbrasil.edoc-2.3.1/docs/conf.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       33 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/contributing.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      245 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/index.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       94 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/installation.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       27 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/readme.rst
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.861213 erpbrasil.edoc-2.3.1/docs/reference/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      126 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/reference/erpbrasil.edoc.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       66 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/reference/index.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       29 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/requirements.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      109 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/spelling_wordlist.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       80 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/docs/usage.rst
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       98 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/requirements.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      508 2023-03-22 14:50:39.869213 erpbrasil.edoc-2.3.1/setup.cfg
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     3749 2023-03-22 14:50:17.000000 erpbrasil.edoc-2.3.1/setup.py
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.857213 erpbrasil.edoc-2.3.1/src/
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.861213 erpbrasil.edoc-2.3.1/src/erpbrasil/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      271 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/__init__.py
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.865213 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      481 2023-03-22 14:50:17.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/__init__.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      397 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/__main__.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6739 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/chave.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      831 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/cli.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     7116 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/edoc.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    11568 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/mde.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     3916 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/mdfe.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    14351 2023-03-22 14:50:01.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/nfce.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    45499 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/nfe.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     3740 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/nfse.py
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.865213 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)        0 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/__init__.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1001 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/cidades.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     2463 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/dsf.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    10310 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/ginfes.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    12756 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/issnet.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6615 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/paulistana.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1264 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/resposta.py
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.861213 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     4556 2023-03-22 14:50:39.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/PKG-INFO
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     2607 2023-03-22 14:50:39.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/SOURCES.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)        1 2023-03-22 14:50:39.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/dependency_links.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       60 2023-03-22 14:50:39.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/entry_points.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       25 2023-03-22 14:50:39.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/namespace_packages.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)        1 2023-03-13 17:07:10.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/not-zip-safe
--rw-rw-r--   0 mileo     (1000) mileo     (1000)      281 2023-03-22 14:50:39.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/requires.txt
--rw-rw-r--   0 mileo     (1000) mileo     (1000)       10 2023-03-22 14:50:39.000000 erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/top_level.txt
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.865213 erpbrasil.edoc-2.3.1/tests/
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.865213 erpbrasil.edoc-2.3.1/tests/fixtures/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     2597 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/dummy_cert.pfx
-drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-03-22 14:50:39.869213 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    11491 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     9234 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     3008 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_chave.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6682 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    11477 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6969 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    10324 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6744 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    16217 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)    17539 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     2497 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6764 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6533 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_status_servico.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)   144902 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     2620 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     3105 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_manifestacao.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     6921 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_nfse_ginfes.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     5431 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_nfse_paulistana.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1261 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_situacao.py
--rw-rw-r--   0 mileo     (1000) mileo     (1000)     1989 2023-03-13 17:05:27.000000 erpbrasil.edoc-2.3.1/tox.ini
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.168731 erpbrasil.edoc-2.4.0/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1424 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/.appveyor.yml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      511 2023-06-23 13:57:31.000000 erpbrasil.edoc-2.4.0/.bumpversion.cfg
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     2893 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/.cookiecutterrc
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      182 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/.coveragerc
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      215 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/.editorconfig
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      915 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/.travis.yml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       64 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/AUTHORS.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1181 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/CHANGELOG.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     2753 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1105 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/LICENSE
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      359 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/MANIFEST.in
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     4556 2023-06-23 13:58:03.168731 erpbrasil.edoc-2.4.0/PKG-INFO
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     3582 2023-06-23 13:57:31.000000 erpbrasil.edoc-2.4.0/README.rst
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.164731 erpbrasil.edoc-2.4.0/ci/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     3995 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/appveyor-bootstrap.py
+-rwxrwxr-x   0 mileo     (1000) mileo     (1000)     3827 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/appveyor-download.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      763 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/appveyor-with-compiler.cmd
+-rwxrwxr-x   0 mileo     (1000) mileo     (1000)     2097 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/bootstrap.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       50 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/requirements.txt
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.164731 erpbrasil.edoc-2.4.0/ci/templates/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1756 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/templates/.appveyor.yml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      956 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/templates/.travis.yml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1816 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/ci/templates/appveyor.yml
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.164731 erpbrasil.edoc-2.4.0/docs/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       28 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/authors.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       30 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/changelog.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1382 2023-06-23 13:57:31.000000 erpbrasil.edoc-2.4.0/docs/conf.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       33 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/contributing.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      245 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/index.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       94 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/installation.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       27 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/readme.rst
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.164731 erpbrasil.edoc-2.4.0/docs/reference/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      126 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/reference/erpbrasil.edoc.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       66 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/reference/index.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       29 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/requirements.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      109 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       80 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/docs/usage.rst
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       98 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/requirements.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      508 2023-06-23 13:58:03.172731 erpbrasil.edoc-2.4.0/setup.cfg
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     3749 2023-06-23 13:57:31.000000 erpbrasil.edoc-2.4.0/setup.py
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.160731 erpbrasil.edoc-2.4.0/src/
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.164731 erpbrasil.edoc-2.4.0/src/erpbrasil/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      271 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/__init__.py
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.168731 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      481 2023-06-23 13:57:31.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/__init__.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      397 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/__main__.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6739 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/chave.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      831 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/cli.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     7116 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/edoc.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    11568 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/mde.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     3916 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/mdfe.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    14351 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/nfce.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    45500 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/nfe.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     3740 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/nfse.py
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.168731 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/__init__.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1037 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/cidades.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     2463 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/dsf.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    10310 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/ginfes.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    12756 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/issnet.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6850 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/paulistana.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1264 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/resposta.py
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.164731 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     4556 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/PKG-INFO
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     2607 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)        1 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       60 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/entry_points.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       25 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)        1 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/not-zip-safe
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)      281 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/requires.txt
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)       10 2023-06-23 13:58:03.000000 erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/top_level.txt
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.168731 erpbrasil.edoc-2.4.0/tests/
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.168731 erpbrasil.edoc-2.4.0/tests/fixtures/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     2597 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/dummy_cert.pfx
+drwxrwxr-x   0 mileo     (1000) mileo     (1000)        0 2023-06-23 13:58:03.168731 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    11491 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     9234 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     3008 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_chave.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6682 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    11477 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6969 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    10324 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6744 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    16217 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)    17539 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     2497 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6764 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6533 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)   144902 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     2620 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     3105 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_manifestacao.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     6921 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_nfse_ginfes.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     5431 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_nfse_paulistana.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1261 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_situacao.py
+-rw-rw-r--   0 mileo     (1000) mileo     (1000)     1989 2023-06-23 13:54:38.000000 erpbrasil.edoc-2.4.0/tox.ini
```

### Comparing `erpbrasil.edoc-2.3.1/.appveyor.yml` & `erpbrasil.edoc-2.4.0/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/.cookiecutterrc` & `erpbrasil.edoc-2.4.0/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/.travis.yml` & `erpbrasil.edoc-2.4.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/CHANGELOG.rst` & `erpbrasil.edoc-2.4.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/CONTRIBUTING.rst` & `erpbrasil.edoc-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/LICENSE` & `erpbrasil.edoc-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/PKG-INFO` & `erpbrasil.edoc-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.3.1
+Version: 2.4.0
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
```

### Comparing `erpbrasil.edoc-2.3.1/README.rst` & `erpbrasil.edoc-2.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     :alt: Coverage Status
     :target: https://codecov.io/github/erpbrasil/erpbrasil.edoc
 
 .. |version| image:: https://img.shields.io/pypi/v/erpbrasil.edoc.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/erpbrasil.edoc
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.3.1.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.4.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.3.1...master
+    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.4.0...master
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/erpbrasil.edoc.svg
     :alt: PyPI Wheel
     :target: https://pypi.org/project/erpbrasil.edoc
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/erpbrasil.edoc.svg
     :alt: Supported versions
```

### Comparing `erpbrasil.edoc-2.3.1/ci/appveyor-bootstrap.py` & `erpbrasil.edoc-2.4.0/ci/appveyor-bootstrap.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/ci/appveyor-download.py` & `erpbrasil.edoc-2.4.0/ci/appveyor-download.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/ci/appveyor-with-compiler.cmd` & `erpbrasil.edoc-2.4.0/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/ci/bootstrap.py` & `erpbrasil.edoc-2.4.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/ci/templates/.appveyor.yml` & `erpbrasil.edoc-2.4.0/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/ci/templates/.travis.yml` & `erpbrasil.edoc-2.4.0/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/ci/templates/appveyor.yml` & `erpbrasil.edoc-2.4.0/ci/templates/appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/docs/conf.py` & `erpbrasil.edoc-2.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'erpbrasil.edoc'
 year = '2019'
 author = 'Luis Felipe Mileo'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '2.3.1'
+version = release = '2.4.0'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/erpbrasil/erpbrasil.edoc/issues/%s', '#'),
     'pr': ('https://github.com/erpbrasil/erpbrasil.edoc/pull/%s', 'PR #'),
 }
```

### Comparing `erpbrasil.edoc-2.3.1/setup.py` & `erpbrasil.edoc-2.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='erpbrasil.edoc',
-    version='2.3.1',
+    version='2.4.0',
     license='MIT',
     description='Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
     author='Luis Felipe Mileo',
```

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/chave.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/chave.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/cli.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/cli.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/edoc.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/edoc.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/mde.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/mde.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/mdfe.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/mdfe.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/nfce.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/nfce.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/nfe.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/nfe.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     AMBIENTE_PRODUCAO: {
         'servidor': 'www1.nfe.fazenda.gov.br',
         WS_DFE_DISTRIBUICAO: 'NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx?wsdl',
         WS_DOWNLOAD_NFE: 'NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx?wsdl',
         WS_NFE_RECEPCAO_EVENTO: 'NFeRecepcaoEvento4/NFeRecepcaoEvento4.asmx?wsdl',  # noqa
     },
     AMBIENTE_HOMOLOGACAO: {
-        'servidor': 'hom.nfe.fazenda.gov.br',
+        'servidor': 'hom1.nfe.fazenda.gov.br',
         WS_DFE_DISTRIBUICAO: 'NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx?wsdl',
         WS_DOWNLOAD_NFE: 'NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx?wsdl',
         WS_NFE_RECEPCAO_EVENTO: 'NFeRecepcaoEvento4/NFeRecepcaoEvento4.asmx?Wsdl',  # noqa
     },
 }
 
 UFAM = {
```

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/nfse.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/nfse.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/cidades.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/cidades.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from erpbrasil.edoc.provedores.issnet import Issnet
 from erpbrasil.edoc.provedores.paulistana import Paulistana
 
 cidades = {
     1501402: Dsf,  # Belem-PA
     2211001: Dsf,  # Teresina - PI
     3132404: Ginfes,  # ITAJUBA - MG
+    3516200: Ginfes,  # Franca - SP
     3170206: Dsf,  # Uberlândia-MG
     3303500: Dsf,  # Nova Iguaçu - RJ
     3509502: Dsf,  # Campinas - SP
     5002704: Dsf,  # Campo Grande - MS
     3550308: Paulistana,  # São Paulo - SP
     3543402: Issnet,    # Ribeirão Preto - SP
     3301702: Issnet,  # Duque de Caxias - RJ
```

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/dsf.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/dsf.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/ginfes.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/ginfes.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/issnet.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/issnet.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/provedores/paulistana.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/provedores/paulistana.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import xml.etree.ElementTree as ET
 
+from base64 import b64encode
 from erpbrasil.edoc.nfse import NFSe
 from erpbrasil.edoc.nfse import ServicoNFSe
 
 try:
     from erpbrasil.assinatura.assinatura import Assinatura
     from nfselib.paulistana.v02 import PedidoCancelamentoNFe
     from nfselib.paulistana.v02 import PedidoConsultaLote
@@ -69,20 +70,21 @@
         else:
             self._servicos = servicos_prod
 
         super(Paulistana, self).__init__(
             transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador)
 
     def _prepara_envia_documento(self, edoc):
+        assinador = Assinatura(self._transmissao.certificado)
         for rps in edoc.RPS:
-            rps.Assinatura = Assinatura(
-                self._transmissao.certificado).assina_tag(
-                rps.Assinatura)
+            data = rps.Assinatura
+            data_bytes = data.encode('ascii')
+            assinatura = assinador.sign_pkcs1v15_sha1(data_bytes)
+            rps.Assinatura = b64encode(assinatura).decode()
         xml_assinado = self.assina_raiz(edoc, '')
-
         return xml_assinado
 
     def _verifica_resposta_envio_sucesso(self, proc_envio):
         return proc_envio.resposta.Cabecalho.Sucesso
 
     def _edoc_situacao_em_processamento(self, proc_recibo):
         # if proc_recibo.resposta.Situacao == 2:
@@ -164,19 +166,20 @@
                     NumeroNFe=int(numero_nfse),
                     CodigoVerificacao=codigo_verificacao.zfill(8),
                 ),
                 AssinaturaCancelamento=assinatura,
             )],
         )
 
+        assinador = Assinatura(self._transmissao.certificado)
         for detalhe in raiz.Detalhe:
-            detalhe.AssinaturaCancelamento = Assinatura(
-                self._transmissao.certificado).assina_tag(
-                detalhe.AssinaturaCancelamento)
-
+            data = detalhe.AssinaturaCancelamento
+            data_bytes = data.encode('ascii')
+            assinatura = assinador.sign_pkcs1v15_sha1(data_bytes)
+            detalhe.AssinaturaCancelamento = b64encode(assinatura).decode()
         xml_assinado = self.assina_raiz(raiz, '')
         return xml_assinado
 
     def analisa_retorno_cancelamento_paulistana(self, processo):
         retorno_mensagem = ''
         status = True
         if not processo.resposta.Cabecalho.Sucesso:
@@ -188,8 +191,7 @@
 
     def assina_raiz(self, raiz, id, getchildren=False):
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
         xml_assinado = Assinatura(self._transmissao.certificado).assina_nfse(
             xml_etree
         )
         return xml_assinado
-        return xml_assinado.replace('\n', '').replace('\r', '')
```

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil/edoc/resposta.py` & `erpbrasil.edoc-2.4.0/src/erpbrasil/edoc/resposta.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/PKG-INFO` & `erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.3.1
+Version: 2.4.0
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
```

### Comparing `erpbrasil.edoc-2.3.1/src/erpbrasil.edoc.egg-info/SOURCES.txt` & `erpbrasil.edoc-2.4.0/src/erpbrasil.edoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/dummy_cert.pfx` & `erpbrasil.edoc-2.4.0/tests/fixtures/dummy_cert.pfx`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_chave.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_chave.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_envia_documento.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_status_servico.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml` & `erpbrasil.edoc-2.4.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc.py` & `erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_manifestacao.py` & `erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_manifestacao.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_nfse_ginfes.py` & `erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_nfse_ginfes.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_nfse_paulistana.py` & `erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_nfse_paulistana.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tests/test_erpbrasil_edoc_situacao.py` & `erpbrasil.edoc-2.4.0/tests/test_erpbrasil_edoc_situacao.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.3.1/tox.ini` & `erpbrasil.edoc-2.4.0/tox.ini`

 * *Files identical despite different names*

