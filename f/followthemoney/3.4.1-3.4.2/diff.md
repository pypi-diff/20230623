# Comparing `tmp/followthemoney-3.4.1.tar.gz` & `tmp/followthemoney-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.4.1.tar", last modified: Thu Jun 22 12:06:23 2023, max compression
+gzip compressed data, was "followthemoney-3.4.2.tar", last modified: Fri Jun 23 08:55:21 2023, max compression
```

## Comparing `followthemoney-3.4.1.tar` & `followthemoney-3.4.2.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.298807 followthemoney-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 12:04:20.000000 followthemoney-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-22 12:04:20.000000 followthemoney-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-22 12:06:23.298807 followthemoney-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-22 12:04:20.000000 followthemoney-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.282807 followthemoney-3.4.1/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.282807 followthemoney-3.4.1/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.286807 followthemoney-3.4.1/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.286807 followthemoney-3.4.1/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.290807 followthemoney-3.4.1/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.290807 followthemoney-3.4.1/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39021 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   110484 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36742 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   105691 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    32360 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   104328 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   109418 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)    99827 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    61028 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   131500 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.298807 followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.298807 followthemoney-3.4.1/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.282807 followthemoney-3.4.1/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:06:01.000000 followthemoney-3.4.1/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-22 12:06:23.298807 followthemoney-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-22 12:04:20.000000 followthemoney-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.825806 followthemoney-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-23 08:53:27.000000 followthemoney-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 08:53:27.000000 followthemoney-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-23 08:55:21.825806 followthemoney-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-23 08:53:27.000000 followthemoney-3.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.813806 followthemoney-3.4.2/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.817806 followthemoney-3.4.2/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.817806 followthemoney-3.4.2/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   118608 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112813 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112460 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   117244 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   100624 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    60112 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   131502 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.825806 followthemoney-3.4.2/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:55:01.000000 followthemoney-3.4.2/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-23 08:55:21.825806 followthemoney-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-23 08:53:27.000000 followthemoney-3.4.2/setup.py
```

### Comparing `followthemoney-3.4.1/LICENSE` & `followthemoney-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/PKG-INFO` & `followthemoney-3.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.1
+Version: 3.4.2
+Summary: UNKNOWN
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -84,7 +86,9 @@
 This will create a new patch release and upload a distribution of it. If
 the changes are more significant, you can run `bumpversion` with the `minor`
 or `major` arguments.
 
 When the schema is updated, please update the docs, ideally including the
 diagrams. For the RDF namespace and JavaScript version of the model, 
 run `make generate`.
+
+
```

### Comparing `followthemoney-3.4.1/README.md` & `followthemoney-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/cli/aggregate.py` & `followthemoney-3.4.2/followthemoney/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/cli/cli.py` & `followthemoney-3.4.2/followthemoney/cli/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/cli/exports.py` & `followthemoney-3.4.2/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/cli/mapping.py` & `followthemoney-3.4.2/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/cli/sieve.py` & `followthemoney-3.4.2/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/cli/util.py` & `followthemoney-3.4.2/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/compare.py` & `followthemoney-3.4.2/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/exc.py` & `followthemoney-3.4.2/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/export/common.py` & `followthemoney-3.4.2/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/export/csv.py` & `followthemoney-3.4.2/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/export/excel.py` & `followthemoney-3.4.2/followthemoney/export/excel.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/export/graph.py` & `followthemoney-3.4.2/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/export/neo4j.py` & `followthemoney-3.4.2/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/export/rdf.py` & `followthemoney-3.4.2/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/graph.py` & `followthemoney-3.4.2/followthemoney/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/helpers.py` & `followthemoney-3.4.2/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/mapping/csv.py` & `followthemoney-3.4.2/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/mapping/entity.py` & `followthemoney-3.4.2/followthemoney/mapping/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/mapping/property.py` & `followthemoney-3.4.2/followthemoney/mapping/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/mapping/query.py` & `followthemoney-3.4.2/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/mapping/source.py` & `followthemoney-3.4.2/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/mapping/sql.py` & `followthemoney-3.4.2/followthemoney/mapping/sql.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/messages.py` & `followthemoney-3.4.2/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/model.py` & `followthemoney-3.4.2/followthemoney/model.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/namespace.py` & `followthemoney-3.4.2/followthemoney/namespace.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/offshore.py` & `followthemoney-3.4.2/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/ontology.py` & `followthemoney-3.4.2/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/property.py` & `followthemoney-3.4.2/followthemoney/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/proxy.py` & `followthemoney-3.4.2/followthemoney/proxy.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Address.yaml` & `followthemoney-3.4.2/followthemoney/schema/Address.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Airplane.yaml` & `followthemoney-3.4.2/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.4.2/followthemoney/schema/Analyzable.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Assessment.yaml` & `followthemoney-3.4.2/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Associate.yaml` & `followthemoney-3.4.2/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.4.2/followthemoney/schema/BankAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Call.yaml` & `followthemoney-3.4.2/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.4.2/followthemoney/schema/CallForTenders.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Company.yaml` & `followthemoney-3.4.2/followthemoney/schema/Company.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Contract.yaml` & `followthemoney-3.4.2/followthemoney/schema/Contract.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.4.2/followthemoney/schema/ContractAward.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.4.2/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.4.2/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.4.2/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Debt.yaml` & `followthemoney-3.4.2/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Directorship.yaml` & `followthemoney-3.4.2/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Document.yaml` & `followthemoney-3.4.2/followthemoney/schema/Document.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -110,12 +110,12 @@
       hidden: true
     processingError:
       label: "Processing error"
       hidden: true
     processingAgent:
       label: "Name and version of the processing agent used to process the Document"
       type: string
-      hidden: true
     processedAt:
       label: "Date and time of the most recent ingestion of the Document"
       type: date
       matchable: false
+      hidden: true
```

### Comparing `followthemoney-3.4.1/followthemoney/schema/Documentation.yml` & `followthemoney-3.4.2/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.4.2/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Email.yaml` & `followthemoney-3.4.2/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Employment.yaml` & `followthemoney-3.4.2/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Event.yaml` & `followthemoney-3.4.2/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Family.yaml` & `followthemoney-3.4.2/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Identification.yaml` & `followthemoney-3.4.2/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Interval.yaml` & `followthemoney-3.4.2/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.4.2/followthemoney/schema/LegalEntity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Membership.yaml` & `followthemoney-3.4.2/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Mention.yaml` & `followthemoney-3.4.2/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Message.yaml` & `followthemoney-3.4.2/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Ownership.yaml` & `followthemoney-3.4.2/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Page.yaml` & `followthemoney-3.4.2/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Passport.yaml` & `followthemoney-3.4.2/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Payment.yaml` & `followthemoney-3.4.2/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Person.yaml` & `followthemoney-3.4.2/followthemoney/schema/Person.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Post.yaml` & `followthemoney-3.4.2/followthemoney/schema/Post.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.4.2/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.4.2/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Representation.yaml` & `followthemoney-3.4.2/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Sanction.yaml` & `followthemoney-3.4.2/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Security.yaml` & `followthemoney-3.4.2/followthemoney/schema/Security.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Similar.yaml` & `followthemoney-3.4.2/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Succession.yaml` & `followthemoney-3.4.2/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Table.yaml` & `followthemoney-3.4.2/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.4.2/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Thing.yaml` & `followthemoney-3.4.2/followthemoney/schema/Thing.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Trip.yaml` & `followthemoney-3.4.2/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.4.2/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.4.2/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.4.2/followthemoney/schema/Vehicle.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema/Vessel.yaml` & `followthemoney-3.4.2/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/schema.py` & `followthemoney-3.4.2/followthemoney/schema.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-06-27 13:42+0200\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
 "Language: ar\n"
-"Language-Team: Arabic (https://www.transifex.com/aleph/teams/76591/ar/)\n"
+"Language-Team: Arabic (https://app.transifex.com/aleph/teams/76591/ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "الرقم الضريبي (الاتحاد الأوروبي)"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "  (RO) ما هو نوع النشاط الذي يسمح للكيان القانوني بتطويره"
 
@@ -402,17 +402,14 @@
 
 msgid "Contract holder"
 msgstr "صاحب العقد"
 
 msgid "Contract procedure"
 msgstr "إجراءات العقد"
 
-msgid "Contract title"
-msgstr "عنوان العقد"
-
 msgid "Contracts"
 msgstr "العقود"
 
 msgid "Contracts awarded"
 msgstr "العقود الممنوحة"
 
 msgid "Contracts issued"
@@ -1323,17 +1320,14 @@
 
 msgid "Place of birth"
 msgstr "مكان الولادة"
 
 msgid "Political party"
 msgstr "حزب سياسي"
 
-msgid "Politician"
-msgstr "سياسي"
-
 msgid "Port of Registration"
 msgstr "ميناء التسجيل"
 
 msgid "Position"
 msgstr "الوضع"
 
 msgid "Predecessor"
@@ -1461,17 +1455,14 @@
 
 msgid "Role"
 msgstr "دور"
 
 msgid "Rouble bank"
 msgstr " بنك روبل"
 
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "مصنف الدول الروسية (ОКСМ)"
-
 msgid "Russian bank account code"
 msgstr "رمز الحساب المصرفي الروسي"
 
 msgid "Russian company ID"
 msgstr "معرف الشركة الروسية"
 
 msgid "Russian industry classifier"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Translations template for PROJECT.
-# Copyright (C) 2022 ORGANIZATION
+# Copyright (C) 2023 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 # 
 # Translators:
 # pudo <friedrich@pudo.org>, 2021
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-06-27 13:42+0200\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
-"Language-Team: Arabic (https://www.transifex.com/aleph/teams/76591/ar/)\n"
+"Language-Team: Arabic (https://app.transifex.com/aleph/teams/76591/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.12.1\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr "لا يمكن كتابة اسم الملكية"
 
@@ -40,19 +40,19 @@
 msgstr "ملكية غير معروفة (1%s):%s"
 
 #: followthemoney/proxy.py:188
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr "الملكية المتبقية%s:%s"
 
-#: followthemoney/schema.py:342
+#: followthemoney/schema.py:373
 msgid "Required"
 msgstr "مطلوب"
 
-#: followthemoney/schema.py:346
+#: followthemoney/schema.py:377
 msgid "Entity validation failed"
 msgstr "فشل التحقق من صحة الكيان"
 
 #. Address.label
 #. CryptoWallet.properties.publicKey.label
 #. Thing.properties.address.label
 #. Thing.properties.addressEntity.label
@@ -89,15 +89,15 @@
 #. Address.properties.postOfficeBox.label
 #: followthemoney/schema/Address.yaml
 msgid "PO Box"
 msgstr ""
 
 #. Address.properties.postOfficeBox.description
 #: followthemoney/schema/Address.yaml
-msgid "A mailbox indentifier at the post office"
+msgid "A mailbox identifier at the post office"
 msgstr ""
 
 #. Address.properties.street.label
 #: followthemoney/schema/Address.yaml
 msgid "Street address"
 msgstr ""
 
@@ -167,14 +167,24 @@
 #: followthemoney/schema/Address.yaml followthemoney/schema/Event.yaml
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml followthemoney/schema/TaxRoll.yaml
 #: followthemoney/schema/Thing.yaml followthemoney/types/country.py:21
 msgid "Country"
 msgstr "الدولة"
 
+#. Address.properties.osmId.label
+#: followthemoney/schema/Address.yaml
+msgid "OpenStreetmap Place ID"
+msgstr ""
+
+#. Address.properties.googlePlaceId.label
+#: followthemoney/schema/Address.yaml
+msgid "Google Places ID"
+msgstr ""
+
 #. Airplane.label
 #: followthemoney/schema/Airplane.yaml
 msgid "Airplane"
 msgstr "طائرة"
 
 #. Airplane.plural
 #: followthemoney/schema/Airplane.yaml
@@ -470,14 +480,24 @@
 msgstr "بنك"
 
 #. BankAccount.properties.accountType.label
 #: followthemoney/schema/BankAccount.yaml
 msgid "Account type"
 msgstr ""
 
+#. BankAccount.properties.openingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Opening date"
+msgstr ""
+
+#. BankAccount.properties.closingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Closing date"
+msgstr ""
+
 #. BankAccount.properties.balance.label
 #. CryptoWallet.properties.balance.label
 #: followthemoney/schema/BankAccount.yaml
 #: followthemoney/schema/CryptoWallet.yaml
 msgid "Balance"
 msgstr "رصيد حساب"
 
@@ -540,14 +560,237 @@
 msgstr "المكالمات المستلمة"
 
 #. Call.properties.receiverNumber.label
 #: followthemoney/schema/Call.yaml
 msgid "Receiver's Number"
 msgstr "رقم المستلم"
 
+#. CallForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders"
+msgstr ""
+
+#. CallForTenders.plural
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Calls for tenders"
+msgstr ""
+
+#. CallForTenders.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid ""
+"A public appeal issued by an authority, possibly on behalf of another, for "
+"buying a specific work, supply or service\n"
+msgstr ""
+
+#. CallForTenders.properties.callId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "CfT unique id"
+msgstr ""
+
+#. CallForTenders.properties.title.label
+#. Contract.properties.title.label
+#. Document.properties.title.label
+#. Person.properties.title.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/Contract.yaml followthemoney/schema/Document.yaml
+#: followthemoney/schema/Person.yaml
+msgid "Title"
+msgstr "عنوان"
+
+#. CallForTenders.properties.authority.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Name of contracting authority"
+msgstr ""
+
+#. CallForTenders.properties.authority.reverse.label
+#. ContractAward.properties.callForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "Call For Tenders"
+msgstr ""
+
+#. CallForTenders.properties.authorityReferenceId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contracting authority reference ID"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Published on behalf of"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Delegated call for tenders"
+msgstr ""
+
+#. CallForTenders.properties.publicationDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of publication/invitation"
+msgstr ""
+
+#. CallForTenders.properties.evaluationMechanism.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Evaluation mechanism"
+msgstr ""
+
+#. CallForTenders.properties.procurementType.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procurement type"
+msgstr ""
+
+#. CallForTenders.properties.directive.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Directive"
+msgstr ""
+
+#. CallForTenders.properties.procedure.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procedure"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders result"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "The nature of the contractual agreement that will result from this CfT"
+msgstr ""
+
+#. CallForTenders.properties.cpvCode.label
+#. ContractAward.properties.cpvCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "CPV code"
+msgstr "رمز الشراء العام"
+
+#. CallForTenders.properties.cpvCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Common Procurement Vocabulary (CPV)"
+msgstr ""
+
+#. CallForTenders.properties.reverseAuctionsIncluded.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Inclusion of e-Auctions"
+msgstr ""
+
+#. CallForTenders.properties.nutsCode.label
+#. ContractAward.properties.nutsCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "NUTS code"
+msgstr "رقم  الوحدات الإقليمية للإحصاءات"
+
+#. CallForTenders.properties.nutsCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Nomenclature of Territorial Units for Statistics (NUTS)"
+msgstr ""
+
+#. CallForTenders.properties.relationToThreshold.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Above or below threshold"
+msgstr ""
+
+#. CallForTenders.properties.paymentOptions.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Payment options"
+msgstr ""
+
+#. CallForTenders.properties.submissionDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Submission deadline"
+msgstr ""
+
+#. CallForTenders.properties.clarificationDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "End of clarification period"
+msgstr ""
+
+#. CallForTenders.properties.awardedInLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract awarded in Lots"
+msgstr ""
+
+#. CallForTenders.properties.numberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Number of lots"
+msgstr ""
+
+#. CallForTenders.properties.lotsNames.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Lots names"
+msgstr ""
+
+#. CallForTenders.properties.tendersForLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenders for lots"
+msgstr ""
+
+#. CallForTenders.properties.maximumNumberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Maximum number of lots"
+msgstr ""
+
+#. CallForTenders.properties.euFunding.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "EU funding"
+msgstr ""
+
+#. CallForTenders.properties.multipleTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Multiple tenders will be accepted"
+msgstr ""
+
+#. CallForTenders.properties.tedUrl.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "TED link for published notices"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Does this call fall under the scope of GPP?"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "European Green Public Procurement (GPP) or green purchasing."
+msgstr ""
+
+#. CallForTenders.properties.certificationCheck.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Certification check"
+msgstr ""
+
+#. CallForTenders.properties.awardingDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of awarding"
+msgstr ""
+
+#. CallForTenders.properties.contractNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract notice date"
+msgstr ""
+
+#. CallForTenders.properties.awardNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Award Notice Date"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenderers"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tender"
+msgstr ""
+
 #. Company.label
 #: followthemoney/schema/Company.yaml
 msgid "Company"
 msgstr "شركة"
 
 #. Company.plural
 #: followthemoney/schema/Company.yaml
@@ -568,17 +811,19 @@
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
 msgid "Jurisdiction"
 msgstr "سلطة القضاء"
 
 #. Company.properties.registrationNumber.label
 #. LegalEntity.properties.registrationNumber.label
 #. RealEstate.properties.registrationNumber.label
+#. Security.properties.registrationNumber.label
 #. Vehicle.properties.registrationNumber.label
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
-#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Vehicle.yaml
+#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Security.yaml
+#: followthemoney/schema/Vehicle.yaml
 msgid "Registration number"
 msgstr "رقم التسجيل"
 
 #. Company.properties.capital.label
 #: followthemoney/schema/Company.yaml
 msgid "Capital"
 msgstr "العاصمة"
@@ -594,14 +839,21 @@
 msgstr "معرّف دافع الضرائب ID في أذربيجان"
 
 #. Company.properties.coatoCode.label
 #: followthemoney/schema/Company.yaml
 msgid "COATO / SOATO / OKATO"
 msgstr "أوكاتو / أوكاتو / أوكاتو"
 
+#. Company.properties.coatoCode.description
+#: followthemoney/schema/Company.yaml
+msgid ""
+"Soviet classifier for territories, regions, districts, villages. Aka. SOATO "
+"and same as OKATO"
+msgstr ""
+
 #. Company.properties.irsCode.label
 #: followthemoney/schema/Company.yaml
 msgid "IRS Number"
 msgstr "رقم IRS"
 
 #. Company.properties.irsCode.description
 #: followthemoney/schema/Company.yaml
@@ -705,24 +957,14 @@
 msgstr "محاكي نظام حقل العمل FSS"
 
 #. Company.properties.fssCode.description
 #: followthemoney/schema/Company.yaml
 msgid "(RU, ФСС) Social Security"
 msgstr "(RU، ФСС) الضمان الاجتماعي"
 
-#. Company.properties.ogrnCode.label
-#: followthemoney/schema/Company.yaml
-msgid "OGRN"
-msgstr "يتم استخدام OGRN في السجل كرقم ملف تسجيل شركة"
-
-#. Company.properties.ogrnCode.description
-#: followthemoney/schema/Company.yaml
-msgid "Major State Registration Number"
-msgstr "رقم تسجيل الدولة"
-
 #. Company.properties.bikCode.label
 #: followthemoney/schema/Company.yaml
 msgid "BIK"
 msgstr "مكتب معلومات الائتمان"
 
 #. Company.properties.bikCode.description
 #: followthemoney/schema/Company.yaml
@@ -746,16 +988,34 @@
 #. Company.properties.oksmCode.label
 #: followthemoney/schema/Company.yaml
 msgid "OKSM"
 msgstr "OKSM"
 
 #. Company.properties.oksmCode.description
 #: followthemoney/schema/Company.yaml
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "مصنف الدول الروسية (ОКСМ)"
+msgid "Russian (ОКСМ) countries classifier"
+msgstr ""
+
+#. Company.properties.isinCode.label
+#. Security.properties.isin.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "ISIN"
+msgstr ""
+
+#. Company.properties.isinCode.description
+#. Security.properties.isin.description
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "International Securities Identification Number"
+msgstr ""
+
+#. Company.properties.ticker.label
+#. Security.properties.ticker.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "Stock ticker symbol"
+msgstr ""
 
 #. Contract.label
 #. ContractAward.properties.contract.label
 #. EconomicActivity.properties.contract.label
 #. Payment.properties.contract.label
 #: followthemoney/schema/Contract.yaml
 #: followthemoney/schema/ContractAward.yaml
@@ -777,19 +1037,14 @@
 msgid ""
 "An contract or contract lot issued by an authority. Multiple lots may be "
 "awarded to different suppliers (see ContractAward).\n"
 msgstr ""
 "عقد صادر عن سلطة. قد يتم منح عقود متعددة لموردين مختلفين (انظر إرساء "
 "العقد).\n"
 
-#. Contract.properties.title.label
-#: followthemoney/schema/Contract.yaml
-msgid "Contract title"
-msgstr "عنوان العقد"
-
 #. Contract.properties.authority.label
 #: followthemoney/schema/Contract.yaml
 msgid "Contract authority"
 msgstr "الجهة التي اصدرت العقد"
 
 #. Contract.properties.authority.plural
 #: followthemoney/schema/Contract.yaml
@@ -937,50 +1192,47 @@
 msgstr "العقود الممنوحة"
 
 #. ContractAward.properties.contract.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lots awarded"
 msgstr "الحصص / الأسهم الممنوحة"
 
+#. ContractAward.properties.callForTenders.reverse.label
+#: followthemoney/schema/ContractAward.yaml
+msgid "Contract Awards"
+msgstr ""
+
 #. ContractAward.properties.lotNumber.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lot number"
 msgstr "رقم الحصة"
 
 #. ContractAward.properties.documentNumber.label
+#. Identification.properties.number.label
 #: followthemoney/schema/ContractAward.yaml
+#: followthemoney/schema/Identification.yaml
 msgid "Document number"
 msgstr "رقم المستند"
 
 #. ContractAward.properties.documentType.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Document type"
 msgstr "نوع المستند"
 
 #. ContractAward.properties.decisionReason.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Decision reason"
 msgstr "سبب القرار"
 
