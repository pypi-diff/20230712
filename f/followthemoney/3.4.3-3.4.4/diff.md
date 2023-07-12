# Comparing `tmp/followthemoney-3.4.3.tar.gz` & `tmp/followthemoney-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.4.3.tar", last modified: Tue Jun 27 13:59:11 2023, max compression
+gzip compressed data, was "followthemoney-3.4.4.tar", last modified: Wed Jul 12 16:39:17 2023, max compression
```

## Comparing `followthemoney-3.4.3.tar` & `followthemoney-3.4.4.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-27 13:57:18.000000 followthemoney-3.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 13:57:18.000000 followthemoney-3.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-27 13:59:11.782174 followthemoney-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-27 13:57:18.000000 followthemoney-3.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   118608 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   112813 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   112460 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   117244 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   100993 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    61741 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   132454 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:58:52.000000 followthemoney-3.4.3/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-27 13:59:11.782174 followthemoney-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-27 13:57:18.000000 followthemoney-3.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-12 16:37:14.000000 followthemoney-3.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 16:37:14.000000 followthemoney-3.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-12 16:39:17.047757 followthemoney-3.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-12 16:37:14.000000 followthemoney-3.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19866 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   118608 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112813 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112460 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   117244 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   101212 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    61971 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   132951 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:38:55.000000 followthemoney-3.4.4/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 16:39:17.047757 followthemoney-3.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-12 16:37:14.000000 followthemoney-3.4.4/setup.py
```

### Comparing `followthemoney-3.4.3/LICENSE` & `followthemoney-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/PKG-INFO` & `followthemoney-3.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.3
-Summary: UNKNOWN
+Version: 3.4.4
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -86,9 +84,7 @@
 This will create a new patch release and upload a distribution of it. If
 the changes are more significant, you can run `bumpversion` with the `minor`
 or `major` arguments.
 
 When the schema is updated, please update the docs, ideally including the
 diagrams. For the RDF namespace and JavaScript version of the model, 
 run `make generate`.
-
-
```

### Comparing `followthemoney-3.4.3/README.md` & `followthemoney-3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/cli/aggregate.py` & `followthemoney-3.4.4/followthemoney/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/cli/cli.py` & `followthemoney-3.4.4/followthemoney/cli/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/cli/exports.py` & `followthemoney-3.4.4/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/cli/mapping.py` & `followthemoney-3.4.4/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/cli/sieve.py` & `followthemoney-3.4.4/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/cli/util.py` & `followthemoney-3.4.4/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/compare.py` & `followthemoney-3.4.4/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/exc.py` & `followthemoney-3.4.4/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/export/common.py` & `followthemoney-3.4.4/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/export/csv.py` & `followthemoney-3.4.4/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/export/excel.py` & `followthemoney-3.4.4/followthemoney/export/excel.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/export/graph.py` & `followthemoney-3.4.4/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/export/neo4j.py` & `followthemoney-3.4.4/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/export/rdf.py` & `followthemoney-3.4.4/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/graph.py` & `followthemoney-3.4.4/followthemoney/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/helpers.py` & `followthemoney-3.4.4/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/mapping/csv.py` & `followthemoney-3.4.4/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/mapping/entity.py` & `followthemoney-3.4.4/followthemoney/mapping/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/mapping/property.py` & `followthemoney-3.4.4/followthemoney/mapping/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/mapping/query.py` & `followthemoney-3.4.4/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/mapping/source.py` & `followthemoney-3.4.4/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/mapping/sql.py` & `followthemoney-3.4.4/followthemoney/mapping/sql.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/messages.py` & `followthemoney-3.4.4/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/model.py` & `followthemoney-3.4.4/followthemoney/model.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/namespace.py` & `followthemoney-3.4.4/followthemoney/namespace.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/offshore.py` & `followthemoney-3.4.4/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/ontology.py` & `followthemoney-3.4.4/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/property.py` & `followthemoney-3.4.4/followthemoney/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/proxy.py` & `followthemoney-3.4.4/followthemoney/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,26 +75,30 @@
         if not cleaned:
             self.id = sanitize_text(self.id)
 
         #: If the input dictionary for the entity proxy contains fields other
         #: than ``id``, ``schema`` or ``properties``, they will be kept in here
         #: and re-added upon serialization.
         self.context = data
-        self._properties: Dict[str, Set[str]] = {}
+        self._properties: Dict[str, List[str]] = {}
         self._size = 0
 
