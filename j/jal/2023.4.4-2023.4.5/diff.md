# Comparing `tmp/jal-2023.4.4.tar.gz` & `tmp/jal-2023.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jal-2023.4.4.tar", last modified: Wed Apr 12 17:26:14 2023, max compression
+gzip compressed data, was "jal-2023.4.5.tar", last modified: Fri Apr 14 18:18:09 2023, max compression
```

## Comparing `jal-2023.4.4.tar` & `jal-2023.4.5.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.935945 jal-2023.4.4/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.4/MANIFEST.in
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-12 17:26:14.935945 jal-2023.4.4/PKG-INFO
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.885945 jal-2023.4.4/docs/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7665 2023-04-11 21:38:54.000000 jal-2023.4.4/docs/README.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.885945 jal-2023.4.4/jal/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-12 17:22:41.000000 jal-2023.4.4/jal/__init__.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3832 2023-04-07 14:10:37.000000 jal-2023.4.4/jal/constants.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.885945 jal-2023.4.4/jal/data_export/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.4/jal/data_export/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-09 17:41:00.000000 jal-2023.4.4/jal/data_export/dlsg.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.892612 jal-2023.4.4/jal/data_export/tax_reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.4/jal/data_export/tax_reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/data_export/tax_reports/portugal.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.4/jal/data_export/tax_reports/portugal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/data_export/tax_reports/russia.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-12 16:52:42.000000 jal-2023.4.4/jal/data_export/tax_reports/russia.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/data_export/taxes.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/data_export/taxes_flow.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.892612 jal-2023.4.4/jal/data_export/templates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.4/jal/data_export/templates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/data_export/templates/tax_prt_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/data_export/templates/tax_prt_shares.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_bonds.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_corporate_actions.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_crypto.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_derivatives.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_fees.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_flow.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_interests.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.4/jal/data_export/templates/tax_rus_trades.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.4/jal/data_export/xlsx.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.895945 jal-2023.4.4/jal/data_import/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.4/jal/data_import/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.895945 jal-2023.4.4/jal/data_import/broker_statements/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.4/jal/data_import/broker_statements/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    63265 2023-04-12 11:02:49.000000 jal-2023.4.4/jal/data_import/broker_statements/ibkr.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.4/jal/data_import/broker_statements/just2trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.4/jal/data_import/broker_statements/kit.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.4/jal/data_import/broker_statements/open_portfolio.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    30709 2023-02-14 12:16:51.000000 jal-2023.4.4/jal/data_import/broker_statements/openbroker.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.4/jal/data_import/broker_statements/psb.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27469 2022-08-21 07:15:06.000000 jal-2023.4.4/jal/data_import/broker_statements/uralsib.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.4/jal/data_import/category_recognizer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.4/jal/data_import/import_schema.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15410 2023-04-07 14:10:37.000000 jal-2023.4.4/jal/data_import/slips.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13093 2023-03-01 17:12:57.000000 jal-2023.4.4/jal/data_import/slips_tax.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35649 2023-04-08 19:51:40.000000 jal-2023.4.4/jal/data_import/statement.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.4/jal/data_import/statement_xls.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-12 11:02:49.000000 jal-2023.4.4/jal/data_import/statement_xml.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.4/jal/data_import/statements.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.899278 jal-2023.4.4/jal/db/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.4/jal/db/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.4/jal/db/account.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-07 15:37:49.000000 jal-2023.4.4/jal/db/asset.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.4/jal/db/backup_restore.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.4/jal/db/balances_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.4/jal/db/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/db/closed_trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.4/jal/db/country.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18460 2023-04-07 14:10:37.000000 jal-2023.4.4/jal/db/db.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.4/jal/db/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-07 14:11:15.000000 jal-2023.4.4/jal/db/holdings_model.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16642 2023-02-23 10:35:04.000000 jal-2023.4.4/jal/db/ledger.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.4/jal/db/operations.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7486 2023-02-28 14:47:51.000000 jal-2023.4.4/jal/db/operations_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.4/jal/db/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15210 2023-02-21 12:19:40.000000 jal-2023.4.4/jal/db/reference_models.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.4/jal/db/settings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.4/jal/db/tag.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6761 2023-03-08 18:16:20.000000 jal-2023.4.4/jal/db/tax_estimator.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.4/jal/db/view_model.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.902612 jal-2023.4.4/jal/img/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/accept.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/add.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/add_child.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.4/jal/img/broom.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/cancel.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.4/jal/img/chart.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/copy.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/delete.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.4/jal/img/ibkr.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.4/jal/img/j2t.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.4/jal/img/jal.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.4/jal/img/kit.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.4/jal/img/list.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.4/jal/img/meatballs.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/new.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.4/jal/img/open_portfolio.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.4/jal/img/openbroker.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.4/jal/img/psb.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.4/jal/img/quik.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/reconcile.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.4/jal/img/remove.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.4/jal/img/tax.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.4/jal/img/uralsib.ico
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.4/jal/jal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.4/jal/jal_init.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.905945 jal-2023.4.4/jal/languages/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.4/jal/languages/en.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.4/jal/languages/en.qm
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.4/jal/languages/ru.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    86944 2023-04-09 17:47:08.000000 jal-2023.4.4/jal/languages/ru.qm
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.905945 jal-2023.4.4/jal/net/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.4/jal/net/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    24616 2023-03-22 16:11:44.000000 jal-2023.4.4/jal/net/downloader.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.4/jal/net/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.4/jal/pypi_description.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.909278 jal-2023.4.4/jal/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.4/jal/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2914 2023-02-14 08:22:42.000000 jal-2023.4.4/jal/reports/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14324 2023-04-07 14:11:15.000000 jal-2023.4.4/jal/reports/deals.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3868 2023-04-07 14:11:15.000000 jal-2023.4.4/jal/reports/holdings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14694 2023-04-07 14:11:15.000000 jal-2023.4.4/jal/reports/income_spending.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2802 2023-02-19 13:19:11.000000 jal-2023.4.4/jal/reports/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8684 2023-03-02 14:48:40.000000 jal-2023.4.4/jal/reports/profit_loss.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.4/jal/reports/reports.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2774 2023-02-16 10:21:05.000000 jal-2023.4.4/jal/reports/tag.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.912612 jal-2023.4.4/jal/ui/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.4/jal/ui/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.915945 jal-2023.4.4/jal/ui/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.4/jal/ui/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_category_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_deals_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_holdings_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4156 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_income_spending_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_peer_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_profit_loss_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_tag_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/reports/ui_tax_estimation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_asset_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_flow_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_login_fns_dlg.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-12 14:15:34.000000 jal-2023.4.4/jal/ui/ui_main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_operations_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_rebuild_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_reference_data_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_select_account_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_select_reference_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_slip_import_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_tax_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-09 17:45:04.000000 jal-2023.4.4/jal/ui/ui_update_quotes_window.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.929278 jal-2023.4.4/jal/updates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.4/jal/updates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.4/jal/updates/jal_delta_10.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.4/jal/updates/jal_delta_11.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.4/jal/updates/jal_delta_12.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.4/jal/updates/jal_delta_13.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.4/jal/updates/jal_delta_14.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.4/jal/updates/jal_delta_15.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.4/jal/updates/jal_delta_16.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.4/jal/updates/jal_delta_17.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.4/jal/updates/jal_delta_18.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.4/jal/updates/jal_delta_19.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.4/jal/updates/jal_delta_20.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.4/jal/updates/jal_delta_21.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.4/jal/updates/jal_delta_22.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.4/jal/updates/jal_delta_23.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.4/jal/updates/jal_delta_24.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.4/jal/updates/jal_delta_25.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.4/jal/updates/jal_delta_26.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.4/jal/updates/jal_delta_27.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.4/jal/updates/jal_delta_28.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.4/jal/updates/jal_delta_29.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.4/jal/updates/jal_delta_30.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.4/jal/updates/jal_delta_31.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.4/jal/updates/jal_delta_32.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.4/jal/updates/jal_delta_33.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.4/jal/updates/jal_delta_34.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.4/jal/updates/jal_delta_35.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.4/jal/updates/jal_delta_36.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.4/jal/updates/jal_delta_37.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.4/jal/updates/jal_delta_38.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.4/jal/updates/jal_delta_39.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.4/jal/updates/jal_delta_40.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.4/jal/updates/jal_delta_41.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.4/jal/updates/jal_delta_42.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.4/jal/updates/jal_delta_43.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.4/jal/updates/jal_delta_44.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.932612 jal-2023.4.4/jal/widgets/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.4/jal/widgets/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3918 2023-01-09 20:51:48.000000 jal-2023.4.4/jal/widgets/abstract_operation_details.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6808 2023-02-23 10:22:46.000000 jal-2023.4.4/jal/widgets/account_select.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13988 2023-02-27 15:59:08.000000 jal-2023.4.4/jal/widgets/asset_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11151 2023-02-23 19:44:39.000000 jal-2023.4.4/jal/widgets/corporate_action_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.935945 jal-2023.4.4/jal/widgets/custom/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.4/jal/widgets/custom/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4422 2023-02-14 11:55:13.000000 jal-2023.4.4/jal/widgets/custom/date_range_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2016 2023-01-09 21:29:20.000000 jal-2023.4.4/jal/widgets/custom/db_lookup_combobox.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4258 2023-04-12 15:18:56.000000 jal-2023.4.4/jal/widgets/custom/log_viewer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13738 2023-03-22 16:11:44.000000 jal-2023.4.4/jal/widgets/delegates.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9321 2023-03-08 16:41:32.000000 jal-2023.4.4/jal/widgets/dividend_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8393 2023-03-31 10:41:38.000000 jal-2023.4.4/jal/widgets/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12298 2023-02-25 18:52:44.000000 jal-2023.4.4/jal/widgets/income_spending_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13197 2023-04-12 07:42:26.000000 jal-2023.4.4/jal/widgets/main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3391 2023-03-08 18:22:55.000000 jal-2023.4.4/jal/widgets/mdi.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.4/jal/widgets/operations_tabs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7010 2023-02-20 13:28:14.000000 jal-2023.4.4/jal/widgets/operations_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5935 2022-08-21 07:15:06.000000 jal-2023.4.4/jal/widgets/price_chart.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5666 2023-03-31 10:41:38.000000 jal-2023.4.4/jal/widgets/qr_scanner.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11082 2023-02-27 16:00:28.000000 jal-2023.4.4/jal/widgets/reference_data.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21662 2023-02-27 15:30:11.000000 jal-2023.4.4/jal/widgets/reference_dialogs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4863 2023-02-19 18:07:24.000000 jal-2023.4.4/jal/widgets/reference_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.4/jal/widgets/register_designer_plugins.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3462 2023-02-23 10:23:05.000000 jal-2023.4.4/jal/widgets/selection_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7701 2023-02-08 10:33:24.000000 jal-2023.4.4/jal/widgets/tax_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6922 2022-12-26 10:36:44.000000 jal-2023.4.4/jal/widgets/trade_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10120 2023-04-07 14:10:37.000000 jal-2023.4.4/jal/widgets/transfer_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-12 17:26:14.885945 jal-2023.4.4/jal.egg-info/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-12 17:26:14.000000 jal-2023.4.4/jal.egg-info/PKG-INFO
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-12 17:26:14.000000 jal-2023.4.4/jal.egg-info/SOURCES.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-12 17:26:14.000000 jal-2023.4.4/jal.egg-info/dependency_links.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-12 17:26:14.000000 jal-2023.4.4/jal.egg-info/entry_points.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       74 2023-04-12 17:26:14.000000 jal-2023.4.4/jal.egg-info/requires.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-12 17:26:14.000000 jal-2023.4.4/jal.egg-info/top_level.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-12 17:26:14.935945 jal-2023.4.4/setup.cfg
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1763 2023-04-12 17:21:50.000000 jal-2023.4.4/setup.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.164846 jal-2023.4.5/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.5/MANIFEST.in
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-14 18:18:09.164846 jal-2023.4.5/PKG-INFO
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.121513 jal-2023.4.5/docs/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7665 2023-04-14 11:26:23.000000 jal-2023.4.5/docs/README.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.124846 jal-2023.4.5/jal/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-14 18:15:15.000000 jal-2023.4.5/jal/__init__.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3832 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/constants.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.124846 jal-2023.4.5/jal/data_export/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.5/jal/data_export/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_export/dlsg.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.128179 jal-2023.4.5/jal/data_export/tax_reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/data_export/tax_reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/tax_reports/portugal.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.5/jal/data_export/tax_reports/portugal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/tax_reports/russia.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_export/tax_reports/russia.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/taxes.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/taxes_flow.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.128179 jal-2023.4.5/jal/data_export/templates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/templates/tax_prt_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/templates/tax_prt_shares.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_bonds.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_corporate_actions.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_crypto.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_derivatives.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_fees.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_flow.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_interests.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_trades.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.5/jal/data_export/xlsx.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.131513 jal-2023.4.5/jal/data_import/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/data_import/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.134846 jal-2023.4.5/jal/data_import/broker_statements/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.5/jal/data_import/broker_statements/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    63265 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_import/broker_statements/ibkr.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/data_import/broker_statements/just2trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/data_import/broker_statements/kit.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.5/jal/data_import/broker_statements/open_portfolio.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    30709 2023-02-14 12:16:51.000000 jal-2023.4.5/jal/data_import/broker_statements/openbroker.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.5/jal/data_import/broker_statements/psb.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27469 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/data_import/broker_statements/uralsib.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.5/jal/data_import/category_recognizer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.5/jal/data_import/import_schema.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15609 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/data_import/slips.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/data_import/slips_tax.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35649 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_import/statement.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.5/jal/data_import/statement_xls.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_import/statement_xml.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.5/jal/data_import/statements.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.138179 jal-2023.4.5/jal/db/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/db/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.5/jal/db/account.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/db/asset.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.5/jal/db/backup_restore.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.5/jal/db/balances_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.5/jal/db/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/db/closed_trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.5/jal/db/country.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18497 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/db.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.5/jal/db/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.5/jal/db/holdings_model.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16687 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/ledger.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/db/operations.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7486 2023-02-28 14:47:51.000000 jal-2023.4.5/jal/db/operations_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.5/jal/db/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15187 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/reference_models.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.5/jal/db/settings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.5/jal/db/tag.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/tax_estimator.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.5/jal/db/view_model.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.138179 jal-2023.4.5/jal/img/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/accept.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/add.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/add_child.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.5/jal/img/broom.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/cancel.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.5/jal/img/chart.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/copy.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/delete.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.5/jal/img/ibkr.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.5/jal/img/j2t.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.5/jal/img/jal.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.5/jal/img/kit.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.5/jal/img/list.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.5/jal/img/meatballs.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/new.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.5/jal/img/open_portfolio.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.5/jal/img/openbroker.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.5/jal/img/psb.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.5/jal/img/quik.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/reconcile.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/remove.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.5/jal/img/tax.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.5/jal/img/uralsib.ico
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.5/jal/jal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/jal_init.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.141513 jal-2023.4.5/jal/languages/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.5/jal/languages/en.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.5/jal/languages/en.qm
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.5/jal/languages/ru.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    86944 2023-04-14 11:26:41.000000 jal-2023.4.5/jal/languages/ru.qm
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.141513 jal-2023.4.5/jal/net/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.5/jal/net/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    24656 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/net/downloader.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.5/jal/net/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.5/jal/pypi_description.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.141513 jal-2023.4.5/jal/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/deals.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/holdings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14756 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/income_spending.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8771 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/profit_loss.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.5/jal/reports/reports.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/tag.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.144846 jal-2023.4.5/jal/ui/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/ui/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.144846 jal-2023.4.5/jal/ui/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.5/jal/ui/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_category_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-14 11:27:05.000000 jal-2023.4.5/jal/ui/reports/ui_deals_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-14 11:27:05.000000 jal-2023.4.5/jal/ui/reports/ui_holdings_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4156 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_income_spending_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_peer_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_profit_loss_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_tag_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_tax_estimation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_asset_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_flow_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_login_fns_dlg.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-12 14:15:34.000000 jal-2023.4.5/jal/ui/ui_main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_operations_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_rebuild_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_reference_data_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_select_account_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_select_reference_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_slip_import_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_tax_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_update_quotes_window.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.158180 jal-2023.4.5/jal/updates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/updates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.5/jal/updates/jal_delta_10.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.5/jal/updates/jal_delta_11.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.5/jal/updates/jal_delta_12.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.5/jal/updates/jal_delta_13.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_14.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_15.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_16.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_17.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.5/jal/updates/jal_delta_18.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.5/jal/updates/jal_delta_19.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.5/jal/updates/jal_delta_20.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.5/jal/updates/jal_delta_21.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.5/jal/updates/jal_delta_22.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.5/jal/updates/jal_delta_23.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.5/jal/updates/jal_delta_24.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.5/jal/updates/jal_delta_25.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.5/jal/updates/jal_delta_26.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.5/jal/updates/jal_delta_27.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.5/jal/updates/jal_delta_28.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.5/jal/updates/jal_delta_29.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.5/jal/updates/jal_delta_30.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.5/jal/updates/jal_delta_31.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.5/jal/updates/jal_delta_32.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.5/jal/updates/jal_delta_33.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.5/jal/updates/jal_delta_34.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.5/jal/updates/jal_delta_35.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.5/jal/updates/jal_delta_36.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.5/jal/updates/jal_delta_37.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/updates/jal_delta_38.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.5/jal/updates/jal_delta_39.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.5/jal/updates/jal_delta_40.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/updates/jal_delta_41.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.5/jal/updates/jal_delta_42.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.5/jal/updates/jal_delta_43.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/updates/jal_delta_44.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.161513 jal-2023.4.5/jal/widgets/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/widgets/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3918 2023-01-09 20:51:48.000000 jal-2023.4.5/jal/widgets/abstract_operation_details.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6844 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/account_select.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14131 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/asset_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11151 2023-02-23 19:44:39.000000 jal-2023.4.5/jal/widgets/corporate_action_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.161513 jal-2023.4.5/jal/widgets/custom/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.5/jal/widgets/custom/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4435 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/custom/date_range_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2016 2023-01-09 21:29:20.000000 jal-2023.4.5/jal/widgets/custom/db_lookup_combobox.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5331 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/custom/log_viewer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13750 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/delegates.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9321 2023-03-08 16:41:32.000000 jal-2023.4.5/jal/widgets/dividend_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8437 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12298 2023-02-25 18:52:44.000000 jal-2023.4.5/jal/widgets/income_spending_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3385 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/mdi.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.5/jal/widgets/operations_tabs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/operations_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6012 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/price_chart.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5666 2023-04-14 18:09:14.000000 jal-2023.4.5/jal/widgets/qr_scanner.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/reference_data.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21798 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/reference_dialogs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4863 2023-02-19 18:07:24.000000 jal-2023.4.5/jal/widgets/reference_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.5/jal/widgets/register_designer_plugins.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3505 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/selection_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/tax_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6922 2022-12-26 10:36:44.000000 jal-2023.4.5/jal/widgets/trade_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10120 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/widgets/transfer_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.124846 jal-2023.4.5/jal.egg-info/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/PKG-INFO
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/SOURCES.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/dependency_links.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/entry_points.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/requires.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/top_level.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-14 18:18:09.164846 jal-2023.4.5/setup.cfg
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.5/setup.py
```

### Comparing `jal-2023.4.4/PKG-INFO` & `jal-2023.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.4
+Version: 2023.4.5
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.4/docs/README.md` & `jal-2023.4.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/constants.py` & `jal-2023.4.5/jal/constants.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/dlsg.py` & `jal-2023.4.5/jal/data_export/dlsg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/tax_reports/portugal.json` & `jal-2023.4.5/jal/data_export/tax_reports/portugal.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/tax_reports/portugal.py` & `jal-2023.4.5/jal/data_export/tax_reports/portugal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/tax_reports/russia.json` & `jal-2023.4.5/jal/data_export/tax_reports/russia.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/tax_reports/russia.py` & `jal-2023.4.5/jal/data_export/tax_reports/russia.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/taxes.py` & `jal-2023.4.5/jal/data_export/taxes.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/taxes_flow.py` & `jal-2023.4.5/jal/data_export/taxes_flow.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_prt_dividends.json` & `jal-2023.4.5/jal/data_export/templates/tax_prt_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_prt_shares.json` & `jal-2023.4.5/jal/data_export/templates/tax_prt_shares.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_bonds.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_bonds.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_corporate_actions.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_corporate_actions.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_crypto.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_crypto.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_derivatives.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_derivatives.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_dividends.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_fees.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_fees.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_flow.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_flow.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_interests.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_interests.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/templates/tax_rus_trades.json` & `jal-2023.4.5/jal/data_export/templates/tax_rus_trades.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_export/xlsx.py` & `jal-2023.4.5/jal/data_export/xlsx.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/broker_statements/ibkr.py` & `jal-2023.4.5/jal/data_import/broker_statements/ibkr.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/broker_statements/just2trade.py` & `jal-2023.4.5/jal/data_import/broker_statements/just2trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/broker_statements/kit.py` & `jal-2023.4.5/jal/data_import/broker_statements/kit.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/broker_statements/open_portfolio.py` & `jal-2023.4.5/jal/data_import/broker_statements/open_portfolio.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/broker_statements/openbroker.py` & `jal-2023.4.5/jal/data_import/broker_statements/openbroker.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/broker_statements/psb.py` & `jal-2023.4.5/jal/data_import/broker_statements/psb.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/broker_statements/uralsib.py` & `jal-2023.4.5/jal/data_import/broker_statements/uralsib.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/category_recognizer.py` & `jal-2023.4.5/jal/data_import/category_recognizer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/import_schema.json` & `jal-2023.4.5/jal/data_import/import_schema.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/slips.py` & `jal-2023.4.5/jal/data_import/slips.py`

 * *Files 26% similar despite different names*

```diff
@@ -106,59 +106,60 @@
             model.setData(index, editor.selected_id)
             model.setData(index.siblingAtColumn(2), 1) # set confidence level to 1
         if index.column() == 3:
             model.setData(index, editor.selected_id)
 
 
 #-----------------------------------------------------------------------------------------------------------------------