-#. ContractAward.properties.cpvCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "CPV code"
-msgstr "رمز الشراء العام"
-
 #. ContractAward.properties.cpvCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Procurement Vocabulary (what type of goods/services, EU)"
 msgstr ""
 "مصطلحات العقرد والمشتريات (أي نوع من السلع / الخدمات ، الاتحاد الأوروبي)"
 
-#. ContractAward.properties.nutsCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "NUTS code"
-msgstr "رقم  الوحدات الإقليمية للإحصاءات"
-
 #. ContractAward.properties.nutsCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Nomencalture of Territorial Units for Statistics (NUTS)"
 msgstr "مصطلحات الوحدات الإقليمية للإحصاءات (NUTS)"
 
 #. ContractAward.properties.amended.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1163,17 +1415,18 @@
 #: followthemoney/schema/Directorship.yaml
 msgid "Director"
 msgstr "مخرج"
 
 #. Directorship.properties.organization.label
 #. Membership.properties.organization.label
 #. Organization.label
+#. Post.properties.organization.label
 #: followthemoney/schema/Directorship.yaml
 #: followthemoney/schema/Membership.yaml
-#: followthemoney/schema/Organization.yaml
+#: followthemoney/schema/Organization.yaml followthemoney/schema/Post.yaml
 msgid "Organization"
 msgstr "منظمة"
 
 #. Directorship.properties.organization.reverse.label
 #: followthemoney/schema/Directorship.yaml
 msgid "Directors"
 msgstr "المخرجون"
@@ -1199,20 +1452,14 @@
 msgstr "المجموع الاختباري"
 
 #. Document.properties.contentHash.description
 #: followthemoney/schema/Document.yaml
 msgid "SHA1 hash of the data"
 msgstr "تجزئة SHA1 للبيانات"
 
-#. Document.properties.title.label
-#. Person.properties.title.label
-#: followthemoney/schema/Document.yaml followthemoney/schema/Person.yaml
-msgid "Title"
-msgstr "عنوان"
-
 #. Document.properties.author.description
 #: followthemoney/schema/Document.yaml
 msgid "The original author, not the uploader"
 msgstr "المؤلف الأصلي ، وليس القائم بالتحميل"
 
 #. Document.properties.generator.label
 #: followthemoney/schema/Document.yaml
@@ -1337,14 +1584,24 @@
 msgstr "حالة المعالجة"
 
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr "حدث خطأ في المعالجة"
 
+#. Document.properties.processingAgent.label
+#: followthemoney/schema/Document.yaml
+msgid "Name and version of the processing agent used to process the Document"
+msgstr ""
+
+#. Document.properties.processedAt.label
+#: followthemoney/schema/Document.yaml
+msgid "Date and time of the most recent ingestion of the Document"
+msgstr ""
+
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr "توثيق"
 
 #. Documentation.plural
 #: followthemoney/schema/Documentation.yml
@@ -1469,22 +1726,14 @@
 #. EconomicActivity.properties.vedCodeDescription.description
 #: followthemoney/schema/EconomicActivity.yaml
 msgid ""
 "(Описание кода ТН ВЭД) Foreign Economic Activity Commodity Code description"
 msgstr "(Описание кода ТН ВЭД) وصف رمز النشاط الاقتصادي الأجنبي"
 
 #. EconomicActivity.properties.goodsDescription.label
-#. Interval.properties.description.label
-#. Thing.properties.description.label
-#: followthemoney/schema/EconomicActivity.yaml
-#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
-msgid "Description"
-msgstr "وصف"
-
-#. EconomicActivity.properties.goodsDescription.description
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Description of goods"
 msgstr "وصف البضائع"
 
 #. EconomicActivity.properties.declarant.label
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Declarant"
@@ -1935,22 +2184,14 @@
 msgstr ""
 
 #. Identification.properties.holder.label
 #: followthemoney/schema/Identification.yaml
 msgid "Identification holder"
 msgstr ""
 
-#. Identification.properties.number.label
-#. Passport.properties.passportNumber.label
-#. Person.properties.passportNumber.label
-#: followthemoney/schema/Identification.yaml
-#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
-msgid "Passport number"
-msgstr "رقم جواز السفر"
-
 #. Identification.properties.authority.label
 #. Sanction.properties.authority.label
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml
 msgid "Authority"
 msgstr "سلطة"
 
@@ -2007,14 +2248,20 @@
 
 #. Interval.properties.summary.label
 #. Thing.properties.summary.label
 #: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
 msgid "Summary"
 msgstr "ملخص"
 
+#. Interval.properties.description.label
+#. Thing.properties.description.label
+#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
+msgid "Description"
+msgstr "وصف"
+
 #. Interval.properties.recordId.label
 #: followthemoney/schema/Interval.yaml
 msgid "Record ID"
 msgstr "رقم التسجيل"
 
 #. Interval.properties.sourceUrl.label
 #. Thing.properties.sourceUrl.label
@@ -2219,14 +2466,24 @@
 msgstr "النزل"
 
 #. LegalEntity.properties.innCode.description
 #: followthemoney/schema/LegalEntity.yaml
 msgid "Russian company ID"
 msgstr "معرف الشركة الروسية"
 
+#. LegalEntity.properties.ogrnCode.label
+#: followthemoney/schema/LegalEntity.yaml
+msgid "OGRN"
+msgstr "يتم استخدام OGRN في السجل كرقم ملف تسجيل شركة"
+
+#. LegalEntity.properties.ogrnCode.description
+#: followthemoney/schema/LegalEntity.yaml
+msgid "Major State Registration Number"
+msgstr "رقم تسجيل الدولة"
+
 #. LegalEntity.properties.leiCode.label
 #: followthemoney/schema/LegalEntity.yaml
 msgid "LEI"
 msgstr ""
 
 #. LegalEntity.properties.leiCode.description
 #: followthemoney/schema/LegalEntity.yaml
@@ -2354,15 +2611,15 @@
 #: followthemoney/schema/Mention.yaml
 msgid "Document mentions"
 msgstr "مستندات تم ذكرها"
 
 #. Mention.properties.name.label
 #. Thing.properties.name.label
 #: followthemoney/schema/Mention.yaml followthemoney/schema/Thing.yaml
-#: followthemoney/types/name.py:26
+#: followthemoney/types/name.py:25
 msgid "Name"
 msgstr "الاسم"
 
 #. Mention.properties.detectedSchema.label
 #: followthemoney/schema/Mention.yaml
 msgid "Detected entity type"
 msgstr "نوع الكيان المكتشف"
@@ -2447,15 +2704,15 @@
 msgstr "منظمات"
 
 #. Organization.description
 #: followthemoney/schema/Organization.yaml
 msgid ""
 "Any type of incorporated entity that cannot be owned by another (see "
 "Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
+"enterprises, depending on their  jurisdiction.\n"
 msgstr ""
 
 #. Ownership.label
 #: followthemoney/schema/Ownership.yaml
 msgid "Ownership"
 msgstr "ملكية"
 
@@ -2578,14 +2835,20 @@
 msgstr "جوازات السفر"
 
 #. Passport.description
 #: followthemoney/schema/Passport.yaml
 msgid "An passport held by a person.\n"
 msgstr ""
 
+#. Passport.properties.passportNumber.label
+#. Person.properties.passportNumber.label
+#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
+msgid "Passport number"
+msgstr "رقم جواز السفر"
+
 #. Passport.properties.surname.label
 #. TaxRoll.properties.surname.label
 #: followthemoney/schema/Passport.yaml followthemoney/schema/TaxRoll.yaml
 msgid "Surname"
 msgstr "إسم العائلة"
 
 #. Passport.properties.givenName.label
@@ -2789,14 +3052,48 @@
 msgstr "الملفات النصية"
 
 #. PlainText.description
 #: followthemoney/schema/PlainText.yaml
 msgid "Text files, like .txt or source code.\n"
 msgstr ""
 
+#. Post.label
+#: followthemoney/schema/Post.yaml
+msgid "Post"
+msgstr ""
+
+#. Post.plural
+#: followthemoney/schema/Post.yaml
+msgid "Posts"
+msgstr ""
+
+#. Post.description
+#: followthemoney/schema/Post.yaml
+msgid ""
+"A post, role or position held by an individual within an organization  or "
+"body. This describes the period for which the position is held, not the "
+"abstract concept of the post.\n"
+msgstr ""
+
+#. Post.properties.holder.label
+#: followthemoney/schema/Post.yaml
+msgid "Holder"
+msgstr ""
+
+#. Post.properties.holder.reverse.label
+#: followthemoney/schema/Post.yaml
+msgid "Posts held"
+msgstr ""
+
+#. Post.properties.wikidataId.label
+#. Thing.properties.wikidataId.label
+#: followthemoney/schema/Post.yaml followthemoney/schema/Thing.yaml
+msgid "Wikidata ID"
+msgstr "معرف Wikidata"
+
 #. Project.plural
 #. ProjectParticipant.properties.participant.reverse.label
 #: followthemoney/schema/Project.yaml
 #: followthemoney/schema/ProjectParticipant.yaml
 msgid "Projects"
 msgstr ""
 
@@ -3027,29 +3324,14 @@
 msgstr ""
 
 #. Security.description
 #: followthemoney/schema/Security.yaml
 msgid "A tradeable financial asset."
 msgstr ""
 
-#. Security.properties.isin.label
-#: followthemoney/schema/Security.yaml
-msgid "ISIN"
-msgstr ""
-
-#. Security.properties.isin.description
-#: followthemoney/schema/Security.yaml
-msgid "International Securities Identification Number"
-msgstr ""
-
-#. Security.properties.ticker.label
-#: followthemoney/schema/Security.yaml
-msgid "Ticker"
-msgstr ""
-
 #. Security.properties.issuer.label
 #: followthemoney/schema/Security.yaml
 msgid "Issuer"
 msgstr ""
 
 #. Security.properties.issuer.reverse.label
 #: followthemoney/schema/Security.yaml
@@ -3057,14 +3339,19 @@
 msgstr ""
 
 #. Security.properties.issueDate.label
 #: followthemoney/schema/Security.yaml
 msgid "Date issued"
 msgstr ""
 
+#. Security.properties.maturityDate.label
+#: followthemoney/schema/Security.yaml
+msgid "Maturity date"
+msgstr ""
+
 #. Security.properties.collateral.label
 #: followthemoney/schema/Security.yaml
 msgid "Collateral"
 msgstr ""
 
 #. Similar.label
 #: followthemoney/schema/Similar.yaml
@@ -3242,19 +3529,14 @@
 msgstr "اسم مستعار ضعيف"
 
 #. Thing.properties.wikipediaUrl.label
 #: followthemoney/schema/Thing.yaml
 msgid "Wikipedia Article"
 msgstr "مقالة ويكيبيديا"
 
-#. Thing.properties.wikidataId.label
-#: followthemoney/schema/Thing.yaml
-msgid "Wikidata ID"
-msgstr "معرف Wikidata"
-
 #. Thing.properties.keywords.label
 #: followthemoney/schema/Thing.yaml
 msgid "Keywords"
 msgstr "الكلمات المفتاحية"
 
 #. Thing.properties.topics.label
 #: followthemoney/schema/Thing.yaml followthemoney/types/topic.py:22
@@ -3375,14 +3657,19 @@
 msgstr "اسم المستخدم"
 
 #. UserAccount.properties.password.label
 #: followthemoney/schema/UserAccount.yaml
 msgid "Password"
 msgstr "كلمة المرور"
 
+#. UserAccount.properties.ipAddress.label
+#: followthemoney/schema/UserAccount.yaml
+msgid "IP address"
+msgstr ""
+
 #. Value.label
 #: followthemoney/schema/Value.yaml
 msgid "Value"
 msgstr "قيمة"
 
 #. Value.plural
 #: followthemoney/schema/Value.yaml
@@ -3724,15 +4011,15 @@
 msgid "MIME-Type"
 msgstr "يشير MIME إلى \"ملحقات بريد إنترنت متعدد الأغراض"
 
 #: followthemoney/types/mimetype.py:25
 msgid "MIME-Types"
 msgstr "أنواع  بريد إنترنت متعدد الأغراض"
 
-#: followthemoney/types/name.py:27
+#: followthemoney/types/name.py:26
 msgid "Names"
 msgstr "أسماء"
 
 #: followthemoney/types/number.py:18
 msgid "Number"
 msgstr "رقم"
 
@@ -3849,16 +4136,16 @@
 msgstr "الأموال"
 
 #: followthemoney/types/topic.py:48
 msgid "Financial advisor"
 msgstr "مستشار مالي"
 
 #: followthemoney/types/topic.py:49
-msgid "Politician"
-msgstr "سياسي"
+msgid "Political"
+msgstr ""
 
 #: followthemoney/types/topic.py:50
 msgid "Close Associate"
 msgstr ""
 
 #: followthemoney/types/topic.py:51
 msgid "Judge"
@@ -3913,18 +4200,22 @@
 msgstr "أصول مجمدة"
 
 #: followthemoney/types/topic.py:65
 msgid "Sanctioned entity"
 msgstr "كيان خاضع للعقوبات"
 
 #: followthemoney/types/topic.py:66
-msgid "Debarred entity"
+msgid "Sanction-linked entity"
 msgstr ""
 
 #: followthemoney/types/topic.py:67
+msgid "Debarred entity"
+msgstr ""
+
+#: followthemoney/types/topic.py:68
 msgid "Person of interest"
 msgstr "الشخص المعني"
 
 #: followthemoney/types/url.py:22
 msgid "URL"
 msgstr "عنوان URL"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: bs\n"
 "Language-Team: Bosnian (https://www.transifex.com/aleph/teams/76591/bs/)\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) VAT broj"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Koji tip aktivnosti legalnog entiteta je dozvoljeno razviti"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-09-28 10:51+0200\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
 "Language: de\n"
-"Language-Team: German (https://www.transifex.com/aleph/teams/76591/de/)\n"
+"Language-Team: German (https://app.transifex.com/aleph/teams/76591/de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) USt-ID"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr ""
 "(RO) Die Art der wirtschaftlichen Tätigkeit, der diese Entität nachgehen darf"
@@ -69,17 +69,14 @@
 
 msgid "A grant of land, rights or property. A type of Contract"
 msgstr "Eine Übertragung von Land, Rechten oder Eigentum"
 
 msgid "A location associated with an entity.\n"
 msgstr "Ein Ort, der mit einer Entität zusammenhängt.\n"
 
-msgid "A mailbox indentifier at the post office"
-msgstr "Eine Postfachnummer bei einer Filiale"
-
 msgid ""
 "A mediatory, intermediary, middleman, or broker acting on behalf of a legal "
 "entity."
 msgstr "Ein Unterhändler oder Broker der im Auftrag einer Rechtsperson handelt"
 
 msgid "A monetary debt between two parties."
 msgstr "Eine Geldschuld zwischen zwei Parteien."
@@ -225,23 +222,14 @@
 
 msgid "Analyzables"
 msgstr "Analysierbare"
 
 msgid "Ancestors"
 msgstr "Ahnen"
 
-msgid ""
-"Any type of incorporated entity that cannot be owned by another (see "
-"Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
-msgstr ""
-"Juristische Personen, die nicht Eigentum einer anderen Person sein können "
-"(siehe Firma). Dies umfasst Stiftungen, Staatsunternehmen und Vereine, je "
-"nach ihrem Sitz.\n"
-
 msgid "Area"
 msgstr "Fläche"
 
 msgid "Article"
 msgstr "Artikel"
 
 msgid "Articles"
@@ -513,17 +501,14 @@
 
 msgid "Contract holder"
 msgstr "Vertragseigner"
 
 msgid "Contract procedure"
 msgstr "Vertragsprozedur"
 
-msgid "Contract title"
-msgstr "Vertragstitel"
-
 msgid "Contracts"
 msgstr "Verträge"
 
 msgid "Contracts awarded"
 msgstr "Vergebene Verträge"
 
 msgid "Contracts issued"
@@ -1501,17 +1486,14 @@
 
 msgid "Political association"
 msgstr "Politische Zugehörigkeit"
 
 msgid "Political party"
 msgstr "Politische Partei"
 
-msgid "Politician"
-msgstr "Politiker"
-
 msgid "Port of Registration"
 msgstr "Anmeldehafen"
 
 msgid "Position"
 msgstr "Stellung"
 
 msgid "Postal code"
@@ -1672,17 +1654,14 @@
 
 msgid "Role"
 msgstr "Rolle"
 
 msgid "Rouble bank"
 msgstr "Rubel-Bank"
 
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Russische Landeskennzeichung (OKCM)"
-
 msgid "Russian bank account code"
 msgstr "Russische Kontonummer"
 
 msgid "Russian company ID"
 msgstr "Russische Firmennummer"
 
 msgid "Russian industry classifier"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Translations template for PROJECT.
-# Copyright (C) 2022 ORGANIZATION
+# Copyright (C) 2023 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 # 
 # Translators:
 # pudo <friedrich@pudo.org>, 2021
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-09-28 10:51+0200\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
-"Language-Team: German (https://www.transifex.com/aleph/teams/76591/de/)\n"
+"Language-Team: German (https://app.transifex.com/aleph/teams/76591/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr "Eigenschaft darf nicht direkt gesetzt werden"
 
@@ -40,19 +40,19 @@
 msgstr "Unbekannte Eigenschaft (%s): %s"
 
 #: followthemoney/proxy.py:188
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr "Pseudofeld (%s): %s"
 
-#: followthemoney/schema.py:342
+#: followthemoney/schema.py:373
 msgid "Required"
 msgstr "Erforderlich"
 
-#: followthemoney/schema.py:346
+#: followthemoney/schema.py:377
 msgid "Entity validation failed"
 msgstr "Prüfung fehlgeschlagen"
 
 #. Address.label
 #. CryptoWallet.properties.publicKey.label
 #. Thing.properties.address.label
 #. Thing.properties.addressEntity.label
@@ -89,16 +89,16 @@
 #. Address.properties.postOfficeBox.label
 #: followthemoney/schema/Address.yaml
 msgid "PO Box"
 msgstr "Postfach"
 
 #. Address.properties.postOfficeBox.description
 #: followthemoney/schema/Address.yaml
-msgid "A mailbox indentifier at the post office"
-msgstr "Eine Postfachnummer bei einer Filiale"
+msgid "A mailbox identifier at the post office"
+msgstr ""
 
 #. Address.properties.street.label
 #: followthemoney/schema/Address.yaml
 msgid "Street address"
 msgstr "Straße"
 
 #. Address.properties.street2.label
@@ -167,14 +167,24 @@
 #: followthemoney/schema/Address.yaml followthemoney/schema/Event.yaml
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml followthemoney/schema/TaxRoll.yaml
 #: followthemoney/schema/Thing.yaml followthemoney/types/country.py:21
 msgid "Country"
 msgstr "Land"
 
+#. Address.properties.osmId.label
+#: followthemoney/schema/Address.yaml
+msgid "OpenStreetmap Place ID"
+msgstr ""
+
+#. Address.properties.googlePlaceId.label
+#: followthemoney/schema/Address.yaml
+msgid "Google Places ID"
+msgstr ""
+
 #. Airplane.label
 #: followthemoney/schema/Airplane.yaml
 msgid "Airplane"
 msgstr "Flugzeug"
 
 #. Airplane.plural
 #: followthemoney/schema/Airplane.yaml
@@ -473,14 +483,24 @@
 msgstr "Bank"
 
 #. BankAccount.properties.accountType.label
 #: followthemoney/schema/BankAccount.yaml
 msgid "Account type"
 msgstr "Kontenart"
 
+#. BankAccount.properties.openingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Opening date"
+msgstr ""
+
+#. BankAccount.properties.closingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Closing date"
+msgstr ""
+
 #. BankAccount.properties.balance.label
 #. CryptoWallet.properties.balance.label
 #: followthemoney/schema/BankAccount.yaml
 #: followthemoney/schema/CryptoWallet.yaml
 msgid "Balance"
 msgstr "Kontostand"
 
@@ -543,14 +563,237 @@
 msgstr "Empfangene Anrufe"
 
 #. Call.properties.receiverNumber.label
 #: followthemoney/schema/Call.yaml
 msgid "Receiver's Number"
 msgstr "Empfängernummer"
 