-        for key, value in properties.items():
+        for key, values in properties.items():
             if key not in self.schema.properties:
                 continue
-            if not cleaned:
-                self.add(key, value, cleaned=cleaned, quiet=True)
+            if cleaned:
+                # This does not call `self.add` as it might be called millions of times
+                # in some context and we want to avoid the performance overhead of doing so.
+                seen: Set[str] = set()
+                seen_add = seen.add
+                unique_values = [v for v in values if not (v in seen or seen_add(v))]
+                self._properties[key] = unique_values
+                self._size += sum([len(v) for v in unique_values])
             else:
-                values = set(value)
-                self._properties[key] = values
-                self._size += sum([len(v) for v in values])
+                self.add(key, values, quiet=True)
 
     def make_id(self, *parts: Any) -> Optional[str]:
         """Generate a (hopefully unique) ID for the given entity, composed
         of the given components, and the :attr:`~key_prefix` defined in
         the proxy.
         """
         self.id = make_entity_id(*parts, key_prefix=self.key_prefix)
@@ -123,19 +127,18 @@
         :param quiet: a reference to an non-existent property will return
             an empty list instead of raising an error.
         :return: A list of values.
         """
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is None:
             return []
-        return list(self._properties.get(prop_name, []))
+        return self._properties.get(prop_name, [])
 
     def first(self, prop: P, quiet: bool = False) -> Optional[str]:
-        """Get only the first value set for the property, in no particular
-        order.
+        """Get only the first value set for the property.
 
         :param prop: can be given as a name or an instance of
             :class:`~followthemoney.property.Property`.
         :param quiet: a reference to an non-existent property will return
             an empty list instead of raising an error.
         :return: A value, or ``None``.
         """
@@ -213,16 +216,17 @@
             value_size = len(value)
             if prop.type.max_size is not None:
                 if self._size + value_size > prop.type.max_size:
                     # msg = "[%s] too large. Rejecting additional values."
                     # log.warning(msg, prop.name)
                     return None
             self._size += value_size