-class ImportSlipDialog(QDialog, Ui_ImportSlipDlg):
+class ImportSlipDialog(QDialog):
     OPERATION_PURCHASE = 1
     OPERATION_RETURN = 2
 
     timestamp_patterns = ['yyyyMMddTHHmm', 'yyyyMMddTHHmmss', 'yyyy-MM-ddTHH:mm', 'yyyy-MM-ddTHH:mm:ss']
 
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.setupUi(self)
+        self.ui = Ui_ImportSlipDlg()
+        self.ui.setupUi(self)
         self.initUi()
         self.model = None
         self.delegate = []
 
-        self.CameraGroup.setVisible(False)
+        self.ui.CameraGroup.setVisible(False)
 
         self.QR_data = ''
         self.slip_json = None
         self.slip_lines = None
 
         self.slipsAPI = SlipsTaxAPI(self)
         self.tensor_flow_present = dependency_present(['tensorflow'])
 
-        self.LoadQRfromFileBtn.clicked.connect(self.loadFileQR)
-        self.GetQRfromClipboardBtn.clicked.connect(self.readClipboardQR)
-        self.GetQRfromCameraBtn.clicked.connect(self.readCameraQR)
-        self.StopCameraBtn.clicked.connect(self.closeCamera)
-        self.ScannerQR.decodedQR.connect(self.onCameraQR)
-        self.GetSlipBtn.clicked.connect(self.downloadSlipJSON)
-        self.LoadJSONfromFileBtn.clicked.connect(self.loadFileSlipJSON)
-        self.AddOperationBtn.clicked.connect(self.addOperation)
-        self.ClearBtn.clicked.connect(self.clearSlipData)
-        self.AssignCategoryBtn.clicked.connect(self.recognizeCategories)
+        self.ui.LoadQRfromFileBtn.clicked.connect(self.loadFileQR)
+        self.ui.GetQRfromClipboardBtn.clicked.connect(self.readClipboardQR)
+        self.ui.GetQRfromCameraBtn.clicked.connect(self.readCameraQR)
+        self.ui.StopCameraBtn.clicked.connect(self.closeCamera)
+        self.ui.ScannerQR.decodedQR.connect(self.onCameraQR)
+        self.ui.GetSlipBtn.clicked.connect(self.downloadSlipJSON)
+        self.ui.LoadJSONfromFileBtn.clicked.connect(self.loadFileSlipJSON)
+        self.ui.AddOperationBtn.clicked.connect(self.addOperation)
+        self.ui.ClearBtn.clicked.connect(self.clearSlipData)
+        self.ui.AssignCategoryBtn.clicked.connect(self.recognizeCategories)
 
-        self.AssignCategoryBtn.setEnabled(self.tensor_flow_present)
+        self.ui.AssignCategoryBtn.setEnabled(self.tensor_flow_present)
 
     def closeEvent(self, arg__1):
-        self.ScannerQR.stopScan()
+        self.ui.ScannerQR.stopScan()
         self.accept()
 
     def initUi(self):
-        self.SlipAmount.setText('')
-        self.FN.setText('')
-        self.FD.setText('')
-        self.FP.setText('')
-        self.SlipType.setCurrentIndex(0)
+        self.ui.SlipAmount.setText('')
+        self.ui.FN.setText('')
+        self.ui.FD.setText('')
+        self.ui.FP.setText('')
+        self.ui.SlipType.setCurrentIndex(0)
 
     #------------------------------------------------------------------------------------------
     # Loads graphics file and tries to read QR-code from it.
     @Slot()
     def loadFileQR(self):
         self.initUi()
         qr_file, _filter = \
@@ -181,23 +182,23 @@
             self.parseQRdata()
         else:
             logging.warning(self.tr("No QR codes found in clipboard"))
 
     @Slot()
     def readCameraQR(self):
         self.initUi()
-        self.CameraGroup.setVisible(True)
-        self.SlipDataGroup.setVisible(False)
-        self.ScannerQR.startScan()
+        self.ui.CameraGroup.setVisible(True)
+        self.ui.SlipDataGroup.setVisible(False)
+        self.ui.ScannerQR.startScan()
 
     @Slot()
     def closeCamera(self):
-        self.ScannerQR.stopScan()
-        self.CameraGroup.setVisible(False)
-        self.SlipDataGroup.setVisible(True)
+        self.ui.ScannerQR.stopScan()
+        self.ui.CameraGroup.setVisible(False)
+        self.ui.SlipDataGroup.setVisible(True)
 
     @Slot()
     def onCameraQR(self, decoded_qr):
         self.QR_data = decoded_qr
         self.closeCamera()
         self.parseQRdata()
 
@@ -209,32 +210,32 @@
         logging.info(self.tr("QR: " + self.QR_data))
         params = parse_qs(self.QR_data)
         try:
             for timestamp_pattern in self.timestamp_patterns:
                 datetime = QDateTime.fromString(params['t'][0], timestamp_pattern)
                 datetime.setTimeSpec(Qt.UTC)
                 if datetime.isValid():
-                    self.SlipTimstamp.setDateTime(datetime)
-            self.SlipAmount.setText(params['s'][0])
-            self.FN.setText(params['fn'][0])
-            self.FD.setText(params['i'][0])
-            self.FP.setText(params['fp'][0])
-            self.SlipType.setCurrentIndex(int(params['n'][0]) - 1)
+                    self.ui.SlipTimstamp.setDateTime(datetime)
+            self.ui.SlipAmount.setText(params['s'][0])
+            self.ui.FN.setText(params['fn'][0])
+            self.ui.FD.setText(params['i'][0])
+            self.ui.FP.setText(params['fp'][0])
+            self.ui.SlipType.setCurrentIndex(int(params['n'][0]) - 1)
         except KeyError:
             logging.warning(self.tr("QR available but pattern isn't recognized: " + self.QR_data))
             return
         self.downloadSlipJSON()
 
     def downloadSlipJSON(self):
-        timestamp = self.SlipTimstamp.dateTime().toSecsSinceEpoch()
+        timestamp = self.ui.SlipTimstamp.dateTime().toSecsSinceEpoch()
 
         attempt = 0
         while True:
-            result = self.slipsAPI.get_slip(timestamp, float(self.SlipAmount.text()), self.FN.text(),
-                                            self.FD.text(), self.FP.text(), self.SlipType.currentIndex() + 1)
+            result = self.slipsAPI.get_slip(timestamp, float(self.ui.SlipAmount.text()), self.ui.FN.text(),
+                                            self.ui.FD.text(), self.ui.FP.text(), self.ui.SlipType.currentIndex() + 1)
             if result != SlipsTaxAPI.Pending:
                 break
             if attempt > 5:
                 logging.warning(self.tr("Max retry count exceeded."))
                 break
             attempt += 1
             time.sleep(0.5) # wait half a second before next attempt
@@ -276,33 +277,33 @@
             operation = int(slip['operationType'])
         else:
             logging.error(self.tr("Can't find 'operationType' tag in json 'ticket'"))
             return
         # Get shop name
         shop_name = ''
         if 'user' in slip:
-            shop_name = self.SlipShopName.setText(slip['user'])
+            shop_name = self.ui.SlipShopName.setText(slip['user'])
         if (not shop_name) and ('userInn' in slip):
             shop_name = self.slipsAPI.get_shop_name_by_inn(slip['userInn'])
-        self.SlipShopName.setText(shop_name)
+        self.ui.SlipShopName.setText(shop_name)
 
-        peer_id = JalPeer.get_id_by_mapped_name(self.SlipShopName.text())
+        peer_id = JalPeer.get_id_by_mapped_name(self.ui.SlipShopName.text())
         if peer_id is not None:
-            self.PeerEdit.selected_id = peer_id
+            self.ui.PeerEdit.selected_id = peer_id
 
         try:
             self.slip_lines = pd.DataFrame(slip['items'])
         except:
             return
 
         # Get date from timestamp
         if 'dateTime' in slip:
             slip_datetime = QDateTime.fromSecsSinceEpoch(int(slip['dateTime']))
             slip_datetime.setTimeSpec(Qt.UTC)
-            self.SlipDateTime.setDateTime(slip_datetime)
+            self.ui.SlipDateTime.setDateTime(slip_datetime)
 
         # Convert price to roubles
         self.slip_lines['price'] = self.slip_lines['price'] / 100
         if operation == self.OPERATION_PURCHASE:
             self.slip_lines['sum'] = -self.slip_lines['sum'] / 100
         elif operation == self.OPERATION_RETURN:
             self.slip_lines['sum'] = self.slip_lines['sum'] / 100
@@ -316,38 +317,38 @@
         self.slip_lines['category'] = 0
         self.slip_lines['confidence'] = 1
         # Assign empty tags
         self.slip_lines['tag'] = None
         self.slip_lines = self.slip_lines[['name', 'category', 'confidence', 'tag', 'sum']]
 
         self.model = PandasLinesModel(self.slip_lines, self)
-        self.LinesTableView.setModel(self.model)
+        self.ui.LinesTableView.setModel(self.model)
 
-        self.delegate = SlipLinesDelegate(self.LinesTableView)
+        self.delegate = SlipLinesDelegate(self.ui.LinesTableView)
         for column in range(self.model.columnCount()):
             if column == 0:
-                self.LinesTableView.horizontalHeader().setSectionResizeMode(column, QHeaderView.Stretch)
+                self.ui.LinesTableView.horizontalHeader().setSectionResizeMode(column, QHeaderView.Stretch)
             elif column == 1:
-                self.LinesTableView.setColumnWidth(column, 200)
+                self.ui.LinesTableView.setColumnWidth(column, 200)
             elif column == 2:
-                self.LinesTableView.setColumnHidden(column, True)
+                self.ui.LinesTableView.setColumnHidden(column, True)
             else:
-                self.LinesTableView.setColumnWidth(column, 100)
-            self.LinesTableView.setItemDelegateForColumn(column, self.delegate)
-        font = self.LinesTableView.horizontalHeader().font()
+                self.ui.LinesTableView.setColumnWidth(column, 100)
+            self.ui.LinesTableView.setItemDelegateForColumn(column, self.delegate)
+        font = self.ui.LinesTableView.horizontalHeader().font()
         font.setBold(True)
-        self.LinesTableView.horizontalHeader().setFont(font)
-        self.LinesTableView.show()
+        self.ui.LinesTableView.horizontalHeader().setFont(font)
+        self.ui.LinesTableView.show()
         self.recognizeCategories()
 
     def addOperation(self):
-        if self.AccountEdit.selected_id == 0:
+        if self.ui.AccountEdit.selected_id == 0:
             logging.warning(self.tr("Not possible to import slip: no account set for import"))
             return
-        if self.PeerEdit.selected_id == 0:
+        if self.ui.PeerEdit.selected_id == 0:
             logging.warning(self.tr("Not possible to import slip: can't import: no peer set for import"))
             return
         if self.slip_lines[self.slip_lines['category'] == 0].shape[0] != 0:
             logging.warning(self.tr("Not possible to import slip: some categories are not set"))
             return
 
         details = []
@@ -356,28 +357,28 @@
                 "category_id": row['category'],
                 "tag_id": row['tag'],
                 "amount": row['sum'],
                 "note": row['name']
             })
             JalCategory(row['category']).add_or_update_mapped_name(row['name'])
         operation = {
-            "timestamp": self.SlipDateTime.dateTime().toSecsSinceEpoch(),
-            "account_id": self.AccountEdit.selected_id,
-            "peer_id": self.PeerEdit.selected_id,
+            "timestamp": self.ui.SlipDateTime.dateTime().toSecsSinceEpoch(),
+            "account_id": self.ui.AccountEdit.selected_id,
+            "peer_id": self.ui.PeerEdit.selected_id,
             "lines": details
         }
         LedgerTransaction.create_new(LedgerTransaction.IncomeSpending, operation)
-        JalPeer(self.PeerEdit.selected_id).add_or_update_mapped_name(self.SlipShopName.text(), )
+        JalPeer(self.ui.PeerEdit.selected_id).add_or_update_mapped_name(self.ui.SlipShopName.text(), )
         self.clearSlipData()
 
     def clearSlipData(self):
         self.QR_data = ''
         self.slip_json = None
         self.slip_lines = None
-        self.LinesTableView.setModel(None)
+        self.ui.LinesTableView.setModel(None)
 
         self.initUi()
 
     @Slot()
     def recognizeCategories(self):
         if not self.tensor_flow_present:
             logging.warning(self.tr("Categories are not recognized: Tensorflow is not found"))
```

### Comparing `jal-2023.4.4/jal/data_import/slips_tax.py` & `jal-2023.4.5/jal/data_import/slips_tax.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,58 +32,59 @@
             auth_code = params['code']
             auth_state = params['state']
             logging.info(self.tr("ESIA login completed"))
             self.response_intercepted.emit(auth_code, auth_state)
 
 
 #-----------------------------------------------------------------------------------------------------------------------
-class LoginFNS(QDialog, Ui_LoginFNSDialog):
+class LoginFNS(QDialog):
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.setupUi(self)
+        self.ui = Ui_LoginFNSDialog()
+        self.ui.setupUi(self)
 
         self.phone_number = ''
         self.web_session = requests.Session()
         self.web_session.headers['ClientVersion'] = '2.9.0'
         self.web_session.headers['Device-Id'] = str(uuid.uuid1())
         self.web_session.headers['Device-OS'] = 'Android'
         self.web_session.headers['Content-Type'] = 'application/json; charset=UTF-8'
         self.web_session.headers['Accept-Encoding'] = 'gzip'
         self.web_session.headers['User-Agent'] = 'okhttp/4.2.2'
         self.web_profile = QWebEngineProfile(self)
         self.web_interceptor = RequestInterceptor(self)
         self.web_interceptor.response_intercepted.connect(self.response_esia)
         self.web_profile.setUrlRequestInterceptor(self.web_interceptor)
-        self.ESIAWebView.setPage(QWebEnginePage(self.web_profile, self))
+        self.ui.ESIAWebView.setPage(QWebEnginePage(self.web_profile, self))
 
-        self.LoginMethodTabs.currentChanged.connect(self.on_tab_changed)
-        self.GetCodeBtn.clicked.connect(self.send_sms)
-        self.SMSLoginBtn.clicked.connect(self.login_sms)
-        self.FNSLoginBtn.clicked.connect(self.login_fns)
+        self.ui.LoginMethodTabs.currentChanged.connect(self.on_tab_changed)
+        self.ui.GetCodeBtn.clicked.connect(self.send_sms)
+        self.ui.SMSLoginBtn.clicked.connect(self.login_sms)
+        self.ui.FNSLoginBtn.clicked.connect(self.login_fns)
 
     def on_tab_changed(self, index):
         if index == 2: # ESIA login selected
             self.login_esia()
 
     def send_sms(self):
         client_secret = JalSettings().getValue('RuTaxClientSecret')
-        self.phone_number = self.PhoneNumberEdit.text().replace('-', '')
+        self.phone_number = self.ui.PhoneNumberEdit.text().replace('-', '')
 
         payload = '{' + f'"client_secret":"{client_secret}","phone":"{self.phone_number}"' + '}'
         response = self.web_session.post('https://irkkt-mobile.nalog.ru:8888/v2/auth/phone/request', data=payload)
         if response.status_code != 204:
             logging.error(self.tr("FNS login failed: ") + f"{response}/{response.text}")
         else:
             logging.info(self.tr("SMS was requested successfully"))
     
     def login_sms(self):
         if not self.phone_number:
             return
         client_secret = JalSettings().getValue('RuTaxClientSecret')
-        code = self.CodeEdit.text()
+        code = self.ui.CodeEdit.text()
 
         payload = '{' + f'"client_secret":"{client_secret}","code":"{code}","phone":"{self.phone_number}"' + '}'
         response = self.web_session.post('https://irkkt-mobile.nalog.ru:8888/v2/auth/phone/verify', data=payload)
         if response.status_code != 200:
             logging.error(self.tr("FNS login failed: ") + f"{response}/{response.text}")
             return
         logging.info(self.tr("FNS login successful: ") + f"{response.text}")
@@ -93,16 +94,16 @@
         settings = JalSettings()
         settings.setValue('RuTaxSessionId', new_session_id)
         settings.setValue('RuTaxRefreshToken', new_refresh_token)
         self.accept()
 
     def login_fns(self):
         client_secret = JalSettings().getValue('RuTaxClientSecret')
-        inn = self.InnEdit.text()
-        password = self.PasswordEdit.text()
+        inn = self.ui.InnEdit.text()
+        password = self.ui.PasswordEdit.text()
 
         payload = '{' + f'"client_secret":"{client_secret}","inn":"{inn}","password":"{password}"' + '}'
         response = self.web_session.post('https://irkkt-mobile.nalog.ru:8888/v2/mobile/users/lkfl/auth', data=payload)
         if response.status_code != 200:
             logging.error(self.tr("FNS login failed: ") + f"{response}/{response.text}")
             return
         logging.info(self.tr("FNS login successful: ") + f"{response.text}")
@@ -117,15 +118,15 @@
     def login_esia(self):
         response = self.web_session.get('https://irkkt-mobile.nalog.ru:8888/v2/mobile/users/esia/auth/url')
         if response.status_code != 200:
             logging.error(self.tr("Get ESIA URL failed: ") + f"{response}/{response.text}")
             return
         json_content = json.loads(response.text)
         auth_url = json_content['url']
-        self.ESIAWebView.load(QUrl(auth_url))
+        self.ui.ESIAWebView.load(QUrl(auth_url))
 
     @Slot()
     def response_esia(self, auth_code, state):
         client_secret = JalSettings().getValue('RuTaxClientSecret')
         payload = '{' + f'"authorization_code": "{auth_code}", "client_secret": "{client_secret}", "state": "{state}"' \
                   + '}'
         response = self.web_session.post('https://irkkt-mobile.nalog.ru:8888/v2/mobile/users/esia/auth', data=payload)