+#. CallForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders"
+msgstr ""
+
+#. CallForTenders.plural
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Calls for tenders"
+msgstr ""
+
+#. CallForTenders.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid ""
+"A public appeal issued by an authority, possibly on behalf of another, for "
+"buying a specific work, supply or service\n"
+msgstr ""
+
+#. CallForTenders.properties.callId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "CfT unique id"
+msgstr ""
+
+#. CallForTenders.properties.title.label
+#. Contract.properties.title.label
+#. Document.properties.title.label
+#. Person.properties.title.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/Contract.yaml followthemoney/schema/Document.yaml
+#: followthemoney/schema/Person.yaml
+msgid "Title"
+msgstr "TItel"
+
+#. CallForTenders.properties.authority.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Name of contracting authority"
+msgstr ""
+
+#. CallForTenders.properties.authority.reverse.label
+#. ContractAward.properties.callForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "Call For Tenders"
+msgstr ""
+
+#. CallForTenders.properties.authorityReferenceId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contracting authority reference ID"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Published on behalf of"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Delegated call for tenders"
+msgstr ""
+
+#. CallForTenders.properties.publicationDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of publication/invitation"
+msgstr ""
+
+#. CallForTenders.properties.evaluationMechanism.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Evaluation mechanism"
+msgstr ""
+
+#. CallForTenders.properties.procurementType.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procurement type"
+msgstr ""
+
+#. CallForTenders.properties.directive.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Directive"
+msgstr ""
+
+#. CallForTenders.properties.procedure.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procedure"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders result"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "The nature of the contractual agreement that will result from this CfT"
+msgstr ""
+
+#. CallForTenders.properties.cpvCode.label
+#. ContractAward.properties.cpvCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "CPV code"
+msgstr "CPV-Code"
+
+#. CallForTenders.properties.cpvCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Common Procurement Vocabulary (CPV)"
+msgstr ""
+
+#. CallForTenders.properties.reverseAuctionsIncluded.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Inclusion of e-Auctions"
+msgstr ""
+
+#. CallForTenders.properties.nutsCode.label
+#. ContractAward.properties.nutsCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "NUTS code"
+msgstr "NUTS-Code"
+
+#. CallForTenders.properties.nutsCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Nomenclature of Territorial Units for Statistics (NUTS)"
+msgstr ""
+
+#. CallForTenders.properties.relationToThreshold.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Above or below threshold"
+msgstr ""
+
+#. CallForTenders.properties.paymentOptions.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Payment options"
+msgstr ""
+
+#. CallForTenders.properties.submissionDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Submission deadline"
+msgstr ""
+
+#. CallForTenders.properties.clarificationDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "End of clarification period"
+msgstr ""
+
+#. CallForTenders.properties.awardedInLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract awarded in Lots"
+msgstr ""
+
+#. CallForTenders.properties.numberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Number of lots"
+msgstr ""
+
+#. CallForTenders.properties.lotsNames.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Lots names"
+msgstr ""
+
+#. CallForTenders.properties.tendersForLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenders for lots"
+msgstr ""
+
+#. CallForTenders.properties.maximumNumberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Maximum number of lots"
+msgstr ""
+
+#. CallForTenders.properties.euFunding.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "EU funding"
+msgstr ""
+
+#. CallForTenders.properties.multipleTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Multiple tenders will be accepted"
+msgstr ""
+
+#. CallForTenders.properties.tedUrl.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "TED link for published notices"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Does this call fall under the scope of GPP?"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "European Green Public Procurement (GPP) or green purchasing."
+msgstr ""
+
+#. CallForTenders.properties.certificationCheck.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Certification check"
+msgstr ""
+
+#. CallForTenders.properties.awardingDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of awarding"
+msgstr ""
+
+#. CallForTenders.properties.contractNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract notice date"
+msgstr ""
+
+#. CallForTenders.properties.awardNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Award Notice Date"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenderers"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tender"
+msgstr ""
+
 #. Company.label
 #: followthemoney/schema/Company.yaml
 msgid "Company"
 msgstr "Firma"
 
 #. Company.plural
 #: followthemoney/schema/Company.yaml
@@ -571,17 +814,19 @@
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
 msgid "Jurisdiction"
 msgstr "Rechtsprechung"
 
 #. Company.properties.registrationNumber.label
 #. LegalEntity.properties.registrationNumber.label
 #. RealEstate.properties.registrationNumber.label
+#. Security.properties.registrationNumber.label
 #. Vehicle.properties.registrationNumber.label
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
-#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Vehicle.yaml
+#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Security.yaml
+#: followthemoney/schema/Vehicle.yaml
 msgid "Registration number"
 msgstr "Registrierungsnummer"
 
 #. Company.properties.capital.label
 #: followthemoney/schema/Company.yaml
 msgid "Capital"
 msgstr "Vermögen"
@@ -597,14 +842,21 @@
 msgstr "Azerbaidschanische Steuernummer"
 
 #. Company.properties.coatoCode.label
 #: followthemoney/schema/Company.yaml
 msgid "COATO / SOATO / OKATO"
 msgstr "COATO / SOATO / OKATO"
 
+#. Company.properties.coatoCode.description
+#: followthemoney/schema/Company.yaml
+msgid ""
+"Soviet classifier for territories, regions, districts, villages. Aka. SOATO "
+"and same as OKATO"
+msgstr ""
+
 #. Company.properties.irsCode.label
 #: followthemoney/schema/Company.yaml
 msgid "IRS Number"
 msgstr "IRS-Nummer"
 
 #. Company.properties.irsCode.description
 #: followthemoney/schema/Company.yaml
@@ -736,16 +988,34 @@
 #. Company.properties.oksmCode.label
 #: followthemoney/schema/Company.yaml
 msgid "OKSM"
 msgstr "OKSM"
 
 #. Company.properties.oksmCode.description
 #: followthemoney/schema/Company.yaml
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Russische Landeskennzeichung (OKCM)"
+msgid "Russian (ОКСМ) countries classifier"
+msgstr ""
+
+#. Company.properties.isinCode.label
+#. Security.properties.isin.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "ISIN"
+msgstr ""
+
+#. Company.properties.isinCode.description
+#. Security.properties.isin.description
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "International Securities Identification Number"
+msgstr ""
+
+#. Company.properties.ticker.label
+#. Security.properties.ticker.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "Stock ticker symbol"
+msgstr ""
 
 #. Contract.label
 #. ContractAward.properties.contract.label
 #. EconomicActivity.properties.contract.label
 #. Payment.properties.contract.label
 #: followthemoney/schema/Contract.yaml
 #: followthemoney/schema/ContractAward.yaml
@@ -767,19 +1037,14 @@
 msgid ""
 "An contract or contract lot issued by an authority. Multiple lots may be "
 "awarded to different suppliers (see ContractAward).\n"
 msgstr ""
 "Ein Vertrag oder Teilvertrag einer öffentlichen Stelle der an mehrere "
 "Lieferanten vergeben sein kann (siehe Zuschlag)\n"
 
-#. Contract.properties.title.label
-#: followthemoney/schema/Contract.yaml
-msgid "Contract title"
-msgstr "Vertragstitel"
-
 #. Contract.properties.authority.label
 #: followthemoney/schema/Contract.yaml
 msgid "Contract authority"
 msgstr "Vergabestelle"
 
 #. Contract.properties.authority.plural
 #: followthemoney/schema/Contract.yaml
@@ -925,49 +1190,46 @@
 msgstr "Vergebene Verträge"
 
 #. ContractAward.properties.contract.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lots awarded"
 msgstr "Erteilte Zuschläge"
 
+#. ContractAward.properties.callForTenders.reverse.label
+#: followthemoney/schema/ContractAward.yaml
+msgid "Contract Awards"
+msgstr ""
+
 #. ContractAward.properties.lotNumber.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lot number"
 msgstr "Zuschlagsnummer"
 
 #. ContractAward.properties.documentNumber.label
+#. Identification.properties.number.label
 #: followthemoney/schema/ContractAward.yaml
+#: followthemoney/schema/Identification.yaml
 msgid "Document number"
 msgstr "Dokumentennummer"
 
 #. ContractAward.properties.documentType.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Document type"
 msgstr "Dokumentenart"
 
 #. ContractAward.properties.decisionReason.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Decision reason"
 msgstr "Entscheidungsgrund"
 
-#. ContractAward.properties.cpvCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "CPV code"
-msgstr "CPV-Code"
-
 #. ContractAward.properties.cpvCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Procurement Vocabulary (what type of goods/services, EU)"
 msgstr "Gemeinsames Vergabevokabular (Art der Dienstleistung oder des Gutes)"
 
-#. ContractAward.properties.nutsCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "NUTS code"
-msgstr "NUTS-Code"
-
 #. ContractAward.properties.nutsCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Nomencalture of Territorial Units for Statistics (NUTS)"
 msgstr "Nomenklatur der Einheiten Territorialer Statistik (NUTS)"
 
 #. ContractAward.properties.amended.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1188,20 +1450,14 @@
 msgstr "Prüfsumme"
 
 #. Document.properties.contentHash.description
 #: followthemoney/schema/Document.yaml
 msgid "SHA1 hash of the data"
 msgstr "SHA1--Summe dieser Datei"
 
-#. Document.properties.title.label
-#. Person.properties.title.label
-#: followthemoney/schema/Document.yaml followthemoney/schema/Person.yaml
-msgid "Title"
-msgstr "TItel"
-
 #. Document.properties.author.description
 #: followthemoney/schema/Document.yaml
 msgid "The original author, not the uploader"
 msgstr "Der ursprüngliche Autor"
 
 #. Document.properties.generator.label
 #: followthemoney/schema/Document.yaml
@@ -1326,14 +1582,24 @@
 msgstr "Verarbeitungsstatus"
 
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr "Verarbeitungsfehler"
 
+#. Document.properties.processingAgent.label
+#: followthemoney/schema/Document.yaml
+msgid "Name and version of the processing agent used to process the Document"
+msgstr ""
+
+#. Document.properties.processedAt.label
+#: followthemoney/schema/Document.yaml
+msgid "Date and time of the most recent ingestion of the Document"
+msgstr ""
+
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr "Dokumentation"
 
 #. Documentation.plural
 #: followthemoney/schema/Documentation.yml
@@ -1461,22 +1727,14 @@
 #: followthemoney/schema/EconomicActivity.yaml
 msgid ""
 "(Описание кода ТН ВЭД) Foreign Economic Activity Commodity Code description"
 msgstr ""
 "(Описание кода ТН ВЭД) Foreign Economic Activity Commodity Code description"
 
 #. EconomicActivity.properties.goodsDescription.label
-#. Interval.properties.description.label
-#. Thing.properties.description.label
-#: followthemoney/schema/EconomicActivity.yaml
-#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
-msgid "Description"
-msgstr "Beschreibung"
-
-#. EconomicActivity.properties.goodsDescription.description
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Description of goods"
 msgstr "Beschreibung der Güter"
 
 #. EconomicActivity.properties.declarant.label
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Declarant"
@@ -1929,22 +2187,14 @@
 msgstr ""
 
 #. Identification.properties.holder.label
 #: followthemoney/schema/Identification.yaml
 msgid "Identification holder"
 msgstr ""
 
-#. Identification.properties.number.label
-#. Passport.properties.passportNumber.label
-#. Person.properties.passportNumber.label
-#: followthemoney/schema/Identification.yaml
-#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
-msgid "Passport number"
-msgstr "Passnummer"
-
 #. Identification.properties.authority.label
 #. Sanction.properties.authority.label
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml
 msgid "Authority"
 msgstr "Behörde"
 
@@ -2001,14 +2251,20 @@
 
 #. Interval.properties.summary.label
 #. Thing.properties.summary.label
 #: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
 msgid "Summary"
 msgstr "Zusammenfassung"
 
+#. Interval.properties.description.label
+#. Thing.properties.description.label
+#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
+msgid "Description"
+msgstr "Beschreibung"
+
 #. Interval.properties.recordId.label
 #: followthemoney/schema/Interval.yaml
 msgid "Record ID"
 msgstr "Eintrags-ID"
 
 #. Interval.properties.sourceUrl.label
 #. Thing.properties.sourceUrl.label
@@ -2445,19 +2701,16 @@
 msgstr "Organisationen"
 
 #. Organization.description
 #: followthemoney/schema/Organization.yaml
 msgid ""
 "Any type of incorporated entity that cannot be owned by another (see "
 "Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
+"enterprises, depending on their  jurisdiction.\n"
 msgstr ""
-"Juristische Personen, die nicht Eigentum einer anderen Person sein können "
-"(siehe Firma). Dies umfasst Stiftungen, Staatsunternehmen und Vereine, je "
-"nach ihrem Sitz.\n"
 
 #. Ownership.label
 #: followthemoney/schema/Ownership.yaml
 msgid "Ownership"
 msgstr "Eigentum"
 
 #. Ownership.plural
@@ -2581,14 +2834,20 @@
 msgstr "Reisepässe"
 
 #. Passport.description
 #: followthemoney/schema/Passport.yaml
 msgid "An passport held by a person.\n"
 msgstr ""
 
+#. Passport.properties.passportNumber.label
+#. Person.properties.passportNumber.label
+#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
+msgid "Passport number"
+msgstr "Passnummer"
+
 #. Passport.properties.surname.label
 #. TaxRoll.properties.surname.label
 #: followthemoney/schema/Passport.yaml followthemoney/schema/TaxRoll.yaml
 msgid "Surname"
 msgstr "Nachname"
 
 #. Passport.properties.givenName.label
@@ -2822,17 +3081,18 @@
 
 #. Post.properties.holder.reverse.label
 #: followthemoney/schema/Post.yaml
 msgid "Posts held"
 msgstr ""
 
 #. Post.properties.wikidataId.label
-#: followthemoney/schema/Post.yaml
-msgid "Wikidata ID of the post"
-msgstr ""
+#. Thing.properties.wikidataId.label
+#: followthemoney/schema/Post.yaml followthemoney/schema/Thing.yaml
+msgid "Wikidata ID"
+msgstr "Wikidata-ID"
 
 #. Project.plural
 #. ProjectParticipant.properties.participant.reverse.label
 #: followthemoney/schema/Project.yaml
 #: followthemoney/schema/ProjectParticipant.yaml
 msgid "Projects"
 msgstr "Projekte"
@@ -3067,29 +3327,14 @@
 msgstr ""
 
 #. Security.description
 #: followthemoney/schema/Security.yaml
 msgid "A tradeable financial asset."
 msgstr ""
 
-#. Security.properties.isin.label
-#: followthemoney/schema/Security.yaml
-msgid "ISIN"
-msgstr ""
-
-#. Security.properties.isin.description
-#: followthemoney/schema/Security.yaml
-msgid "International Securities Identification Number"
-msgstr ""
-
-#. Security.properties.ticker.label
-#: followthemoney/schema/Security.yaml
-msgid "Ticker"
-msgstr ""
-
 #. Security.properties.issuer.label
 #: followthemoney/schema/Security.yaml
 msgid "Issuer"
 msgstr ""
 
 #. Security.properties.issuer.reverse.label
 #: followthemoney/schema/Security.yaml
@@ -3097,14 +3342,19 @@
 msgstr ""
 
 #. Security.properties.issueDate.label
 #: followthemoney/schema/Security.yaml
 msgid "Date issued"
 msgstr ""
 
+#. Security.properties.maturityDate.label
+#: followthemoney/schema/Security.yaml
+msgid "Maturity date"
+msgstr ""
+
 #. Security.properties.collateral.label
 #: followthemoney/schema/Security.yaml
 msgid "Collateral"
 msgstr ""
 
 #. Similar.label
 #: followthemoney/schema/Similar.yaml
@@ -3284,19 +3534,14 @@
 msgstr "Umgangsname"
 
 #. Thing.properties.wikipediaUrl.label
 #: followthemoney/schema/Thing.yaml
 msgid "Wikipedia Article"
 msgstr "Wikipedia-Artikel"
 
-#. Thing.properties.wikidataId.label
-#: followthemoney/schema/Thing.yaml
-msgid "Wikidata ID"
-msgstr "Wikidata-ID"
-
 #. Thing.properties.keywords.label
 #: followthemoney/schema/Thing.yaml
 msgid "Keywords"
 msgstr "Schlüsselworte"
 
 #. Thing.properties.topics.label
 #: followthemoney/schema/Thing.yaml followthemoney/types/topic.py:22
@@ -3417,14 +3662,19 @@
 msgstr "Benuztername"
 
 #. UserAccount.properties.password.label
 #: followthemoney/schema/UserAccount.yaml
 msgid "Password"
 msgstr "Passwort"
 
+#. UserAccount.properties.ipAddress.label
+#: followthemoney/schema/UserAccount.yaml
+msgid "IP address"
+msgstr ""
+
 #. Value.label
 #: followthemoney/schema/Value.yaml
 msgid "Value"
 msgstr "Wert"
 
 #. Value.plural
 #: followthemoney/schema/Value.yaml
@@ -3893,16 +4143,16 @@
 msgstr "Fonds"
 
 #: followthemoney/types/topic.py:48
 msgid "Financial advisor"
 msgstr "Finanzberater"
 
 #: followthemoney/types/topic.py:49
-msgid "Politician"
-msgstr "Politiker"
+msgid "Political"
+msgstr ""
 
 #: followthemoney/types/topic.py:50
 msgid "Close Associate"
 msgstr ""
 
 #: followthemoney/types/topic.py:51
 msgid "Judge"
@@ -3957,18 +4207,22 @@
 msgstr "Gesperrte Guthaben"
 
 #: followthemoney/types/topic.py:65
 msgid "Sanctioned entity"
 msgstr "Sanktionierte Entität"
 
 #: followthemoney/types/topic.py:66
-msgid "Debarred entity"
+msgid "Sanction-linked entity"
 msgstr ""
 
 #: followthemoney/types/topic.py:67
+msgid "Debarred entity"
+msgstr ""
+
+#: followthemoney/types/topic.py:68
 msgid "Person of interest"
 msgstr "Zielperson"
 
 #: followthemoney/types/url.py:22
 msgid "URL"
 msgstr "URL"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-06-27 13:42+0200\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
 "Language: es\n"
-"Language-Team: Spanish (https://www.transifex.com/aleph/teams/76591/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/aleph/teams/76591/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) Número VAT"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr ""
 "(RO) ¿Qué tipo de actividad se le permite desarrollar a una entidad legal?"
@@ -400,17 +400,14 @@
 
 msgid "Contract holder"
 msgstr "Titular del contrato"
 
 msgid "Contract procedure"
 msgstr "Procedimiento contractual"
 
-msgid "Contract title"
-msgstr "Título del contrato"
-
 msgid "Contracts"
 msgstr "Contratos"
 
 msgid "Contracts awarded"
 msgstr "Contratos adjudicados"
 
 msgid "Contracts issued"
@@ -1299,17 +1296,14 @@
 
 msgid "Place of birth"
 msgstr "Lugar de nacimiento"
 
 msgid "Political party"
 msgstr "Partido político"
 
-msgid "Politician"
-msgstr "Político"
-
 msgid "Port of Registration"
 msgstr "Puerto de registro"
 
 msgid "Position"
 msgstr "Cargo"
 
 msgid "Predecessor"
@@ -1438,17 +1432,14 @@
 
 msgid "Role"
 msgstr "Papel"
 
 msgid "Rouble bank"
 msgstr "Banco de rublos"
 
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Clasificador de países ruso (ОКСМ)"
-
 msgid "Russian bank account code"
 msgstr "Código de cuenta bancaria rusa"
 
 msgid "Russian company ID"
 msgstr "Identificador de empresa rusa"
 
 msgid "Russian industry classifier"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Translations template for PROJECT.
-# Copyright (C) 2022 ORGANIZATION
+# Copyright (C) 2023 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 # 
 # Translators:
 # pudo <friedrich@pudo.org>, 2021
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-06-27 13:42+0200\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
-"Language-Team: Spanish (https://www.transifex.com/aleph/teams/76591/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/aleph/teams/76591/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.12.1\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr "No se puede escribir la propiedad"
 
@@ -40,19 +40,19 @@
 msgstr "Propiedad desconocida (%s): %s"
 
 #: followthemoney/proxy.py:188
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr "Propiedad Stub (%s): %s"
 
-#: followthemoney/schema.py:342
+#: followthemoney/schema.py:373
 msgid "Required"
 msgstr "Obligatorio"
 
-#: followthemoney/schema.py:346
+#: followthemoney/schema.py:377
 msgid "Entity validation failed"
 msgstr "Error en la validación de la propiedad"
 
 #. Address.label
 #. CryptoWallet.properties.publicKey.label
 #. Thing.properties.address.label
 #. Thing.properties.addressEntity.label
@@ -89,15 +89,15 @@
 #. Address.properties.postOfficeBox.label
 #: followthemoney/schema/Address.yaml
 msgid "PO Box"
 msgstr ""
 
 #. Address.properties.postOfficeBox.description
 #: followthemoney/schema/Address.yaml
-msgid "A mailbox indentifier at the post office"
+msgid "A mailbox identifier at the post office"
 msgstr ""
 
 #. Address.properties.street.label
 #: followthemoney/schema/Address.yaml
 msgid "Street address"
 msgstr ""
 
@@ -167,14 +167,24 @@
 #: followthemoney/schema/Address.yaml followthemoney/schema/Event.yaml
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml followthemoney/schema/TaxRoll.yaml
 #: followthemoney/schema/Thing.yaml followthemoney/types/country.py:21
 msgid "Country"
 msgstr "País"
 
+#. Address.properties.osmId.label
+#: followthemoney/schema/Address.yaml
+msgid "OpenStreetmap Place ID"
+msgstr ""
+
+#. Address.properties.googlePlaceId.label
+#: followthemoney/schema/Address.yaml
+msgid "Google Places ID"
+msgstr ""
+
 #. Airplane.label
 #: followthemoney/schema/Airplane.yaml
 msgid "Airplane"
 msgstr "Aeronave"
 
 #. Airplane.plural
 #: followthemoney/schema/Airplane.yaml
@@ -470,14 +480,24 @@
 msgstr "Banco"
 
 #. BankAccount.properties.accountType.label
 #: followthemoney/schema/BankAccount.yaml
 msgid "Account type"
 msgstr ""
 
+#. BankAccount.properties.openingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Opening date"
+msgstr ""
+
+#. BankAccount.properties.closingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Closing date"
+msgstr ""
+
 #. BankAccount.properties.balance.label
 #. CryptoWallet.properties.balance.label
 #: followthemoney/schema/BankAccount.yaml
 #: followthemoney/schema/CryptoWallet.yaml
 msgid "Balance"
 msgstr "Saldo"
 
@@ -540,14 +560,237 @@
 msgstr "Llamadas recibidas"
 
 #. Call.properties.receiverNumber.label
 #: followthemoney/schema/Call.yaml
 msgid "Receiver's Number"
 msgstr "Número del receptor"
 