-            self._properties.setdefault(prop.name, set())
-            self._properties[prop.name].add(value)
+            self._properties.setdefault(prop.name, list())
+            if value not in self._properties[prop.name]:
+                self._properties[prop.name].append(value)
         return None
 
     def set(
         self,
         prop: P,
         values: Any,
         cleaned: bool = False,
@@ -271,15 +275,15 @@
         :param quiet: a reference to an non-existent property will return
             an empty list instead of raising an error.
         """
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is not None and prop_name in self._properties:
             try:
                 self._properties[prop_name].remove(value)
-            except KeyError:
+            except (KeyError, ValueError):
                 pass
 
     def iterprops(self) -> List[Property]:
         """Iterate across all the properties for which a value is set in
         the proxy (but do not return their values)."""
         return [self.schema.properties[p] for p in self._properties.keys()]
```

### Comparing `followthemoney-3.4.3/followthemoney/schema/Address.yaml` & `followthemoney-3.4.4/followthemoney/schema/Address.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Airplane.yaml` & `followthemoney-3.4.4/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.4.4/followthemoney/schema/Analyzable.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Assessment.yaml` & `followthemoney-3.4.4/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Associate.yaml` & `followthemoney-3.4.4/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.4.4/followthemoney/schema/BankAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Call.yaml` & `followthemoney-3.4.4/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.4.4/followthemoney/schema/CallForTenders.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Company.yaml` & `followthemoney-3.4.4/followthemoney/schema/Company.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Contract.yaml` & `followthemoney-3.4.4/followthemoney/schema/Contract.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.4.4/followthemoney/schema/ContractAward.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.4.4/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.4.4/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.4.4/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Debt.yaml` & `followthemoney-3.4.4/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Directorship.yaml` & `followthemoney-3.4.4/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Document.yaml` & `followthemoney-3.4.4/followthemoney/schema/Document.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Documentation.yml` & `followthemoney-3.4.4/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.4.4/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Email.yaml` & `followthemoney-3.4.4/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Employment.yaml` & `followthemoney-3.4.4/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Event.yaml` & `followthemoney-3.4.4/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Family.yaml` & `followthemoney-3.4.4/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Identification.yaml` & `followthemoney-3.4.4/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Interval.yaml` & `followthemoney-3.4.4/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.4.4/followthemoney/schema/LegalEntity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Membership.yaml` & `followthemoney-3.4.4/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Mention.yaml` & `followthemoney-3.4.4/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Message.yaml` & `followthemoney-3.4.4/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Ownership.yaml` & `followthemoney-3.4.4/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Page.yaml` & `followthemoney-3.4.4/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Passport.yaml` & `followthemoney-3.4.4/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Payment.yaml` & `followthemoney-3.4.4/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Person.yaml` & `followthemoney-3.4.4/followthemoney/schema/Person.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -36,20 +36,25 @@
     fatherName:
       label: Patronymic
     motherName:
       label: Matronymic
     lastName:
       label: Last name
       rdf: http://xmlns.com/foaf/0.1/lastName
+    nameSuffix:
+      label: Name suffix
     birthDate:
       label: Birth date
       type: date
       rdf: http://xmlns.com/foaf/0.1/birthday
     birthPlace:
       label: Place of birth
+    birthCountry:
+      label: Country of birth
+      type: country
     deathDate:
       label: Death date
       type: date
     position:
       label: Position
       matchable: false
     nationality:
```

### Comparing `followthemoney-3.4.3/followthemoney/schema/Post.yaml` & `followthemoney-3.4.4/followthemoney/schema/Post.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.4.4/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.4.4/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Representation.yaml` & `followthemoney-3.4.4/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Sanction.yaml` & `followthemoney-3.4.4/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Security.yaml` & `followthemoney-3.4.4/followthemoney/schema/Security.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Similar.yaml` & `followthemoney-3.4.4/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Succession.yaml` & `followthemoney-3.4.4/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Table.yaml` & `followthemoney-3.4.4/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.4.4/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Thing.yaml` & `followthemoney-3.4.4/followthemoney/schema/Thing.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Trip.yaml` & `followthemoney-3.4.4/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.4.4/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.4.4/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.4.4/followthemoney/schema/Vehicle.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema/Vessel.yaml` & `followthemoney-3.4.4/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/schema.py` & `followthemoney-3.4.4/followthemoney/schema.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ar\n"
 "Language-Team: Arabic (https://app.transifex.com/aleph/teams/76591/ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "الرقم الضريبي (الاتحاد الأوروبي)"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "  (RO) ما هو نوع النشاط الذي يسمح للكيان القانوني بتطويره"
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

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
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) VAT broj"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Koji tip aktivnosti legalnog entiteta je dozvoljeno razviti"
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
 "Language: de\n"
 "Language-Team: German (https://app.transifex.com/aleph/teams/76591/de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) USt-ID"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr ""
 "(RO) Die Art der wirtschaftlichen Tätigkeit, der diese Entität nachgehen darf"
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: es\n"
 "Language-Team: Spanish (https://app.transifex.com/aleph/teams/76591/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) Número VAT"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr ""
 "(RO) ¿Qué tipo de actividad se le permite desarrollar a una entidad legal?"
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: fr\n"
 "Language-Team: French (https://app.transifex.com/aleph/teams/76591/fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "Numéro de TVA intracommunautaire"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Type d’activité qu’une entité légale est autorisée à mener"
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/fr/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/messages.pot` & `followthemoney-3.4.4/followthemoney/translations/messages.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-27 15:36+0200\n"
+"POT-Creation-Date: 2023-07-12 18:31+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -25,20 +25,20 @@
 msgid "Invalid value"
 msgstr ""
 
 #: followthemoney/proxy.py:62
 msgid "No schema for entity."
 msgstr ""
 
-#: followthemoney/proxy.py:115
+#: followthemoney/proxy.py:119
 #, python-format
 msgid "Unknown property (%s): %s"
 msgstr ""
 
-#: followthemoney/proxy.py:188
+#: followthemoney/proxy.py:191
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr ""
 
 #: followthemoney/schema.py:377
 msgid "Required"
 msgstr ""
@@ -2984,14 +2984,24 @@
 msgstr ""
 
 #. Person.properties.lastName.label
 #: followthemoney/schema/Person.yaml
 msgid "Last name"
 msgstr ""
 
+#. Person.properties.nameSuffix.label
+#: followthemoney/schema/Person.yaml
+msgid "Name suffix"
+msgstr ""
+
+#. Person.properties.birthCountry.label
+#: followthemoney/schema/Person.yaml
+msgid "Country of birth"
+msgstr ""
+
 #. Person.properties.deathDate.label
 #: followthemoney/schema/Person.yaml
 msgid "Death date"
 msgstr ""
 
 #. Person.properties.position.label
 #: followthemoney/schema/Person.yaml
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-23 10:41+0200\n"
+"POT-Creation-Date: 2023-06-27 15:36+0200\n"
 "PO-Revision-Date: 2022-11-21 11:38+0000\n"
 "Last-Translator: jen occrp, 2023\n"
 "Language: ru\n"
 "Language-Team: Russian (https://app.transifex.com/aleph/teams/76591/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "(EU) VAT number"
 msgstr "(ЕС) Регистрационный номер плательщика НДС"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Классификатор экономической деятельности"
 
@@ -812,14 +812,17 @@
 
 msgid "Date of publishing"
 msgstr "Дата публикации"
 
 msgid "Dates"
 msgstr "Даты"
 
+msgid "De-registration Date"
+msgstr "Дата снятия с регистрации"
+
 msgid "Death date"
 msgstr "Дата смерти"
 
 msgid "Debarred entity"
 msgstr "Физическое или юридическое лицо, лишённое полномочий"
 
 msgid "Debt"
@@ -1848,14 +1851,20 @@
 
 msgid "Procedure"
 msgstr "Процедура"
 
 msgid "Procedure number"
 msgstr "Номер процедуры"
 
+msgid "Processed at"
+msgstr "Дата обработки документа"
+
+msgid "Processing agent"
+msgstr "Документ обработан"
+
 msgid "Processing error"
 msgstr "Ошибка обработки"
 
 msgid "Processing status"
 msgstr "Статус обработки"
 
 msgid "Procurement method"
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 # jen occrp, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-23 10:41+0200\n"
+"POT-Creation-Date: 2023-06-27 15:36+0200\n"
 "PO-Revision-Date: 2022-11-21 11:38+0000\n"
 "Last-Translator: jen occrp, 2023\n"
 "Language-Team: Russian (https://app.transifex.com/aleph/teams/76591/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: followthemoney/property.py:166
+#: followthemoney/property.py:165
 msgid "Property cannot be written"
 msgstr "Не удалось сохранить свойство"
 
-#: followthemoney/property.py:169
+#: followthemoney/property.py:168
 msgid "Invalid value"
 msgstr "Недопустимое значение"
 
 #: followthemoney/proxy.py:62
 msgid "No schema for entity."
 msgstr "Для сущности отсутствует схема."
 
@@ -41,19 +41,19 @@
 msgstr "Неизвестный параметр (1%s): 1%s"
 
 #: followthemoney/proxy.py:188
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr "Неизвестное свойство (1%s): 1%s"
 
-#: followthemoney/schema.py:373
+#: followthemoney/schema.py:377
 msgid "Required"
 msgstr "Обязательное значение"
 
-#: followthemoney/schema.py:377
+#: followthemoney/schema.py:381
 msgid "Entity validation failed"
 msgstr "Сущность не прошла валидацию"
 
 #. Address.label
 #. CryptoWallet.properties.publicKey.label
 #. Thing.properties.address.label
 #. Thing.properties.addressEntity.label
@@ -1601,19 +1601,29 @@
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr "Ошибка обработки"
 
 #. Document.properties.processingAgent.label
 #: followthemoney/schema/Document.yaml
+msgid "Processing agent"
+msgstr "Документ обработан"
+
+#. Document.properties.processingAgent.description
+#: followthemoney/schema/Document.yaml
 msgid "Name and version of the processing agent used to process the Document"
 msgstr "Имя и версия обработчика документа"
 
 #. Document.properties.processedAt.label
 #: followthemoney/schema/Document.yaml
+msgid "Processed at"
+msgstr "Дата обработки документа"
+
+#. Document.properties.processedAt.description
+#: followthemoney/schema/Document.yaml
 msgid "Date and time of the most recent ingestion of the Document"
 msgstr "Дата и время последней загрузки документа"
 
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr "Документация"
@@ -3762,14 +3772,19 @@
 msgstr "Дата постройки"
 
 #. Vehicle.properties.registrationDate.label
 #: followthemoney/schema/Vehicle.yaml
 msgid "Registration Date"
 msgstr "Дата регистрации"
 
+#. Vehicle.properties.deregistrationDate.label
+#: followthemoney/schema/Vehicle.yaml
+msgid "De-registration Date"
+msgstr "Дата снятия с регистрации"
+
 #. Vessel.label
 #: followthemoney/schema/Vessel.yaml
 msgid "Vessel"
 msgstr "Судно"
 
 #. Vessel.plural
 #: followthemoney/schema/Vessel.yaml
```

### Comparing `followthemoney-3.4.3/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/__init__.py` & `followthemoney-3.4.4/followthemoney/types/__init__.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/address.py` & `followthemoney-3.4.4/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/checksum.py` & `followthemoney-3.4.4/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/common.py` & `followthemoney-3.4.4/followthemoney/types/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/country.py` & `followthemoney-3.4.4/followthemoney/types/country.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/date.py` & `followthemoney-3.4.4/followthemoney/types/date.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/email.py` & `followthemoney-3.4.4/followthemoney/types/email.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/entity.py` & `followthemoney-3.4.4/followthemoney/types/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/gender.py` & `followthemoney-3.4.4/followthemoney/types/gender.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/iban.py` & `followthemoney-3.4.4/followthemoney/types/iban.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/identifier.py` & `followthemoney-3.4.4/followthemoney/types/identifier.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/ip.py` & `followthemoney-3.4.4/followthemoney/types/ip.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/json.py` & `followthemoney-3.4.4/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/language.py` & `followthemoney-3.4.4/followthemoney/types/language.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/mimetype.py` & `followthemoney-3.4.4/followthemoney/types/mimetype.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/name.py` & `followthemoney-3.4.4/followthemoney/types/name.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/number.py` & `followthemoney-3.4.4/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/phone.py` & `followthemoney-3.4.4/followthemoney/types/phone.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/registry.py` & `followthemoney-3.4.4/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/string.py` & `followthemoney-3.4.4/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/topic.py` & `followthemoney-3.4.4/followthemoney/types/topic.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/types/url.py` & `followthemoney-3.4.4/followthemoney/types/url.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney/util.py` & `followthemoney-3.4.4/followthemoney/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.4.4/followthemoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.3
-Summary: UNKNOWN
+Version: 3.4.4
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -86,9 +84,7 @@
 This will create a new patch release and upload a distribution of it. If
 the changes are more significant, you can run `bumpversion` with the `minor`
 or `major` arguments.
 
 When the schema is updated, please update the docs, ideally including the
 diagrams. For the RDF namespace and JavaScript version of the model, 
 run `make generate`.
-
-
```

### Comparing `followthemoney-3.4.3/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.4.4/followthemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.3/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.4.4/followthemoney.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,7 @@
 csv = followthemoney.cli.exports:export_csv
 cypher = followthemoney.cli.exports:export_cypher
 excel = followthemoney.cli.exports:export_excel
 gexf = followthemoney.cli.exports:export_gexf
 mapping = followthemoney.cli.mapping:run_mapping
 rdf = followthemoney.cli.exports:export_rdf
 sieve = followthemoney.cli.sieve:sieve
-
```

### Comparing `followthemoney-3.4.3/followthemoney.egg-info/requires.txt` & `followthemoney-3.4.4/followthemoney.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 babel<3.0.0,>=2.9.1
 pyyaml<7.0.0,>=5.0.0
 types-PyYAML
 sqlalchemy2-stubs
 banal<1.1.0,>=1.0.1
-click<9.0.0,>=8.0
+click<8.1.4,>=8.0
 stringcase<2.0.0,>=1.2.0
 requests<3.0.0,>=2.21.0
 python-levenshtein<1.0.0,>=0.12.0
 normality<3.0.0,>=2.1.1
 sqlalchemy<3.0.0,>=1.2.0
 countrynames<2.0.0,>=1.13.0
 languagecodes<2.0.0,>=1.1.0
```

### Comparing `followthemoney-3.4.3/setup.py` & `followthemoney-3.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.4.3",
+    version="3.4.4",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
@@ -31,15 +31,15 @@
     zip_safe=False,
     install_requires=[
         "babel >= 2.9.1, < 3.0.0",
         "pyyaml >= 5.0.0, < 7.0.0",
         "types-PyYAML",
         "sqlalchemy2-stubs",
         "banal >= 1.0.1, < 1.1.0",
-        "click >= 8.0, < 9.0.0",
+        "click >= 8.0, < 8.1.4",
         "stringcase >= 1.2.0, < 2.0.0",
         "requests >= 2.21.0, < 3.0.0",
         "python-levenshtein >= 0.12.0, < 1.0.0",
         "normality >= 2.1.1, < 3.0.0",
         "sqlalchemy >= 1.2.0, < 3.0.0",
         "countrynames >= 1.13.0, < 2.0.0",
         "languagecodes >= 1.1.0, < 2.0.0",
```