```

### Comparing `jal-2023.4.4/jal/data_import/statement.py` & `jal-2023.4.5/jal/data_import/statement.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/statement_xls.py` & `jal-2023.4.5/jal/data_import/statement_xls.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/statement_xml.py` & `jal-2023.4.5/jal/data_import/statement_xml.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/data_import/statements.py` & `jal-2023.4.5/jal/data_import/statements.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/account.py` & `jal-2023.4.5/jal/db/account.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/asset.py` & `jal-2023.4.5/jal/db/asset.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/backup_restore.py` & `jal-2023.4.5/jal/db/backup_restore.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/balances_model.py` & `jal-2023.4.5/jal/db/balances_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/category.py` & `jal-2023.4.5/jal/db/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/closed_trade.py` & `jal-2023.4.5/jal/db/closed_trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/country.py` & `jal-2023.4.5/jal/db/country.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/db.py` & `jal-2023.4.5/jal/db/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,18 @@
 # ----------------------------------------------------------------------------------------------------------------------
 class JalDB:
     _tables = []
     _instances_with_cache = []
 
     # By default, db objects don't cache data. But if and object may cache db data we need to track it so parameter
     # 'cached' to be set to True. Such objects should implement invalidate_cache(), class_cache() methods also.
-    def __init__(self, cached=None):
+    def __init__(self, cached=None, **kwargs):
         if cached:
             self._instances_with_cache.append(self)
+        super().__init__()
 
     def tr(self, text):
         return QApplication.translate("JalDB", text)
 
     # -------------------------------------------------------------------------------------------------------------------
     # This function:
     # 1) checks that DB file is present and contains some data
```

### Comparing `jal-2023.4.4/jal/db/helpers.py` & `jal-2023.4.5/jal/db/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/holdings_model.py` & `jal-2023.4.5/jal/db/holdings_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/ledger.py` & `jal-2023.4.5/jal/db/ledger.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 from jal.db.operations import LedgerTransaction, LedgerError
 from jal.widgets.helpers import ts2dt, ts2d
 from jal.ui.ui_rebuild_window import Ui_ReBuildDialog
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Class to display window with ledger rebuild configuration options
-class RebuildDialog(QDialog, Ui_ReBuildDialog):
+class RebuildDialog(QDialog):
     def __init__(self, parent, frontier):
-        QDialog.__init__(self)
-        self.setupUi(self)
+        super().__init__(parent)
+        self.ui = Ui_ReBuildDialog()
+        self.ui.setupUi(self)
 
-        self.LastRadioButton.toggle()   # Set default option selection
+        self.ui.LastRadioButton.toggle()   # Set default option selection
         self.frontier = frontier
         frontier_text = ts2d(frontier)
-        self.FrontierDateLabel.setText(frontier_text)
-        self.CustomDateEdit.setDate(QDate.currentDate())
+        self.ui.FrontierDateLabel.setText(frontier_text)
+        self.ui.CustomDateEdit.setDate(QDate.currentDate())
 
         # center dialog with respect to parent window
         x = parent.x() + parent.width()/2 - self.width()/2
         y = parent.y() + parent.height()/2 - self.height()/2
         self.setGeometry(x, y, self.width(), self.height())
 
     def isFastAndDirty(self):
-        return self.FastAndDirty.isChecked()
+        return self.ui.FastAndDirty.isChecked()
 
     def getTimestamp(self):
-        if self.LastRadioButton.isChecked():
+        if self.ui.LastRadioButton.isChecked():
             return self.frontier
-        elif self.DateRadionButton.isChecked():
-            return self.CustomDateEdit.dateTime().toSecsSinceEpoch()
+        elif self.ui.DateRadionButton.isChecked():
+            return self.ui.CustomDateEdit.dateTime().toSecsSinceEpoch()
         else:  # self.AllRadioButton.isChecked()
             return 0
 
 
 # ===================================================================================================================
 # Subclasses dictionary to store last amount/value for [book, account, asset]
 # Differs from dictionary in a way that __getitem__() method uses DB-stored values for initialization
```

### Comparing `jal-2023.4.4/jal/db/operations.py` & `jal-2023.4.5/jal/db/operations.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/operations_model.py` & `jal-2023.4.5/jal/db/operations_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/peer.py` & `jal-2023.4.5/jal/db/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/reference_models.py` & `jal-2023.4.5/jal/db/reference_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._group_by = None
         self._filter_by = ''
         self._filter_value = None
         self._sort_by = None
         self._hidden = []
         self._stretch = None
         self._default_values = {}   # To fill in default values for fields allowed to be NULL
-        QSqlRelationalTableModel.__init__(self, parent=parent_view, db=self.connection())
+        super().__init__(parent=parent_view, db=self.connection())
         self.setJoinMode(QSqlRelationalTableModel.LeftJoin)
         self.setTable(self._table)
         self.setEditStrategy(QSqlTableModel.OnManualSubmit)
         self.select()
         # This is auxiliary 'plain' model of the same table - to be given as QCompleter source of data
         self._completion_model = QSqlTableModel(parent=parent_view, db=self.connection())
         self._completion_model.setTable(self._table)
```

### Comparing `jal-2023.4.4/jal/db/settings.py` & `jal-2023.4.5/jal/db/settings.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/db/tax_estimator.py` & `jal-2023.4.5/jal/db/tax_estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,27 +69,28 @@
             else:
                 self._view.setItemDelegateForColumn(i, self._float_delegate4)
         font = self._view.horizontalHeader().font()
         font.setBold(True)
         self._view.horizontalHeader().setFont(font)
 
 
-class TaxEstimator(MdiWidget, Ui_TaxEstimationDialog):
+class TaxEstimator(MdiWidget):
     TAX_RATE = {
         'pt': Decimal('0.28'),
         'ru': Decimal('0.13')
     }
     TAX_CURRENCY = {
         'pt': 'EUR',
         'ru': 'RUB'
     }
 
     def __init__(self, country_code, account_id, asset_id, asset_qty, parent=None):
-        super(TaxEstimator, self).__init__(parent)
-        self.setupUi(self)
+        super().__init__(parent)
+        self.ui = Ui_TaxEstimationDialog()
+        self.ui.setupUi(self)
 
         self.country = JalCountry(data={'code': country_code}, search=True)
         self.account_id = account_id
         self.asset_id = asset_id
         self.asset_name = JalAsset(self.asset_id).symbol(JalAccount(account_id).currency())
         self.asset_qty = asset_qty
         self.dataframe = None
@@ -104,19 +105,19 @@
         self.quote = 0
         self.rate = 1
         self.currency_name = ''
         self.prepare_tax()
         if self.dataframe is None:
             return
 
-        self.QuoteLbl.setText(f"{self.quote:.4f}")
-        self.RateLbl.setText(f"{self.rate:.4f} {self.currency_name}/{self.tax_currency_symbol}")
+        self.ui.QuoteLbl.setText(f"{self.quote:.4f}")
+        self.ui.RateLbl.setText(f"{self.rate:.4f} {self.currency_name}/{self.tax_currency_symbol}")
 
-        self.model = TaxEstimatorModel(self.DealsView, self.dataframe, self.currency_name, self.tax_currency_symbol)
-        self.DealsView.setModel(self.model)
+        self.model = TaxEstimatorModel(self.ui.DealsView, self.dataframe, self.currency_name, self.tax_currency_symbol)
+        self.ui.DealsView.setModel(self.model)
         self.model.configureView()
         self.ready = True
 
     def prepare_tax(self):
         try:
             tax_rate = self.TAX_RATE[self.country.code()]
         except KeyError:
```

### Comparing `jal-2023.4.4/jal/db/view_model.py` & `jal-2023.4.5/jal/db/view_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/accept.png` & `jal-2023.4.5/jal/img/accept.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/add.png` & `jal-2023.4.5/jal/img/add.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/add_child.png` & `jal-2023.4.5/jal/img/add_child.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/cancel.png` & `jal-2023.4.5/jal/img/cancel.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/chart.png` & `jal-2023.4.5/jal/img/chart.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/copy.png` & `jal-2023.4.5/jal/img/copy.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/delete.png` & `jal-2023.4.5/jal/img/delete.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/ibkr.png` & `jal-2023.4.5/jal/img/ibkr.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/j2t.png` & `jal-2023.4.5/jal/img/j2t.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/jal.png` & `jal-2023.4.5/jal/img/jal.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/kit.png` & `jal-2023.4.5/jal/img/kit.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/list.png` & `jal-2023.4.5/jal/img/list.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/new.png` & `jal-2023.4.5/jal/img/new.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/open_portfolio.png` & `jal-2023.4.5/jal/img/open_portfolio.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/openbroker.ico` & `jal-2023.4.5/jal/img/openbroker.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/psb.ico` & `jal-2023.4.5/jal/img/psb.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/quik.ico` & `jal-2023.4.5/jal/img/quik.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/reconcile.png` & `jal-2023.4.5/jal/img/reconcile.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/remove.png` & `jal-2023.4.5/jal/img/remove.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/tax.png` & `jal-2023.4.5/jal/img/tax.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/img/uralsib.ico` & `jal-2023.4.5/jal/img/uralsib.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/jal.py` & `jal-2023.4.5/jal/jal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/jal_init.sql` & `jal-2023.4.5/jal/jal_init.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/languages/en.qm` & `jal-2023.4.5/jal/languages/en.qm`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/languages/ru.qm` & `jal-2023.4.5/jal/languages/ru.qm`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/net/downloader.py` & `jal-2023.4.5/jal/net/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,44 +15,45 @@
 from jal.db.asset import JalAsset
 from jal.net.helpers import get_web_data, post_web_data, isEnglish
 
 
 # ===================================================================================================================
 # UI dialog class
 # ===================================================================================================================
-class QuotesUpdateDialog(QDialog, Ui_UpdateQuotesDlg):
+class QuotesUpdateDialog(QDialog):
     def __init__(self, parent):
-        QDialog.__init__(self, parent=parent)
-        self.setupUi(self)
-        self.StartDateEdit.setDate(QDate.currentDate().addMonths(-1))
-        self.EndDateEdit.setDate(QDate.currentDate())
+        super().__init__(parent=parent)
+        self.ui = Ui_UpdateQuotesDlg()
+        self.ui.setupUi(self)
+        self.ui.StartDateEdit.setDate(QDate.currentDate().addMonths(-1))
+        self.ui.EndDateEdit.setDate(QDate.currentDate())
         sources = JalAsset.get_sources_list()
         for source in sources:
             if source != MarketDataFeed.NA:
-                item = QListWidgetItem(sources[source], self.SourcesList)
+                item = QListWidgetItem(sources[source], self.ui.SourcesList)
                 item.setData(Qt.UserRole, source)
                 item.setCheckState(Qt.Checked)
-                self.SourcesList.addItem(item)
+                self.ui.SourcesList.addItem(item)
 
         # center dialog with respect to parent window
         x = parent.x() + parent.width() / 2 - self.width() / 2
         y = parent.y() + parent.height() / 2 - self.height() / 2
         self.setGeometry(x, y, self.width(), self.height())
 
     def getStartDate(self):
-        return self.StartDateEdit.dateTime().toSecsSinceEpoch()
+        return self.ui.StartDateEdit.dateTime().toSecsSinceEpoch()
 
     def getEndDate(self):
-        return self.EndDateEdit.dateTime().toSecsSinceEpoch()
+        return self.ui.EndDateEdit.dateTime().toSecsSinceEpoch()
 
     # Returns a list that contains IDs of all checked data sources
     def getSourceList(self):
         checked = []
-        for item_index in range(self.SourcesList.count()):
-            item = self.SourcesList.item(item_index)
+        for item_index in range(self.ui.SourcesList.count()):
+            item = self.ui.SourcesList.item(item_index)
             if item.checkState() == Qt.Checked:
                 checked.append(item.data(Qt.UserRole))
         return checked
 
 
 # ===================================================================================================================
 # Worker class
```

### Comparing `jal-2023.4.4/jal/net/helpers.py` & `jal-2023.4.5/jal/net/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/pypi_description.md` & `jal-2023.4.5/jal/pypi_description.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/reports/category.py` & `jal-2023.4.5/jal/reports/category.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,42 +31,43 @@
         super().__init__()
         self.group = self.tr("Operations")
         self.name = self.tr("by Category")
         self.window_class = "CategoryReportWindow"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class CategoryReportWindow(MdiWidget, Ui_CategoryReportWidget):
+class CategoryReportWindow(MdiWidget):
     def __init__(self, parent: Reports, settings: dict = None):
-        MdiWidget.__init__(self, parent.mdi_area())
-        self.setupUi(self)
+        super().__init__(parent.mdi_area())
+        self.ui = Ui_CategoryReportWidget()
+        self.ui.setupUi(self)
         self._parent = parent
 
-        self.category_model = CategoryOperationsModel(self.ReportTableView)
-        self.ReportTableView.setModel(self.category_model)
+        self.category_model = CategoryOperationsModel(self.ui.ReportTableView)
+        self.ui.ReportTableView.setModel(self.category_model)
         self.category_model.configureView()
 
         self.connect_signals_and_slots()
 
         if settings is not None:
-            self.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
-            self.ReportCategoryEdit.selected_id = settings['category_id']
+            self.ui.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
+            self.ui.ReportCategoryEdit.selected_id = settings['category_id']
             self.onCategoryChange()
 
     def connect_signals_and_slots(self):
-        self.ReportRange.changed.connect(self.ReportTableView.model().setDateRange)
-        self.ReportCategoryEdit.changed.connect(self.onCategoryChange)
-        self.ReportTableView.selectionModel().selectionChanged.connect(self.onOperationSelect)
+        self.ui.ReportRange.changed.connect(self.ui.ReportTableView.model().setDateRange)
+        self.ui.ReportCategoryEdit.changed.connect(self.onCategoryChange)
+        self.ui.ReportTableView.selectionModel().selectionChanged.connect(self.onOperationSelect)
 
     @Slot()
     def onCategoryChange(self):
-        self.ReportTableView.model().setCategory(self.ReportCategoryEdit.selected_id)
+        self.ui.ReportTableView.model().setCategory(self.ui.ReportCategoryEdit.selected_id)
 
     @Slot()
     def onOperationSelect(self, selected, _deselected):
         idx = selected.indexes()
         if idx:
             selected_row = idx[0].row()
-            operation_type, operation_id = self.ReportTableView.model().get_operation(selected_row)
-            self.OperationDetails.show_operation(operation_type, operation_id)
+            operation_type, operation_id = self.ui.ReportTableView.model().get_operation(selected_row)
+            self.ui.OperationDetails.show_operation(operation_type, operation_id)
         else:
-            self.OperationDetails.show_operation(LedgerTransaction.NA, 0)
+            self.ui.OperationDetails.show_operation(LedgerTransaction.NA, 0)
```

### Comparing `jal-2023.4.4/jal/reports/deals.py` & `jal-2023.4.5/jal/reports/deals.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,38 +292,39 @@
     def __init__(self):
         super().__init__()
         self.name = self.name = self.tr("Deals by Account")
         self.window_class = "DealsReportWindow"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class DealsReportWindow(MdiWidget, Ui_DealsReportWidget):
+class DealsReportWindow(MdiWidget):
     def __init__(self, parent: Reports, settings: dict = None):
-        MdiWidget.__init__(self, parent.mdi_area())
-        self.setupUi(self)
+        super().__init__(parent.mdi_area())
+        self.ui = Ui_DealsReportWidget()
+        self.ui.setupUi(self)
         self._parent = parent
 
         # Add available groupings
-        self.GroupCombo.addItem(self.tr("<None>"), "")
-        self.GroupCombo.addItem(self.tr("Asset"), "symbol")
-        self.GroupCombo.addItem(self.tr("Close"), "close_date")
-        self.GroupCombo.addItem(self.tr("Asset - Open - Close"), "symbol;open_date;close_date")
-        self.GroupCombo.addItem(self.tr("Open - Close"), "open_date;close_date")
-        self.GroupCombo.addItem(self.tr("Close - Open"), "close_date;open_date")
+        self.ui.GroupCombo.addItem(self.tr("<None>"), "")
+        self.ui.GroupCombo.addItem(self.tr("Asset"), "symbol")
+        self.ui.GroupCombo.addItem(self.tr("Close"), "close_date")
+        self.ui.GroupCombo.addItem(self.tr("Asset - Open - Close"), "symbol;open_date;close_date")
+        self.ui.GroupCombo.addItem(self.tr("Open - Close"), "open_date;close_date")
+        self.ui.GroupCombo.addItem(self.tr("Close - Open"), "close_date;open_date")
 
-        self.trades_model = ClosedTradesModel(self.ReportTreeView)
-        self.ReportTreeView.setModel(self.trades_model)
+        self.trades_model = ClosedTradesModel(self.ui.ReportTreeView)
+        self.ui.ReportTreeView.setModel(self.trades_model)
 
         self.connect_signals_and_slots()
 
     def connect_signals_and_slots(self):
-        self.ReportAccountBtn.changed.connect(self.onAccountChange)
-        self.ReportRange.changed.connect(self.ReportTreeView.model().setDatesRange)
-        self.GroupCombo.currentIndexChanged.connect(self.onGroupingChange)
+        self.ui.ReportAccountBtn.changed.connect(self.onAccountChange)
+        self.ui.ReportRange.changed.connect(self.ui.ReportTreeView.model().setDatesRange)
+        self.ui.GroupCombo.currentIndexChanged.connect(self.onGroupingChange)
 
     @Slot()
     def onAccountChange(self):
-        self.ReportTreeView.model().setAccount(self.ReportAccountBtn.account_id)
+        self.ui.ReportTreeView.model().setAccount(self.ui.ReportAccountBtn.account_id)
 
     @Slot()
     def onGroupingChange(self, idx):
-        self.ReportTreeView.model().setGrouping(self.GroupCombo.itemData(idx))
+        self.ui.ReportTreeView.model().setGrouping(self.ui.GroupCombo.itemData(idx))
```

### Comparing `jal-2023.4.4/jal/reports/holdings.py` & `jal-2023.4.5/jal/reports/holdings.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,55 +20,56 @@
     def __init__(self):
         super().__init__()
         self.name = self.tr("Holdings")
         self.window_class = "HoldingsReportWindow"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class HoldingsReportWindow(MdiWidget, Ui_HoldingsWidget):
+class HoldingsReportWindow(MdiWidget):
     def __init__(self, parent: Reports, settings: dict = None):
-        MdiWidget.__init__(self, parent.mdi_area())
-        self.setupUi(self)
+        super().__init__(parent.mdi_area())
+        self.ui = Ui_HoldingsWidget()
+        self.ui.setupUi(self)
         self._parent = parent
         self.name = self.tr("Holdings")
 
-        self.holdings_model = HoldingsModel(self.HoldingsTableView)
-        self.HoldingsTableView.setModel(self.holdings_model)
+        self.holdings_model = HoldingsModel(self.ui.HoldingsTableView)
+        self.ui.HoldingsTableView.setModel(self.holdings_model)
         self.holdings_model.configureView()
-        self.HoldingsTableView.setContextMenuPolicy(Qt.CustomContextMenu)
+        self.ui.HoldingsTableView.setContextMenuPolicy(Qt.CustomContextMenu)
 
         self.connect_signals_and_slots()
 
         # Setup holdings parameters
         current_time = QDateTime.currentDateTime()
         current_time.setTimeSpec(Qt.UTC)  # We use UTC everywhere so need to force TZ info
-        self.HoldingsDate.setDateTime(current_time)
-        self.HoldingsCurrencyCombo.setIndex(JalAsset.get_base_currency())
+        self.ui.HoldingsDate.setDateTime(current_time)
+        self.ui.HoldingsCurrencyCombo.setIndex(JalAsset.get_base_currency())
 
     def connect_signals_and_slots(self):