+#. CallForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders"
+msgstr ""
+
+#. CallForTenders.plural
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Calls for tenders"
+msgstr ""
+
+#. CallForTenders.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid ""
+"A public appeal issued by an authority, possibly on behalf of another, for "
+"buying a specific work, supply or service\n"
+msgstr ""
+
+#. CallForTenders.properties.callId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "CfT unique id"
+msgstr ""
+
+#. CallForTenders.properties.title.label
+#. Contract.properties.title.label
+#. Document.properties.title.label
+#. Person.properties.title.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/Contract.yaml followthemoney/schema/Document.yaml
+#: followthemoney/schema/Person.yaml
+msgid "Title"
+msgstr "Título"
+
+#. CallForTenders.properties.authority.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Name of contracting authority"
+msgstr ""
+
+#. CallForTenders.properties.authority.reverse.label
+#. ContractAward.properties.callForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "Call For Tenders"
+msgstr ""
+
+#. CallForTenders.properties.authorityReferenceId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contracting authority reference ID"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Published on behalf of"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Delegated call for tenders"
+msgstr ""
+
+#. CallForTenders.properties.publicationDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of publication/invitation"
+msgstr ""
+
+#. CallForTenders.properties.evaluationMechanism.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Evaluation mechanism"
+msgstr ""
+
+#. CallForTenders.properties.procurementType.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procurement type"
+msgstr ""
+
+#. CallForTenders.properties.directive.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Directive"
+msgstr ""
+
+#. CallForTenders.properties.procedure.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procedure"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders result"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "The nature of the contractual agreement that will result from this CfT"
+msgstr ""
+
+#. CallForTenders.properties.cpvCode.label
+#. ContractAward.properties.cpvCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "CPV code"
+msgstr "Código CPV"
+
+#. CallForTenders.properties.cpvCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Common Procurement Vocabulary (CPV)"
+msgstr ""
+
+#. CallForTenders.properties.reverseAuctionsIncluded.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Inclusion of e-Auctions"
+msgstr ""
+
+#. CallForTenders.properties.nutsCode.label
+#. ContractAward.properties.nutsCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "NUTS code"
+msgstr "Código NUTS"
+
+#. CallForTenders.properties.nutsCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Nomenclature of Territorial Units for Statistics (NUTS)"
+msgstr ""
+
+#. CallForTenders.properties.relationToThreshold.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Above or below threshold"
+msgstr ""
+
+#. CallForTenders.properties.paymentOptions.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Payment options"
+msgstr ""
+
+#. CallForTenders.properties.submissionDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Submission deadline"
+msgstr ""
+
+#. CallForTenders.properties.clarificationDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "End of clarification period"
+msgstr ""
+
+#. CallForTenders.properties.awardedInLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract awarded in Lots"
+msgstr ""
+
+#. CallForTenders.properties.numberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Number of lots"
+msgstr ""
+
+#. CallForTenders.properties.lotsNames.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Lots names"
+msgstr ""
+
+#. CallForTenders.properties.tendersForLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenders for lots"
+msgstr ""
+
+#. CallForTenders.properties.maximumNumberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Maximum number of lots"
+msgstr ""
+
+#. CallForTenders.properties.euFunding.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "EU funding"
+msgstr ""
+
+#. CallForTenders.properties.multipleTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Multiple tenders will be accepted"
+msgstr ""
+
+#. CallForTenders.properties.tedUrl.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "TED link for published notices"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Does this call fall under the scope of GPP?"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "European Green Public Procurement (GPP) or green purchasing."
+msgstr ""
+
+#. CallForTenders.properties.certificationCheck.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Certification check"
+msgstr ""
+
+#. CallForTenders.properties.awardingDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of awarding"
+msgstr ""
+
+#. CallForTenders.properties.contractNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract notice date"
+msgstr ""
+
+#. CallForTenders.properties.awardNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Award Notice Date"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenderers"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tender"
+msgstr ""
+
 #. Company.label
 #: followthemoney/schema/Company.yaml
 msgid "Company"
 msgstr "Empresa"
 
 #. Company.plural
 #: followthemoney/schema/Company.yaml
@@ -568,17 +811,19 @@
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
 msgid "Jurisdiction"
 msgstr "Jurisdicción"
 
 #. Company.properties.registrationNumber.label
 #. LegalEntity.properties.registrationNumber.label
 #. RealEstate.properties.registrationNumber.label
+#. Security.properties.registrationNumber.label
 #. Vehicle.properties.registrationNumber.label
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
-#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Vehicle.yaml
+#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Security.yaml
+#: followthemoney/schema/Vehicle.yaml
 msgid "Registration number"
 msgstr "Número de registro"
 
 #. Company.properties.capital.label
 #: followthemoney/schema/Company.yaml
 msgid "Capital"
 msgstr "Capital"
@@ -594,14 +839,21 @@
 msgstr "Identificación fiscal de Azerbaiyán"
 
 #. Company.properties.coatoCode.label
 #: followthemoney/schema/Company.yaml
 msgid "COATO / SOATO / OKATO"
 msgstr "COATO / SOATO / OKATO"
 
+#. Company.properties.coatoCode.description
+#: followthemoney/schema/Company.yaml
+msgid ""
+"Soviet classifier for territories, regions, districts, villages. Aka. SOATO "
+"and same as OKATO"
+msgstr ""
+
 #. Company.properties.irsCode.label
 #: followthemoney/schema/Company.yaml
 msgid "IRS Number"
 msgstr "Número de IRS"
 
 #. Company.properties.irsCode.description
 #: followthemoney/schema/Company.yaml
@@ -705,27 +957,14 @@
 msgstr "FSS"
 
 #. Company.properties.fssCode.description
 #: followthemoney/schema/Company.yaml
 msgid "(RU, ФСС) Social Security"
 msgstr "(RU, ФСС) Seguridad Social"
 
-#. Company.properties.ogrnCode.label
-#: followthemoney/schema/Company.yaml
-msgid "OGRN"
-msgstr ""
-"OGRN - Número Principal de Registro del Estado de la inscripción realizada "
-"en el Registro sobre la formación de una empresa rusa - consta de 12 dígitos"
-" -"
-
-#. Company.properties.ogrnCode.description
-#: followthemoney/schema/Company.yaml
-msgid "Major State Registration Number"
-msgstr "Número Principal de Registro del Estado"
-
 #. Company.properties.bikCode.label
 #: followthemoney/schema/Company.yaml
 msgid "BIK"
 msgstr "BIK"
 
 #. Company.properties.bikCode.description
 #: followthemoney/schema/Company.yaml
@@ -750,16 +989,34 @@
 #. Company.properties.oksmCode.label
 #: followthemoney/schema/Company.yaml
 msgid "OKSM"
 msgstr "OKSM"
 
 #. Company.properties.oksmCode.description
 #: followthemoney/schema/Company.yaml
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Clasificador de países ruso (ОКСМ)"
+msgid "Russian (ОКСМ) countries classifier"
+msgstr ""
+
+#. Company.properties.isinCode.label
+#. Security.properties.isin.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "ISIN"
+msgstr ""
+
+#. Company.properties.isinCode.description
+#. Security.properties.isin.description
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "International Securities Identification Number"
+msgstr ""
+
+#. Company.properties.ticker.label
+#. Security.properties.ticker.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "Stock ticker symbol"
+msgstr ""
 
 #. Contract.label
 #. ContractAward.properties.contract.label
 #. EconomicActivity.properties.contract.label
 #. Payment.properties.contract.label
 #: followthemoney/schema/Contract.yaml
 #: followthemoney/schema/ContractAward.yaml
@@ -781,19 +1038,14 @@
 msgid ""
 "An contract or contract lot issued by an authority. Multiple lots may be "
 "awarded to different suppliers (see ContractAward).\n"
 msgstr ""
 "Un contrato o lote de contratos emitido por una autoridad. Se pueden "
 "adjudicar varios lotes a varios proveedores (ver ContractAward).\n"
 
-#. Contract.properties.title.label
-#: followthemoney/schema/Contract.yaml
-msgid "Contract title"
-msgstr "Título del contrato"
-
 #. Contract.properties.authority.label
 #: followthemoney/schema/Contract.yaml
 msgid "Contract authority"
 msgstr "Autoridad contractual"
 
 #. Contract.properties.authority.plural
 #: followthemoney/schema/Contract.yaml
@@ -940,50 +1192,47 @@
 msgstr "Contratos adjudicados"
 
 #. ContractAward.properties.contract.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lots awarded"
 msgstr "Lotes adjudicados"
 
+#. ContractAward.properties.callForTenders.reverse.label
+#: followthemoney/schema/ContractAward.yaml
+msgid "Contract Awards"
+msgstr ""
+
 #. ContractAward.properties.lotNumber.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lot number"
 msgstr "Número de lote"
 
 #. ContractAward.properties.documentNumber.label
+#. Identification.properties.number.label
 #: followthemoney/schema/ContractAward.yaml
+#: followthemoney/schema/Identification.yaml
 msgid "Document number"
 msgstr "Número de documento"
 
 #. ContractAward.properties.documentType.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Document type"
 msgstr "Tipo de documento"
 
 #. ContractAward.properties.decisionReason.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Decision reason"
 msgstr "Motivo de la decisión"
 
-#. ContractAward.properties.cpvCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "CPV code"
-msgstr "Código CPV"
-
 #. ContractAward.properties.cpvCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Procurement Vocabulary (what type of goods/services, EU)"
 msgstr ""
 "Vocabulario de procura en contratos (qué tipo de bienes/servicios, UE)"
 
-#. ContractAward.properties.nutsCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "NUTS code"
-msgstr "Código NUTS"
-
 #. ContractAward.properties.nutsCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Nomencalture of Territorial Units for Statistics (NUTS)"
 msgstr "Nomenclatura de Unidades Territoriales para Estadística (NUTS)"
 
 #. ContractAward.properties.amended.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1168,17 +1417,18 @@
 #: followthemoney/schema/Directorship.yaml
 msgid "Director"
 msgstr "Director"
 
 #. Directorship.properties.organization.label
 #. Membership.properties.organization.label
 #. Organization.label
+#. Post.properties.organization.label
 #: followthemoney/schema/Directorship.yaml
 #: followthemoney/schema/Membership.yaml
-#: followthemoney/schema/Organization.yaml
+#: followthemoney/schema/Organization.yaml followthemoney/schema/Post.yaml
 msgid "Organization"
 msgstr "Organización"
 
 #. Directorship.properties.organization.reverse.label
 #: followthemoney/schema/Directorship.yaml
 msgid "Directors"
 msgstr "Directores"
@@ -1204,20 +1454,14 @@
 msgstr "Comprobación"
 
 #. Document.properties.contentHash.description
 #: followthemoney/schema/Document.yaml
 msgid "SHA1 hash of the data"
 msgstr "Hash SHA1 de los datos"
 
-#. Document.properties.title.label
-#. Person.properties.title.label
-#: followthemoney/schema/Document.yaml followthemoney/schema/Person.yaml
-msgid "Title"
-msgstr "Título"
-
 #. Document.properties.author.description
 #: followthemoney/schema/Document.yaml
 msgid "The original author, not the uploader"
 msgstr "El autor original, no quien subió el archivo"
 
 #. Document.properties.generator.label
 #: followthemoney/schema/Document.yaml
@@ -1343,14 +1587,24 @@
 msgstr "Estado de procesamiento"
 
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr "Error de procesamiento"
 
+#. Document.properties.processingAgent.label
+#: followthemoney/schema/Document.yaml
+msgid "Name and version of the processing agent used to process the Document"
+msgstr ""
+
+#. Document.properties.processedAt.label
+#: followthemoney/schema/Document.yaml
+msgid "Date and time of the most recent ingestion of the Document"
+msgstr ""
+
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr "Documentación"
 
 #. Documentation.plural
 #: followthemoney/schema/Documentation.yml
@@ -1478,22 +1732,14 @@
 msgid ""
 "(Описание кода ТН ВЭД) Foreign Economic Activity Commodity Code description"
 msgstr ""
 "(Описание кода ТН ВЭД) Descripción del código de productos básicos de "
 "actividad económica exterior"
 
 #. EconomicActivity.properties.goodsDescription.label
-#. Interval.properties.description.label
-#. Thing.properties.description.label
-#: followthemoney/schema/EconomicActivity.yaml
-#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
-msgid "Description"
-msgstr "Descripción"
-
-#. EconomicActivity.properties.goodsDescription.description
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Description of goods"
 msgstr "Descripción de los bienes"
 
 #. EconomicActivity.properties.declarant.label
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Declarant"
@@ -1946,22 +2192,14 @@
 msgstr ""
 
 #. Identification.properties.holder.label
 #: followthemoney/schema/Identification.yaml
 msgid "Identification holder"
 msgstr ""
 
-#. Identification.properties.number.label
-#. Passport.properties.passportNumber.label
-#. Person.properties.passportNumber.label
-#: followthemoney/schema/Identification.yaml
-#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
-msgid "Passport number"
-msgstr "Número de pasaporte"
-
 #. Identification.properties.authority.label
 #. Sanction.properties.authority.label
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml
 msgid "Authority"
 msgstr "Autoridad"
 
@@ -2018,14 +2256,20 @@
 
 #. Interval.properties.summary.label
 #. Thing.properties.summary.label
 #: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
 msgid "Summary"
 msgstr "Resumen"
 
+#. Interval.properties.description.label
+#. Thing.properties.description.label
+#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
+msgid "Description"
+msgstr "Descripción"
+
 #. Interval.properties.recordId.label
 #: followthemoney/schema/Interval.yaml
 msgid "Record ID"
 msgstr "Identificador del registro"
 
 #. Interval.properties.sourceUrl.label
 #. Thing.properties.sourceUrl.label
@@ -2232,14 +2476,27 @@
 msgstr "INN"
 
 #. LegalEntity.properties.innCode.description
 #: followthemoney/schema/LegalEntity.yaml
 msgid "Russian company ID"
 msgstr "Identificador de empresa rusa"
 
+#. LegalEntity.properties.ogrnCode.label
+#: followthemoney/schema/LegalEntity.yaml
+msgid "OGRN"
+msgstr ""
+"OGRN - Número Principal de Registro del Estado de la inscripción realizada "
+"en el Registro sobre la formación de una empresa rusa - consta de 12 dígitos"
+" -"
+
+#. LegalEntity.properties.ogrnCode.description
+#: followthemoney/schema/LegalEntity.yaml
+msgid "Major State Registration Number"
+msgstr "Número Principal de Registro del Estado"
+
 #. LegalEntity.properties.leiCode.label
 #: followthemoney/schema/LegalEntity.yaml
 msgid "LEI"
 msgstr ""
 
 #. LegalEntity.properties.leiCode.description
 #: followthemoney/schema/LegalEntity.yaml
@@ -2361,15 +2618,15 @@
 #: followthemoney/schema/Mention.yaml
 msgid "Document mentions"
 msgstr ""
 
 #. Mention.properties.name.label
 #. Thing.properties.name.label
 #: followthemoney/schema/Mention.yaml followthemoney/schema/Thing.yaml
-#: followthemoney/types/name.py:26
+#: followthemoney/types/name.py:25
 msgid "Name"
 msgstr "Nombre"
 
 #. Mention.properties.detectedSchema.label
 #: followthemoney/schema/Mention.yaml
 msgid "Detected entity type"
 msgstr ""
@@ -2454,15 +2711,15 @@
 msgstr "Organizaciones"
 
 #. Organization.description
 #: followthemoney/schema/Organization.yaml
 msgid ""
 "Any type of incorporated entity that cannot be owned by another (see "
 "Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
+"enterprises, depending on their  jurisdiction.\n"
 msgstr ""
 
 #. Ownership.label
 #: followthemoney/schema/Ownership.yaml
 msgid "Ownership"
 msgstr "Propiedad"
 
@@ -2585,14 +2842,20 @@
 msgstr "Pasaportes"
 
 #. Passport.description
 #: followthemoney/schema/Passport.yaml
 msgid "An passport held by a person.\n"
 msgstr ""
 
+#. Passport.properties.passportNumber.label
+#. Person.properties.passportNumber.label
+#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
+msgid "Passport number"
+msgstr "Número de pasaporte"
+
 #. Passport.properties.surname.label
 #. TaxRoll.properties.surname.label
 #: followthemoney/schema/Passport.yaml followthemoney/schema/TaxRoll.yaml
 msgid "Surname"
 msgstr "Apellido"
 
 #. Passport.properties.givenName.label
@@ -2797,14 +3060,48 @@
 msgstr "Archivos de texto"
 
 #. PlainText.description
 #: followthemoney/schema/PlainText.yaml
 msgid "Text files, like .txt or source code.\n"
 msgstr ""
 
+#. Post.label
+#: followthemoney/schema/Post.yaml
+msgid "Post"
+msgstr ""
+
+#. Post.plural
+#: followthemoney/schema/Post.yaml
+msgid "Posts"
+msgstr ""
+
+#. Post.description
+#: followthemoney/schema/Post.yaml
+msgid ""
+"A post, role or position held by an individual within an organization  or "
+"body. This describes the period for which the position is held, not the "
+"abstract concept of the post.\n"
+msgstr ""
+
+#. Post.properties.holder.label
+#: followthemoney/schema/Post.yaml
+msgid "Holder"
+msgstr ""
+
+#. Post.properties.holder.reverse.label
+#: followthemoney/schema/Post.yaml
+msgid "Posts held"
+msgstr ""
+
+#. Post.properties.wikidataId.label
+#. Thing.properties.wikidataId.label
+#: followthemoney/schema/Post.yaml followthemoney/schema/Thing.yaml
+msgid "Wikidata ID"
+msgstr "Identificación de Wikidata"
+
 #. Project.plural
 #. ProjectParticipant.properties.participant.reverse.label
 #: followthemoney/schema/Project.yaml
 #: followthemoney/schema/ProjectParticipant.yaml
 msgid "Projects"
 msgstr ""
 
@@ -3038,29 +3335,14 @@
 msgstr ""
 
 #. Security.description
 #: followthemoney/schema/Security.yaml
 msgid "A tradeable financial asset."
 msgstr ""
 
-#. Security.properties.isin.label
-#: followthemoney/schema/Security.yaml
-msgid "ISIN"
-msgstr ""
-
-#. Security.properties.isin.description
-#: followthemoney/schema/Security.yaml
-msgid "International Securities Identification Number"
-msgstr ""
-
-#. Security.properties.ticker.label
-#: followthemoney/schema/Security.yaml
-msgid "Ticker"
-msgstr ""
-
 #. Security.properties.issuer.label
 #: followthemoney/schema/Security.yaml
 msgid "Issuer"
 msgstr ""
 
 #. Security.properties.issuer.reverse.label
 #: followthemoney/schema/Security.yaml
@@ -3068,14 +3350,19 @@
 msgstr ""
 
 #. Security.properties.issueDate.label
 #: followthemoney/schema/Security.yaml
 msgid "Date issued"
 msgstr ""
 
+#. Security.properties.maturityDate.label
+#: followthemoney/schema/Security.yaml
+msgid "Maturity date"
+msgstr ""
+
 #. Security.properties.collateral.label
 #: followthemoney/schema/Security.yaml
 msgid "Collateral"
 msgstr ""
 
 #. Similar.label
 #: followthemoney/schema/Similar.yaml
@@ -3253,19 +3540,14 @@
 msgstr "Weak alias"
 
 #. Thing.properties.wikipediaUrl.label
 #: followthemoney/schema/Thing.yaml
 msgid "Wikipedia Article"
 msgstr "Artículo en Wikipedia"
 
-#. Thing.properties.wikidataId.label
-#: followthemoney/schema/Thing.yaml
-msgid "Wikidata ID"
-msgstr "Identificación de Wikidata"
-
 #. Thing.properties.keywords.label
 #: followthemoney/schema/Thing.yaml
 msgid "Keywords"
 msgstr "Palarbas clave"
 
 #. Thing.properties.topics.label
 #: followthemoney/schema/Thing.yaml followthemoney/types/topic.py:22
@@ -3386,14 +3668,19 @@
 msgstr "Nombre de usuario"
 
 #. UserAccount.properties.password.label
 #: followthemoney/schema/UserAccount.yaml
 msgid "Password"
 msgstr "Contraseña"
 
+#. UserAccount.properties.ipAddress.label
+#: followthemoney/schema/UserAccount.yaml
+msgid "IP address"
+msgstr ""
+
 #. Value.label
 #: followthemoney/schema/Value.yaml
 msgid "Value"
 msgstr "Valor"
 
 #. Value.plural
 #: followthemoney/schema/Value.yaml
@@ -3735,15 +4022,15 @@
 msgid "MIME-Type"
 msgstr "Tipo de MIME"
 
 #: followthemoney/types/mimetype.py:25
 msgid "MIME-Types"
 msgstr "Tipos de MIME"
 
-#: followthemoney/types/name.py:27
+#: followthemoney/types/name.py:26
 msgid "Names"
 msgstr "Nombres"
 
 #: followthemoney/types/number.py:18
 msgid "Number"
 msgstr "Número"
 
@@ -3860,16 +4147,16 @@
 msgstr "Fondo"
 
 #: followthemoney/types/topic.py:48
 msgid "Financial advisor"
 msgstr "Asesor financiero"
 
 #: followthemoney/types/topic.py:49
-msgid "Politician"
-msgstr "Político"
+msgid "Political"
+msgstr ""
 
 #: followthemoney/types/topic.py:50
 msgid "Close Associate"
 msgstr ""
 
 #: followthemoney/types/topic.py:51
 msgid "Judge"
@@ -3924,18 +4211,22 @@
 msgstr "Activo congelado"
 
 #: followthemoney/types/topic.py:65
 msgid "Sanctioned entity"
 msgstr "Entidad sancionada"
 
 #: followthemoney/types/topic.py:66
-msgid "Debarred entity"
+msgid "Sanction-linked entity"
 msgstr ""
 
 #: followthemoney/types/topic.py:67
+msgid "Debarred entity"
+msgstr ""
+
+#: followthemoney/types/topic.py:68
 msgid "Person of interest"
 msgstr "Persona de interés"
 
 #: followthemoney/types/url.py:22
 msgid "URL"
 msgstr "URL"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-06-27 13:42+0200\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: Jean-Philippe Menotti, 2022\n"
 "Language: fr\n"
-"Language-Team: French (https://www.transifex.com/aleph/teams/76591/fr/)\n"
+"Language-Team: French (https://app.transifex.com/aleph/teams/76591/fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "Numéro de TVA intracommunautaire"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Type d’activité qu’une entité légale est autorisée à mener"
 
@@ -106,17 +106,14 @@
 msgstr ""
 "Une concession de terrain, de droits ou de bien immobilier. Un type de "
 "contrat"
 
 msgid "A location associated with an entity.\n"
 msgstr "Un emplacement associé à une entité.\n"
 
-msgid "A mailbox indentifier at the post office"
-msgstr "Identifiant de boîte au bureau de poste"
-
 msgid ""
 "A mediatory, intermediary, middleman, or broker acting on behalf of a legal "
 "entity."
 msgstr ""
 "Un médiateur, intermédiaire, négociateur ou courtier qui agit au nom d’une "
 "entité juridique."
 
@@ -301,23 +298,14 @@
 "if something is a person or company.\n"
 msgstr ""
 "Toute partie à une procédure juridique, telle que la propriété d’un actif, "
 "la gouvernance d’entreprise ou les interactions sociales. Catégorie souvent "
 "utilisée quand les données brutes ne précisent pas si quelque chose est une "
 "personne ou une entreprise.\n"
 
-msgid ""
-"Any type of incorporated entity that cannot be owned by another (see "
-"Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
-msgstr ""
-"Tout type d’entité constituée qui ne peut être détenue par une autre (voir "
-"Société). Il peut s’agir d’une organisation caritative, d’une fondation ou "
-"d’une entreprise détenue par un État, en fonction de sa juridiction.\n"
-
 msgid "Area"
 msgstr "Surface"
 
 msgid "Article"
 msgstr "Article"
 
 msgid "Articles"
@@ -602,17 +590,14 @@
 
 msgid "Contract holder"
 msgstr "Titulaire du contrat"
 
 msgid "Contract procedure"
 msgstr "Procédure du contrat"
 
-msgid "Contract title"
-msgstr "Titre du contrat"
-
 msgid "Contracts"
 msgstr "Contrats"
 
 msgid "Contracts awarded"
 msgstr "Contrats attribués"
 
 msgid "Contracts issued"
@@ -1642,17 +1627,14 @@
 
 msgid "Political association"
 msgstr "Association politique"
 
 msgid "Political party"
 msgstr "Parti politique"
 
-msgid "Politician"
-msgstr "Responsable politique"
-
 msgid "Port of Registration"
 msgstr "Port d’immatriculation"
 
 msgid "Position"
 msgstr "Profession"
 
 msgid "Postal code"
@@ -1817,17 +1799,14 @@
 
 msgid "Role"
 msgstr "Rôle"
 
 msgid "Rouble bank"
 msgstr "Banque en roubles"
 
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Code (ОКСМ) russe de classement des pays"
-
 msgid "Russian bank account code"
 msgstr "Code de compte bancaire russe"
 
 msgid "Russian company ID"
 msgstr "Numéro d’identification d’entreprise en Russie"
 
 msgid "Russian industry classifier"
@@ -2057,17 +2036,14 @@
 
 msgid "Thread topic"
 msgstr "Sujet de la conversation"
 
 msgid "Tibet"
 msgstr "Tibet"
 
-msgid "Ticker"
-msgstr "Ticker"
-
 msgid "Title"
 msgstr "Titre"
 
 msgid "Title number"
 msgstr "Numéro de titre"
 
 msgid "To"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/fr/followthemoney.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,52 +7,52 @@
 # Jean-Philippe Menotti, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-06-27 13:42+0200\n"
+"POT-Creation-Date: 2022-03-04 14:36+0100\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: Jean-Philippe Menotti, 2022\n"
 "Language-Team: French (https://www.transifex.com/aleph/teams/76591/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.1\n"
 "Language: fr\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr "Impossible d’inscrire la propriété"
 
 #: followthemoney/property.py:169
 msgid "Invalid value"
 msgstr "Valeur non valable"
 
-#: followthemoney/proxy.py:62
+#: followthemoney/proxy.py:59
 msgid "No schema for entity."
 msgstr "Pas de schéma pour l’entité."
 
-#: followthemoney/proxy.py:115
+#: followthemoney/proxy.py:112
 #, python-format
 msgid "Unknown property (%s): %s"
 msgstr "Propriété inconnue (%s) : %s"
 
-#: followthemoney/proxy.py:188
+#: followthemoney/proxy.py:185
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr "Propriété Stub (%s) : %s"
 
-#: followthemoney/schema.py:342
+#: followthemoney/schema.py:335
 msgid "Required"
 msgstr "Obligatoire"
 
-#: followthemoney/schema.py:346
+#: followthemoney/schema.py:339
 msgid "Entity validation failed"
 msgstr "Échec de la validation de l’entité"
 
 #. Address.label
 #. CryptoWallet.properties.publicKey.label
 #. Thing.properties.address.label
 #. Thing.properties.addressEntity.label
@@ -1984,29 +1984,23 @@
 
 #. Image.label
 #: followthemoney/schema/Image.yaml
 msgid "Image"
 msgstr "Image"
 
 #. Image.plural
-#. Image.properties.pictured.reverse.label
 #: followthemoney/schema/Image.yaml
 msgid "Images"
 msgstr "Images"
 
 #. Image.description
 #: followthemoney/schema/Image.yaml
 msgid "An image file.\n"
 msgstr "Un fichier image.\n"
 
-#. Image.properties.pictured.label
-#: followthemoney/schema/Image.yaml
-msgid "Pictured"
-msgstr ""
-
 #. Interest.label
 #: followthemoney/schema/Interest.yaml
 msgid "Interest"
 msgstr "Intérêt"
 
 #. Interest.properties.role.label
 #: followthemoney/schema/Interest.yaml
@@ -2253,24 +2247,14 @@
 msgstr "INN"
 
 #. LegalEntity.properties.innCode.description
 #: followthemoney/schema/LegalEntity.yaml
 msgid "Russian company ID"
 msgstr "Numéro d’identification d’entreprise en Russie"
 
-#. LegalEntity.properties.leiCode.label
-#: followthemoney/schema/LegalEntity.yaml
-msgid "LEI"
-msgstr ""
-
-#. LegalEntity.properties.leiCode.description
-#: followthemoney/schema/LegalEntity.yaml
-msgid "Legal Entity Identifier"
-msgstr ""
-
 #. LegalEntity.properties.dunsCode.label
 #: followthemoney/schema/LegalEntity.yaml
 msgid "D-U-N-S"
 msgstr "D-U-N-S"
 
 #. LegalEntity.properties.dunsCode.description
 #: followthemoney/schema/LegalEntity.yaml
@@ -2644,15 +2628,14 @@
 #: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
 msgid "Place of birth"
 msgstr "Lieu de naissance"
 
 #. Passport.properties.gender.label
 #. Person.properties.gender.label
 #: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
-#: followthemoney/types/gender.py:40
 msgid "Gender"
 msgstr "Sexe"
 
 #. Passport.properties.personalNumber.label
 #: followthemoney/schema/Passport.yaml
 msgid "Personal number"
 msgstr "Numéro d’identification personnel"
@@ -2798,15 +2781,15 @@
 
 #. Person.properties.ethnicity.label
 #: followthemoney/schema/Person.yaml
 msgid "Ethnicity"
 msgstr "Ethnie"
 
 #. Person.properties.religion.label
-#: followthemoney/schema/Person.yaml followthemoney/types/topic.py:62
+#: followthemoney/schema/Person.yaml followthemoney/types/topic.py:61
 msgid "Religion"
 msgstr "Religion"
 
 #. Person.properties.political.label
 #: followthemoney/schema/Person.yaml
 msgid "Political association"
 msgstr "Association politique"
@@ -3105,66 +3088,14 @@
 msgstr "Date d’émission"
 
 #. Security.properties.collateral.label
 #: followthemoney/schema/Security.yaml
 msgid "Collateral"
 msgstr "Garantie"
 
-#. Similar.label
-#: followthemoney/schema/Similar.yaml
-msgid "Similar"
-msgstr ""
-
-#. Similar.plural
-#: followthemoney/schema/Similar.yaml
-msgid "Similar entities"
-msgstr ""
-
-#. Similar.description
-#: followthemoney/schema/Similar.yaml
-msgid ""
-"A link between two entities that are presumed to be the same, e.g. as the "
-"outcome of a probabilistic record linkage process.\n"
-msgstr ""
-
-#. Similar.properties.candidate.label
-#: followthemoney/schema/Similar.yaml
-msgid "Candidate"
-msgstr ""
-
-#. Similar.properties.candidate.reverse.label
-#: followthemoney/schema/Similar.yaml
-msgid "Similar to this"
-msgstr ""
-
-#. Similar.properties.match.label
-#: followthemoney/schema/Similar.yaml
-msgid "Match"
-msgstr ""
-
-#. Similar.properties.match.reverse.label
-#: followthemoney/schema/Similar.yaml
-msgid "Similar as this"
-msgstr ""
-
-#. Similar.properties.confidenceScore.label
-#: followthemoney/schema/Similar.yaml
-msgid "Confidence score"
-msgstr ""
-
-#. Similar.properties.criteria.label
-#: followthemoney/schema/Similar.yaml
-msgid "Matching criteria"
-msgstr ""
-
-#. Similar.properties.matcher.label
-#: followthemoney/schema/Similar.yaml
-msgid "Matcher"
-msgstr ""
-
 #. Succession.label
 #: followthemoney/schema/Succession.yaml
 msgid "Succession"
 msgstr "Succession"
 
 #. Succession.plural
 #: followthemoney/schema/Succession.yaml
@@ -3323,51 +3254,14 @@
 msgstr "Entités dérivées"
 
 #. Thing.properties.createdAt.label
 #: followthemoney/schema/Thing.yaml
 msgid "Created at"
 msgstr "Créé à"
 
-#. Trip.label
-#: followthemoney/schema/Trip.yaml
-msgid "Trip"
-msgstr ""
-
-#. Trip.plural
-#. Trip.properties.vehicle.reverse.label
-#: followthemoney/schema/Trip.yaml
-msgid "Trips"
-msgstr ""
-
-#. Trip.properties.startLocation.label
-#: followthemoney/schema/Trip.yaml
-msgid "Start location"
-msgstr ""
-
-#. Trip.properties.startLocation.reverse.label
-#: followthemoney/schema/Trip.yaml
-msgid "Trips departing"
-msgstr ""
-
-#. Trip.properties.endLocation.label
-#: followthemoney/schema/Trip.yaml
-msgid "End location"
-msgstr ""
-
-#. Trip.properties.endLocation.reverse.label
-#: followthemoney/schema/Trip.yaml
-msgid "Trips incoming"
-msgstr ""
-
-#. Trip.properties.vehicle.label
-#. Vehicle.label
-#: followthemoney/schema/Trip.yaml followthemoney/schema/Vehicle.yaml
-msgid "Vehicle"
-msgstr "Véhicule"
-
 #. UnknownLink.label
 #: followthemoney/schema/UnknownLink.yaml
 msgid "Other link"
 msgstr "Autre lien"
 
 #. UnknownLink.plural
 #: followthemoney/schema/UnknownLink.yaml
@@ -3451,14 +3345,19 @@
 msgstr "Montant en USD"
 
 #. Value.properties.amountEur.label
 #: followthemoney/schema/Value.yaml
 msgid "Amount in EUR"
 msgstr "Montant en EUR"
 
+#. Vehicle.label
+#: followthemoney/schema/Vehicle.yaml
+msgid "Vehicle"
+msgstr "Véhicule"
+
 #. Vehicle.plural
 #: followthemoney/schema/Vehicle.yaml
 msgid "Vehicles"
 msgstr "Véhicules"
 
 #. Vehicle.properties.model.label
 #: followthemoney/schema/Vehicle.yaml
@@ -3645,32 +3544,32 @@
 msgstr "Tchécoslovaquie"
 
 #: followthemoney/types/country.py:38
 msgid "Soviet Union"
 msgstr "Union soviétique"
 
 #: followthemoney/types/country.py:39
-msgid "Abkhazia (Occupied Georgia)"
-msgstr ""
+msgid "Abkhazia"
+msgstr "Abkhazie"
 
 #: followthemoney/types/country.py:40
-msgid "South Ossetia (Occupied Georgia)"
-msgstr ""
+msgid "South Ossetia"
+msgstr "Ossétie du Sud"
 
 #: followthemoney/types/country.py:41
-msgid "Luhansk (Occupied Ukraine)"
-msgstr ""
+msgid "Luhansk (Ukraine)"
+msgstr "Louhansk (Ukraine)"
 
 #: followthemoney/types/country.py:42
-msgid "Donetsk (Occupied Ukraine)"
-msgstr ""
+msgid "Donetsk (Ukraine)"
+msgstr "Donetsk (Ukraine)"
 
 #: followthemoney/types/country.py:43
-msgid "Crimea (Occupied Ukraine)"
-msgstr ""
+msgid "Crimea (Ukraine)"
+msgstr "Crimée (Ukraine)"
 
 #: followthemoney/types/country.py:44
 msgid "Somaliland"
 msgstr "Somaliland"
 
 #: followthemoney/types/country.py:45
 msgid "Northern Cyprus"
@@ -3697,16 +3596,16 @@
 msgstr "Écosse"
 
 #: followthemoney/types/country.py:51
 msgid "Northern Ireland"
 msgstr "Irlande du Nord"
 
 #: followthemoney/types/country.py:52
-msgid "Transnistria (PMR)"
-msgstr ""
+msgid "Transnistria"
+msgstr "Transnistrie"
 
 #: followthemoney/types/date.py:27
 msgid "Dates"
 msgstr "Dates"
 
 #: followthemoney/types/email.py:25
 msgid "E-Mail Address"
@@ -3721,30 +3620,14 @@
 msgstr "Entités"
 
 #: followthemoney/types/entity.py:61
 #, python-format
 msgid "Self-relationship (%s): %s"
 msgstr "Auto-relation (%s) : %s"
 
-#: followthemoney/types/gender.py:41
-msgid "Genders"
-msgstr ""
-
-#: followthemoney/types/gender.py:46
-msgid "male"
-msgstr ""
-
-#: followthemoney/types/gender.py:47
-msgid "female"
-msgstr ""
-
-#: followthemoney/types/gender.py:48
-msgid "other"
-msgstr ""
-
 #: followthemoney/types/iban.py:25
 msgid "IBANs"
 msgstr "IBAN"
 
 #: followthemoney/types/identifier.py:21
 msgid "Identifier"
 msgstr "Identifiant"
@@ -3930,50 +3813,46 @@
 msgstr "Comptable"
 
 #: followthemoney/types/topic.py:56
 msgid "Spy"
 msgstr "Espion"
 
 #: followthemoney/types/topic.py:57
-msgid "Oligarch"
-msgstr ""
-
-#: followthemoney/types/topic.py:58
 msgid "Journalist"
 msgstr "Journaliste"
 
-#: followthemoney/types/topic.py:59
+#: followthemoney/types/topic.py:58
 msgid "Activist"
 msgstr "Activiste"
 
-#: followthemoney/types/topic.py:60
+#: followthemoney/types/topic.py:59
 msgid "Political party"
 msgstr "Parti politique"
 
-#: followthemoney/types/topic.py:61
+#: followthemoney/types/topic.py:60
 msgid "Union"
 msgstr "Syndicat"
 
-#: followthemoney/types/topic.py:63
+#: followthemoney/types/topic.py:62
 msgid "Military"
 msgstr "Militaire"
 
-#: followthemoney/types/topic.py:64
+#: followthemoney/types/topic.py:63
 msgid "Frozen asset"
 msgstr "Actif gelé"
 
-#: followthemoney/types/topic.py:65
+#: followthemoney/types/topic.py:64
 msgid "Sanctioned entity"
 msgstr "Entité sanctionnée"
 
-#: followthemoney/types/topic.py:66
+#: followthemoney/types/topic.py:65
 msgid "Debarred entity"
 msgstr "Entité exclue"
 
-#: followthemoney/types/topic.py:67
+#: followthemoney/types/topic.py:66
 msgid "Person of interest"
 msgstr "Personne d’intérêt"
 
 #: followthemoney/types/url.py:22
 msgid "URL"
 msgstr "URL"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # Translations template for PROJECT.
-# Copyright (C) 2022 ORGANIZATION
+# Copyright (C) 2023 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 # 
 # Translators:
 # Jean-Philippe Menotti, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-03-04 14:36+0100\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: Jean-Philippe Menotti, 2022\n"
-"Language-Team: French (https://www.transifex.com/aleph/teams/76591/fr/)\n"
+"Language-Team: French (https://app.transifex.com/aleph/teams/76591/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.12.1\n"
 "Language: fr\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr "Impossible d’inscrire la propriété"
 
 #: followthemoney/property.py:169
 msgid "Invalid value"
 msgstr "Valeur non valable"
 
-#: followthemoney/proxy.py:59
+#: followthemoney/proxy.py:62
 msgid "No schema for entity."
 msgstr "Pas de schéma pour l’entité."
 
-#: followthemoney/proxy.py:112
+#: followthemoney/proxy.py:115
 #, python-format
 msgid "Unknown property (%s): %s"
 msgstr "Propriété inconnue (%s) : %s"
 
-#: followthemoney/proxy.py:185
+#: followthemoney/proxy.py:188
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr "Propriété Stub (%s) : %s"
 
-#: followthemoney/schema.py:335
+#: followthemoney/schema.py:373
 msgid "Required"
 msgstr "Obligatoire"
 
-#: followthemoney/schema.py:339
+#: followthemoney/schema.py:377
 msgid "Entity validation failed"
 msgstr "Échec de la validation de l’entité"
 
 #. Address.label
 #. CryptoWallet.properties.publicKey.label
 #. Thing.properties.address.label
 #. Thing.properties.addressEntity.label
@@ -89,16 +89,16 @@
 #. Address.properties.postOfficeBox.label
 #: followthemoney/schema/Address.yaml
 msgid "PO Box"
 msgstr "Boîte postale"
 
 #. Address.properties.postOfficeBox.description
 #: followthemoney/schema/Address.yaml
-msgid "A mailbox indentifier at the post office"
-msgstr "Identifiant de boîte au bureau de poste"
+msgid "A mailbox identifier at the post office"
+msgstr ""
 
 #. Address.properties.street.label
 #: followthemoney/schema/Address.yaml
 msgid "Street address"
 msgstr "Rue"
 
 #. Address.properties.street2.label
@@ -167,14 +167,24 @@
 #: followthemoney/schema/Address.yaml followthemoney/schema/Event.yaml
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml followthemoney/schema/TaxRoll.yaml
 #: followthemoney/schema/Thing.yaml followthemoney/types/country.py:21
 msgid "Country"
 msgstr "Pays"
 
+#. Address.properties.osmId.label
+#: followthemoney/schema/Address.yaml
+msgid "OpenStreetmap Place ID"
+msgstr ""
+
+#. Address.properties.googlePlaceId.label
+#: followthemoney/schema/Address.yaml
+msgid "Google Places ID"
+msgstr ""
+
 #. Airplane.label
 #: followthemoney/schema/Airplane.yaml
 msgid "Airplane"
 msgstr "Avion"
 
 #. Airplane.plural
 #: followthemoney/schema/Airplane.yaml
@@ -475,14 +485,24 @@
 msgstr "Banque"
 
 #. BankAccount.properties.accountType.label
 #: followthemoney/schema/BankAccount.yaml
 msgid "Account type"
 msgstr "Type de compte"
 
+#. BankAccount.properties.openingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Opening date"
+msgstr ""
+
+#. BankAccount.properties.closingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Closing date"
+msgstr ""
+
 #. BankAccount.properties.balance.label
 #. CryptoWallet.properties.balance.label
 #: followthemoney/schema/BankAccount.yaml
 #: followthemoney/schema/CryptoWallet.yaml
 msgid "Balance"
 msgstr "Solde"
 
@@ -545,14 +565,237 @@
 msgstr "Appels reçus"
 
 #. Call.properties.receiverNumber.label
 #: followthemoney/schema/Call.yaml
 msgid "Receiver's Number"
 msgstr "Numéro du destinataire"
 
+#. CallForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders"
+msgstr ""
+
+#. CallForTenders.plural
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Calls for tenders"
+msgstr ""
+
+#. CallForTenders.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid ""
+"A public appeal issued by an authority, possibly on behalf of another, for "
+"buying a specific work, supply or service\n"
+msgstr ""
+
+#. CallForTenders.properties.callId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "CfT unique id"
+msgstr ""
+
+#. CallForTenders.properties.title.label
+#. Contract.properties.title.label
+#. Document.properties.title.label
+#. Person.properties.title.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/Contract.yaml followthemoney/schema/Document.yaml
+#: followthemoney/schema/Person.yaml
+msgid "Title"
+msgstr "Titre"
+
+#. CallForTenders.properties.authority.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Name of contracting authority"
+msgstr ""
+
+#. CallForTenders.properties.authority.reverse.label
+#. ContractAward.properties.callForTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "Call For Tenders"
+msgstr ""
+
+#. CallForTenders.properties.authorityReferenceId.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contracting authority reference ID"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Published on behalf of"
+msgstr ""
+
+#. CallForTenders.properties.onBehalfOf.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Delegated call for tenders"
+msgstr ""
+
+#. CallForTenders.properties.publicationDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of publication/invitation"
+msgstr ""
+
+#. CallForTenders.properties.evaluationMechanism.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Evaluation mechanism"
+msgstr ""
+
+#. CallForTenders.properties.procurementType.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procurement type"
+msgstr ""
+
+#. CallForTenders.properties.directive.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Directive"
+msgstr ""
+
+#. CallForTenders.properties.procedure.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Procedure"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Call for tenders result"
+msgstr ""
+
+#. CallForTenders.properties.involvesOutcome.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "The nature of the contractual agreement that will result from this CfT"
+msgstr ""
+
+#. CallForTenders.properties.cpvCode.label
+#. ContractAward.properties.cpvCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "CPV code"
+msgstr "Code CPV"
+
+#. CallForTenders.properties.cpvCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Common Procurement Vocabulary (CPV)"
+msgstr ""
+
+#. CallForTenders.properties.reverseAuctionsIncluded.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Inclusion of e-Auctions"
+msgstr ""
+
+#. CallForTenders.properties.nutsCode.label
+#. ContractAward.properties.nutsCode.label
+#: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
+msgid "NUTS code"
+msgstr "Code NUTS"
+
+#. CallForTenders.properties.nutsCode.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Nomenclature of Territorial Units for Statistics (NUTS)"
+msgstr ""
+
+#. CallForTenders.properties.relationToThreshold.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Above or below threshold"
+msgstr ""
+
+#. CallForTenders.properties.paymentOptions.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Payment options"
+msgstr ""
+
+#. CallForTenders.properties.submissionDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Submission deadline"
+msgstr ""
+
+#. CallForTenders.properties.clarificationDeadline.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "End of clarification period"
+msgstr ""
+
+#. CallForTenders.properties.awardedInLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract awarded in Lots"
+msgstr ""
+
+#. CallForTenders.properties.numberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Number of lots"
+msgstr ""
+
+#. CallForTenders.properties.lotsNames.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Lots names"
+msgstr ""
+
+#. CallForTenders.properties.tendersForLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenders for lots"
+msgstr ""
+
+#. CallForTenders.properties.maximumNumberOfLots.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Maximum number of lots"
+msgstr ""
+
+#. CallForTenders.properties.euFunding.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "EU funding"
+msgstr ""
+
+#. CallForTenders.properties.multipleTenders.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Multiple tenders will be accepted"
+msgstr ""
+
+#. CallForTenders.properties.tedUrl.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "TED link for published notices"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Does this call fall under the scope of GPP?"
+msgstr ""
+
+#. CallForTenders.properties.fallsUnderGPPScope.description
+#: followthemoney/schema/CallForTenders.yaml
+msgid "European Green Public Procurement (GPP) or green purchasing."
+msgstr ""
+
+#. CallForTenders.properties.certificationCheck.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Certification check"
+msgstr ""
+
+#. CallForTenders.properties.awardingDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Date of awarding"
+msgstr ""
+
+#. CallForTenders.properties.contractNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Contract notice date"
+msgstr ""
+
+#. CallForTenders.properties.awardNoticeDate.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Award Notice Date"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tenderers"
+msgstr ""
+
+#. CallForTenders.properties.tenderers.reverse.label
+#: followthemoney/schema/CallForTenders.yaml
+msgid "Tender"
+msgstr ""
+
 #. Company.label
 #: followthemoney/schema/Company.yaml
 msgid "Company"
 msgstr "Société"
 
 #. Company.plural
 #: followthemoney/schema/Company.yaml