-        self.HoldingsDate.dateChanged.connect(self.HoldingsTableView.model().setDate)
-        self.HoldingsCurrencyCombo.changed.connect(self.HoldingsTableView.model().setCurrency)
-        self.HoldingsTableView.customContextMenuRequested.connect(self.onHoldingsContextMenu)
-        self.SaveButton.pressed.connect(partial(self._parent.save_report, self.name, self.HoldingsTableView.model()))
+        self.ui.HoldingsDate.dateChanged.connect(self.ui.HoldingsTableView.model().setDate)
+        self.ui.HoldingsCurrencyCombo.changed.connect(self.ui.HoldingsTableView.model().setCurrency)
+        self.ui.HoldingsTableView.customContextMenuRequested.connect(self.onHoldingsContextMenu)
+        self.ui.SaveButton.pressed.connect(partial(self._parent.save_report, self.name, self.ui.HoldingsTableView.model()))
 
     @Slot()
     def onHoldingsContextMenu(self, pos):
-        index = self.HoldingsTableView.indexAt(pos)
-        contextMenu = QMenu(self.HoldingsTableView)
-        actionShowChart = QAction(icon=load_icon("chart.png"), text=self.tr("Show Price Chart"), parent=self.HoldingsTableView)
+        index = self.ui.HoldingsTableView.indexAt(pos)
+        contextMenu = QMenu(self.ui.HoldingsTableView)
+        actionShowChart = QAction(icon=load_icon("chart.png"), text=self.tr("Show Price Chart"), parent=self.ui.HoldingsTableView)
         actionShowChart.triggered.connect(partial(self.showPriceChart, index))
         contextMenu.addAction(actionShowChart)
         tax_submenu = contextMenu.addMenu(load_icon("tax.png"), self.tr("Estimate tax"))
-        actionEstimateTaxPt = QAction(text=self.tr("Portugal"), parent=self.HoldingsTableView)
+        actionEstimateTaxPt = QAction(text=self.tr("Portugal"), parent=self.ui.HoldingsTableView)
         actionEstimateTaxPt.triggered.connect(partial(self.estimateRussianTax, index, 'pt'))
         tax_submenu.addAction(actionEstimateTaxPt)
-        actionEstimateTaxRu = QAction(text=self.tr("Russia"), parent=self.HoldingsTableView)
+        actionEstimateTaxRu = QAction(text=self.tr("Russia"), parent=self.ui.HoldingsTableView)
         actionEstimateTaxRu.triggered.connect(partial(self.estimateRussianTax, index, 'ru'))
         tax_submenu.addAction(actionEstimateTaxRu)
-        contextMenu.popup(self.HoldingsTableView.viewport().mapToGlobal(pos))
+        contextMenu.popup(self.ui.HoldingsTableView.viewport().mapToGlobal(pos))
 
     @Slot()
     def showPriceChart(self, index):
         model = index.model()
         account, asset, currency, asset_qty = model.get_data_for_tax(index)
         self._parent.mdi_area().addSubWindow(ChartWindow(account, asset, currency, asset_qty))
```

### Comparing `jal-2023.4.4/jal/reports/income_spending.py` & `jal-2023.4.5/jal/reports/income_spending.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,49 +323,50 @@
     def __init__(self):
         super().__init__()
         self.name = self.tr("Income & Spending")
         self.window_class = "IncomeSpendingReportWindow"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class IncomeSpendingReportWindow(MdiWidget, Ui_IncomeSpendingReportWidget):
+class IncomeSpendingReportWindow(MdiWidget):
     def __init__(self, parent: Reports, settings: dict = None):
-        MdiWidget.__init__(self, parent.mdi_area())
-        self.setupUi(self)
+        super().__init__(parent.mdi_area())
+        self.ui = Ui_IncomeSpendingReportWidget()
+        self.ui.setupUi(self)
         self._parent = parent
         self.name = self.tr("Income & Spending")
         self.current_index = None  # this is used in onOperationContextMenu() to track item for menu
 
-        self.income_spending_model = IncomeSpendingReportModel(self.ReportTreeView)
-        self.ReportTreeView.setModel(self.income_spending_model)
-        self.ReportTreeView.setContextMenuPolicy(Qt.CustomContextMenu)
+        self.income_spending_model = IncomeSpendingReportModel(self.ui.ReportTreeView)
+        self.ui.ReportTreeView.setModel(self.income_spending_model)
+        self.ui.ReportTreeView.setContextMenuPolicy(Qt.CustomContextMenu)
 
         # Operations view context menu
-        self.contextMenu = QMenu(self.ReportTreeView)
+        self.contextMenu = QMenu(self.ui.ReportTreeView)
         self.actionDetails = QAction(load_icon("list.png"), self.tr("Show operations"), self)
         self.contextMenu.addAction(self.actionDetails)
 
         self.connect_signals_and_slots()
 
         if settings is None:
-            begin, end = self.ReportRange.getRange()
+            begin, end = self.ui.ReportRange.getRange()
             settings = {'begin_ts': begin, 'end_ts': end, 'currency_id': JalAsset.get_base_currency()}
-        self.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
-        self.CurrencyCombo.setIndex(settings['currency_id'])
+        self.ui.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
+        self.ui.CurrencyCombo.setIndex(settings['currency_id'])
 
     def connect_signals_and_slots(self):
-        self.ReportRange.changed.connect(self.ReportTreeView.model().setDatesRange)
-        self.CurrencyCombo.changed.connect(self.ReportTreeView.model().setCurrency)
-        self.ReportTreeView.customContextMenuRequested.connect(self.onCellContextMenu)
+        self.ui.ReportRange.changed.connect(self.ui.ReportTreeView.model().setDatesRange)
+        self.ui.CurrencyCombo.changed.connect(self.ui.ReportTreeView.model().setCurrency)
+        self.ui.ReportTreeView.customContextMenuRequested.connect(self.onCellContextMenu)
         self.actionDetails.triggered.connect(self.showDetailsReport)
-        self.SaveButton.pressed.connect(partial(self._parent.save_report, self.name, self.ReportTreeView.model()))
+        self.ui.SaveButton.pressed.connect(partial(self._parent.save_report, self.name, self.ui.ReportTreeView.model()))
 
     @Slot()
     def onCellContextMenu(self, position):
-        self.current_index = self.ReportTreeView.indexAt(position)
+        self.current_index = self.ui.ReportTreeView.indexAt(position)
         if self.current_index.isValid() and self.current_index.column() != 0:
-            self.contextMenu.popup(self.ReportTreeView.viewport().mapToGlobal(position))
+            self.contextMenu.popup(self.ui.ReportTreeView.viewport().mapToGlobal(position))
 
     @Slot()
     def showDetailsReport(self):
         details = self.income_spending_model.data(self.current_index, Qt.UserRole)
         self._parent.show_report("CategoryReportWindow", details)
```

### Comparing `jal-2023.4.4/jal/reports/peer.py` & `jal-2023.4.5/jal/reports/peer.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,42 +31,43 @@
         super().__init__()
         self.group = self.tr("Operations")
         self.name = self.tr("by Peer")
         self.window_class = "PeerReportWindow"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class PeerReportWindow(MdiWidget, Ui_PeerReportWidget):
+class PeerReportWindow(MdiWidget):
     def __init__(self, parent: Reports, settings: dict = None):
-        MdiWidget.__init__(self, parent.mdi_area())
-        self.setupUi(self)
+        super().__init__(parent.mdi_area())
+        self.ui = Ui_PeerReportWidget()
+        self.ui.setupUi(self)
         self._parent = parent
 
-        self.peer_model = PeerOperationsModel(self.ReportTableView)
-        self.ReportTableView.setModel(self.peer_model)
+        self.peer_model = PeerOperationsModel(self.ui.ReportTableView)
+        self.ui.ReportTableView.setModel(self.peer_model)
         self.peer_model.configureView()
 
         self.connect_signals_and_slots()
 
         if settings is not None:
-            self.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
-            self.ReportPeerEdit.selected_id = settings['peer_id']
+            self.ui.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
+            self.ui.ReportPeerEdit.selected_id = settings['peer_id']
             self.onPeerChange()
 
     def connect_signals_and_slots(self):
-        self.ReportRange.changed.connect(self.ReportTableView.model().setDateRange)
-        self.ReportPeerEdit.changed.connect(self.onPeerChange)
-        self.ReportTableView.selectionModel().selectionChanged.connect(self.onOperationSelect)
+        self.ui.ReportRange.changed.connect(self.ui.ReportTableView.model().setDateRange)
+        self.ui.ReportPeerEdit.changed.connect(self.onPeerChange)
+        self.ui.ReportTableView.selectionModel().selectionChanged.connect(self.onOperationSelect)
 
     @Slot()
     def onPeerChange(self):
-        self.ReportTableView.model().setPeer(self.ReportPeerEdit.selected_id)
+        self.ui.ReportTableView.model().setPeer(self.ui.ReportPeerEdit.selected_id)
 
     @Slot()
     def onOperationSelect(self, selected, _deselected):
         idx = selected.indexes()
         if idx:
             selected_row = idx[0].row()
-            operation_type, operation_id = self.ReportTableView.model().get_operation(selected_row)
-            self.OperationDetails.show_operation(operation_type, operation_id)
+            operation_type, operation_id = self.ui.ReportTableView.model().get_operation(selected_row)
+            self.ui.OperationDetails.show_operation(operation_type, operation_id)
         else:
-            self.OperationDetails.show_operation(LedgerTransaction.NA, 0)
+            self.ui.OperationDetails.show_operation(LedgerTransaction.NA, 0)
```

### Comparing `jal-2023.4.4/jal/reports/profit_loss.py` & `jal-2023.4.5/jal/reports/profit_loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import decimal
 from functools import partial
 from decimal import Decimal
 
 from PySide6.QtCore import Qt, Slot, QObject, QAbstractTableModel
 from jal.ui.reports.ui_profit_loss_report import Ui_ProfitLossReportWidget
 from jal.reports.reports import Reports
 from jal.db.account import JalAccount
@@ -112,15 +113,15 @@
                 row_name = self.tr("Period end")
                 money_p = money_0
                 assets_p = assets_0
             else:
                 row_name = f"{month['year']} {self.month_name[month['month'] - 1]}"
             try:
                 rel_change = ((values['money'] + values['assets']) - (money_p + assets_p)) / (money_p + assets_p)
-            except ZeroDivisionError:
+            except (ZeroDivisionError, decimal.InvalidOperation):
                 rel_change = Decimal('0')
             data_row = [row_name, values['money'], values['transfers'], values['dividends'], values['interest'],
                         values['fees'], values['taxes'], values['assets'], values['p&l'],
                         values['total'], (values['money'] + values['assets']) - (money_p + assets_p),
                         rel_change]
             self._data.append(data_row)
             money_p = values['money']
@@ -153,29 +154,30 @@
     def __init__(self):
         super().__init__()
         self.name = self.tr("P&L by Account")
         self.window_class = "ProfitLossReportWindow"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class ProfitLossReportWindow(MdiWidget, Ui_ProfitLossReportWidget):
+class ProfitLossReportWindow(MdiWidget):
     def __init__(self, parent: Reports, settings: dict = None):
-        MdiWidget.__init__(self, parent.mdi_area())
-        self.setupUi(self)
+        super().__init__(parent.mdi_area())
+        self.ui = Ui_ProfitLossReportWidget()
+        self.ui.setupUi(self)
         self._parent = parent
         self.name = self.tr("P&L by Account")
 
-        self.pl_model = ProfitLossModel(self.ReportTableView)
-        self.ReportTableView.setModel(self.pl_model)
+        self.pl_model = ProfitLossModel(self.ui.ReportTableView)
+        self.ui.ReportTableView.setModel(self.pl_model)
 
         self.connect_signals_and_slots()
 
     def connect_signals_and_slots(self):
-        self.ReportRange.changed.connect(self.ReportTableView.model().setDatesRange)
-        self.ReportAccountEdit.changed.connect(self.onAccountChange)
-        self.SaveButton.pressed.connect(partial(self._parent.save_report, self.name, self.ReportTableView.model()))
+        self.ui.ReportRange.changed.connect(self.ui.ReportTableView.model().setDatesRange)
+        self.ui.ReportAccountEdit.changed.connect(self.onAccountChange)
+        self.ui.SaveButton.pressed.connect(partial(self._parent.save_report, self.name, self.ui.ReportTableView.model()))
 
     @Slot()
     def onAccountChange(self):
-        account_id = self.ReportAccountEdit.selected_id
-        self.ReportTableView.model().setAccount(account_id)
-        self.CurrencyLbl.setText(self.tr("Currency: ") + JalAsset(JalAccount(account_id).currency()).symbol())
+        account_id = self.ui.ReportAccountEdit.selected_id
+        self.ui.ReportTableView.model().setAccount(account_id)
+        self.ui.CurrencyLbl.setText(self.tr("Currency: ") + JalAsset(JalAccount(account_id).currency()).symbol())
```

### Comparing `jal-2023.4.4/jal/reports/reports.py` & `jal-2023.4.5/jal/reports/reports.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/reports/tag.py` & `jal-2023.4.5/jal/reports/tag.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,42 +31,43 @@
         super().__init__()
         self.group = self.tr("Operations")
         self.name = self.tr("by Tag")
         self.window_class = "TagReportWindow"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class TagReportWindow(MdiWidget, Ui_TagReportWidget):
+class TagReportWindow(MdiWidget):
     def __init__(self, parent: Reports, settings: dict = None):
-        MdiWidget.__init__(self, parent.mdi_area())
-        self.setupUi(self)
+        super().__init__(parent.mdi_area())
+        self.ui = Ui_TagReportWidget()
+        self.ui.setupUi(self)
         self._parent = parent
 
-        self.tag_model = TagOperationsModel(self.ReportTableView)
-        self.ReportTableView.setModel(self.tag_model)
+        self.tag_model = TagOperationsModel(self.ui.ReportTableView)
+        self.ui.ReportTableView.setModel(self.tag_model)
         self.tag_model.configureView()
 
         self.connect_signals_and_slots()
 
         if settings is not None:
-            self.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
-            self.ReportTagEdit.selected_id = settings['tag_id']
+            self.ui.ReportRange.setRange(settings['begin_ts'], settings['end_ts'])
+            self.ui.ReportTagEdit.selected_id = settings['tag_id']
             self.onTagChange()
 
     def connect_signals_and_slots(self):
-        self.ReportRange.changed.connect(self.ReportTableView.model().setDateRange)
-        self.ReportTagEdit.changed.connect(self.onTagChange)
-        self.ReportTableView.selectionModel().selectionChanged.connect(self.onOperationSelect)
+        self.ui.ReportRange.changed.connect(self.ui.ReportTableView.model().setDateRange)
+        self.ui.ReportTagEdit.changed.connect(self.onTagChange)
+        self.ui.ReportTableView.selectionModel().selectionChanged.connect(self.onOperationSelect)
 
     @Slot()
     def onTagChange(self):
-        self.ReportTableView.model().setTag(self.ReportTagEdit.selected_id)
+        self.ui.ReportTableView.model().setTag(self.ui.ReportTagEdit.selected_id)
 
     @Slot()
     def onOperationSelect(self, selected, _deselected):
         idx = selected.indexes()
         if idx:
             selected_row = idx[0].row()
-            operation_type, operation_id = self.ReportTableView.model().get_operation(selected_row)
-            self.OperationDetails.show_operation(operation_type, operation_id)
+            operation_type, operation_id = self.ui.ReportTableView.model().get_operation(selected_row)
+            self.ui.OperationDetails.show_operation(operation_type, operation_id)
         else:
-            self.OperationDetails.show_operation(LedgerTransaction.NA, 0)
+            self.ui.OperationDetails.show_operation(LedgerTransaction.NA, 0)
```

### Comparing `jal-2023.4.4/jal/ui/reports/ui_category_report.py` & `jal-2023.4.5/jal/ui/reports/ui_category_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/reports/ui_deals_report.py` & `jal-2023.4.5/jal/ui/reports/ui_deals_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/reports/ui_holdings_report.py` & `jal-2023.4.5/jal/ui/reports/ui_holdings_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/reports/ui_income_spending_report.py` & `jal-2023.4.5/jal/ui/reports/ui_income_spending_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/reports/ui_peer_report.py` & `jal-2023.4.5/jal/ui/reports/ui_peer_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/reports/ui_profit_loss_report.py` & `jal-2023.4.5/jal/ui/reports/ui_profit_loss_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/reports/ui_tag_report.py` & `jal-2023.4.5/jal/ui/reports/ui_tag_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/reports/ui_tax_estimation.py` & `jal-2023.4.5/jal/ui/reports/ui_tax_estimation.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_asset_dlg.py` & `jal-2023.4.5/jal/ui/ui_asset_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_flow_export_widget.py` & `jal-2023.4.5/jal/ui/ui_flow_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_login_fns_dlg.py` & `jal-2023.4.5/jal/ui/ui_login_fns_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_main_window.py` & `jal-2023.4.5/jal/ui/ui_main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_operations_widget.py` & `jal-2023.4.5/jal/ui/ui_operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_rebuild_window.py` & `jal-2023.4.5/jal/ui/ui_rebuild_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_reference_data_dlg.py` & `jal-2023.4.5/jal/ui/ui_reference_data_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_select_account_dlg.py` & `jal-2023.4.5/jal/ui/ui_select_account_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_select_reference_dlg.py` & `jal-2023.4.5/jal/ui/ui_select_reference_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_slip_import_dlg.py` & `jal-2023.4.5/jal/ui/ui_slip_import_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_tax_export_widget.py` & `jal-2023.4.5/jal/ui/ui_tax_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/ui/ui_update_quotes_window.py` & `jal-2023.4.5/jal/ui/ui_update_quotes_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_10.sql` & `jal-2023.4.5/jal/updates/jal_delta_10.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_11.sql` & `jal-2023.4.5/jal/updates/jal_delta_11.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_12.sql` & `jal-2023.4.5/jal/updates/jal_delta_12.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_13.sql` & `jal-2023.4.5/jal/updates/jal_delta_13.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_14.sql` & `jal-2023.4.5/jal/updates/jal_delta_14.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_15.sql` & `jal-2023.4.5/jal/updates/jal_delta_15.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_16.sql` & `jal-2023.4.5/jal/updates/jal_delta_16.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_17.sql` & `jal-2023.4.5/jal/updates/jal_delta_17.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_18.sql` & `jal-2023.4.5/jal/updates/jal_delta_18.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_19.sql` & `jal-2023.4.5/jal/updates/jal_delta_19.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_20.sql` & `jal-2023.4.5/jal/updates/jal_delta_20.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_21.sql` & `jal-2023.4.5/jal/updates/jal_delta_21.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_22.sql` & `jal-2023.4.5/jal/updates/jal_delta_22.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_23.sql` & `jal-2023.4.5/jal/updates/jal_delta_23.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_25.sql` & `jal-2023.4.5/jal/updates/jal_delta_25.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_26.sql` & `jal-2023.4.5/jal/updates/jal_delta_26.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_27.sql` & `jal-2023.4.5/jal/updates/jal_delta_27.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_28.sql` & `jal-2023.4.5/jal/updates/jal_delta_28.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_29.sql` & `jal-2023.4.5/jal/updates/jal_delta_29.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_30.sql` & `jal-2023.4.5/jal/updates/jal_delta_30.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_31.sql` & `jal-2023.4.5/jal/updates/jal_delta_31.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_32.sql` & `jal-2023.4.5/jal/updates/jal_delta_32.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_33.sql` & `jal-2023.4.5/jal/updates/jal_delta_33.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_34.sql` & `jal-2023.4.5/jal/updates/jal_delta_34.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_35.sql` & `jal-2023.4.5/jal/updates/jal_delta_35.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_36.sql` & `jal-2023.4.5/jal/updates/jal_delta_36.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_37.sql` & `jal-2023.4.5/jal/updates/jal_delta_37.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_38.sql` & `jal-2023.4.5/jal/updates/jal_delta_38.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_40.sql` & `jal-2023.4.5/jal/updates/jal_delta_40.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_41.sql` & `jal-2023.4.5/jal/updates/jal_delta_41.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_42.sql` & `jal-2023.4.5/jal/updates/jal_delta_42.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_43.sql` & `jal-2023.4.5/jal/updates/jal_delta_43.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/updates/jal_delta_44.sql` & `jal-2023.4.5/jal/updates/jal_delta_44.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/abstract_operation_details.py` & `jal-2023.4.5/jal/widgets/abstract_operation_details.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/account_select.py` & `jal-2023.4.5/jal/widgets/account_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,37 +51,38 @@
         self.account_id = 0
 
 
 #-----------------------------------------------------------------------------------------------------------------------
 # Dialog for account selection
 # Constructor takes description to show and recent_account for default choice.
 # Selected account won't be equal to current_account