@@ -578,17 +821,19 @@
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
 msgid "Jurisdiction"
 msgstr "Juridiction"
 
 #. Company.properties.registrationNumber.label
 #. LegalEntity.properties.registrationNumber.label
 #. RealEstate.properties.registrationNumber.label
+#. Security.properties.registrationNumber.label
 #. Vehicle.properties.registrationNumber.label
 #: followthemoney/schema/Company.yaml followthemoney/schema/LegalEntity.yaml
-#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Vehicle.yaml
+#: followthemoney/schema/RealEstate.yaml followthemoney/schema/Security.yaml
+#: followthemoney/schema/Vehicle.yaml
 msgid "Registration number"
 msgstr "Numéro d’enregistrement"
 
 #. Company.properties.capital.label
 #: followthemoney/schema/Company.yaml
 msgid "Capital"
 msgstr "Capital"
@@ -604,14 +849,21 @@
 msgstr "Numéro d’identification fiscale en Azerbaïdjan"
 
 #. Company.properties.coatoCode.label
 #: followthemoney/schema/Company.yaml
 msgid "COATO / SOATO / OKATO"
 msgstr "COATO / SOATO / OKATO"
 
+#. Company.properties.coatoCode.description
+#: followthemoney/schema/Company.yaml
+msgid ""
+"Soviet classifier for territories, regions, districts, villages. Aka. SOATO "
+"and same as OKATO"
+msgstr ""
+
 #. Company.properties.irsCode.label
 #: followthemoney/schema/Company.yaml
 msgid "IRS Number"
 msgstr "Numéro IRS"
 
 #. Company.properties.irsCode.description
 #: followthemoney/schema/Company.yaml
@@ -714,24 +966,14 @@
 msgstr "FSS"
 
 #. Company.properties.fssCode.description
 #: followthemoney/schema/Company.yaml
 msgid "(RU, ФСС) Social Security"
 msgstr "(RU, ФСС) Sécurité sociale"
 
-#. Company.properties.ogrnCode.label
-#: followthemoney/schema/Company.yaml
-msgid "OGRN"
-msgstr "OGRN"
-
-#. Company.properties.ogrnCode.description
-#: followthemoney/schema/Company.yaml
-msgid "Major State Registration Number"
-msgstr "Principal numéro d’enregistrement de l’État"
-
 #. Company.properties.bikCode.label
 #: followthemoney/schema/Company.yaml
 msgid "BIK"
 msgstr "BIK"
 
 #. Company.properties.bikCode.description
 #: followthemoney/schema/Company.yaml
@@ -756,16 +998,34 @@
 #. Company.properties.oksmCode.label
 #: followthemoney/schema/Company.yaml
 msgid "OKSM"
 msgstr "OKSM"
 
 #. Company.properties.oksmCode.description
 #: followthemoney/schema/Company.yaml
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Code (ОКСМ) russe de classement des pays"
+msgid "Russian (ОКСМ) countries classifier"
+msgstr ""
+
+#. Company.properties.isinCode.label
+#. Security.properties.isin.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "ISIN"
+msgstr "ISIN"
+
+#. Company.properties.isinCode.description
+#. Security.properties.isin.description
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "International Securities Identification Number"
+msgstr "Numéro international d’identification des titres"
+
+#. Company.properties.ticker.label
+#. Security.properties.ticker.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "Stock ticker symbol"
+msgstr ""
 
 #. Contract.label
 #. ContractAward.properties.contract.label
 #. EconomicActivity.properties.contract.label
 #. Payment.properties.contract.label
 #: followthemoney/schema/Contract.yaml
 #: followthemoney/schema/ContractAward.yaml
@@ -788,19 +1048,14 @@
 "An contract or contract lot issued by an authority. Multiple lots may be "
 "awarded to different suppliers (see ContractAward).\n"
 msgstr ""
 "Un contrat ou un lot de contrat émis par une autorité. Des lots multiples "
 "peuvent être attribués à différents fournisseurs (voir attribution des "
 "contrats).\n"
 
-#. Contract.properties.title.label
-#: followthemoney/schema/Contract.yaml
-msgid "Contract title"
-msgstr "Titre du contrat"
-
 #. Contract.properties.authority.label
 #: followthemoney/schema/Contract.yaml
 msgid "Contract authority"
 msgstr "Autorité du contrat"
 
 #. Contract.properties.authority.plural
 #: followthemoney/schema/Contract.yaml
@@ -947,50 +1202,47 @@
 msgstr "Contrats attribués"
 
 #. ContractAward.properties.contract.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lots awarded"
 msgstr "Lots attribués"
 
+#. ContractAward.properties.callForTenders.reverse.label
+#: followthemoney/schema/ContractAward.yaml
+msgid "Contract Awards"
+msgstr ""
+
 #. ContractAward.properties.lotNumber.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lot number"
 msgstr "Numéro de lot"
 
 #. ContractAward.properties.documentNumber.label
+#. Identification.properties.number.label
 #: followthemoney/schema/ContractAward.yaml
+#: followthemoney/schema/Identification.yaml
 msgid "Document number"
 msgstr "Numéro de document"
 
 #. ContractAward.properties.documentType.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Document type"
 msgstr "Type de document"
 
 #. ContractAward.properties.decisionReason.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Decision reason"
 msgstr "Raison de la décision"
 
-#. ContractAward.properties.cpvCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "CPV code"
-msgstr "Code CPV"
-
 #. ContractAward.properties.cpvCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Procurement Vocabulary (what type of goods/services, EU)"
 msgstr ""
 "Vocabulaire commun pour les marchés publics (type de biens/services, UE)"
 
-#. ContractAward.properties.nutsCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "NUTS code"
-msgstr "Code NUTS"
-
 #. ContractAward.properties.nutsCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Nomencalture of Territorial Units for Statistics (NUTS)"
 msgstr "Nomenclature des unités territoriales statistiques (NUTS)"
 
 #. ContractAward.properties.amended.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1177,17 +1429,18 @@
 #: followthemoney/schema/Directorship.yaml
 msgid "Director"
 msgstr "Directeur"
 
 #. Directorship.properties.organization.label
 #. Membership.properties.organization.label
 #. Organization.label
+#. Post.properties.organization.label
 #: followthemoney/schema/Directorship.yaml
 #: followthemoney/schema/Membership.yaml
-#: followthemoney/schema/Organization.yaml
+#: followthemoney/schema/Organization.yaml followthemoney/schema/Post.yaml
 msgid "Organization"
 msgstr "Organisation"
 
 #. Directorship.properties.organization.reverse.label
 #: followthemoney/schema/Directorship.yaml
 msgid "Directors"
 msgstr "Administrateurs"
@@ -1213,20 +1466,14 @@
 msgstr "Somme de contrôle"
 
 #. Document.properties.contentHash.description
 #: followthemoney/schema/Document.yaml
 msgid "SHA1 hash of the data"
 msgstr "SHA1 hash des données"
 
-#. Document.properties.title.label
-#. Person.properties.title.label
-#: followthemoney/schema/Document.yaml followthemoney/schema/Person.yaml
-msgid "Title"
-msgstr "Titre"
-
 #. Document.properties.author.description
 #: followthemoney/schema/Document.yaml
 msgid "The original author, not the uploader"
 msgstr "L’auteur original, pas la personne à l’origine de l’envoi"
 
 #. Document.properties.generator.label
 #: followthemoney/schema/Document.yaml
@@ -1351,14 +1598,24 @@
 msgstr "État du traitement"
 
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr "Erreur de traitement"
 
+#. Document.properties.processingAgent.label
+#: followthemoney/schema/Document.yaml
+msgid "Name and version of the processing agent used to process the Document"
+msgstr ""
+
+#. Document.properties.processedAt.label
+#: followthemoney/schema/Document.yaml
+msgid "Date and time of the most recent ingestion of the Document"
+msgstr ""
+
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr "Documentation"
 
 #. Documentation.plural
 #: followthemoney/schema/Documentation.yml
@@ -1489,22 +1746,14 @@
 msgid ""
 "(Описание кода ТН ВЭД) Foreign Economic Activity Commodity Code description"
 msgstr ""
 "(Описание кода ТН ВЭД) Description du code de la nomenclature unique des "
 "marchandises pour les activités économiques étrangères"
 
 #. EconomicActivity.properties.goodsDescription.label
-#. Interval.properties.description.label
-#. Thing.properties.description.label
-#: followthemoney/schema/EconomicActivity.yaml
-#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
-msgid "Description"
-msgstr "Description"
-
-#. EconomicActivity.properties.goodsDescription.description
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Description of goods"
 msgstr "Description des marchandises"
 
 #. EconomicActivity.properties.declarant.label
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Declarant"
@@ -1963,44 +2212,42 @@
 " les listes électorales et d’autres instruments comparables.\n"
 
 #. Identification.properties.holder.label
 #: followthemoney/schema/Identification.yaml
 msgid "Identification holder"
 msgstr "Titulaire de l’identification"
 
-#. Identification.properties.number.label
-#. Passport.properties.passportNumber.label
-#. Person.properties.passportNumber.label
-#: followthemoney/schema/Identification.yaml
-#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
-msgid "Passport number"
-msgstr "Numéro de passeport"
-
 #. Identification.properties.authority.label
 #. Sanction.properties.authority.label
 #: followthemoney/schema/Identification.yaml
 #: followthemoney/schema/Sanction.yaml
 msgid "Authority"
 msgstr "Autorité"
 
 #. Image.label
 #: followthemoney/schema/Image.yaml
 msgid "Image"
 msgstr "Image"
 
 #. Image.plural
+#. Image.properties.pictured.reverse.label
 #: followthemoney/schema/Image.yaml
 msgid "Images"
 msgstr "Images"
 
 #. Image.description
 #: followthemoney/schema/Image.yaml
 msgid "An image file.\n"
 msgstr "Un fichier image.\n"
 
+#. Image.properties.pictured.label
+#: followthemoney/schema/Image.yaml
+msgid "Pictured"
+msgstr ""
+
 #. Interest.label
 #: followthemoney/schema/Interest.yaml
 msgid "Interest"
 msgstr "Intérêt"
 
 #. Interest.properties.role.label
 #: followthemoney/schema/Interest.yaml
@@ -2029,14 +2276,20 @@
 
 #. Interval.properties.summary.label
 #. Thing.properties.summary.label
 #: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
 msgid "Summary"
 msgstr "Résumé"
 
+#. Interval.properties.description.label
+#. Thing.properties.description.label
+#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
+msgid "Description"
+msgstr "Description"
+
 #. Interval.properties.recordId.label
 #: followthemoney/schema/Interval.yaml
 msgid "Record ID"
 msgstr "Identifiant du registre"
 
 #. Interval.properties.sourceUrl.label
 #. Thing.properties.sourceUrl.label
@@ -2247,14 +2500,34 @@
 msgstr "INN"
 
 #. LegalEntity.properties.innCode.description
 #: followthemoney/schema/LegalEntity.yaml
 msgid "Russian company ID"
 msgstr "Numéro d’identification d’entreprise en Russie"
 
+#. LegalEntity.properties.ogrnCode.label
+#: followthemoney/schema/LegalEntity.yaml
+msgid "OGRN"
+msgstr "OGRN"
+
+#. LegalEntity.properties.ogrnCode.description
+#: followthemoney/schema/LegalEntity.yaml
+msgid "Major State Registration Number"
+msgstr "Principal numéro d’enregistrement de l’État"
+
+#. LegalEntity.properties.leiCode.label
+#: followthemoney/schema/LegalEntity.yaml
+msgid "LEI"
+msgstr ""
+
+#. LegalEntity.properties.leiCode.description
+#: followthemoney/schema/LegalEntity.yaml
+msgid "Legal Entity Identifier"
+msgstr ""
+
 #. LegalEntity.properties.dunsCode.label
 #: followthemoney/schema/LegalEntity.yaml
 msgid "D-U-N-S"
 msgstr "D-U-N-S"
 
 #. LegalEntity.properties.dunsCode.description
 #: followthemoney/schema/LegalEntity.yaml
@@ -2368,15 +2641,15 @@
 #: followthemoney/schema/Mention.yaml
 msgid "Document mentions"
 msgstr "Mentions de document"
 
 #. Mention.properties.name.label
 #. Thing.properties.name.label
 #: followthemoney/schema/Mention.yaml followthemoney/schema/Thing.yaml
-#: followthemoney/types/name.py:26
+#: followthemoney/types/name.py:25
 msgid "Name"
 msgstr "Nom"
 
 #. Mention.properties.detectedSchema.label
 #: followthemoney/schema/Mention.yaml
 msgid "Detected entity type"
 msgstr "Type d’entité détecté"
@@ -2461,19 +2734,16 @@
 msgstr "Organisations"
 
 #. Organization.description
 #: followthemoney/schema/Organization.yaml
 msgid ""
 "Any type of incorporated entity that cannot be owned by another (see "
 "Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
+"enterprises, depending on their  jurisdiction.\n"
 msgstr ""
-"Tout type d’entité constituée qui ne peut être détenue par une autre (voir "
-"Société). Il peut s’agir d’une organisation caritative, d’une fondation ou "
-"d’une entreprise détenue par un État, en fonction de sa juridiction.\n"
 
 #. Ownership.label
 #: followthemoney/schema/Ownership.yaml
 msgid "Ownership"
 msgstr "Propriété"
 
 #. Ownership.plural
@@ -2599,14 +2869,20 @@
 msgstr "Passeports"
 
 #. Passport.description
 #: followthemoney/schema/Passport.yaml
 msgid "An passport held by a person.\n"
 msgstr "Un passeport détenu par une personne.\n"
 
+#. Passport.properties.passportNumber.label
+#. Person.properties.passportNumber.label
+#: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
+msgid "Passport number"
+msgstr "Numéro de passeport"
+
 #. Passport.properties.surname.label
 #. TaxRoll.properties.surname.label
 #: followthemoney/schema/Passport.yaml followthemoney/schema/TaxRoll.yaml
 msgid "Surname"
 msgstr "Nom"
 
 #. Passport.properties.givenName.label
@@ -2628,14 +2904,15 @@
 #: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
 msgid "Place of birth"
 msgstr "Lieu de naissance"
 
 #. Passport.properties.gender.label
 #. Person.properties.gender.label
 #: followthemoney/schema/Passport.yaml followthemoney/schema/Person.yaml
+#: followthemoney/types/gender.py:40
 msgid "Gender"
 msgstr "Sexe"
 
 #. Passport.properties.personalNumber.label
 #: followthemoney/schema/Passport.yaml
 msgid "Personal number"
 msgstr "Numéro d’identification personnel"
@@ -2781,15 +3058,15 @@
 
 #. Person.properties.ethnicity.label
 #: followthemoney/schema/Person.yaml
 msgid "Ethnicity"
 msgstr "Ethnie"
 
 #. Person.properties.religion.label
-#: followthemoney/schema/Person.yaml followthemoney/types/topic.py:61
+#: followthemoney/schema/Person.yaml followthemoney/types/topic.py:62
 msgid "Religion"
 msgstr "Religion"
 
 #. Person.properties.political.label
 #: followthemoney/schema/Person.yaml
 msgid "Political association"
 msgstr "Association politique"
@@ -2810,14 +3087,48 @@
 msgstr "Fichiers texte"
 
 #. PlainText.description
 #: followthemoney/schema/PlainText.yaml
 msgid "Text files, like .txt or source code.\n"
 msgstr "Fichiers texte, comme des fichiers .txt ou du code source.\n"
 
+#. Post.label
+#: followthemoney/schema/Post.yaml
+msgid "Post"
+msgstr ""
+
+#. Post.plural
+#: followthemoney/schema/Post.yaml
+msgid "Posts"
+msgstr ""
+
+#. Post.description
+#: followthemoney/schema/Post.yaml
+msgid ""
+"A post, role or position held by an individual within an organization  or "
+"body. This describes the period for which the position is held, not the "
+"abstract concept of the post.\n"
+msgstr ""
+
+#. Post.properties.holder.label
+#: followthemoney/schema/Post.yaml
+msgid "Holder"
+msgstr ""
+
+#. Post.properties.holder.reverse.label
+#: followthemoney/schema/Post.yaml
+msgid "Posts held"
+msgstr ""
+
+#. Post.properties.wikidataId.label
+#. Thing.properties.wikidataId.label
+#: followthemoney/schema/Post.yaml followthemoney/schema/Thing.yaml
+msgid "Wikidata ID"
+msgstr "Identifiant Wikidata"
+
 #. Project.plural
 #. ProjectParticipant.properties.participant.reverse.label
 #: followthemoney/schema/Project.yaml
 #: followthemoney/schema/ProjectParticipant.yaml
 msgid "Projects"
 msgstr "Projets"
 
@@ -3053,29 +3364,14 @@
 msgstr "Valeurs/Titres"
 
 #. Security.description
 #: followthemoney/schema/Security.yaml
 msgid "A tradeable financial asset."
 msgstr "Un actif financier négociable."
 
-#. Security.properties.isin.label
-#: followthemoney/schema/Security.yaml
-msgid "ISIN"
-msgstr "ISIN"
-
-#. Security.properties.isin.description
-#: followthemoney/schema/Security.yaml
-msgid "International Securities Identification Number"
-msgstr "Numéro international d’identification des titres"
-
-#. Security.properties.ticker.label
-#: followthemoney/schema/Security.yaml
-msgid "Ticker"
-msgstr "Ticker"
-
 #. Security.properties.issuer.label
 #: followthemoney/schema/Security.yaml
 msgid "Issuer"
 msgstr "Émetteur"
 
 #. Security.properties.issuer.reverse.label
 #: followthemoney/schema/Security.yaml
@@ -3083,19 +3379,76 @@
 msgstr "Titres émis"
 
 #. Security.properties.issueDate.label
 #: followthemoney/schema/Security.yaml
 msgid "Date issued"
 msgstr "Date d’émission"
 
+#. Security.properties.maturityDate.label
+#: followthemoney/schema/Security.yaml
+msgid "Maturity date"
+msgstr ""
+
 #. Security.properties.collateral.label
 #: followthemoney/schema/Security.yaml
 msgid "Collateral"
 msgstr "Garantie"
 
+#. Similar.label
+#: followthemoney/schema/Similar.yaml
+msgid "Similar"
+msgstr ""
+
+#. Similar.plural
+#: followthemoney/schema/Similar.yaml
+msgid "Similar entities"
+msgstr ""
+
+#. Similar.description
+#: followthemoney/schema/Similar.yaml
+msgid ""
+"A link between two entities that are presumed to be the same, e.g. as the "
+"outcome of a probabilistic record linkage process.\n"
+msgstr ""
+
+#. Similar.properties.candidate.label
+#: followthemoney/schema/Similar.yaml
+msgid "Candidate"
+msgstr ""
+
+#. Similar.properties.candidate.reverse.label
+#: followthemoney/schema/Similar.yaml
+msgid "Similar to this"
+msgstr ""
+
+#. Similar.properties.match.label
+#: followthemoney/schema/Similar.yaml
+msgid "Match"
+msgstr ""
+
+#. Similar.properties.match.reverse.label
+#: followthemoney/schema/Similar.yaml
+msgid "Similar as this"
+msgstr ""
+
+#. Similar.properties.confidenceScore.label
+#: followthemoney/schema/Similar.yaml
+msgid "Confidence score"
+msgstr ""
+
+#. Similar.properties.criteria.label
+#: followthemoney/schema/Similar.yaml
+msgid "Matching criteria"
+msgstr ""
+
+#. Similar.properties.matcher.label
+#: followthemoney/schema/Similar.yaml
+msgid "Matcher"
+msgstr ""
+
 #. Succession.label
 #: followthemoney/schema/Succession.yaml
 msgid "Succession"
 msgstr "Succession"
 
 #. Succession.plural
 #: followthemoney/schema/Succession.yaml