-class SelectAccountDialog(QDialog, Ui_SelectAccountDlg):
+class SelectAccountDialog(QDialog):
     def __init__(self, description, current_account, recent_account=None):
-        QDialog.__init__(self)
-        self.setupUi(self)
+        super().__init__()
+        self.ui = Ui_SelectAccountDlg()
+        self.ui.setupUi(self)
         self.account_id = recent_account
         self.store_account = False
         self.current_account = current_account
 
-        self.DescriptionLbl.setText(description)
+        self.ui.DescriptionLbl.setText(description)
         if self.account_id:
-            self.AccountWidget.selected_id = self.account_id
+            self.ui.AccountWidget.selected_id = self.account_id
         center_window(self)
 
     @Slot()
     def closeEvent(self, event):
-        self.account_id = self.AccountWidget.selected_id
-        self.store_account = self.ReuseAccount.isChecked()
-        if self.AccountWidget.selected_id == 0:
+        self.account_id = self.ui.AccountWidget.selected_id
+        self.store_account = self.ui.ReuseAccount.isChecked()
+        if self.ui.AccountWidget.selected_id == 0:
             QMessageBox().warning(None, self.tr("No selection"), self.tr("Invalid account selected"), QMessageBox.Ok)
             event.ignore()
             return
 
-        if self.AccountWidget.selected_id == self.current_account:
+        if self.ui.AccountWidget.selected_id == self.current_account:
             QMessageBox().warning(None, self.tr("No selection"), self.tr("Please select different account"),
                                   QMessageBox.Ok)
             event.ignore()
             return
 
         self.setResult(QDialog.Accepted)
         event.accept()
```

### Comparing `jal-2023.4.4/jal/widgets/asset_dialog.py` & `jal-2023.4.5/jal/widgets/asset_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from decimal import Decimal
-from PySide6.QtCore import Qt, Property, QDateTime, QLocale
+from PySide6.QtCore import Qt, Property, QDateTime, QTimeZone, QLocale
 from PySide6.QtSql import QSqlRelation, QSqlRelationalDelegate
 from PySide6.QtWidgets import QDialog, QDataWidgetMapper, QStyledItemDelegate, QComboBox, QLineEdit
 from jal.ui.ui_asset_dlg import Ui_AssetDialog
 from jal.constants import PredefinedAsset, AssetData
 from jal.db.helpers import load_icon, localize_decimal
 from jal.widgets.delegates import DateTimeEditWithReset, BoolDelegate
 from jal.db.reference_models import AbstractReferenceListModel
@@ -17,56 +17,57 @@
                          ("type_id", 'Asset type'),
                          ("full_name", self.tr("Asset name")),
                          ("isin", self.tr("ISIN")),
                          ("country_id", self.tr("Country")),
                          ("base_asset", self.tr("Base asset"))]
 
 
-class AssetDialog(QDialog, Ui_AssetDialog):
-    def __init__(self):
-        QDialog.__init__(self)
-        self.setupUi(self)
+class AssetDialog(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.ui = Ui_AssetDialog()
+        self.ui.setupUi(self)
         self._asset_id = -1
         # Custom model to allow common submit errors handling and error message display
         self._model = AssetsListModel("assets", self)
 
         self._mapper = QDataWidgetMapper(self._model)
         self._mapper.setModel(self._model)
         self._mapper.setSubmitPolicy(QDataWidgetMapper.AutoSubmit)
 
-        self._mapper.addMapping(self.NameEdit, self._model.fieldIndex("full_name"))
-        self._mapper.addMapping(self.isinEdit, self._model.fieldIndex("isin"))
-        self._mapper.addMapping(self.TypeCombo, self._model.fieldIndex("type_id"))
-        self._mapper.addMapping(self.CountryCombo, self._model.fieldIndex("country_id"))
-        self._mapper.addMapping(self.BaseAssetSelector, self._model.fieldIndex("base_asset"))
+        self._mapper.addMapping(self.ui.NameEdit, self._model.fieldIndex("full_name"))
+        self._mapper.addMapping(self.ui.isinEdit, self._model.fieldIndex("isin"))
+        self._mapper.addMapping(self.ui.TypeCombo, self._model.fieldIndex("type_id"))
+        self._mapper.addMapping(self.ui.CountryCombo, self._model.fieldIndex("country_id"))
+        self._mapper.addMapping(self.ui.BaseAssetSelector, self._model.fieldIndex("base_asset"))
 
         self._model.select()
 
-        self._symbols_model = SymbolsListModel("asset_tickers", self.SymbolsTable)
-        self.SymbolsTable.setModel(self._symbols_model)
+        self._symbols_model = SymbolsListModel("asset_tickers", self.ui.SymbolsTable)
+        self.ui.SymbolsTable.setModel(self._symbols_model)
         self._symbols_model.select()
         self._symbols_model.configureView()
 
-        self._data_model = ExtraDataModel("asset_data", self.DataTable)
-        self.DataTable.setModel(self._data_model)
+        self._data_model = ExtraDataModel("asset_data", self.ui.DataTable)
+        self.ui.DataTable.setModel(self._data_model)
         self._data_model.select()
         self._data_model.configureView()
 
-        self.AddSymbolButton.setIcon(load_icon("add.png"))
-        self.RemoveSymbolButton.setIcon(load_icon("delete.png"))
-        self.AddDataButton.setIcon(load_icon("add.png"))
-        self.RemoveDataButton.setIcon(load_icon("delete.png"))
-        self.OkButton.setIcon(load_icon("accept.png"))
-        self.CancelButton.setIcon(load_icon("cancel.png"))
-
-        self.TypeCombo.currentIndexChanged.connect(self.onTypeUpdate)
-        self.AddSymbolButton.clicked.connect(self.onAddSymbol)
-        self.RemoveSymbolButton.clicked.connect(self.onRemoveSymbol)
-        self.AddDataButton.clicked.connect(self.onAddData)
-        self.RemoveDataButton.clicked.connect(self.onRemoveData)
+        self.ui.AddSymbolButton.setIcon(load_icon("add.png"))
+        self.ui.RemoveSymbolButton.setIcon(load_icon("delete.png"))
+        self.ui.AddDataButton.setIcon(load_icon("add.png"))
+        self.ui.RemoveDataButton.setIcon(load_icon("delete.png"))
+        self.ui.OkButton.setIcon(load_icon("accept.png"))
+        self.ui.CancelButton.setIcon(load_icon("cancel.png"))
+
+        self.ui.TypeCombo.currentIndexChanged.connect(self.onTypeUpdate)
+        self.ui.AddSymbolButton.clicked.connect(self.onAddSymbol)
+        self.ui.RemoveSymbolButton.clicked.connect(self.onRemoveSymbol)
+        self.ui.AddDataButton.clicked.connect(self.onAddData)
+        self.ui.RemoveDataButton.clicked.connect(self.onRemoveData)
 
     def getSelectedId(self):
         return self._asset_id
 
     def setSelectedId(self, asset_id):
         self._asset_id = asset_id
         self._model.setFilter(f"id={self._asset_id}")
@@ -104,40 +105,40 @@
 
     def reject(self) -> None:
         for model in [self._data_model, self._symbols_model, self._model]:
             model.revertAll()
         super().reject()
 
     def onTypeUpdate(self, _index):
-        if self.TypeCombo.key == PredefinedAsset.Derivative:
-            self.BaseAssetSelector.setEnabled(True)
-            self.isinEdit.setEnabled(False)
-        elif self.TypeCombo.key == PredefinedAsset.Money or self.TypeCombo.key == PredefinedAsset.Commodity:
-            self.BaseAssetSelector.setEnabled(False)
-            self.isinEdit.setEnabled(False)
+        if self.ui.TypeCombo.key == PredefinedAsset.Derivative:
+            self.ui.BaseAssetSelector.setEnabled(True)
+            self.ui.isinEdit.setEnabled(False)
+        elif self.ui.TypeCombo.key == PredefinedAsset.Money or self.ui.TypeCombo.key == PredefinedAsset.Commodity:
+            self.ui.BaseAssetSelector.setEnabled(False)
+            self.ui.isinEdit.setEnabled(False)
         else:
-            self.BaseAssetSelector.setEnabled(False)
-            self.isinEdit.setEnabled(True)
+            self.ui.BaseAssetSelector.setEnabled(False)
+            self.ui.isinEdit.setEnabled(True)
 
     def onAddSymbol(self):
-        idx = self.SymbolsTable.selectionModel().selection().indexes()
+        idx = self.ui.SymbolsTable.selectionModel().selection().indexes()
         current_index = idx[0] if idx else self._symbols_model.index(0, 0)
         self._symbols_model.addElement(current_index)
 
     def onRemoveSymbol(self):
-        idx = self.SymbolsTable.selectionModel().selection().indexes()
+        idx = self.ui.SymbolsTable.selectionModel().selection().indexes()
         current_index = idx[0] if idx else self._symbols_model.index(0, 0)
         self._symbols_model.removeElement(current_index)
 
     def onAddData(self):
-        idx = self.DataTable.selectionModel().selection().indexes()
+        idx = self.ui.DataTable.selectionModel().selection().indexes()
         current_index = idx[0] if idx else self._data_model.index(0, 0)
         self._data_model.addElement(current_index)
     def onRemoveData(self):
-        idx = self.DataTable.selectionModel().selection().indexes()
+        idx = self.ui.DataTable.selectionModel().selection().indexes()
         current_index = idx[0] if idx else self._data_model.index(0, 0)
         self._data_model.removeElement(current_index)
 
 
 class SymbolsListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
         AbstractReferenceListModel.__init__(self, table, parent_view)
@@ -222,15 +223,15 @@
         elif index.column() == self._value:
             type_idx = index.model().data(index.sibling(index.row(), self._key), role=Qt.EditRole)
             if self.types[type_idx][1] == "str":
                 editor.setText(index.model().data(index, Qt.EditRole))
             elif self.types[type_idx][1] == "date":
                 try:
                     timestamp = int(index.model().data(index, Qt.EditRole))
-                    editor.setDateTime(QDateTime.fromSecsSinceEpoch(timestamp, spec=Qt.UTC))
+                    editor.setDateTime(QDateTime.fromSecsSinceEpoch(timestamp, QTimeZone(0)))
                 except ValueError:
                     QStyledItemDelegate.setEditorData(self, editor, index)
             elif self.types[type_idx][1] == "float":
                 try:
                     amount = Decimal(index.model().data(index, Qt.EditRole))
                 except (ValueError, TypeError):
                     amount = Decimal('0')
```

### Comparing `jal-2023.4.4/jal/widgets/corporate_action_widget.py` & `jal-2023.4.5/jal/widgets/corporate_action_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/custom/date_range_selector.py` & `jal-2023.4.5/jal/widgets/custom/date_range_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide6.QtCore import Qt, Signal, Slot, QDateTime, Property
+from PySide6.QtCore import Qt, Signal, Slot, Property, QDateTime, QTimeZone
 from PySide6.QtWidgets import QWidget, QComboBox, QHBoxLayout, QLabel, QDateEdit
 from jal.widgets.helpers import ManipulateDate
 
 
 ITEM_NAME = 0
 ITEM_METHOD = 1
 # ----------------------------------------------------------------------------------------------------------------------
@@ -78,16 +78,16 @@
     def connect_signals_and_slots(self):
         self.range_combo.currentIndexChanged.connect(self.onRangeChange)
         self.from_date.dateChanged.connect(self.onFromChange)
         self.to_date.dateChanged.connect(self.onToChange)
 
     def _update_range(self):
         self.changing_range = True
-        self.from_date.setDateTime(QDateTime.fromSecsSinceEpoch(self._begin, spec=Qt.UTC))
-        self.to_date.setDateTime(QDateTime.fromSecsSinceEpoch(self._end, spec=Qt.UTC))
+        self.from_date.setDateTime(QDateTime.fromSecsSinceEpoch(self._begin, QTimeZone(0)))
+        self.to_date.setDateTime(QDateTime.fromSecsSinceEpoch(self._end, QTimeZone(0)))
         self.changing_range = False
         self.changed.emit(self._begin, self._end)
 
     def setRange(self, begin_ts, end_ts):
         self._begin = begin_ts
         self._end = end_ts
         self._update_range()
```

### Comparing `jal-2023.4.4/jal/widgets/custom/db_lookup_combobox.py` & `jal-2023.4.5/jal/widgets/custom/db_lookup_combobox.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/custom/log_viewer.py` & `jal-2023.4.5/jal/widgets/custom/log_viewer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,85 @@
+import os
 import logging
 from jal.constants import CustomColor
 from PySide6.QtCore import Qt, Slot
 from PySide6.QtWidgets import QApplication, QPlainTextEdit, QLabel, QPushButton
 from PySide6.QtGui import QBrush
 
 
-class LogViewer(QPlainTextEdit, logging.Handler):
+# Adapter class to have custom log handler that may be passed to logger.addHandler/logger.removeHandler methods and
+# then forward all messages parent view to display them
+class LogHandler(logging.Handler):
+    def __init__(self, parent_view):
+        self._parent_view = parent_view
+        super().__init__()
+
+    def emit(self, record, **kwargs):
+        message = self.format(record)
+        self._parent_view.displayMessage(record.levelno, message)
+
+
+# A GUI class to display messages from python logging unit in a normal multi-line text area
+class LogViewer(QPlainTextEdit):
     def __init__(self, parent=None):
-        QPlainTextEdit.__init__(self, parent)
-        logging.Handler.__init__(self)
+        super().__init__(parent)
         self.app = QApplication.instance()
+        self._logger = None     # Here an instance of current logger will be stored
+        self._log_handler = LogHandler(self)
         self.setReadOnly(True)
         self.status_bar = None    # Status bar where notifications and control are located
         self.expandButton = None  # Button that shows/hides log window
         self.notification = None  # Here is QLabel element to display LOG update status
         self.clear_color = None   # Variable to store initial "clear" background color
         self.collapsed_text = self.tr("▶ logs")
         self.expanded_text = self.tr("▲ logs")
 
-    def emit(self, record, **kwargs):
+    def startLogging(self):
+        self._logger = logging.getLogger()
+        self._logger.addHandler(self._log_handler)
+        log_level = os.environ.get('LOGLEVEL', 'INFO').upper()
+        self._logger.setLevel(log_level)
+        self._log_handler.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s - %(message)s'))
+
+    def stopLogging(self):
+        self._logger.removeHandler(self._log_handler)    # Removing handler (but it doesn't prevent exception at exit)
+        logging.raiseExceptions = False                  # Silencing logging module exceptions
+
+    def displayMessage(self, level: int, message: str):
         predefinded_colors = {
             logging.DEBUG: CustomColor.Grey,
             logging.INFO: self.clear_color,
             logging.WARNING: CustomColor.LightRed,
             logging.ERROR: CustomColor.LightRed,
             logging.CRITICAL: CustomColor.LightRed
         }
         try:
-            msg_color = predefinded_colors[record.levelno]
+            msg_color = predefinded_colors[level]
         except KeyError:
-            self.appendPlainText(self.tr("Unknown logging level provided: ") + f"{record.levelno}")
+            self.appendPlainText(self.tr("Unknown logging level provided: ") + f"{level}")
             msg_color = CustomColor.LightRed
 
         # Store message in log window
-        msg = self.format(record)
         tf = self.currentCharFormat()
         tf.setForeground(QBrush(msg_color))
         self.setCurrentCharFormat(tf)
-        self.appendPlainText(msg)
+        self.appendPlainText(message)
 
         # Show in status bar
         if self.notification:
             palette = self.notification.palette()
             palette.setColor(self.notification.foregroundRole(), msg_color)
             self.notification.setPalette(palette)
-            msg = msg.replace('\n', "; ")  # Get rid of new lines in error message
+            msg = message.replace('\n', "; ")  # Get rid of new lines in error message
             elided_text = self.notification.fontMetrics().elidedText(msg, Qt.ElideRight, self.get_available_width())
             self.notification.setText(elided_text)
         # Set button color
         if self.expandButton:
             palette = self.expandButton.palette()
             palette.setColor(self.expandButton.foregroundRole(), msg_color)
-
         self.app.processEvents()
 
     def showEvent(self, event):
         self.cleanNotification()
         super().showEvent(event)
 
     def setStatusBar(self, status_bar):
@@ -68,15 +92,14 @@
         self.expandButton.clicked.connect(self.showLogs)
         self.status_bar.addWidget(self.expandButton)
 
         self.notification = QLabel(self)
         self.status_bar.addWidget(self.notification)
         self.notification.setAutoFillBackground(True)
         self.clear_color = self.expandButton.palette().color(self.notification.foregroundRole())
-        self.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s - %(message)s'))
 
     def removeStatusBar(self):
         self.cleanNotification()
         self.notification = None
 
     def cleanNotification(self):
         if self.notification:
```

### Comparing `jal-2023.4.4/jal/widgets/delegates.py` & `jal-2023.4.5/jal/widgets/delegates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 from decimal import Decimal, InvalidOperation
 from PySide6.QtWidgets import QWidget, QStyledItemDelegate, QLineEdit, QDateTimeEdit, QTreeView
-from PySide6.QtCore import Qt, QModelIndex, QEvent, QLocale, QDateTime, QDate, QTime
+from PySide6.QtCore import Qt, QModelIndex, QEvent, QLocale, QDateTime, QDate, QTime, QTimeZone
 from PySide6.QtGui import QDoubleValidator, QBrush, QKeyEvent
 from jal.constants import CustomColor
 from jal.widgets.reference_selector import AssetSelector, PeerSelector, CategorySelector, TagSelector
 from jal.db.db import JalModel
 from jal.db.helpers import localize_decimal, delocalize_decimal
 from jal.db.account import JalAccount
 
@@ -86,15 +86,15 @@
         return editor
 
     def setEditorData(self, editor, index):
         timestamp = index.model().data(index, Qt.EditRole)
         if timestamp == '':
             QStyledItemDelegate.setEditorData(self, editor, index)
         else:
-            editor.setDateTime(QDateTime.fromSecsSinceEpoch(timestamp, spec=Qt.UTC))
+            editor.setDateTime(QDateTime.fromSecsSinceEpoch(timestamp, QTimeZone(0)))
 
     def setModelData(self, editor, model, index):
         timestamp = editor.dateTime().toSecsSinceEpoch()
         model.setData(index, timestamp)
 
     def paint(self, painter, option, index):
         super().paint(painter, option, index)
```

### Comparing `jal-2023.4.4/jal/widgets/dividend_widget.py` & `jal-2023.4.5/jal/widgets/dividend_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/helpers.py` & `jal-2023.4.5/jal/widgets/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
                            'begin_ts': month_start_ts(year, month), 'end_ts': month_end_ts(year, month)})
     return result
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Function takes an image and searches for QR in it. Content of first found QR is returned. Otherwise - empty string.
 def decodeQR(qr_image: QImage) -> str:
+    if qr_image.isNull():
+        return ''
     if not dependency_present(['pyzbar']):
         logging.warning("Package pyzbar not found for QR recognition.")
         return ''
     qr_image.convertTo(QImage.Format_Grayscale8)
     # bytesPerXXX is more accurate than width and height
     data = (qr_image.bits().tobytes(), qr_image.bytesPerLine(), int(qr_image.sizeInBytes()/qr_image.bytesPerLine()))
     barcodes = pyzbar.decode(data, symbols=[pyzbar.ZBarSymbol.QRCODE])
```

### Comparing `jal-2023.4.4/jal/widgets/income_spending_widget.py` & `jal-2023.4.5/jal/widgets/income_spending_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/main_window.py` & `jal-2023.4.5/jal/widgets/main_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,85 +27,83 @@
 from jal.db.ledger import Ledger
 from jal.data_import.statements import Statements
 from jal.reports.reports import Reports
 from jal.data_import.slips import ImportSlipDialog
 
 
 #-----------------------------------------------------------------------------------------------------------------------
-class MainWindow(QMainWindow, Ui_JAL_MainWindow):
+class MainWindow(QMainWindow):
     def __init__(self, language):
         super().__init__()
         self.running = False
-        self.setupUi(self)
+        self.ui = Ui_JAL_MainWindow()
+        self.ui.setupUi(self)
         self.restoreGeometry(base64.decodebytes(JalSettings().getValue('WindowGeometry', '').encode('utf-8')))
         self.restoreState(base64.decodebytes(JalSettings().getValue('WindowState', '').encode('utf-8')))
 
         self.ledger = Ledger()
 
         # Customize Status bar and logs
         self.ProgressBar = QProgressBar(self)
-        self.StatusBar.addPermanentWidget(self.ProgressBar)
+        self.ui.StatusBar.addPermanentWidget(self.ProgressBar)
         self.ProgressBar.setVisible(False)
         self.ledger.setProgressBar(self, self.ProgressBar)
-        self.Logs.setStatusBar(self.StatusBar)
-        self.logger = logging.getLogger()
-        self.logger.addHandler(self.Logs)
-        log_level = os.environ.get('LOGLEVEL', 'INFO').upper()
-        self.logger.setLevel(log_level)
+        self.ui.Logs.setStatusBar(self.ui.StatusBar)
+        self.ui.Logs.startLogging()
 
         self.currentLanguage = language
 
         self.downloader = QuoteDownloader()
         self.statements = Statements(self)
-        self.reports = Reports(self, self.mdiArea)
+        self.reports = Reports(self, self.ui.mdiArea)
         self.backup = JalBackup(self, get_dbfilename(get_app_path()))
         self.estimator = None
         self.price_chart = None
 
-        self.actionImportSlipRU.setEnabled(dependency_present(['PySide6.QtMultimedia']))
+        self.ui.actionImportSlipRU.setEnabled(dependency_present(['PySide6.QtMultimedia']))
 
         self.actionAbout = QAction(text=self.tr("About"), parent=self)
-        self.MainMenu.addAction(self.actionAbout)
+        self.ui.MainMenu.addAction(self.actionAbout)
 
-        self.langGroup = QActionGroup(self.menuLanguage)
+        self.langGroup = QActionGroup(self.ui.menuLanguage)
         self.createLanguageMenu()
 
-        self.statementGroup = QActionGroup(self.menuStatement)
+        self.statementGroup = QActionGroup(self.ui.menuStatement)
         self.createStatementsImportMenu()
 
-        self.reportsGroup = QActionGroup(self.menuReports)
+        self.reportsGroup = QActionGroup(self.ui.menuReports)
         self.createReportsMenu()
 
         self.setWindowIcon(load_icon("jal.png"))
 
         self.connect_signals_and_slots()
 
-        self.actionOperations.trigger()
+        self.ui.actionOperations.trigger()
 
     def connect_signals_and_slots(self):
-        self.actionExit.triggered.connect(QApplication.instance().quit)
-        self.actionOperations.triggered.connect(self.createOperationsWindow)
+        self.ui.actionExit.triggered.connect(QApplication.instance().quit)
+        self.ui.actionOperations.triggered.connect(self.createOperationsWindow)
         self.actionAbout.triggered.connect(self.showAboutWindow)
         self.langGroup.triggered.connect(self.onLanguageChanged)
         self.statementGroup.triggered.connect(self.statements.load)
         self.reportsGroup.triggered.connect(self.reports.show)
-        self.action_LoadQuotes.triggered.connect(partial(self.downloader.showQuoteDownloadDialog, self))
-        self.actionImportSlipRU.triggered.connect(self.importSlip)
-        self.actionBackup.triggered.connect(self.backup.create)
-        self.actionRestore.triggered.connect(self.backup.restore)
-        self.action_Re_build_Ledger.triggered.connect(partial(self.ledger.showRebuildDialog, self))
-        self.actionAccounts.triggered.connect(partial(self.onDataDialog, "accounts"))
-        self.actionAssets.triggered.connect(partial(self.onDataDialog, "assets"))
-        self.actionPeers.triggered.connect(partial(self.onDataDialog, "agents"))
-        self.actionCategories.triggered.connect(partial(self.onDataDialog, "categories"))
-        self.actionTags.triggered.connect(partial(self.onDataDialog, "tags"))
-        self.actionQuotes.triggered.connect(partial(self.onDataDialog, "quotes"))
-        self.actionBaseCurrency.triggered.connect(partial(self.onDataDialog, "base_currency"))
-        self.PrepareTaxForms.triggered.connect(partial(TaxWidget.showInMDI, self.mdiArea))
-        self.PrepareFlowReport.triggered.connect(partial(MoneyFlowWidget.showInMDI, self.mdiArea))
+        self.ui.action_LoadQuotes.triggered.connect(partial(self.downloader.showQuoteDownloadDialog, self))
+        self.ui.actionImportSlipRU.triggered.connect(self.importSlip)
+        self.ui.actionBackup.triggered.connect(self.backup.create)
+        self.ui.actionRestore.triggered.connect(self.backup.restore)
+        self.ui.action_Re_build_Ledger.triggered.connect(partial(self.ledger.showRebuildDialog, self))
+        self.ui.actionAccounts.triggered.connect(partial(self.onDataDialog, "accounts"))
+        self.ui.actionAssets.triggered.connect(partial(self.onDataDialog, "assets"))
+        self.ui.actionPeers.triggered.connect(partial(self.onDataDialog, "agents"))
+        self.ui.actionCategories.triggered.connect(partial(self.onDataDialog, "categories"))
+        self.ui.actionTags.triggered.connect(partial(self.onDataDialog, "tags"))
+        self.ui.actionQuotes.triggered.connect(partial(self.onDataDialog, "quotes"))
+        self.ui.actionBaseCurrency.triggered.connect(partial(self.onDataDialog, "base_currency"))
+        self.ui.PrepareTaxForms.triggered.connect(partial(TaxWidget.showInMDI, self.ui.mdiArea))
+        self.ui.PrepareFlowReport.triggered.connect(partial(MoneyFlowWidget.showInMDI, self.ui.mdiArea))
         self.downloader.download_completed.connect(self.updateWidgets)
         self.ledger.updated.connect(self.updateWidgets)
         self.statements.load_completed.connect(self.onStatementImport)
 
     @Slot()
     def showEvent(self, event):
         super().showEvent(event)
@@ -132,30 +130,29 @@
                                      QMessageBox.Yes, QMessageBox.No) == QMessageBox.Yes:
                 self.ledger.rebuild()
 
     @Slot()
     def closeEvent(self, event):
         JalSettings().setValue('WindowGeometry', base64.encodebytes(self.saveGeometry().data()).decode('utf-8'))
         JalSettings().setValue('WindowState', base64.encodebytes(self.saveState().data()).decode('utf-8'))
-        self.logger.removeHandler(self.Logs)    # Removing handler (but it doesn't prevent exception at exit)
-        logging.raiseExceptions = False         # Silencing logging module exceptions
+        self.ui.Logs.stopLogging()
         super().closeEvent(event)
 
     def createLanguageMenu(self):
         langPath = get_app_path() + Setup.LANG_PATH + os.sep
 
         langDirectory = QDir(langPath)
         for language_file in langDirectory.entryList(['*.qm']):
             language_code = language_file.split('.')[0]
             language = QLocale.languageToString(QLocale(language_code).language())
             language_icon = QIcon(langPath + language_code + '.png')
             action = QAction(language_icon, language, self)
             action.setCheckable(True)
             action.setData(language_code)
-            self.menuLanguage.addAction(action)
+            self.ui.menuLanguage.addAction(action)
             self.langGroup.addAction(action)
 
     @Slot()
     def onLanguageChanged(self, action):
         language_code = action.data()
         if language_code != self.currentLanguage:
             JalSettings().setLanguage(language_code)
@@ -173,36 +170,36 @@
             statement_name = statement['name'].replace('&', '&&')  # & -> && to prevent shortcut creation
             if statement['icon']:
                 statement_icon = load_icon(statement['icon'])
                 action = QAction(statement_icon, statement_name, self)
             else:
                 action = QAction(statement_name, self)
             action.setData(i)
-            self.menuStatement.addAction(action)
+            self.ui.menuStatement.addAction(action)
             self.statementGroup.addAction(action)
 
     # Create menu entry for all known reports based on self.reports.sources values
     def createReportsMenu(self):
         groups = {}
         for i, report in enumerate(self.reports.items):
             action = QAction(report['name'].replace('&', '&&'), self)  # & -> && to prevent shortcut creation
             action.setData(i)
             if report['group']:
                 if report['group'] not in groups:
-                    groups[report['group']] = QMenu(report['group'], self.menuReports)
-                    self.menuReports.addAction(groups[report['group']].menuAction())
+                    groups[report['group']] = QMenu(report['group'], self.ui.menuReports)
+                    self.ui.menuReports.addAction(groups[report['group']].menuAction())
                 submenu = groups[report['group']]
                 submenu.addAction(action)
             else:
-                self.menuReports.addAction(action)
+                self.ui.menuReports.addAction(action)
             self.reportsGroup.addAction(action)
 
     @Slot()
     def createOperationsWindow(self):
-        operations_window = self.mdiArea.addSubWindow(OperationsWidget(self), maximized=True)
+        operations_window = self.ui.mdiArea.addSubWindow(OperationsWidget(self), maximized=True)
         operations_window.widget().dbUpdated.connect(self.ledger.rebuild)
 
     @Slot()
     def showAboutWindow(self):
         about_box = QMessageBox(self)
         about_box.setAttribute(Qt.WA_DeleteOnClose)
         about_box.setWindowTitle(self.tr("About"))
@@ -215,16 +212,16 @@
                      "</p><p><a href=mailto:jal@gmx.ru>jal@gmx.ru</a></p>" + \
                      "<p><a href=https://t.me/jal_support>Telegram</a></p>"
         about_box.setInformativeText(about_text)
         about_box.show()
 
     def showProgressBar(self, visible=False):
         self.ProgressBar.setVisible(visible)
-        self.centralwidget.setEnabled(not visible)
-        self.MainMenu.setEnabled(not visible)
+        self.ui.centralwidget.setEnabled(not visible)
+        self.ui.MainMenu.setEnabled(not visible)
 
     @Slot()
     def importSlip(self):
         dialog = ImportSlipDialog(self)
         dialog.finished.connect(self.onSlipImportFinished)
         dialog.open()
 
@@ -250,15 +247,15 @@
             BaseCurrencyDialog().exec()
         else:
             assert False, f"Unexpected dialog call: '{dlg_type}'"
         self.ledger.rebuild()
 
     @Slot()
     def updateWidgets(self):
-        for window in self.mdiArea.subWindowList():
+        for window in self.ui.mdiArea.subWindowList():
             window.widget().refresh()
 
     @Slot()
     def onStatementImport(self, timestamp, totals):
         self.ledger.rebuild()
         for account_id in totals:
             account = JalAccount(account_id)
```

### Comparing `jal-2023.4.4/jal/widgets/mdi.py` & `jal-2023.4.5/jal/widgets/mdi.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # ----------------------------------------------------------------------------------------------------------------------
 # Base class that is used for any other widget which should be displayed inside JAL MainWindow MDI
 # implemented as TabbedMdiArea() class (below)
 class MdiWidget(QWidget):
     onClose = Signal(QWidget)
 
     def __init__(self, parent=None):
-        QWidget.__init__(self, parent)
+        super().__init__(parent)
 
     @Slot()
     def closeEvent(self, event):
         self.onClose.emit(self.parent())
         super().closeEvent(event)
 
     def refresh(self):
```

### Comparing `jal-2023.4.4/jal/widgets/operations_tabs.py` & `jal-2023.4.5/jal/widgets/operations_tabs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/operations_widget.py` & `jal-2023.4.5/jal/widgets/operations_widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,131 +10,132 @@
 from jal.db.asset import JalAsset
 from jal.db.balances_model import BalancesModel
 from jal.db.operations_model import OperationsModel
 from jal.db.operations import LedgerTransaction
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class OperationsWidget(MdiWidget, Ui_OperationsWidget):
+class OperationsWidget(MdiWidget):
     dbUpdated = Signal()
 
     def __init__(self, parent=None):
-        MdiWidget.__init__(self, parent)
-        self.setupUi(self)
+        super().__init__(parent)
+        self.ui = Ui_OperationsWidget()
+        self.ui.setupUi(self)
 
         self.current_index = None  # this is used in onOperationContextMenu() to track item for menu
 
         # Set icons
-        self.NewOperationBtn.setIcon(load_icon("new.png"))
-        self.CopyOperationBtn.setIcon(load_icon("copy.png"))
-        self.DeleteOperationBtn.setIcon(load_icon("delete.png"))
+        self.ui.NewOperationBtn.setIcon(load_icon("new.png"))
+        self.ui.CopyOperationBtn.setIcon(load_icon("copy.png"))
+        self.ui.DeleteOperationBtn.setIcon(load_icon("delete.png"))
 
         # Operations view context menu
-        self.contextMenu = QMenu(self.OperationsTableView)
+        self.contextMenu = QMenu(self.ui.OperationsTableView)
         self.actionReconcile = QAction(load_icon("reconcile.png"), self.tr("Reconcile"), self)
         self.actionCopy = QAction(load_icon("copy.png"), self.tr("Copy"), self)
         self.actionDelete = QAction(load_icon("delete.png"), self.tr("Delete"), self)
         self.contextMenu.addAction(self.actionReconcile)
         self.contextMenu.addSeparator()
         self.contextMenu.addAction(self.actionCopy)
         self.contextMenu.addAction(self.actionDelete)
 
         # Customize UI configuration
-        self.balances_model = BalancesModel(self.BalancesTableView)
-        self.BalancesTableView.setModel(self.balances_model)
+        self.balances_model = BalancesModel(self.ui.BalancesTableView)
+        self.ui.BalancesTableView.setModel(self.balances_model)
         self.balances_model.configureView()
 
-        self.operations_model = OperationsModel(self.OperationsTableView)
-        self.operations_filtered_model = QSortFilterProxyModel(self.OperationsTableView)
+        self.operations_model = OperationsModel(self.ui.OperationsTableView)
+        self.operations_filtered_model = QSortFilterProxyModel(self.ui.OperationsTableView)
         self.operations_filtered_model.setSourceModel(self.operations_model)
         self.operations_filtered_model.setFilterCaseSensitivity(Qt.CaseInsensitive)
-        self.OperationsTableView.setModel(self.operations_filtered_model)
+        self.ui.OperationsTableView.setModel(self.operations_filtered_model)
         self.operations_model.configureView()
-        self.OperationsTableView.setContextMenuPolicy(Qt.CustomContextMenu)
+        self.ui.OperationsTableView.setContextMenuPolicy(Qt.CustomContextMenu)
 
         self.connect_signals_and_slots()
 
         self.NewOperationMenu = QMenu()
-        self.OperationsTabs.dbUpdated.connect(self.dbUpdated)
-        self.OperationsTabs.dbUpdated.connect(self.operations_model.refresh)
-        for key, name in self.OperationsTabs.get_operations_list().items():
+        self.ui.OperationsTabs.dbUpdated.connect(self.dbUpdated)
+        self.ui.OperationsTabs.dbUpdated.connect(self.operations_model.refresh)
+        for key, name in self.ui.OperationsTabs.get_operations_list().items():
             self.NewOperationMenu.addAction(name, partial(self.createOperation, key))
-        self.NewOperationBtn.setMenu(self.NewOperationMenu)
+        self.ui.NewOperationBtn.setMenu(self.NewOperationMenu)
 
         # Setup balance and holdings parameters
         current_time = QDateTime.currentDateTime()
         current_time.setTimeSpec(Qt.UTC)  # We use UTC everywhere so need to force TZ info
-        self.BalanceDate.setDateTime(current_time)
-        self.BalancesCurrencyCombo.setIndex(JalAsset.get_base_currency())
+        self.ui.BalanceDate.setDateTime(current_time)
+        self.ui.BalancesCurrencyCombo.setIndex(JalAsset.get_base_currency())
 
-        self.OperationsTableView.selectRow(0)
-        self.DateRange.setCurrentIndex(0)
+        self.ui.OperationsTableView.selectRow(0)
+        self.ui.DateRange.setCurrentIndex(0)
 
     def connect_signals_and_slots(self):
         self.actionReconcile.triggered.connect(self.reconcileAtCurrentOperation)
-        self.BalanceDate.dateChanged.connect(self.BalancesTableView.model().setDate)
-        self.BalancesCurrencyCombo.changed.connect(self.BalancesTableView.model().setCurrency)
-        self.BalancesTableView.doubleClicked.connect(self.OnBalanceDoubleClick)
-        self.ShowInactiveCheckBox.stateChanged.connect(self.BalancesTableView.model().toggleActive)
-        self.DateRange.changed.connect(self.operations_model.setDateRange)
-        self.ChooseAccountBtn.changed.connect(self.operations_model.setAccount)
-        self.SearchString.editingFinished.connect(self.updateOperationsFilter)
-        self.OperationsTableView.selectionModel().selectionChanged.connect(self.OnOperationChange)
-        self.OperationsTableView.customContextMenuRequested.connect(self.onOperationContextMenu)
-        self.DeleteOperationBtn.clicked.connect(self.deleteOperation)
+        self.ui.BalanceDate.dateChanged.connect(self.ui.BalancesTableView.model().setDate)
+        self.ui.BalancesCurrencyCombo.changed.connect(self.ui.BalancesTableView.model().setCurrency)
+        self.ui.BalancesTableView.doubleClicked.connect(self.OnBalanceDoubleClick)
+        self.ui.ShowInactiveCheckBox.stateChanged.connect(self.ui.BalancesTableView.model().toggleActive)
+        self.ui.DateRange.changed.connect(self.operations_model.setDateRange)
+        self.ui.ChooseAccountBtn.changed.connect(self.operations_model.setAccount)
+        self.ui.SearchString.editingFinished.connect(self.updateOperationsFilter)
+        self.ui.OperationsTableView.selectionModel().selectionChanged.connect(self.OnOperationChange)
+        self.ui.OperationsTableView.customContextMenuRequested.connect(self.onOperationContextMenu)
+        self.ui.DeleteOperationBtn.clicked.connect(self.deleteOperation)
         self.actionDelete.triggered.connect(self.deleteOperation)
-        self.CopyOperationBtn.clicked.connect(self.OperationsTabs.copy_operation)
-        self.actionCopy.triggered.connect(self.OperationsTabs.copy_operation)
+        self.ui.CopyOperationBtn.clicked.connect(self.ui.OperationsTabs.copy_operation)
+        self.actionCopy.triggered.connect(self.ui.OperationsTabs.copy_operation)
 
     @Slot()
     def deleteOperation(self):
         if QMessageBox().warning(None, self.tr("Confirmation"),
                                  self.tr("Are you sure to delete selected transacion(s)?"),
                                  QMessageBox.Yes, QMessageBox.No) == QMessageBox.No:
             return
         rows = []