@@ -3219,19 +3572,14 @@
 msgstr "Alias faible"
 
 #. Thing.properties.wikipediaUrl.label
 #: followthemoney/schema/Thing.yaml
 msgid "Wikipedia Article"
 msgstr "Article sur Wikipedia"
 
-#. Thing.properties.wikidataId.label
-#: followthemoney/schema/Thing.yaml
-msgid "Wikidata ID"
-msgstr "Identifiant Wikidata"
-
 #. Thing.properties.keywords.label
 #: followthemoney/schema/Thing.yaml
 msgid "Keywords"
 msgstr "Mots-clés"
 
 #. Thing.properties.topics.label
 #: followthemoney/schema/Thing.yaml followthemoney/types/topic.py:22
@@ -3254,14 +3602,51 @@
 msgstr "Entités dérivées"
 
 #. Thing.properties.createdAt.label
 #: followthemoney/schema/Thing.yaml
 msgid "Created at"
 msgstr "Créé à"
 
+#. Trip.label
+#: followthemoney/schema/Trip.yaml
+msgid "Trip"
+msgstr ""
+
+#. Trip.plural
+#. Trip.properties.vehicle.reverse.label
+#: followthemoney/schema/Trip.yaml
+msgid "Trips"
+msgstr ""
+
+#. Trip.properties.startLocation.label
+#: followthemoney/schema/Trip.yaml
+msgid "Start location"
+msgstr ""
+
+#. Trip.properties.startLocation.reverse.label
+#: followthemoney/schema/Trip.yaml
+msgid "Trips departing"
+msgstr ""
+
+#. Trip.properties.endLocation.label
+#: followthemoney/schema/Trip.yaml
+msgid "End location"
+msgstr ""
+
+#. Trip.properties.endLocation.reverse.label
+#: followthemoney/schema/Trip.yaml
+msgid "Trips incoming"
+msgstr ""
+
+#. Trip.properties.vehicle.label
+#. Vehicle.label
+#: followthemoney/schema/Trip.yaml followthemoney/schema/Vehicle.yaml
+msgid "Vehicle"
+msgstr "Véhicule"
+
 #. UnknownLink.label
 #: followthemoney/schema/UnknownLink.yaml
 msgid "Other link"
 msgstr "Autre lien"
 
 #. UnknownLink.plural
 #: followthemoney/schema/UnknownLink.yaml
@@ -3315,14 +3700,19 @@
 msgstr "Nom d’utilisateur"
 
 #. UserAccount.properties.password.label
 #: followthemoney/schema/UserAccount.yaml
 msgid "Password"
 msgstr "Mot de passe"
 
+#. UserAccount.properties.ipAddress.label
+#: followthemoney/schema/UserAccount.yaml
+msgid "IP address"
+msgstr ""
+
 #. Value.label
 #: followthemoney/schema/Value.yaml
 msgid "Value"
 msgstr "Valeur"
 
 #. Value.plural
 #: followthemoney/schema/Value.yaml
@@ -3345,19 +3735,14 @@
 msgstr "Montant en USD"
 
 #. Value.properties.amountEur.label
 #: followthemoney/schema/Value.yaml
 msgid "Amount in EUR"
 msgstr "Montant en EUR"
 
-#. Vehicle.label
-#: followthemoney/schema/Vehicle.yaml
-msgid "Vehicle"
-msgstr "Véhicule"
-
 #. Vehicle.plural
 #: followthemoney/schema/Vehicle.yaml
 msgid "Vehicles"
 msgstr "Véhicules"
 
 #. Vehicle.properties.model.label
 #: followthemoney/schema/Vehicle.yaml
@@ -3544,32 +3929,32 @@
 msgstr "Tchécoslovaquie"
 
 #: followthemoney/types/country.py:38
 msgid "Soviet Union"
 msgstr "Union soviétique"
 
 #: followthemoney/types/country.py:39
-msgid "Abkhazia"
-msgstr "Abkhazie"
+msgid "Abkhazia (Occupied Georgia)"
+msgstr ""
 
 #: followthemoney/types/country.py:40
-msgid "South Ossetia"
-msgstr "Ossétie du Sud"
+msgid "South Ossetia (Occupied Georgia)"
+msgstr ""
 
 #: followthemoney/types/country.py:41
-msgid "Luhansk (Ukraine)"
-msgstr "Louhansk (Ukraine)"
+msgid "Luhansk (Occupied Ukraine)"
+msgstr ""
 
 #: followthemoney/types/country.py:42
-msgid "Donetsk (Ukraine)"
-msgstr "Donetsk (Ukraine)"
+msgid "Donetsk (Occupied Ukraine)"
+msgstr ""
 
 #: followthemoney/types/country.py:43
-msgid "Crimea (Ukraine)"
-msgstr "Crimée (Ukraine)"
+msgid "Crimea (Occupied Ukraine)"
+msgstr ""
 
 #: followthemoney/types/country.py:44
 msgid "Somaliland"
 msgstr "Somaliland"
 
 #: followthemoney/types/country.py:45
 msgid "Northern Cyprus"
@@ -3596,16 +3981,16 @@
 msgstr "Écosse"
 
 #: followthemoney/types/country.py:51
 msgid "Northern Ireland"
 msgstr "Irlande du Nord"
 
 #: followthemoney/types/country.py:52
-msgid "Transnistria"
-msgstr "Transnistrie"
+msgid "Transnistria (PMR)"
+msgstr ""
 
 #: followthemoney/types/date.py:27
 msgid "Dates"
 msgstr "Dates"
 
 #: followthemoney/types/email.py:25
 msgid "E-Mail Address"
@@ -3620,14 +4005,30 @@
 msgstr "Entités"
 
 #: followthemoney/types/entity.py:61
 #, python-format
 msgid "Self-relationship (%s): %s"
 msgstr "Auto-relation (%s) : %s"
 
+#: followthemoney/types/gender.py:41
+msgid "Genders"
+msgstr ""
+
+#: followthemoney/types/gender.py:46
+msgid "male"
+msgstr ""
+
+#: followthemoney/types/gender.py:47
+msgid "female"
+msgstr ""
+
+#: followthemoney/types/gender.py:48
+msgid "other"
+msgstr ""
+
 #: followthemoney/types/iban.py:25
 msgid "IBANs"
 msgstr "IBAN"
 
 #: followthemoney/types/identifier.py:21
 msgid "Identifier"
 msgstr "Identifiant"
@@ -3656,15 +4057,15 @@
 msgid "MIME-Type"
 msgstr "Type MIME"
 
 #: followthemoney/types/mimetype.py:25
 msgid "MIME-Types"
 msgstr "Types MIME"
 
-#: followthemoney/types/name.py:27
+#: followthemoney/types/name.py:26
 msgid "Names"
 msgstr "Noms"
 
 #: followthemoney/types/number.py:18
 msgid "Number"
 msgstr "Numéro"
 
@@ -3781,16 +4182,16 @@
 msgstr "Fonds"
 
 #: followthemoney/types/topic.py:48
 msgid "Financial advisor"
 msgstr "Conseiller financier"
 
 #: followthemoney/types/topic.py:49
-msgid "Politician"
-msgstr "Responsable politique"
+msgid "Political"
+msgstr ""
 
 #: followthemoney/types/topic.py:50
 msgid "Close Associate"
 msgstr "Proche collaborateur"
 
 #: followthemoney/types/topic.py:51
 msgid "Judge"
@@ -3813,46 +4214,54 @@
 msgstr "Comptable"
 
 #: followthemoney/types/topic.py:56
 msgid "Spy"
 msgstr "Espion"
 
 #: followthemoney/types/topic.py:57
+msgid "Oligarch"
+msgstr ""
+
+#: followthemoney/types/topic.py:58
 msgid "Journalist"
 msgstr "Journaliste"
 
-#: followthemoney/types/topic.py:58
+#: followthemoney/types/topic.py:59
 msgid "Activist"
 msgstr "Activiste"
 
-#: followthemoney/types/topic.py:59
+#: followthemoney/types/topic.py:60
 msgid "Political party"
 msgstr "Parti politique"
 
-#: followthemoney/types/topic.py:60
+#: followthemoney/types/topic.py:61
 msgid "Union"
 msgstr "Syndicat"
 
-#: followthemoney/types/topic.py:62
+#: followthemoney/types/topic.py:63
 msgid "Military"
 msgstr "Militaire"
 
-#: followthemoney/types/topic.py:63
+#: followthemoney/types/topic.py:64
 msgid "Frozen asset"
 msgstr "Actif gelé"
 
-#: followthemoney/types/topic.py:64
+#: followthemoney/types/topic.py:65
 msgid "Sanctioned entity"
 msgstr "Entité sanctionnée"
 
-#: followthemoney/types/topic.py:65
+#: followthemoney/types/topic.py:66
+msgid "Sanction-linked entity"
+msgstr ""
+
+#: followthemoney/types/topic.py:67
 msgid "Debarred entity"
 msgstr "Entité exclue"
 
-#: followthemoney/types/topic.py:66
+#: followthemoney/types/topic.py:68
 msgid "Person of interest"
 msgstr "Personne d’intérêt"
 
 #: followthemoney/types/url.py:22
 msgid "URL"
 msgstr "URL"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/messages.pot` & `followthemoney-3.4.2/followthemoney/translations/messages.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-01-04 09:58+0100\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr ""
 
 #: followthemoney/property.py:169
 msgid "Invalid value"
@@ -84,15 +84,15 @@
 #. Address.properties.postOfficeBox.label
 #: followthemoney/schema/Address.yaml
 msgid "PO Box"
 msgstr ""
 
 #. Address.properties.postOfficeBox.description
 #: followthemoney/schema/Address.yaml
-msgid "A mailbox indentifier at the post office"
+msgid "A mailbox identifier at the post office"
 msgstr ""
 
 #. Address.properties.street.label
 #: followthemoney/schema/Address.yaml
 msgid "Street address"
 msgstr ""
 
@@ -475,14 +475,24 @@
 msgstr ""
 
 #. BankAccount.properties.accountType.label
 #: followthemoney/schema/BankAccount.yaml
 msgid "Account type"
 msgstr ""
 
+#. BankAccount.properties.openingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Opening date"
+msgstr ""
+
+#. BankAccount.properties.closingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Closing date"
+msgstr ""
+
 #. BankAccount.properties.balance.label
 #. CryptoWallet.properties.balance.label
 #: followthemoney/schema/BankAccount.yaml
 #: followthemoney/schema/CryptoWallet.yaml
 msgid "Balance"
 msgstr ""
 
@@ -568,28 +578,32 @@
 
 #. CallForTenders.properties.callId.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "CfT unique id"
 msgstr ""
 
 #. CallForTenders.properties.title.label
+#. Contract.properties.title.label
 #. Document.properties.title.label
 #. Person.properties.title.label
 #: followthemoney/schema/CallForTenders.yaml
-#: followthemoney/schema/Document.yaml followthemoney/schema/Person.yaml
+#: followthemoney/schema/Contract.yaml followthemoney/schema/Document.yaml
+#: followthemoney/schema/Person.yaml
 msgid "Title"
 msgstr ""
 
 #. CallForTenders.properties.authority.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Name of contracting authority"
 msgstr ""
 
 #. CallForTenders.properties.authority.reverse.label
+#. ContractAward.properties.callForTenders.label
 #: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
 msgid "Call For Tenders"
 msgstr ""
 
 #. CallForTenders.properties.authorityReferenceId.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Contracting authority reference ID"
 msgstr ""
@@ -636,31 +650,35 @@
 
 #. CallForTenders.properties.involvesOutcome.description
 #: followthemoney/schema/CallForTenders.yaml
 msgid "The nature of the contractual agreement that will result from this CfT"
 msgstr ""
 
 #. CallForTenders.properties.cpvCode.label
+#. ContractAward.properties.cpvCode.label
 #: followthemoney/schema/CallForTenders.yaml
-msgid "CPV codes"
+#: followthemoney/schema/ContractAward.yaml
+msgid "CPV code"
 msgstr ""
 
 #. CallForTenders.properties.cpvCode.description
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Common Procurement Vocabulary (CPV)"
 msgstr ""
 
 #. CallForTenders.properties.reverseAuctionsIncluded.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Inclusion of e-Auctions"
 msgstr ""
 
 #. CallForTenders.properties.nutsCode.label
+#. ContractAward.properties.nutsCode.label
 #: followthemoney/schema/CallForTenders.yaml
-msgid "NUTS codes"
+#: followthemoney/schema/ContractAward.yaml
+msgid "NUTS code"
 msgstr ""
 
 #. CallForTenders.properties.nutsCode.description
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Nomenclature of Territorial Units for Statistics (NUTS)"
 msgstr ""
 
@@ -816,14 +834,21 @@
 msgstr ""
 
 #. Company.properties.coatoCode.label
 #: followthemoney/schema/Company.yaml
 msgid "COATO / SOATO / OKATO"
 msgstr ""
 
+#. Company.properties.coatoCode.description
+#: followthemoney/schema/Company.yaml
+msgid ""
+"Soviet classifier for territories, regions, districts, villages. Aka. "
+"SOATO and same as OKATO"
+msgstr ""
+
 #. Company.properties.irsCode.label
 #: followthemoney/schema/Company.yaml
 msgid "IRS Number"
 msgstr ""
 
 #. Company.properties.irsCode.description
 #: followthemoney/schema/Company.yaml
@@ -950,15 +975,33 @@
 #. Company.properties.oksmCode.label
 #: followthemoney/schema/Company.yaml
 msgid "OKSM"
 msgstr ""
 
 #. Company.properties.oksmCode.description
 #: followthemoney/schema/Company.yaml
-msgid "Russian (ОКСМ) countries classifer"
+msgid "Russian (ОКСМ) countries classifier"
+msgstr ""
+
+#. Company.properties.isinCode.label
+#. Security.properties.isin.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "ISIN"
+msgstr ""
+
+#. Company.properties.isinCode.description
+#. Security.properties.isin.description
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "International Securities Identification Number"
+msgstr ""
+
+#. Company.properties.ticker.label
+#. Security.properties.ticker.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "Stock ticker symbol"
 msgstr ""
 
 #. Contract.label
 #. ContractAward.properties.contract.label
 #. EconomicActivity.properties.contract.label
 #. Payment.properties.contract.label
 #: followthemoney/schema/Contract.yaml followthemoney/schema/ContractAward.yaml
@@ -977,19 +1020,14 @@
 #. Contract.description
 #: followthemoney/schema/Contract.yaml
 msgid ""
 "An contract or contract lot issued by an authority. Multiple lots may be "
 "awarded to different suppliers (see ContractAward).\n"
 msgstr ""
 
-#. Contract.properties.title.label
-#: followthemoney/schema/Contract.yaml
-msgid "Contract title"
-msgstr ""
-
 #. Contract.properties.authority.label
 #: followthemoney/schema/Contract.yaml
 msgid "Contract authority"
 msgstr ""
 
 #. Contract.properties.authority.plural
 #: followthemoney/schema/Contract.yaml
@@ -1135,19 +1173,14 @@
 msgstr ""
 
 #. ContractAward.properties.contract.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lots awarded"
 msgstr ""
 
-#. ContractAward.properties.callForTenders.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "Call For Tender"
-msgstr ""
-
 #. ContractAward.properties.callForTenders.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Awards"
 msgstr ""
 
 #. ContractAward.properties.lotNumber.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1167,29 +1200,19 @@
 msgstr ""
 
 #. ContractAward.properties.decisionReason.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Decision reason"
 msgstr ""
 
-#. ContractAward.properties.cpvCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "CPV code"
-msgstr ""
-
 #. ContractAward.properties.cpvCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Procurement Vocabulary (what type of goods/services, EU)"
 msgstr ""
 
-#. ContractAward.properties.nutsCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "NUTS code"
-msgstr ""
-
 #. ContractAward.properties.nutsCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Nomencalture of Territorial Units for Statistics (NUTS)"
 msgstr ""
 
 #. ContractAward.properties.amended.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1541,14 +1564,24 @@
 msgstr ""
 
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr ""
 
+#. Document.properties.processingAgent.label
+#: followthemoney/schema/Document.yaml
+msgid "Name and version of the processing agent used to process the Document"
+msgstr ""
+
+#. Document.properties.processedAt.label
+#: followthemoney/schema/Document.yaml
+msgid "Date and time of the most recent ingestion of the Document"
+msgstr ""
+
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr ""
 
 #. Documentation.plural
 #: followthemoney/schema/Documentation.yml
@@ -1674,22 +1707,14 @@
 #: followthemoney/schema/EconomicActivity.yaml
 msgid ""
 "(Описание кода ТН ВЭД) Foreign Economic Activity Commodity Code "
 "description"
 msgstr ""
 
 #. EconomicActivity.properties.goodsDescription.label
-#. Interval.properties.description.label
-#. Thing.properties.description.label
-#: followthemoney/schema/EconomicActivity.yaml
-#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
-msgid "Description"
-msgstr ""
-
-#. EconomicActivity.properties.goodsDescription.description
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Description of goods"
 msgstr ""
 
 #. EconomicActivity.properties.declarant.label
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Declarant"
@@ -2203,14 +2228,20 @@
 
 #. Interval.properties.summary.label
 #. Thing.properties.summary.label
 #: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
 msgid "Summary"
 msgstr ""
 
+#. Interval.properties.description.label
+#. Thing.properties.description.label
+#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
+msgid "Description"
+msgstr ""
+
 #. Interval.properties.recordId.label
 #: followthemoney/schema/Interval.yaml
 msgid "Record ID"
 msgstr ""
 
 #. Interval.properties.sourceUrl.label
 #. Thing.properties.sourceUrl.label
@@ -2645,15 +2676,15 @@
 msgstr ""
 
 #. Organization.description
 #: followthemoney/schema/Organization.yaml
 msgid ""
 "Any type of incorporated entity that cannot be owned by another (see "
 "Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
+"enterprises, depending on their  jurisdiction.\n"
 msgstr ""
 
 #. Ownership.label
 #: followthemoney/schema/Ownership.yaml
 msgid "Ownership"
 msgstr ""
 
@@ -3022,16 +3053,17 @@
 
 #. Post.properties.holder.reverse.label
 #: followthemoney/schema/Post.yaml
 msgid "Posts held"
 msgstr ""
 
 #. Post.properties.wikidataId.label
-#: followthemoney/schema/Post.yaml
-msgid "Wikidata ID of the post"
+#. Thing.properties.wikidataId.label
+#: followthemoney/schema/Post.yaml followthemoney/schema/Thing.yaml
+msgid "Wikidata ID"
 msgstr ""
 
 #. Project.plural
 #. ProjectParticipant.properties.participant.reverse.label
 #: followthemoney/schema/Project.yaml
 #: followthemoney/schema/ProjectParticipant.yaml
 msgid "Projects"
@@ -3262,29 +3294,14 @@
 msgstr ""
 
 #. Security.description
 #: followthemoney/schema/Security.yaml
 msgid "A tradeable financial asset."
 msgstr ""
 
-#. Security.properties.isin.label
-#: followthemoney/schema/Security.yaml
-msgid "ISIN"
-msgstr ""
-
-#. Security.properties.isin.description
-#: followthemoney/schema/Security.yaml
-msgid "International Securities Identification Number"
-msgstr ""
-
-#. Security.properties.ticker.label
-#: followthemoney/schema/Security.yaml
-msgid "Ticker"
-msgstr ""
-
 #. Security.properties.issuer.label
 #: followthemoney/schema/Security.yaml
 msgid "Issuer"
 msgstr ""
 
 #. Security.properties.issuer.reverse.label
 #: followthemoney/schema/Security.yaml
@@ -3482,19 +3499,14 @@
 msgstr ""
 
 #. Thing.properties.wikipediaUrl.label
 #: followthemoney/schema/Thing.yaml
 msgid "Wikipedia Article"
 msgstr ""
 
-#. Thing.properties.wikidataId.label
-#: followthemoney/schema/Thing.yaml
-msgid "Wikidata ID"
-msgstr ""
-
 #. Thing.properties.keywords.label
 #: followthemoney/schema/Thing.yaml
 msgid "Keywords"
 msgstr ""
 
 #. Thing.properties.topics.label
 #: followthemoney/schema/Thing.yaml followthemoney/types/topic.py:22
@@ -4094,15 +4106,15 @@
 msgstr ""
 
 #: followthemoney/types/topic.py:48
 msgid "Financial advisor"
 msgstr ""
 
 #: followthemoney/types/topic.py:49
-msgid "Politician"
+msgid "Political"
 msgstr ""
 
 #: followthemoney/types/topic.py:50
 msgid "Close Associate"
 msgstr ""
 
 #: followthemoney/types/topic.py:51
@@ -4158,18 +4170,22 @@
 msgstr ""
 
 #: followthemoney/types/topic.py:65
 msgid "Sanctioned entity"
 msgstr ""
 
 #: followthemoney/types/topic.py:66
-msgid "Debarred entity"
+msgid "Sanction-linked entity"
 msgstr ""
 
 #: followthemoney/types/topic.py:67
+msgid "Debarred entity"
+msgstr ""
+
+#: followthemoney/types/topic.py:68
 msgid "Person of interest"
 msgstr ""
 
 #: followthemoney/types/url.py:22
 msgid "URL"
 msgstr ""
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-11-21 13:57+0100\n"
-"PO-Revision-Date: 2022-11-21 11:38+0000\n"
-"Last-Translator: jen occrp, 2022\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
+"PO-Revision-Date: 2021-05-07 13:11+0000\n"
+"Last-Translator: jen occrp, 2023\n"
 "Language: ru\n"
-"Language-Team: Russian (https://www.transifex.com/aleph/teams/76591/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/aleph/teams/76591/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(ЕС) Регистрационный номер плательщика НДС"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Классификатор экономической деятельности"
 
@@ -101,17 +101,14 @@
 msgstr ""
 "Связь между двумя предположительно тождественными сущностями, например, в "
 "результате вероятностного сопоставления записей.\n"
 
 msgid "A location associated with an entity.\n"
 msgstr "Местоположение, ассоциированное с сущностью.\n"
 