-        for index in self.OperationsTableView.selectionModel().selectedRows():
+        for index in self.ui.OperationsTableView.selectionModel().selectedRows():
             rows.append(index.row())
         self.operations_model.deleteRows(rows)
         self.dbUpdated.emit()
 
     @Slot()
     def createOperation(self, operation_type):
-        self.OperationsTabs.new_operation(operation_type, self.operations_model.getAccount())
+        self.ui.OperationsTabs.new_operation(operation_type, self.operations_model.getAccount())
 
     @Slot()
     def updateOperationsFilter(self):
-        self.OperationsTableView.model().setFilterFixedString(self.SearchString.text())
-        self.OperationsTableView.model().setFilterKeyColumn(-1)
+        self.ui.OperationsTableView.model().setFilterFixedString(self.ui.SearchString.text())
+        self.ui.OperationsTableView.model().setFilterKeyColumn(-1)
 
     @Slot()
     def OnBalanceDoubleClick(self, index):
-        self.ChooseAccountBtn.account_id = index.model().getAccountId(index.row())
+        self.ui.ChooseAccountBtn.account_id = index.model().getAccountId(index.row())
 
     @Slot()
     def OnOperationChange(self, selected, _deselected):
         op_type = LedgerTransaction.NA
         op_id = 0
-        if len(self.OperationsTableView.selectionModel().selectedRows()) == 1:
+        if len(self.ui.OperationsTableView.selectionModel().selectedRows()) == 1:
             idx = selected.indexes()
             if idx:
                 selected_row = self.operations_filtered_model.mapToSource(idx[0]).row()
                 op_type, op_id = self.operations_model.get_operation(selected_row)
-        self.OperationsTabs.show_operation(op_type, op_id)
+        self.ui.OperationsTabs.show_operation(op_type, op_id)
 
     @Slot()
     def onOperationContextMenu(self, pos):
-        self.current_index = self.OperationsTableView.indexAt(pos)
-        if len(self.OperationsTableView.selectionModel().selectedRows()) != 1:
+        self.current_index = self.ui.OperationsTableView.indexAt(pos)
+        if len(self.ui.OperationsTableView.selectionModel().selectedRows()) != 1:
             self.actionReconcile.setEnabled(False)
             self.actionCopy.setEnabled(False)
         else:
             self.actionReconcile.setEnabled(True)
             self.actionCopy.setEnabled(True)
-        self.contextMenu.popup(self.OperationsTableView.viewport().mapToGlobal(pos))
+        self.contextMenu.popup(self.ui.OperationsTableView.viewport().mapToGlobal(pos))
 
     @Slot()
     def reconcileAtCurrentOperation(self):
         idx = self.operations_model.index(self.current_index.row(), 0)  # we need only row to address fields by name
         timestamp = self.operations_model.data(idx, Qt.UserRole, field="timestamp")
         account_id = self.operations_model.data(idx, Qt.UserRole, field="account_id")
         JalAccount(account_id).reconcile(timestamp)
```

### Comparing `jal-2023.4.4/jal/widgets/price_chart.py` & `jal-2023.4.5/jal/widgets/price_chart.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from math import log10, floor, ceil
+from decimal import Decimal
 
 from PySide6.QtCore import Qt, QMargins, QDateTime, QDate
 from PySide6.QtWidgets import QWidget, QHBoxLayout
 from PySide6.QtCharts import QChartView, QLineSeries, QScatterSeries, QDateTimeAxis, QValueAxis
 from jal.db.account import JalAccount
 from jal.db.asset import JalAsset
 from jal.constants import CustomColor
@@ -104,22 +105,22 @@
             min_price = min([x['quote'] for x in self.quotes] + [x['price'] for x in self.trades])
             max_price = max([x['quote'] for x in self.quotes] + [x['price'] for x in self.trades])
             min_ts = min([x['timestamp'] for x in self.quotes] + [x['timestamp'] for x in self.trades]) / 1000
             max_ts = max([x['timestamp'] for x in self.quotes] + [x['timestamp'] for x in self.trades]) / 1000
         else:
             self.range = [0, 0, 0, 0]
             return
-        # push range apart if we have too close points
+        # push range apart if we have very close points
         if min_price == max_price:
-            min_price = 0.95 * min_price
-            max_price = 1.05 * max_price
+            min_price = Decimal('0.95') * min_price
+            max_price = Decimal('1.05') * max_price
         if min_ts == max_ts:
             min_ts = 0.95 * min_ts
             max_ts = 1.05 * max_ts
         # Round min/max values to near "round" values in order to have 10 nice intervals
-        step = 10 ** floor(log10(max_price - min_price))
+        step = Decimal(10) ** Decimal(floor(Decimal.log10(max_price - min_price)))
         min_price = floor(min_price / step) * step
         max_price = ceil(max_price / step) * step
         # Add a gap at the beginning and end
         min_ts = int(min_ts - 86400 * 3)
         max_ts = int(max_ts + 86400 * 3)
         self.range = [min_ts, max_ts, min_price, max_price]
```

### Comparing `jal-2023.4.4/jal/widgets/qr_scanner.py` & `jal-2023.4.5/jal/widgets/qr_scanner.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/reference_data.py` & `jal-2023.4.5/jal/widgets/reference_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from jal.ui.ui_reference_data_dlg import Ui_ReferenceDataDialog
 from jal.db.helpers import load_icon
 
 
 # --------------------------------------------------------------------------------------------------------------
 # Class to display and edit table with reference data (accounts, categories, tags...)
 # --------------------------------------------------------------------------------------------------------------
-class ReferenceDataDialog(QDialog, Ui_ReferenceDataDialog):
+class ReferenceDataDialog(QDialog):
     # tree_view - table will be displayed as hierarchical tree with help of 2 columns: 'id', 'pid' in sql table
     def __init__(self, parent=None):
-        QDialog.__init__(self)
-        self.setupUi(self)
+        super().__init__(parent)
+        self.ui = Ui_ReferenceDataDialog()
+        self.ui.setupUi(self)
         self._parent = parent
         self.model = None
         self._view = None
         self._previous_row = -1
         self.selected_id = 0
         self.p_selected_name = ''
         self._filter_text = ''
@@ -32,42 +33,42 @@
         self.search_field = None
         self.search_text = ""
         self.tree_view = False
         self.toolbar = None
         self.custom_editor = False
         self.custom_context_menu = False
 
-        self.AddChildBtn.setVisible(False)
-        self.GroupLbl.setVisible(False)
-        self.GroupCombo.setVisible(False)
-        self.SearchFrame.setVisible(False)
-
-        self.AddBtn.setIcon(load_icon("add.png"))
-        self.AddChildBtn.setIcon(load_icon("add_child.png"))
-        self.RemoveBtn.setIcon(load_icon("delete.png"))
-        self.CommitBtn.setIcon(load_icon("accept.png"))
-        self.RevertBtn.setIcon(load_icon("cancel.png"))
-
-        self.SearchString.textChanged.connect(self.OnSearchChange)
-        self.GroupCombo.currentIndexChanged.connect(self.OnGroupChange)
-        self.Toggle.stateChanged.connect(self.OnToggleChange)
-        self.AddBtn.clicked.connect(self.OnAdd)
-        self.AddChildBtn.clicked.connect(self.OnChildAdd)
-        self.RemoveBtn.clicked.connect(self.OnRemove)
-        self.CommitBtn.clicked.connect(self.OnCommit)
-        self.RevertBtn.clicked.connect(self.OnRevert)
-        self.DataView.doubleClicked.connect(self.OnDoubleClicked)
-        self.DataView.clicked.connect(self.OnClicked)
-        self.TreeView.doubleClicked.connect(self.OnDoubleClicked)
-        self.TreeView.clicked.connect(self.OnClicked)
+        self.ui.AddChildBtn.setVisible(False)
+        self.ui.GroupLbl.setVisible(False)
+        self.ui.GroupCombo.setVisible(False)
+        self.ui.SearchFrame.setVisible(False)
+
+        self.ui.AddBtn.setIcon(load_icon("add.png"))
+        self.ui.AddChildBtn.setIcon(load_icon("add_child.png"))
+        self.ui.RemoveBtn.setIcon(load_icon("delete.png"))
+        self.ui.CommitBtn.setIcon(load_icon("accept.png"))
+        self.ui.RevertBtn.setIcon(load_icon("cancel.png"))
+
+        self.ui.SearchString.textChanged.connect(self.OnSearchChange)
+        self.ui.GroupCombo.currentIndexChanged.connect(self.OnGroupChange)
+        self.ui.Toggle.stateChanged.connect(self.OnToggleChange)
+        self.ui.AddBtn.clicked.connect(self.OnAdd)
+        self.ui.AddChildBtn.clicked.connect(self.OnChildAdd)
+        self.ui.RemoveBtn.clicked.connect(self.OnRemove)
+        self.ui.CommitBtn.clicked.connect(self.OnCommit)
+        self.ui.RevertBtn.clicked.connect(self.OnRevert)
+        self.ui.DataView.doubleClicked.connect(self.OnDoubleClicked)
+        self.ui.DataView.clicked.connect(self.OnClicked)
+        self.ui.TreeView.doubleClicked.connect(self.OnDoubleClicked)
+        self.ui.TreeView.clicked.connect(self.OnClicked)
 
     def _init_completed(self):
-        self.DataView.setVisible(not self.tree_view)
-        self.TreeView.setVisible(self.tree_view)
-        self._view = self.TreeView if self.tree_view else self.DataView
+        self.ui.DataView.setVisible(not self.tree_view)
+        self.ui.TreeView.setVisible(self.tree_view)
+        self._view = self.ui.TreeView if self.tree_view else self.ui.DataView
         self._view.selectionModel().selectionChanged.connect(self.OnRowSelected)
         self._view.setContextMenuPolicy(Qt.CustomContextMenu)
         self._view.customContextMenuRequested.connect(self.onDataViewContextMenu)
         self.model.dataChanged.connect(self.OnDataChanged)
         self.setFilter()
 
     def onDataViewContextMenu(self, pos):
@@ -80,28 +81,28 @@
             index = self._view.indexAt(pos)
             menu_title = QWidgetAction(self._view)
             title_lbl = QLabel()
             title_lbl.setText(self.tr("Change type to:"))
             menu_title.setDefaultWidget(title_lbl)
             contextMenu.addAction(menu_title)
             contextMenu.addSeparator()
-            for i in range(self.GroupCombo.count()):
-                contextMenu.addAction(self.GroupCombo.itemText(i),
-                                      partial(self.updateItemType, index, self.GroupCombo.itemData(i)))
+            for i in range(self.ui.GroupCombo.count()):
+                contextMenu.addAction(self.ui.GroupCombo.itemText(i),
+                                      partial(self.updateItemType, index, self.ui.GroupCombo.itemData(i)))
         contextMenu.popup(self._view.viewport().mapToGlobal(pos))
 
     @Slot()
     def updateItemType(self, index, new_type):
         self.model.updateItemType(index, new_type)
-        self.CommitBtn.setEnabled(True)
-        self.RevertBtn.setEnabled(True)
+        self.ui.CommitBtn.setEnabled(True)
+        self.ui.RevertBtn.setEnabled(True)
 
     @Slot()
     def closeEvent(self, event):
-        if self.CommitBtn.isEnabled():    # There are uncommitted changed in a table
+        if self.ui.CommitBtn.isEnabled():    # There are uncommitted changed in a table
             if QMessageBox().warning(self, self.tr("Confirmation"),
                                      self.tr("You have uncommitted changes. Do you want to close?"),
                                      QMessageBox.Yes, QMessageBox.No) == QMessageBox.No:
                 event.ignore()
                 return
             else:
                 self.model.revertAll()
@@ -130,62 +131,62 @@
     def selected_name_changed(self):
         pass
 
     SelectedName = Property(str, getSelectedName, setSelectedName, notify=selected_name_changed)
 
     @Slot()
     def OnDataChanged(self):
-        self.CommitBtn.setEnabled(True)
-        self.RevertBtn.setEnabled(True)
+        self.ui.CommitBtn.setEnabled(True)
+        self.ui.RevertBtn.setEnabled(True)
 
     @Slot()
     def OnAdd(self):
         if self.custom_editor:
             editor = self.customEditor()
             editor.createNewRecord()
             editor.exec()
             self.model.select()
             self.locateItem(editor.selected_id)
         else:
             idx = self._view.selectionModel().selection().indexes()
             current_index = idx[0] if idx else self.model.index(0, 0)
             self.model.addElement(current_index, in_group=self.group_id)
-            self.CommitBtn.setEnabled(True)
-            self.RevertBtn.setEnabled(True)
+            self.ui.CommitBtn.setEnabled(True)
+            self.ui.RevertBtn.setEnabled(True)
 
     @Slot()
     def OnChildAdd(self):
         if self.tree_view:
-            idx = self.TreeView.selectionModel().selection().indexes()
+            idx = self.ui.TreeView.selectionModel().selection().indexes()
             current_index = idx[0] if idx else self.model.index(0, 0)
             self.model.addChildElement(current_index)
-            self.CommitBtn.setEnabled(True)
-            self.RevertBtn.setEnabled(True)
+            self.ui.CommitBtn.setEnabled(True)
+            self.ui.RevertBtn.setEnabled(True)
 
     @Slot()
     def OnRemove(self):
         idx = self._view.selectionModel().selection().indexes()
         current_index = idx[0] if idx else self.model.index(0, 0)
         self.model.removeElement(current_index)
-        self.CommitBtn.setEnabled(True)
-        self.RevertBtn.setEnabled(True)
+        self.ui.CommitBtn.setEnabled(True)
+        self.ui.RevertBtn.setEnabled(True)
 
     @Slot()
     def OnCommit(self):
         if not self.model.submitAll():
             return
         self.model.invalidate_cache()
-        self.CommitBtn.setEnabled(False)
-        self.RevertBtn.setEnabled(False)
+        self.ui.CommitBtn.setEnabled(False)
+        self.ui.RevertBtn.setEnabled(False)
 
     @Slot()
     def OnRevert(self):
         self.model.revertAll()
-        self.CommitBtn.setEnabled(False)
-        self.RevertBtn.setEnabled(False)
+        self.ui.CommitBtn.setEnabled(False)
+        self.ui.RevertBtn.setEnabled(False)
 
     def setFilterValue(self, filter_value):
         if self.filter_field is None:
             return
         self._filter_value = filter_value
         self.setFilter()
 
@@ -224,15 +225,15 @@
             self._filter_text += line + " AND "
         self._filter_text = self._filter_text[:-len(" AND ")]
 
         self.model.setFilter(self._filter_text)
 
     @Slot()
     def OnSearchChange(self):
-        self.search_text = self.SearchString.text()
+        self.search_text = self.ui.SearchString.text()
         self.setFilter()
 
     @Slot()
     def OnRowSelected(self, selected, _deselected):
         idx = selected.indexes()
         if idx:
             self.selected_id = self.model.getId(idx[0])
@@ -255,15 +256,15 @@
         if self.selection_enabled:
             self.setResult(QDialog.Accepted)
             self.close()
 
     @Slot()
     def OnGroupChange(self, list_id):
         self.OnRevert()  # Discard all possible changes
-        self.group_id = self.GroupCombo.itemData(list_id)
+        self.group_id = self.ui.GroupCombo.itemData(list_id)
         self.setFilter()
 
     @Slot()
     def OnToggleChange(self, state):
         if state == 0:
             self.toggle_state = False
         else:
```

### Comparing `jal-2023.4.4/jal/widgets/reference_dialogs.py` & `jal-2023.4.5/jal/widgets/reference_dialogs.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,42 +60,42 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("active"), self._bool_delegate)
 
 
 class AccountListDialog(ReferenceDataDialog):
     def __init__(self):
         ReferenceDataDialog.__init__(self)
         self.table = "accounts"
-        self.model = AccountListModel(self.table, self.DataView)
-        self.DataView.setModel(self.model)
+        self.model = AccountListModel(self.table, self.ui.DataView)
+        self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
 
     def setup_ui(self):
         self.search_field = "accounts.name"
         self.setWindowTitle(self.tr("Accounts"))
-        self.SearchFrame.setVisible(True)
-        self.Toggle.setVisible(True)
+        self.ui.SearchFrame.setVisible(True)
+        self.ui.Toggle.setVisible(True)
         self.toggle_field = "active"
-        self.Toggle.setText(self.tr("Show inactive"))
+        self.ui.Toggle.setText(self.tr("Show inactive"))
 
-        self.GroupLbl.setVisible(True)
-        self.GroupLbl.setText(self.tr("Account type:"))
-        self.GroupCombo.setVisible(True)
+        self.ui.GroupLbl.setVisible(True)
+        self.ui.GroupLbl.setText(self.tr("Account type:"))
+        self.ui.GroupCombo.setVisible(True)
         self.group_field = self.model.group_by
-        PredefindedAccountType().load2combo(self.GroupCombo)
+        PredefindedAccountType().load2combo(self.ui.GroupCombo)
         self.group_id = 1
 
     def locateItem(self, item_id):
         type_id = self.model.getGroupId(item_id)
         if type_id == 0:
             return
-        self.GroupCombo.setCurrentIndex(type_id-1)
+        self.ui.GroupCombo.setCurrentIndex(type_id-1)
         item_idx = self.model.locateItem(item_id, use_filter=self._filter_text)
-        self.DataView.setCurrentIndex(item_idx)
+        self.ui.DataView.setCurrentIndex(item_idx)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class AssetListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
         AbstractReferenceListModel.__init__(self, table, parent_view)
         pk = QSqlIndex()   # Manual primary key setup is required as we use underlying sql view instead of sql table
@@ -128,46 +128,46 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("quote_source"), self._lookup_delegate)
 
 
 class AssetListDialog(ReferenceDataDialog):
     def __init__(self):
         ReferenceDataDialog.__init__(self)
         self.table = "assets_ext"
-        self.model = AssetListModel(self.table, self.DataView)
-        self.DataView.setModel(self.model)
+        self.model = AssetListModel(self.table, self.ui.DataView)
+        self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
 
     def setup_ui(self):
         self.search_field = "assets_ext.full_name"
         self.setWindowTitle(self.tr("Assets"))
-        self.SearchFrame.setVisible(True)
-        self.Toggle.setVisible(False)
+        self.ui.SearchFrame.setVisible(True)
+        self.ui.Toggle.setVisible(False)
 
         self.custom_editor = True
-        self.DataView.setEditTriggers(QAbstractItemView.NoEditTriggers)
+        self.ui.DataView.setEditTriggers(QAbstractItemView.NoEditTriggers)
 
-        self.GroupLbl.setVisible(True)
-        self.GroupLbl.setText(self.tr("Asset type:"))
-        self.GroupCombo.setVisible(True)
+        self.ui.GroupLbl.setVisible(True)
+        self.ui.GroupLbl.setText(self.tr("Asset type:"))
+        self.ui.GroupCombo.setVisible(True)
         self.group_field = self.model.group_by
-        PredefinedAsset().load2combo(self.GroupCombo)
+        PredefinedAsset().load2combo(self.ui.GroupCombo)
         self.group_id = 1
 
     def locateItem(self, item_id):
         type_id = self.model.getGroupId(item_id)
         if type_id == 0:
             return
-        self.GroupCombo.setCurrentIndex(type_id-1)
+        self.ui.GroupCombo.setCurrentIndex(type_id-1)
         item_idx = self.model.locateItem(item_id, use_filter=self._filter_text)
-        self.DataView.setCurrentIndex(item_idx)
+        self.ui.DataView.setCurrentIndex(item_idx)
 
     def customEditor(self):