-msgid "A mailbox indentifier at the post office"
-msgstr "Номер абонентского ящика в почтовом отделении"
-
 msgid ""
 "A mediatory, intermediary, middleman, or broker acting on behalf of a legal "
 "entity."
 msgstr "Медиатор, посредник или брокер юридического лица"
 
 msgid "A monetary debt between two parties."
 msgstr "Кредитно-денежные отношения двух сторон."
@@ -314,23 +311,14 @@
 "Any party to legal proceedings, such as asset ownership, corporate "
 "governance or social interactions. Often used when raw data does not specify "
 "if something is a person or company.\n"
 msgstr ""
 "Любой участник судопроизводства, как то: владения (активами), корпоративного "
 "контроля или социального взаимодействия.\n"
 
-msgid ""
-"Any type of incorporated entity that cannot be owned by another (see "
-"Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
-msgstr ""
-"Любой тип юридического лица, который не может быть объектом собственности "
-"(см. Компания). Например, благотворительные организации, фонды или "
-"государственные предприятия, в зависимости от юрисдикции.\n"
-
 msgid "Area"
 msgstr "Участок"
 
 msgid "Article"
 msgstr "Статья"
 
 msgid "Articles"
@@ -467,32 +455,26 @@
 
 msgid "COD CAEM"
 msgstr "CAEM-код"
 
 msgid "CPV code"
 msgstr "CPV-код"
 
-msgid "CPV codes"
-msgstr "CPV-код"
-
 msgid "CRS Number"
 msgstr "Номер береговой радиостанции"
 
 msgid "CSV alternative version checksum"
 msgstr "Дополнительная контрольная сумма для CSV"
 
 msgid "Cadastral code"
 msgstr "Кадастровый код"
 
 msgid "Call"
 msgstr "Звонок"
 
-msgid "Call For Tender"
-msgstr "Тендер"
-
 msgid "Call For Tenders"
 msgstr "Тендер"
 
 msgid "Call Sign"
 msgstr "Позывной"
 
 msgid "Call for tenders"
@@ -584,14 +566,17 @@
 
 msgid "Close Associate"
 msgstr "Тесно связанное лицо"
 
 msgid "Close date"
 msgstr "Дата закрытия"
 
+msgid "Closing date"
+msgstr "Дата закрытия"
+
 msgid "Co-occurring countries"
 msgstr "Совместно встречающиеся страны"
 
 msgid "Co-occurring e-mail addresses"
 msgstr "Совместно встречающиеся эл. адреса"
 
 msgid "Co-occurring phone numbers"
@@ -659,17 +644,14 @@
 
 msgid "Contract notice date"
 msgstr "Дата заключения контракта"
 
 msgid "Contract procedure"
 msgstr "Процедура присуждения контракта"
 
-msgid "Contract title"
-msgstr "Наименование контракта"
-
 msgid "Contracting authority reference ID"
 msgstr "Регистрационный номер заказчика"
 
 msgid "Contracts"
 msgstr "Контракты"
 
 msgid "Contracts awarded"
@@ -1159,14 +1141,17 @@
 
 msgid "Goods originated"
 msgstr "Отправитель товаров"
 
 msgid "Goods received"
 msgstr "Получатель товаров"
 
+msgid "Google Places ID"
+msgstr "Google Places ID"
+
 msgid "Government"
 msgstr "Правительство"
 
 msgid "Gross Registered Tonnage"
 msgstr "Брутто-регистровый тоннаж"
 
 msgid "HTML"
@@ -1207,14 +1192,17 @@
 
 msgid "IMO Number"
 msgstr "Номер ИМО"
 
 msgid "INN"
 msgstr "ИНН"
 
+msgid "IP address"
+msgstr "IP-адрес"
+
 msgid "IP-Address"
 msgstr "IP-адрес"
 
 msgid "IP-Addresses"
 msgstr "IP-адреса"
 
 msgid "IPO"
@@ -1526,17 +1514,14 @@
 
 msgid "Municipal government"
 msgstr "Муниципальные власти"
 
 msgid "NUTS code"
 msgstr "NUTS-код"
 
-msgid "NUTS codes"
-msgstr "NUTS-код"
-
 msgid "Nagorno-Karabakh"
 msgstr "Нагорный Карабах"
 
 msgid "Name"
 msgstr "Имя"
 
 msgid "Name of contracting authority"
@@ -1632,14 +1617,20 @@
 
 msgid "Oligarch"
 msgstr "Олигарх"
 
 msgid "OpenCorporates URL"
 msgstr "Ссылка на OpenCorporates"
 
+msgid "OpenStreetmap Place ID"
+msgstr "OpenStreetmap ID места"
+
+msgid "Opening date"
+msgstr "Дата открытия"
+
 msgid "Operator"
 msgstr "Оператор"
 
 msgid "Organization"
 msgstr "Организация"
 
 msgid "Organizations"
@@ -1797,17 +1788,14 @@
 
 msgid "Political association"
 msgstr "Политическая ассоциация"
 
 msgid "Political party"
 msgstr "Политическая партия"
 
-msgid "Politician"
-msgstr "Политик"
-
 msgid "Port of Registration"
 msgstr "Порт приписки"
 
 msgid "Position"
 msgstr "Должность"
 
 msgid "Post"
@@ -1989,17 +1977,14 @@
 
 msgid "Role"
 msgstr "Роль, функция"
 
 msgid "Rouble bank"
 msgstr "Наименование банка (рубли)"
 
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Общероссийский классификатор стран мира"
-
 msgid "Russian bank account code"
 msgstr "Банковский идентификационный код"
 
 msgid "Russian company ID"
 msgstr "Идентификационный номер налогоплательщика"
 
 msgid "Russian industry classifier"
@@ -2265,17 +2250,14 @@
 
 msgid "Thread topic"
 msgstr "Тема ветви дискуссии"
 
 msgid "Tibet"
 msgstr "Тибет"
 
-msgid "Ticker"
-msgstr "Тикер"
-
 msgid "Title"
 msgstr "Название"
 
 msgid "Title number"
 msgstr "Номер свидетельства о праве собственности"
 
 msgid "To"
@@ -2446,17 +2428,14 @@
 
 msgid "Website address"
 msgstr "Адрес сайта"
 
 msgid "Wikidata ID"
 msgstr "Wikidata ID"
 
-msgid "Wikidata ID of the post"
-msgstr "Wikidata ID должности"
-
 msgid "Wikipedia Article"
 msgstr "Статья в Википедии"
 
 msgid "Workbook"
 msgstr "Рабочая тетрадь"
 
 msgid "Workbooks"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 # jen occrp, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-10 14:09+0100\n"
+"POT-Creation-Date: 2023-06-23 10:41+0200\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: jen occrp, 2023\n"
-"Language-Team: Russian (https://www.transifex.com/aleph/teams/76591/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/aleph/teams/76591/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr "Не удалось сохранить свойство"
 
@@ -90,16 +90,16 @@
 #. Address.properties.postOfficeBox.label
 #: followthemoney/schema/Address.yaml
 msgid "PO Box"
 msgstr "Абонентский ящик"
 
 #. Address.properties.postOfficeBox.description
 #: followthemoney/schema/Address.yaml
-msgid "A mailbox indentifier at the post office"
-msgstr "Номер абонентского ящика в почтовом отделении"
+msgid "A mailbox identifier at the post office"
+msgstr ""
 
 #. Address.properties.street.label
 #: followthemoney/schema/Address.yaml
 msgid "Street address"
 msgstr "Адрес (улица)"
 
 #. Address.properties.street2.label
@@ -593,28 +593,32 @@
 
 #. CallForTenders.properties.callId.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "CfT unique id"
 msgstr "ID тендера"
 
 #. CallForTenders.properties.title.label
+#. Contract.properties.title.label
 #. Document.properties.title.label
 #. Person.properties.title.label
 #: followthemoney/schema/CallForTenders.yaml
-#: followthemoney/schema/Document.yaml followthemoney/schema/Person.yaml
+#: followthemoney/schema/Contract.yaml followthemoney/schema/Document.yaml
+#: followthemoney/schema/Person.yaml
 msgid "Title"
 msgstr "Название"
 
 #. CallForTenders.properties.authority.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Name of contracting authority"
 msgstr "Наименование заказчика"
 
 #. CallForTenders.properties.authority.reverse.label
+#. ContractAward.properties.callForTenders.label
 #: followthemoney/schema/CallForTenders.yaml
+#: followthemoney/schema/ContractAward.yaml
 msgid "Call For Tenders"
 msgstr "Тендер"
 
 #. CallForTenders.properties.authorityReferenceId.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Contracting authority reference ID"
 msgstr "Регистрационный номер заказчика"
@@ -661,31 +665,35 @@
 
 #. CallForTenders.properties.involvesOutcome.description
 #: followthemoney/schema/CallForTenders.yaml
 msgid "The nature of the contractual agreement that will result from this CfT"
 msgstr "Характер договорного соглашения вследствие завершения данного тендера"
 
 #. CallForTenders.properties.cpvCode.label
+#. ContractAward.properties.cpvCode.label
 #: followthemoney/schema/CallForTenders.yaml
-msgid "CPV codes"
+#: followthemoney/schema/ContractAward.yaml
+msgid "CPV code"
 msgstr "CPV-код"
 
 #. CallForTenders.properties.cpvCode.description
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Common Procurement Vocabulary (CPV)"
 msgstr "Товарная классификация (CPV)"
 
 #. CallForTenders.properties.reverseAuctionsIncluded.label
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Inclusion of e-Auctions"
 msgstr "Включает электронный аукцион"
 
 #. CallForTenders.properties.nutsCode.label
+#. ContractAward.properties.nutsCode.label
 #: followthemoney/schema/CallForTenders.yaml
-msgid "NUTS codes"
+#: followthemoney/schema/ContractAward.yaml
+msgid "NUTS code"
 msgstr "NUTS-код"
 
 #. CallForTenders.properties.nutsCode.description
 #: followthemoney/schema/CallForTenders.yaml
 msgid "Nomenclature of Territorial Units for Statistics (NUTS)"
 msgstr "Номенклатура территориальных единиц (NUTS)"
 
@@ -847,14 +855,21 @@
 msgstr "Номер налогоплательщика в Азербайжане"
 
 #. Company.properties.coatoCode.label
 #: followthemoney/schema/Company.yaml
 msgid "COATO / SOATO / OKATO"
 msgstr "ОКАТО"
 
+#. Company.properties.coatoCode.description
+#: followthemoney/schema/Company.yaml
+msgid ""
+"Soviet classifier for territories, regions, districts, villages. Aka. SOATO "
+"and same as OKATO"
+msgstr ""
+
 #. Company.properties.irsCode.label
 #: followthemoney/schema/Company.yaml
 msgid "IRS Number"
 msgstr "ИНН"
 
 #. Company.properties.irsCode.description
 #: followthemoney/schema/Company.yaml
@@ -984,16 +999,34 @@
 #. Company.properties.oksmCode.label
 #: followthemoney/schema/Company.yaml
 msgid "OKSM"
 msgstr "ОКСМ"
 
 #. Company.properties.oksmCode.description
 #: followthemoney/schema/Company.yaml
-msgid "Russian (ОКСМ) countries classifer"
-msgstr "Общероссийский классификатор стран мира"
+msgid "Russian (ОКСМ) countries classifier"
+msgstr ""
+
+#. Company.properties.isinCode.label
+#. Security.properties.isin.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "ISIN"
+msgstr "ISIN-код"
+
+#. Company.properties.isinCode.description
+#. Security.properties.isin.description
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "International Securities Identification Number"
+msgstr "Международный идентификационный код ценной бумаги"
+
+#. Company.properties.ticker.label
+#. Security.properties.ticker.label
+#: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
+msgid "Stock ticker symbol"
+msgstr ""
 
 #. Contract.label
 #. ContractAward.properties.contract.label
 #. EconomicActivity.properties.contract.label
 #. Payment.properties.contract.label
 #: followthemoney/schema/Contract.yaml
 #: followthemoney/schema/ContractAward.yaml
@@ -1016,19 +1049,14 @@
 "An contract or contract lot issued by an authority. Multiple lots may be "
 "awarded to different suppliers (see ContractAward).\n"
 msgstr ""
 "Контракт или лот, размещённый гос. органом. Исполнителями отдельных лотов в "
 "рамках одного контракта могут быть определены различные поставщики (см. "
 "Контракты).\n"
 
-#. Contract.properties.title.label
-#: followthemoney/schema/Contract.yaml
-msgid "Contract title"
-msgstr "Наименование контракта"
-
 #. Contract.properties.authority.label
 #: followthemoney/schema/Contract.yaml
 msgid "Contract authority"
 msgstr "Заказчик"
 
 #. Contract.properties.authority.plural
 #: followthemoney/schema/Contract.yaml
@@ -1176,19 +1204,14 @@
 msgstr "Получено контрактов"
 
 #. ContractAward.properties.contract.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Lots awarded"
 msgstr "Лоты"
 
-#. ContractAward.properties.callForTenders.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "Call For Tender"
-msgstr "Тендер"
-
 #. ContractAward.properties.callForTenders.reverse.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Awards"
 msgstr "Гос. контракты"
 
 #. ContractAward.properties.lotNumber.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1208,29 +1231,19 @@
 msgstr "Тип документа"
 
 #. ContractAward.properties.decisionReason.label
 #: followthemoney/schema/ContractAward.yaml
 msgid "Decision reason"
 msgstr "Причина решения"
 
-#. ContractAward.properties.cpvCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "CPV code"
-msgstr "CPV-код"
-
 #. ContractAward.properties.cpvCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Contract Procurement Vocabulary (what type of goods/services, EU)"
 msgstr "Единый закупочный классификатор (классификация товаров/услуг, ЕС)"
 
-#. ContractAward.properties.nutsCode.label
-#: followthemoney/schema/ContractAward.yaml
-msgid "NUTS code"
-msgstr "NUTS-код"
-
 #. ContractAward.properties.nutsCode.description
 #: followthemoney/schema/ContractAward.yaml
 msgid "Nomencalture of Territorial Units for Statistics (NUTS)"
 msgstr "Номенклатура территориальных единиц (NUTS)"
 
 #. ContractAward.properties.amended.label
 #: followthemoney/schema/ContractAward.yaml
@@ -1584,14 +1597,24 @@
 msgstr "Статус обработки"
 
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr "Ошибка обработки"
 
+#. Document.properties.processingAgent.label
+#: followthemoney/schema/Document.yaml
+msgid "Name and version of the processing agent used to process the Document"
+msgstr ""
+
+#. Document.properties.processedAt.label
+#: followthemoney/schema/Document.yaml
+msgid "Date and time of the most recent ingestion of the Document"
+msgstr ""
+
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr "Документация"
 
 #. Documentation.plural
 #: followthemoney/schema/Documentation.yml
@@ -2700,19 +2723,16 @@
 msgstr "Организации"
 
 #. Organization.description
 #: followthemoney/schema/Organization.yaml
 msgid ""
 "Any type of incorporated entity that cannot be owned by another (see "
 "Company). This might include charities, foundations or state-owned "
-"enterprises, depending on their  juristiction.\n"
+"enterprises, depending on their  jurisdiction.\n"
 msgstr ""
-"Любой тип юридического лица, который не может быть объектом собственности "
-"(см. Компания). Например, благотворительные организации, фонды или "
-"государственные предприятия, в зависимости от юрисдикции.\n"
 
 #. Ownership.label
 #: followthemoney/schema/Ownership.yaml
 msgid "Ownership"
 msgstr "Структура собственности"
 
 #. Ownership.plural
@@ -3084,17 +3104,18 @@
 
 #. Post.properties.holder.reverse.label
 #: followthemoney/schema/Post.yaml
 msgid "Posts held"
 msgstr "Занимаемые должности"
 
 #. Post.properties.wikidataId.label
-#: followthemoney/schema/Post.yaml
-msgid "Wikidata ID of the post"
-msgstr "Wikidata ID должности"
+#. Thing.properties.wikidataId.label
+#: followthemoney/schema/Post.yaml followthemoney/schema/Thing.yaml
+msgid "Wikidata ID"
+msgstr "Wikidata ID"
 
 #. Project.plural
 #. ProjectParticipant.properties.participant.reverse.label
 #: followthemoney/schema/Project.yaml
 #: followthemoney/schema/ProjectParticipant.yaml
 msgid "Projects"
 msgstr "Проекты"
@@ -3329,29 +3350,14 @@
 msgstr "Ценные бумаги"
 
 #. Security.description
 #: followthemoney/schema/Security.yaml
 msgid "A tradeable financial asset."
 msgstr "Котируемый финансовый актив."
 
-#. Security.properties.isin.label
-#: followthemoney/schema/Security.yaml
-msgid "ISIN"
-msgstr "ISIN-код"
-
-#. Security.properties.isin.description
-#: followthemoney/schema/Security.yaml
-msgid "International Securities Identification Number"
-msgstr "Международный идентификационный код ценной бумаги"
-
-#. Security.properties.ticker.label
-#: followthemoney/schema/Security.yaml
-msgid "Ticker"
-msgstr "Тикер"
-
 #. Security.properties.issuer.label
 #: followthemoney/schema/Security.yaml
 msgid "Issuer"
 msgstr "Эмитент"
 
 #. Security.properties.issuer.reverse.label
 #: followthemoney/schema/Security.yaml
@@ -3553,19 +3559,14 @@
 msgstr "Другое название"
 
 #. Thing.properties.wikipediaUrl.label
 #: followthemoney/schema/Thing.yaml
 msgid "Wikipedia Article"
 msgstr "Статья в Википедии"
 
-#. Thing.properties.wikidataId.label
-#: followthemoney/schema/Thing.yaml
-msgid "Wikidata ID"
-msgstr "Wikidata ID"
-
 #. Thing.properties.keywords.label
 #: followthemoney/schema/Thing.yaml
 msgid "Keywords"
 msgstr "Ключевые слова"
 
 #. Thing.properties.topics.label
 #: followthemoney/schema/Thing.yaml followthemoney/types/topic.py:22
@@ -4167,16 +4168,16 @@
 msgstr "Фонд"
 
 #: followthemoney/types/topic.py:48
 msgid "Financial advisor"
 msgstr "Финансовый консультант"
 
 #: followthemoney/types/topic.py:49
-msgid "Politician"
-msgstr "Политик"
+msgid "Political"
+msgstr ""
 
 #: followthemoney/types/topic.py:50
 msgid "Close Associate"
 msgstr "Тесно связанное лицо"
 
 #: followthemoney/types/topic.py:51
 msgid "Judge"
@@ -4231,18 +4232,22 @@
 msgstr "Замороженный актив"
 
 #: followthemoney/types/topic.py:65
 msgid "Sanctioned entity"
 msgstr "Объект санкций"
 
 #: followthemoney/types/topic.py:66
+msgid "Sanction-linked entity"
+msgstr ""
+
+#: followthemoney/types/topic.py:67
 msgid "Debarred entity"
 msgstr "Физическое или юридическое лицо, лишённое полномочий"
 
-#: followthemoney/types/topic.py:67
+#: followthemoney/types/topic.py:68
 msgid "Person of interest"
 msgstr "Подозрительный персонаж"
 
 #: followthemoney/types/url.py:22
 msgid "URL"
 msgstr "Ссылка"
```

### Comparing `followthemoney-3.4.1/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/__init__.py` & `followthemoney-3.4.2/followthemoney/types/__init__.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/address.py` & `followthemoney-3.4.2/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/checksum.py` & `followthemoney-3.4.2/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/common.py` & `followthemoney-3.4.2/followthemoney/types/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/country.py` & `followthemoney-3.4.2/followthemoney/types/country.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/date.py` & `followthemoney-3.4.2/followthemoney/types/date.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/email.py` & `followthemoney-3.4.2/followthemoney/types/email.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/entity.py` & `followthemoney-3.4.2/followthemoney/types/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/gender.py` & `followthemoney-3.4.2/followthemoney/types/gender.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/iban.py` & `followthemoney-3.4.2/followthemoney/types/iban.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/identifier.py` & `followthemoney-3.4.2/followthemoney/types/identifier.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/ip.py` & `followthemoney-3.4.2/followthemoney/types/ip.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/json.py` & `followthemoney-3.4.2/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/language.py` & `followthemoney-3.4.2/followthemoney/types/language.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/mimetype.py` & `followthemoney-3.4.2/followthemoney/types/mimetype.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/name.py` & `followthemoney-3.4.2/followthemoney/types/name.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/number.py` & `followthemoney-3.4.2/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/phone.py` & `followthemoney-3.4.2/followthemoney/types/phone.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/registry.py` & `followthemoney-3.4.2/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/string.py` & `followthemoney-3.4.2/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/topic.py` & `followthemoney-3.4.2/followthemoney/types/topic.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/types/url.py` & `followthemoney-3.4.2/followthemoney/types/url.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney/util.py` & `followthemoney-3.4.2/followthemoney/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.4.2/followthemoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.1
+Version: 3.4.2
+Summary: UNKNOWN
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -84,7 +86,9 @@
 This will create a new patch release and upload a distribution of it. If
 the changes are more significant, you can run `bumpversion` with the `minor`
 or `major` arguments.
 
 When the schema is updated, please update the docs, ideally including the
 diagrams. For the RDF namespace and JavaScript version of the model, 
 run `make generate`.
+
+
```

### Comparing `followthemoney-3.4.1/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.4.2/followthemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.4.2/followthemoney.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 csv = followthemoney.cli.exports:export_csv
 cypher = followthemoney.cli.exports:export_cypher
 excel = followthemoney.cli.exports:export_excel
 gexf = followthemoney.cli.exports:export_gexf
 mapping = followthemoney.cli.mapping:run_mapping
 rdf = followthemoney.cli.exports:export_rdf
 sieve = followthemoney.cli.sieve:sieve
+
```

### Comparing `followthemoney-3.4.1/followthemoney.egg-info/requires.txt` & `followthemoney-3.4.2/followthemoney.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.1/setup.py` & `followthemoney-3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.4.1",
+    version="3.4.2",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
```