-        return AssetDialog()
+        return AssetDialog(self)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class PeerTreeModel(SqlTreeModel):
     def __init__(self, table, parent_view):
         super().__init__(table, parent_view)
         self._columns = [("name", self.tr("Name")),
@@ -198,33 +198,33 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("actions_count"), self._int_delegate)
 
 
 class PeerListDialog(ReferenceDataDialog):
     def __init__(self, parent):
         ReferenceDataDialog.__init__(self, parent)
         self.table = "agents"
-        self.model = PeerTreeModel(self.table, self.TreeView)
-        self.TreeView.setModel(self.model)
+        self.model = PeerTreeModel(self.table, self.ui.TreeView)
+        self.ui.TreeView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
         self._menu_peer_id = 0
         self._menu_peer_name = ''
         self.actionShowUsage = QAction(text=self.tr("Show operations with Peer"), parent=self)
         self.actionReplace = QAction(text=self.tr("Replace with..."), parent=self)
         self.actionShowUsage.triggered.connect(self.showUsageReport)
         self.actionReplace.triggered.connect(self.replacePeer)
 
     def setup_ui(self):
         self.search_field = "name"
         self.tree_view = True
-        self.AddChildBtn.setVisible(True)
-        self.SearchFrame.setVisible(True)
+        self.ui.AddChildBtn.setVisible(True)
+        self.ui.SearchFrame.setVisible(True)
         self.setWindowTitle(self.tr("Peers"))
-        self.Toggle.setVisible(False)
+        self.ui.Toggle.setVisible(False)
         if hasattr(self._parent, "reports"):  # Activate menu only if dialog is called from main window menu
             self.custom_context_menu = True
 
     def locateItem(self, item_id):
         self.model.locateItem(item_id)
         
     def customizeContextMenu(self, menu: QMenu, index):
@@ -272,33 +272,33 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("often"), self._bool_delegate)
 
 
 class CategoryListDialog(ReferenceDataDialog):
     def __init__(self, parent):
         ReferenceDataDialog.__init__(self, parent)
         self.table = "categories"
-        self.model = CategoryTreeModel(self.table, self.TreeView)
-        self.TreeView.setModel(self.model)
+        self.model = CategoryTreeModel(self.table, self.ui.TreeView)
+        self.ui.TreeView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
         self._menu_category_id = 0
         self._menu_category_name = ''
         self.actionShowUsage = QAction(text=self.tr("Show operations with Category"), parent=self)
         self.actionReplace = QAction(text=self.tr("Replace with..."), parent=self)
         self.actionShowUsage.triggered.connect(self.showUsageReport)
         self.actionReplace.triggered.connect(self.replaceCategory)
 
     def setup_ui(self):
         self.search_field = "name"
         self.tree_view = True
-        self.AddChildBtn.setVisible(True)
-        self.SearchFrame.setVisible(True)
+        self.ui.AddChildBtn.setVisible(True)
+        self.ui.SearchFrame.setVisible(True)
         self.setWindowTitle(self.tr("Categories"))
-        self.Toggle.setVisible(False)
+        self.ui.Toggle.setVisible(False)
         if hasattr(self._parent, "reports"):  # Activate menu only if dialog is called from main window menu
             self.custom_context_menu = True
 
     def locateItem(self, item_id):
         self.model.locateItem(item_id)
 
     def customizeContextMenu(self, menu: QMenu, index):
@@ -334,37 +334,37 @@
         self._stretch = "tag"
 
 
 class TagsListDialog(ReferenceDataDialog):
     def __init__(self, parent):
         ReferenceDataDialog.__init__(self, parent)
         self.table = "tags"
-        self.model = TagListModel(self.table, self.DataView)
-        self.DataView.setModel(self.model)
+        self.model = TagListModel(self.table, self.ui.DataView)
+        self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
         self._menu_tag_id = 0
         self._menu_tag_name = ''
         self.actionShowUsage = QAction(text=self.tr("Show operations with Tag"), parent=self)
         self.actionReplace = QAction(text=self.tr("Replace with..."), parent=self)
         self.actionShowUsage.triggered.connect(self.showUsageReport)
         self.actionReplace.triggered.connect(self.replaceTag)
 
     def setup_ui(self):
         self.search_field = "tag"
         self.setWindowTitle(self.tr("Tags"))
-        self.SearchFrame.setVisible(True)
-        self.Toggle.setVisible(False)
+        self.ui.SearchFrame.setVisible(True)
+        self.ui.Toggle.setVisible(False)
         if hasattr(self._parent, "reports"):  # Activate menu only if dialog is called from main window menu
             self.custom_context_menu = True
 
     def locateItem(self, item_id):
         item_idx = self.model.locateItem(item_id)
-        self.DataView.setCurrentIndex(item_idx)
+        self.ui.DataView.setCurrentIndex(item_idx)
 
     def customizeContextMenu(self, menu: QMenu, index):
         self._menu_tag_id = self.model.getId(index)
         self._menu_tag_name = self.model.getName(index)
         menu.addAction(self.actionShowUsage)
         menu.addAction(self.actionReplace)
 
@@ -416,25 +416,25 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("currency_id"), self._lookup_delegate)
 
 
 class QuotesListDialog(ReferenceDataDialog):
     def __init__(self):
         ReferenceDataDialog.__init__(self)
         self.table = "quotes"
-        self.model = QuotesListModel(self.table, self.DataView)
-        self.DataView.setModel(self.model)
+        self.model = QuotesListModel(self.table, self.ui.DataView)
+        self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
 
     def setup_ui(self):
         self.search_field = "asset_id-assets_ext-id-symbol"
-        self.SearchFrame.setVisible(True)
+        self.ui.SearchFrame.setVisible(True)
         self.setWindowTitle(self.tr("Quotes"))
-        self.Toggle.setVisible(False)
+        self.ui.Toggle.setVisible(False)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class BaseCurrencyListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
         AbstractReferenceListModel.__init__(self, table, parent_view)
         self._columns = [("id", ''),
@@ -459,18 +459,18 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("currency_id"), self._lookup_delegate)
 
 
 class BaseCurrencyDialog(ReferenceDataDialog):
     def __init__(self):
         ReferenceDataDialog.__init__(self)
         self.table = "base_currency"
-        self.model = BaseCurrencyListModel(self.table, self.DataView)
-        self.DataView.setModel(self.model)
+        self.model = BaseCurrencyListModel(self.table, self.ui.DataView)
+        self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
 
     def setup_ui(self):
         self.setWindowTitle(self.tr("Base currency"))
-        self.Toggle.setVisible(False)
+        self.ui.Toggle.setVisible(False)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `jal-2023.4.4/jal/widgets/reference_selector.py` & `jal-2023.4.5/jal/widgets/reference_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/register_designer_plugins.py` & `jal-2023.4.5/jal/widgets/register_designer_plugins.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/selection_dialog.py` & `jal-2023.4.5/jal/widgets/selection_dialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from jal.widgets.reference_selector import PeerSelector
 from jal.widgets.reference_selector import CategorySelector
 from jal.widgets.reference_selector import TagSelector
 
 
 #-----------------------------------------------------------------------------------------------------------------------
 # Common base GUI dialog class for selector dialogs. Takes window title and label comment to describe selection
-class SelectReferenceDialog(QDialog, Ui_SelectReferenceDlg):
+class SelectReferenceDialog(QDialog):
     def __init__(self, title, description):
-        QDialog.__init__(self)
-        self.setupUi(self)
+        super().__init__(self)
+        self.ui = Ui_SelectReferenceDlg()
+        self.ui.setupUi(self)
         self.selected_id = 0
         self.setWindowTitle(title)
-        self.DescriptionLabel.setText(description)
+        self.ui.DescriptionLabel.setText(description)
         center_window(self)
 
     @Slot()
     def closeEvent(self, event):
         if self.selected_id == 0:
             QMessageBox().warning(None, self.tr("No selection"), self.tr("You should select something"), QMessageBox.Ok)
             event.ignore()
@@ -30,47 +31,47 @@
 
 #-----------------------------------------------------------------------------------------------------------------------
 # Dialog for peer selection
 # Constructor takes description to show and default_peer for initial choice
 class SelectPeerDialog(SelectReferenceDialog):
     def __init__(self, description, default_peer=0):
         SelectReferenceDialog.__init__(self, self.tr("Please select peer"), description)
-        self.PeerWidget = PeerSelector(self.SelectorFrame)
-        self.FrameLayout.addWidget(self.PeerWidget)
+        self.PeerWidget = PeerSelector(self.ui.SelectorFrame)
+        self.ui.FrameLayout.addWidget(self.PeerWidget)
         self.PeerWidget.selected_id = self.selected_id = default_peer
 
     @Slot()
     def closeEvent(self, event):
         self.selected_id = self.PeerWidget.selected_id
         super().closeEvent(event)
         
         
 #-----------------------------------------------------------------------------------------------------------------------
 # Dialog for category selection
 # Constructor takes description to show and default_category for initial choice
 class SelectCategoryDialog(SelectReferenceDialog):
     def __init__(self, description, default_category=0):
         SelectReferenceDialog.__init__(self, self.tr("Please select category"), description)
-        self.CategoryWidget = CategorySelector(self.SelectorFrame)
-        self.FrameLayout.addWidget(self.CategoryWidget)
+        self.CategoryWidget = CategorySelector(self.ui.SelectorFrame)
+        self.ui.FrameLayout.addWidget(self.CategoryWidget)
         self.CategoryWidget.selected_id = self.selected_id = default_category
 
     @Slot()
     def closeEvent(self, event):
         self.selected_id = self.CategoryWidget.selected_id
         super().closeEvent(event)
 
 
 #-----------------------------------------------------------------------------------------------------------------------
 # Dialog for tag selection
 # Constructor takes description to show and default_tag for initial choice
 class SelectTagDialog(SelectReferenceDialog):
     def __init__(self, description, default_tag=0):
         SelectReferenceDialog.__init__(self, self.tr("Please select tag"), description)
-        self.TagWidget = TagSelector(self.SelectorFrame)
-        self.FrameLayout.addWidget(self.TagWidget)
+        self.TagWidget = TagSelector(self.ui.SelectorFrame)
+        self.ui.FrameLayout.addWidget(self.TagWidget)
         self.TagWidget.selected_id = self.selected_id = default_tag
 
     @Slot()
     def closeEvent(self, event):
         self.selected_id = self.TagWidget.selected_id
         super().closeEvent(event)
```

### Comparing `jal-2023.4.4/jal/widgets/tax_widget.py` & `jal-2023.4.5/jal/widgets/tax_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 from jal.db.peer import JalPeer
 from jal.data_export.taxes import TaxReport
 from jal.data_export.taxes_flow import TaxesFlowRus
 from jal.data_export.xlsx import XLSX
 from jal.data_export.dlsg import DLSG
 
 
-class TaxWidget(MdiWidget, Ui_TaxWidget):
-    def __init__(self):
-        MdiWidget.__init__(self)
-        self.setupUi(self)
-
-        self.Country.clear()
-        self.Country.addItems([TaxReport.countries[x]['name'] for x in TaxReport.countries])
-        self.Country.currentIndexChanged.connect(self.OnCountryChange)
-        self.Year.setValue(datetime.now().year - 1)   # Set previous year by default
-        self.XlsSelectBtn.pressed.connect(partial(self.OnFileBtn, 'XLS'))
-        self.DlsgSelectBtn.pressed.connect(partial(self.OnFileBtn, 'DLSG'))
-        self.SaveButton.pressed.connect(self.SaveReport)
-        self.Country.setCurrentIndex(TaxReport.RUSSIA)
+class TaxWidget(MdiWidget):
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.ui = Ui_TaxWidget()
+        self.ui.setupUi(self)
+
+        self.ui.Country.clear()
+        self.ui.Country.addItems([TaxReport.countries[x]['name'] for x in TaxReport.countries])
+        self.ui.Country.currentIndexChanged.connect(self.OnCountryChange)
+        self.ui.Year.setValue(datetime.now().year - 1)   # Set previous year by default
+        self.ui.XlsSelectBtn.pressed.connect(partial(self.OnFileBtn, 'XLS'))
+        self.ui.DlsgSelectBtn.pressed.connect(partial(self.OnFileBtn, 'DLSG'))
+        self.ui.SaveButton.pressed.connect(self.SaveReport)
+        self.ui.Country.setCurrentIndex(TaxReport.RUSSIA)
 
     def OnCountryChange(self, item_id):
         if item_id == TaxReport.PORTUGAL:
-            self.RussianSpecificFrame.setVisible(False)
+            self.ui.RussianSpecificFrame.setVisible(False)
         elif item_id == TaxReport.RUSSIA:
-            self.RussianSpecificFrame.setVisible(True)
+            self.ui.RussianSpecificFrame.setVisible(True)
         else:
             raise ValueError("Selected item has no country handler in code")
         # Refresh and adjust MDI-window size
         if not self.parent() is None:
             self.parent().update()
             QApplication.processEvents()
             if not self.parent().isMaximized():  # Prevent size-change of maximized MDI
@@ -50,51 +51,51 @@
     @staticmethod
     def showInMDI(parent_mdi):
         parent_mdi.addSubWindow(TaxWidget(), maximized=False)
 
     @Slot()
     def OnFileBtn(self, type):
         if type == 'XLS':
-            selector = (self.tr("Save tax reports to:"), self.tr("Excel files (*.xlsx)"), '.xlsx', self.XlsFileName)
+            selector = (self.tr("Save tax reports to:"), self.tr("Excel files (*.xlsx)"), '.xlsx', self.ui.XlsFileName)
         elif type == 'DLSG':
             last_digit = self.year % 10
             selector = (self.tr("Save tax form to:"), self.tr(f"Tax form (*.dc{last_digit})"),
-                        f".dc{last_digit}", self.DlsgFileName)
+                        f".dc{last_digit}", self.ui.DlsgFileName)
         else:
             raise ValueError
         filename = QFileDialog.getSaveFileName(self, selector[0], ".", selector[1])
         if filename[0]:
             if filename[1] == selector[1] and filename[0][-len(selector[2]):] != selector[2]:
                 selector[3].setText(filename[0] + selector[2])
             else:
                 selector[3].setText(filename[0])
 
     def getYear(self):
-        return self.Year.value()
+        return self.ui.Year.value()
 
     def getXlsFilename(self):
-        return self.XlsFileName.text()
+        return self.ui.XlsFileName.text()
 
     def getAccount(self):
-        return self.AccountWidget.selected_id
+        return self.ui.AccountWidget.selected_id
 
     def getDlsgState(self):
-        return self.DlsgGroup.isChecked()
+        return self.ui.DlsgGroup.isChecked()
 
     def getDslgFilename(self):
-        return self.DlsgFileName.text()
+        return self.ui.DlsgFileName.text()
 
     def getBrokerAsIncomeName(self):
-        return self.IncomeSourceBroker.isChecked()
+        return self.ui.IncomeSourceBroker.isChecked()
 
     def getDividendsOnly(self):
-        return self.DividendsOnly.isChecked()
+        return self.ui.DividendsOnly.isChecked()
 
     def getNoSettlement(self):
-        return self.NoSettlement.isChecked()
+        return self.ui.NoSettlement.isChecked()
 
     year = Property(int, fget=getYear)
     xls_filename = Property(str, fget=getXlsFilename)
     account = Property(int, fget=getAccount)
     update_dlsg = Property(bool, fget=getDlsgState)
     dlsg_filename = Property(str, fget=getDslgFilename)
     dlsg_broker_as_income = Property(bool, fget=getBrokerAsIncomeName)
@@ -103,15 +104,15 @@
 
     @Slot()
     def SaveReport(self):
         if not self.account:
             QMessageBox().warning(self, self.tr("Data are incomplete"),
                                   self.tr("You haven't selected an account for tax report"), QMessageBox.Ok)
             return
-        taxes = TaxReport.create_report(self.Country.currentIndex())
+        taxes = TaxReport.create_report(self.ui.Country.currentIndex())
 
         tax_report = taxes.prepare_tax_report(self.year, self.account, use_settlement=(not self.no_settelement))
         if not tax_report:
             logging.warning(self.tr("Tax report is empty"))
             return
 
         reports_xls = XLSX(self.xls_filename)
@@ -135,44 +136,45 @@
                 tax_forms.save(self.dlsg_filename)
                 logging.info(self.tr("Tax report saved to file ") + f"'{self.dlsg_filename}'")
             except:
                 logging.error(self.tr("Can't write tax form into file ") + f"'{self.dlsg_filename}'" +
                               f"\n{traceback.format_exc()}")
 
 
-class MoneyFlowWidget(MdiWidget, Ui_MoneyFlowWidget):
-    def __init__(self):
-        MdiWidget.__init__(self)
-        self.setupUi(self)
-
-        self.Year.setValue(datetime.now().year - 1)  # Set previous year by default
-        self.XlsSelectBtn.pressed.connect(self.OnFileBtn)
-        self.SaveButton.pressed.connect(self.SaveReport)
+class MoneyFlowWidget(MdiWidget):
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.ui = Ui_MoneyFlowWidget()
+        self.ui.setupUi(self)
+
+        self.ui.Year.setValue(datetime.now().year - 1)  # Set previous year by default
+        self.ui.XlsSelectBtn.pressed.connect(self.OnFileBtn)
+        self.ui.SaveButton.pressed.connect(self.SaveReport)
 
     # Displays tax widget in a given MDI area.
     # It is implemented as a separate static method in order to prevent unexpected object deletion
     @staticmethod
     def showInMDI(parent_mdi):
-        parent_mdi.addSubWindow(MoneyFlowWidget(), maximized=False)
+        parent_mdi.addSubWindow(MoneyFlowWidget(parent_mdi), maximized=False)
 
     @Slot()
     def OnFileBtn(self):
-        selector = (self.tr("Save money flow report to:"), self.tr("Excel files (*.xlsx)"), '.xlsx', self.XlsFileName)
+        selector = (self.tr("Save money flow report to:"), self.tr("Excel files (*.xlsx)"), '.xlsx', self.ui.XlsFileName)
         filename = QFileDialog.getSaveFileName(self, selector[0], ".", selector[1])
         if filename[0]:
             if filename[1] == selector[1] and filename[0][-len(selector[2]):] != selector[2]:
                 selector[3].setText(filename[0] + selector[2])
             else:
                 selector[3].setText(filename[0])
 
     def getYear(self):
-        return self.Year.value()
+        return self.ui.Year.value()
 
     def getXlsFilename(self):
-        return self.XlsFileName.text()
+        return self.ui.XlsFileName.text()
 
     year = Property(int, fget=getYear)
     xls_filename = Property(str, fget=getXlsFilename)
 
     @Slot()
     def SaveReport(self):
         taxes_flow = TaxesFlowRus()
```

### Comparing `jal-2023.4.4/jal/widgets/trade_widget.py` & `jal-2023.4.5/jal/widgets/trade_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal/widgets/transfer_widget.py` & `jal-2023.4.5/jal/widgets/transfer_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/jal.egg-info/PKG-INFO` & `jal-2023.4.5/jal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.4
+Version: 2023.4.5
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.4/jal.egg-info/SOURCES.txt` & `jal-2023.4.5/jal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jal-2023.4.4/setup.py` & `jal-2023.4.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "Topic :: Office/Business :: Financial",
         "Topic :: Office/Business :: Financial :: Accounting",
         "Topic :: Office/Business :: Financial :: Investment",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python"
     ],
-    install_requires=["lxml", "pandas", "PySide6>=6.2.0,<6.5.0", "requests", "XlsxWriter", "jsonschema", "sqlparse"],
+    install_requires=["lxml", "pandas", "PySide6>=6.2.0", "requests", "XlsxWriter", "jsonschema", "sqlparse"],
     entry_points={
         'console_scripts': ['jal=jal.jal:main', ]
     },
     include_package_data=True,
     package_data={
         '': ['*.sql', '*.json', 'languages/*.qm', 'languages/*.png', 'pypi_description.md', 'img/*.ico', 'img/*.png']
     }
```

