# Comparing `tmp/airbyte-1.1.1.tar.gz` & `tmp/airbyte-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-1.1.1.tar", last modified: Wed Apr 12 00:45:14 2023, max compression
+gzip compressed data, was "airbyte-1.2.0.tar", last modified: Fri Apr 14 00:44:40 2023, max compression
```

## Comparing `airbyte-1.1.1.tar` & `airbyte-1.2.0.tar`

### file list

```diff
@@ -1,296 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.344617 airbyte-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 00:44:57.000000 airbyte-1.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-12 00:45:14.344617 airbyte-1.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3408 2023-04-12 00:44:57.000000 airbyte-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:45:14.344617 airbyte-1.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-12 00:44:57.000000 airbyte-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.292614 airbyte-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.292614 airbyte-1.1.1/src/airbyte/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4147 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/destinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4852 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.292614 airbyte-1.1.1/src/airbyte/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.296615 airbyte-1.1.1/src/airbyte/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/canceljob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/createconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/createdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      690 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/createjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/createsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/createworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/getconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/getdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/getjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/getsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/getworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/listconnections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/listdestinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/listjobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1663 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/listsources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/operations/listworkspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.340617 airbyte-1.1.1/src/airbyte/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    48677 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1511 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/connectioncreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1848 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/connectionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/connectionschedulecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/connectionscheduleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/connectionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/connectionstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3478 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9302 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_aws_datalake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4632 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11890 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10639 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_bigquery_denormalized.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1996 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_cassandra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6174 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_convex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_databend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8062 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_databricks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3515 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_elasticsearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3777 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_firestore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21101 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_keen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_kinesis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_mariadb_columnstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_meilisearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9235 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8155 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6089 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6790 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11178 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2760 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_pubsub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5831 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_pulsar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_rabbitmq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8064 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_redis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14025 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_rockset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18946 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8554 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_s3_glue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_scylla.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_sftp_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16133 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destination_typesense.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destinationcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destinationresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/destinationsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/geographyenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/jobcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/jobresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/jobsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/jobstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/jobtypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/scheduletypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_airtable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7535 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_alloydb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_amazon_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5171 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_amazon_seller_partner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3935 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3040 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_amplitude.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_apify_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_asana.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3326 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_auth0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_aws_cloudtrail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_azure_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_bamboo_hr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_bigcommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2755 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_bing_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2519 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_braintree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_braze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2240 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_chargebee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2021 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_chartmogul.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5739 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2909 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_clickup_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_close_com.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_coda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_coin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_coinmarketcap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_configcat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_confluence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_datascope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_delighted.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_dixa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_dockerhub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_dremio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2754 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_e2e_test_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_emailoctopus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_exchange_rates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17598 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_facebook_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_facebook_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2141 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_faker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4626 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_fauna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10324 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_file_secure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_freshcaller.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1970 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_freshdesk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_freshsales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_getlago.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4341 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_github.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4152 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_gitlab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_glassfrog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9633 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_gnews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5213 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_analytics_data_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4971 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_analytics_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_directory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_search_console.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3280 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_webfonts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_google_workspace_admin_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_greenhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_gridly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1689 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_harvest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_hubplanner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_hubspot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_insightly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_instagram.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_instatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_intercom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_ip2whois.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_iterable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3198 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_jira.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_k6_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1924 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_klarna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1332 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_klaviyo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_kustomer_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_launchdarkly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_lemlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3583 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_linkedin_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3010 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_linkedin_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_linnworks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1112 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_lokalise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2746 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_mailchimp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_mailgun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1473 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_mailjet_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1761 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_marketo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_metabase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_microsoft_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5916 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_mixpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2588 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_monday.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12234 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_my_hours.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12863 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_netsuite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_notion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_nytimes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3007 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      755 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_omnisend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_onesignal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3403 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_openweather.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10232 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_orb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_orbit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1813 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_outreach.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1989 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_paypal_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1749 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_paystack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_pendo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_persistiq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2551 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_pexels_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_pinterest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_pipedrive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3920 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_pocket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_pokeapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_polygon_stock_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7554 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_posthog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_postmarkapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_prestashop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_public_apis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_punk_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_pypi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_qualaroo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_railz.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_recharge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_recreation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_recruitee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_recurly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2267 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_retently.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_rki_covid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_rss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13331 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3785 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_salesforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3520 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_salesforce_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3552 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_salesloft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_sap_fieldglass.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_secoda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_sendgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_sendinblue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3353 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_senseforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_sentry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_sftp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_sftp_bulk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3217 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_shopify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_shortio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4288 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_slack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_smaily.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_smartengage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4183 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_smartsheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_snapchat_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4413 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_sonar_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_spacex_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_square.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_strava.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2529 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_stripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_survey_sparrow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3738 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_surveymonkey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_tempo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_the_guardian_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4994 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_tiktok_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_todoist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_trello.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3853 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_trustpilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1797 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_tvmaze_schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_twilio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_twilio_taskrouter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_twitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1789 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_typeform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_us_census.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_vantage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_webflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_whisky_hunter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_wikipedia_pageviews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_woocommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_xero.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_xkcd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_yandex_metrica.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_younium.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_youtube_analytics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_chat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3150 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_sunshine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2067 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_support.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_talk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1889 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zenloop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3102 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zoho_crm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zoom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/source_zuora.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/sourcecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/sourceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/sourcesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/workspacecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/workspaceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      816 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/models/shared/workspacesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3310 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.344617 airbyte-1.1.1/src/airbyte/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-04-12 00:44:57.000000 airbyte-1.1.1/src/airbyte/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:45:14.292614 airbyte-1.1.1/src/airbyte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-12 00:45:14.000000 airbyte-1.1.1/src/airbyte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-12 00:45:14.000000 airbyte-1.1.1/src/airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:45:14.000000 airbyte-1.1.1/src/airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 00:45:14.000000 airbyte-1.1.1/src/airbyte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 00:45:14.000000 airbyte-1.1.1/src/airbyte.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.793377 airbyte-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 00:44:32.000000 airbyte-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-14 00:44:40.793377 airbyte-1.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5540 2023-04-14 00:44:32.000000 airbyte-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:44:40.793377 airbyte-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-14 00:44:32.000000 airbyte-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.765377 airbyte-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.769377 airbyte-1.2.0/src/airbyte/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4743 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/destinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4852 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.769377 airbyte-1.2.0/src/airbyte/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.769377 airbyte-1.2.0/src/airbyte/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/canceljob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/createconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/createdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      690 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/createjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/createsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/createworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/deleteconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/deletedestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/deletesource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/getconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/getdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/getjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/getsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/getstreamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/getworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/listconnections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/listdestinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/listjobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1663 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/listsources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/operations/listworkspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.793377 airbyte-1.2.0/src/airbyte/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49282 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3230 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/connectioncreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/connectionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/connectionschedulecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/connectionscheduleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/connectionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/connectionstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3478 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9302 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_aws_datalake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4632 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12180 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10929 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_bigquery_denormalized.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1996 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_cassandra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6174 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_convex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_databend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8062 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_databricks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3515 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_elasticsearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3777 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_firestore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21101 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_keen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_kinesis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_mariadb_columnstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_meilisearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9235 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8155 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6089 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6790 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11178 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2760 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_pubsub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5831 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_pulsar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_rabbitmq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8064 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_redis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14025 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_rockset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18946 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_s3_glue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_scylla.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_sftp_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16133 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destination_typesense.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destinationcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destinationresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/destinationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/geographyenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/jobcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/jobresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/jobsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/jobstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/jobtypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/scheduletypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_airtable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7535 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_alloydb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_amazon_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5171 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_amazon_seller_partner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3935 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2390 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_amplitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_apify_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_asana.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3326 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_auth0.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_aws_cloudtrail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3061 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_azure_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_bamboo_hr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_bigcommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2755 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_bing_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2519 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_braintree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_braze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2240 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_chargebee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2021 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_chartmogul.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5739 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2909 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_clickup_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_close_com.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_coda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_coin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_coinmarketcap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_configcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_confluence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_datascope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_delighted.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_dixa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_dockerhub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_dremio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2754 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_e2e_test_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_emailoctopus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_exchange_rates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17598 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_facebook_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_facebook_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2141 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_faker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4626 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_fauna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10324 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_file_secure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_freshcaller.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1970 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_freshdesk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_freshsales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_getlago.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4341 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_github.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4152 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_gitlab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_glassfrog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9633 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_gnews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5213 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_analytics_data_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4971 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_analytics_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_directory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_search_console.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3280 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_webfonts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_greenhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_gridly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_harvest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_hubplanner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3668 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_hubspot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_insightly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_instagram.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_instatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_intercom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_ip2whois.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_iterable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_jira.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_k6_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1924 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_klarna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1332 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_klaviyo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_kustomer_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_launchdarkly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_lemlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3583 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_linkedin_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3010 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_linkedin_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_linnworks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1112 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_lokalise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2746 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_mailchimp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_mailgun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1473 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_mailjet_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1973 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_marketo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_metabase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_microsoft_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6254 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_mixpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2588 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_monday.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12234 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_my_hours.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12863 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_netsuite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_notion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_nytimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3007 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      755 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_omnisend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_onesignal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3403 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_openweather.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10232 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_orb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_orbit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1813 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_outreach.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1989 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_paypal_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1749 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_paystack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_pendo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_persistiq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2551 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_pexels_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_pinterest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_pipedrive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3920 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_pocket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_pokeapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_polygon_stock_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7554 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_posthog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_postmarkapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_prestashop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_public_apis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_punk_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_pypi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_qualaroo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3543 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_quickbooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_railz.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_recharge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_recreation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_recruitee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_recurly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2267 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_retently.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_rki_covid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_rss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13331 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3785 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_salesforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3520 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_salesforce_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3552 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_salesloft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_sap_fieldglass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_secoda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_sendgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_sendinblue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3353 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_senseforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_sentry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_sftp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_sftp_bulk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3217 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_shopify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_shortio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4288 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_slack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_smaily.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_smartengage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4183 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_smartsheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_snapchat_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4413 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_sonar_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_spacex_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_square.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_strava.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2529 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_stripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_survey_sparrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3738 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_surveymonkey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_tempo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_the_guardian_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4470 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_tiktok_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_todoist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_trello.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3853 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_trustpilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1797 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_tvmaze_schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_twilio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_twilio_taskrouter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_twitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1789 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_typeform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_us_census.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_vantage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_webflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_whisky_hunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_wikipedia_pageviews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_woocommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_xero.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_xkcd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_yandex_metrica.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_younium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_youtube_analytics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_chat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3150 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_sunshine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2067 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_talk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1889 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zenloop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3102 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zoho_crm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zoom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/source_zuora.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/sourcecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/sourceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/sourcesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/streamconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/streamconfigurations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/streamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/workspacecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      857 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/workspaceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      816 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/models/shared/workspacesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4628 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/sources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1838 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.793377 airbyte-1.2.0/src/airbyte/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-04-14 00:44:32.000000 airbyte-1.2.0/src/airbyte/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:44:40.769377 airbyte-1.2.0/src/airbyte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-14 00:44:40.000000 airbyte-1.2.0/src/airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-04-14 00:44:40.000000 airbyte-1.2.0/src/airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:44:40.000000 airbyte-1.2.0/src/airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 00:44:40.000000 airbyte-1.2.0/src/airbyte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 00:44:40.000000 airbyte-1.2.0/src/airbyte.egg-info/top_level.txt
```

### Comparing `airbyte-1.1.1/LICENSE.md` & `airbyte-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/setup.py` & `airbyte-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="airbyte",
-    version="1.1.1",
+    version="1.2.0",
     author="Speakeasy",
     description="Python Client SDK for Airbyte API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `airbyte-1.1.1/src/airbyte/connections.py` & `airbyte-1.2.0/src/airbyte/connections.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,14 +46,31 @@
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectionResponse])
                 res.connection_response = out
         elif http_res.status_code in [400, 403]:
             pass
 
         return res
 
+    def delete_connection(self, request: operations.DeleteConnectionRequest) -> operations.DeleteConnectionResponse:
+        r"""Get Connection details"""
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.DeleteConnectionRequest, base_url, '/connections/{connectionId}', request)
+        
+        
+        client = self._security_client
+        
+        http_res = client.request('DELETE', url)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+
+        return res
+
     def get_connection(self, request: operations.GetConnectionRequest) -> operations.GetConnectionResponse:
         r"""Get Connection details"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetConnectionRequest, base_url, '/connections/{connectionId}', request)
```

### Comparing `airbyte-1.1.1/src/airbyte/destinations.py` & `airbyte-1.2.0/src/airbyte/destinations.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,31 @@
                 out = utils.unmarshal_json(http_res.text, Optional[shared.DestinationResponse])
                 res.destination_response = out
         elif http_res.status_code in [400, 403, 404]:
             pass
 
         return res
 
+    def delete_destination(self, request: operations.DeleteDestinationRequest) -> operations.DeleteDestinationResponse:
+        r"""Get Connection details"""
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.DeleteDestinationRequest, base_url, '/destinations/{destinationId}', request)
+        
+        
+        client = self._security_client
+        
+        http_res = client.request('DELETE', url)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.DeleteDestinationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+
+        return res
+
     def get_destination(self, request: operations.GetDestinationRequest) -> operations.GetDestinationResponse:
         r"""Get Destination details"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDestinationRequest, base_url, '/destinations/{destinationId}', request)
```

### Comparing `airbyte-1.1.1/src/airbyte/jobs.py` & `airbyte-1.2.0/src/airbyte/jobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/__init__.py` & `airbyte-1.2.0/src/airbyte/models/operations/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 
 from .canceljob import *
 from .createconnection import *
 from .createdestination import *
 from .createjob import *
 from .createsource import *
 from .createworkspace import *
+from .deleteconnection import *
+from .deletedestination import *
+from .deletesource import *
 from .getconnection import *
 from .getdestination import *
 from .getjob import *
 from .getsource import *
+from .getstreamproperties import *
 from .getworkspace import *
 from .listconnections import *
 from .listdestinations import *
 from .listjobs import *
 from .listsources import *
 from .listworkspaces import *
 
-__all__ = ["CancelJobRequest","CancelJobResponse","CreateConnectionResponse","CreateDestinationResponse","CreateJobResponse","CreateSourceResponse","CreateWorkspaceResponse","GetConnectionRequest","GetConnectionResponse","GetDestinationRequest","GetDestinationResponse","GetJobRequest","GetJobResponse","GetSourceRequest","GetSourceResponse","GetWorkspaceRequest","GetWorkspaceResponse","ListConnectionsRequest","ListConnectionsResponse","ListDestinationsRequest","ListDestinationsResponse","ListJobsRequest","ListJobsResponse","ListSourcesRequest","ListSourcesResponse","ListWorkspacesRequest","ListWorkspacesResponse"]
+__all__ = ["CancelJobRequest","CancelJobResponse","CreateConnectionResponse","CreateDestinationResponse","CreateJobResponse","CreateSourceResponse","CreateWorkspaceResponse","DeleteConnectionRequest","DeleteConnectionResponse","DeleteDestinationRequest","DeleteDestinationResponse","DeleteSourceRequest","DeleteSourceResponse","GetConnectionRequest","GetConnectionResponse","GetDestinationRequest","GetDestinationResponse","GetJobRequest","GetJobResponse","GetSourceRequest","GetSourceResponse","GetStreamPropertiesRequest","GetStreamPropertiesResponse","GetWorkspaceRequest","GetWorkspaceResponse","ListConnectionsRequest","ListConnectionsResponse","ListDestinationsRequest","ListDestinationsResponse","ListJobsRequest","ListJobsResponse","ListSourcesRequest","ListSourcesResponse","ListWorkspacesRequest","ListWorkspacesResponse"]
```

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/canceljob.py` & `airbyte-1.2.0/src/airbyte/models/operations/canceljob.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/createconnection.py` & `airbyte-1.2.0/src/airbyte/models/operations/createconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/createdestination.py` & `airbyte-1.2.0/src/airbyte/models/operations/createdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/createjob.py` & `airbyte-1.2.0/src/airbyte/models/operations/createjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/createsource.py` & `airbyte-1.2.0/src/airbyte/models/operations/createsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/createworkspace.py` & `airbyte-1.2.0/src/airbyte/models/operations/createworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/getconnection.py` & `airbyte-1.2.0/src/airbyte/models/operations/getconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/getdestination.py` & `airbyte-1.2.0/src/airbyte/models/operations/getdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/getjob.py` & `airbyte-1.2.0/src/airbyte/models/operations/getjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/getsource.py` & `airbyte-1.2.0/src/airbyte/models/operations/getsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/getworkspace.py` & `airbyte-1.2.0/src/airbyte/models/operations/getworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/listconnections.py` & `airbyte-1.2.0/src/airbyte/models/operations/listconnections.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/listdestinations.py` & `airbyte-1.2.0/src/airbyte/models/operations/listdestinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/listjobs.py` & `airbyte-1.2.0/src/airbyte/models/operations/listjobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/listsources.py` & `airbyte-1.2.0/src/airbyte/models/operations/listsources.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/operations/listworkspaces.py` & `airbyte-1.2.0/src/airbyte/models/operations/listworkspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/__init__.py` & `airbyte-1.2.0/src/airbyte/models/shared/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .connectioncreaterequest import *
 from .connectionresponse import *
 from .connectionschedulecreate import *
 from .connectionscheduleresponse import *
 from .connectionsresponse import *
 from .connectionstatusenum_enum import *
+from .connectionsyncmodeenum_enum import *
 from .destination_amazon_sqs import *
 from .destination_aws_datalake import *
 from .destination_azure_blob_storage import *
 from .destination_bigquery import *
 from .destination_bigquery_denormalized import *
 from .destination_cassandra import *
 from .destination_clickhouse import *
@@ -61,14 +62,15 @@
 from .source_amazon_seller_partner import *
 from .source_amazon_sqs import *
 from .source_amplitude import *
 from .source_apify_dataset import *
 from .source_asana import *
 from .source_auth0 import *
 from .source_aws_cloudtrail import *
+from .source_azure_blob_storage import *
 from .source_azure_table import *
 from .source_bamboo_hr import *
 from .source_bigcommerce import *
 from .source_bigquery import *
 from .source_bing_ads import *
 from .source_braintree import *
 from .source_braze import *
@@ -173,14 +175,15 @@
 from .source_posthog import *
 from .source_postmarkapp import *
 from .source_prestashop import *
 from .source_public_apis import *
 from .source_punk_api import *
 from .source_pypi import *
 from .source_qualaroo import *
+from .source_quickbooks import *
 from .source_railz import *
 from .source_recharge import *
 from .source_recreation import *
 from .source_recruitee import *
 from .source_recurly import *
 from .source_redshift import *
 from .source_retently import *
@@ -242,12 +245,15 @@
 from .source_zenloop import *
 from .source_zoho_crm import *
 from .source_zoom import *
 from .source_zuora import *
 from .sourcecreaterequest import *
 from .sourceresponse import *
 from .sourcesresponse import *
+from .streamconfiguration import *
+from .streamconfigurations import *
+from .streamproperties import *
 from .workspacecreaterequest import *
 from .workspaceresponse import *
 from .workspacesresponse import *
 
-__all__ = ["ConnectionCreateRequest","ConnectionResponse","ConnectionScheduleCreate","ConnectionScheduleResponse","ConnectionStatusEnumEnum","ConnectionsResponse","DestinationAmazonSqs","DestinationAmazonSqsAWSRegionEnum","DestinationAmazonSqsAmazonSqsEnum","DestinationAwsDatalake","DestinationAwsDatalakeAwsDatalakeEnum","DestinationAwsDatalakeChooseHowToPartitionDataEnum","DestinationAwsDatalakeCredentialsIAMRole","DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum","DestinationAwsDatalakeCredentialsIAMUser","DestinationAwsDatalakeCredentialsIAMUserCredentialsTitleEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSON","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONFormatTypeWildcardEnum","DestinationAwsDatalakeFormatParquetColumnarStorage","DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatParquetColumnarStorageFormatTypeWildcardEnum","DestinationAwsDatalakeS3BucketRegionEnum","DestinationAzureBlobStorage","DestinationAzureBlobStorageAzureBlobStorageEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValues","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationBigquery","DestinationBigqueryBigqueryEnum","DestinationBigqueryDatasetLocationEnum","DestinationBigqueryDenormalized","DestinationBigqueryDenormalizedBigqueryDenormalizedEnum","DestinationBigqueryDenormalizedDatasetLocationEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStaging","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum","DestinationBigqueryDenormalizedLoadingMethodStandardInserts","DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryLoadingMethodGCSStaging","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryLoadingMethodGCSStagingMethodEnum","DestinationBigqueryLoadingMethodStandardInserts","DestinationBigqueryLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryTransformationQueryRunTypeEnum","DestinationCassandra","DestinationCassandraCassandraEnum","DestinationClickhouse","DestinationClickhouseClickhouseEnum","DestinationClickhouseTunnelMethodNoTunnel","DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum","DestinationClickhouseTunnelMethodPasswordAuthentication","DestinationClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationClickhouseTunnelMethodSSHKeyAuthentication","DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationConvex","DestinationConvexConvexEnum","DestinationCreateRequest","DestinationDatabend","DestinationDatabendDatabendEnum","DestinationDatabricks","DestinationDatabricksDataSourceAmazonS3","DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum","DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum","DestinationDatabricksDataSourceAzureBlobStorage","DestinationDatabricksDataSourceAzureBlobStorageDataSourceTypeEnum","DestinationDatabricksDataSourceRecommendedManagedTables","DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum","DestinationDatabricksDatabricksEnum","DestinationDynamodb","DestinationDynamodbDynamoDBRegionEnum","DestinationDynamodbDynamodbEnum","DestinationElasticsearch","DestinationElasticsearchAuthenticationMethodAPIKeySecret","DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum","DestinationElasticsearchAuthenticationMethodUsernamePassword","DestinationElasticsearchAuthenticationMethodUsernamePasswordMethodEnum","DestinationElasticsearchElasticsearchEnum","DestinationFirebolt","DestinationFireboltFireboltEnum","DestinationFireboltLoadingMethodExternalTableViaS3","DestinationFireboltLoadingMethodExternalTableViaS3MethodEnum","DestinationFireboltLoadingMethodSQLInserts","DestinationFireboltLoadingMethodSQLInsertsMethodEnum","DestinationFirestore","DestinationFirestoreFirestoreEnum","DestinationGCSGCSBucketRegionEnum","DestinationGcs","DestinationGcsCredentialHMACKey","DestinationGcsCredentialHMACKeyCredentialTypeEnum","DestinationGcsFormatAvroApacheAvro","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflate","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompression","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappy","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecXz","DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandard","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationGcsFormatAvroApacheAvroFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValues","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIP","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSON","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationGcsFormatParquetColumnarStorage","DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum","DestinationGcsFormatParquetColumnarStorageFormatTypeEnum","DestinationGcsGcsEnum","DestinationGoogleSheets","DestinationGoogleSheetsAuthenticationViaGoogleOAuth","DestinationGoogleSheetsGoogleSheetsEnum","DestinationKeen","DestinationKeenKeenEnum","DestinationKinesis","DestinationKinesisKinesisEnum","DestinationMariadbColumnstore","DestinationMariadbColumnstoreMariadbColumnstoreEnum","DestinationMariadbColumnstoreTunnelMethodNoTunnel","DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodPasswordAuthentication","DestinationMariadbColumnstoreTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthentication","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMeilisearch","DestinationMeilisearchMeilisearchEnum","DestinationMongodb","DestinationMongodbAuthTypeLoginPassword","DestinationMongodbAuthTypeLoginPasswordAuthorizationEnum","DestinationMongodbAuthTypeNone","DestinationMongodbAuthTypeNoneAuthorizationEnum","DestinationMongodbInstanceTypeMongoDBAtlas","DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum","DestinationMongodbInstanceTypeReplicaSet","DestinationMongodbInstanceTypeReplicaSetInstanceEnum","DestinationMongodbInstanceTypeStandaloneMongoDbInstance","DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","DestinationMongodbMongodbEnum","DestinationMongodbTunnelMethodNoTunnel","DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum","DestinationMongodbTunnelMethodPasswordAuthentication","DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMongodbTunnelMethodSSHKeyAuthentication","DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMssql","DestinationMssqlMssqlEnum","DestinationMssqlSslMethodEncryptedTrustServerCertificate","DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","DestinationMssqlSslMethodEncryptedVerifyCertificate","DestinationMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","DestinationMssqlTunnelMethodNoTunnel","DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMssqlTunnelMethodPasswordAuthentication","DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMssqlTunnelMethodSSHKeyAuthentication","DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMysql","DestinationMysqlMysqlEnum","DestinationMysqlTunnelMethodNoTunnel","DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMysqlTunnelMethodPasswordAuthentication","DestinationMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMysqlTunnelMethodSSHKeyAuthentication","DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationOracle","DestinationOracleOracleEnum","DestinationOracleTunnelMethodNoTunnel","DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum","DestinationOracleTunnelMethodPasswordAuthentication","DestinationOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationOracleTunnelMethodSSHKeyAuthentication","DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPostgres","DestinationPostgresPostgresEnum","DestinationPostgresSslModeAllow","DestinationPostgresSslModeAllowModeEnum","DestinationPostgresSslModeDisable","DestinationPostgresSslModeDisableModeEnum","DestinationPostgresSslModePrefer","DestinationPostgresSslModePreferModeEnum","DestinationPostgresSslModeRequire","DestinationPostgresSslModeRequireModeEnum","DestinationPostgresSslModeVerifyCa","DestinationPostgresSslModeVerifyCaModeEnum","DestinationPostgresSslModeVerifyFull","DestinationPostgresSslModeVerifyFullModeEnum","DestinationPostgresTunnelMethodNoTunnel","DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum","DestinationPostgresTunnelMethodPasswordAuthentication","DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationPostgresTunnelMethodSSHKeyAuthentication","DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPubsub","DestinationPubsubPubsubEnum","DestinationPulsar","DestinationPulsarCompressionTypeEnum","DestinationPulsarPulsarEnum","DestinationPulsarTopicTypeEnum","DestinationRabbitmq","DestinationRabbitmqRabbitmqEnum","DestinationRedis","DestinationRedisCacheTypeEnum","DestinationRedisRedisEnum","DestinationRedisSslModeDisable","DestinationRedisSslModeDisableModeEnum","DestinationRedisSslModeVerifyFull","DestinationRedisSslModeVerifyFullModeEnum","DestinationRedisTunnelMethodNoTunnel","DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedisTunnelMethodPasswordAuthentication","DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedisTunnelMethodSSHKeyAuthentication","DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshift","DestinationRedshiftRedshiftEnum","DestinationRedshiftTunnelMethodNoTunnel","DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedshiftTunnelMethodPasswordAuthentication","DestinationRedshiftTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedshiftTunnelMethodSSHKeyAuthentication","DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshiftUploadingMethodS3Staging","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingMethodEnum","DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum","DestinationRedshiftUploadingMethodStandard","DestinationRedshiftUploadingMethodStandardMethodEnum","DestinationResponse","DestinationRockset","DestinationRocksetRocksetEnum","DestinationS3","DestinationS3FormatAvroApacheAvro","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecDeflate","DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompression","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecSnappy","DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecXz","DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecZstandard","DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationS3FormatAvroApacheAvroFormatTypeEnum","DestinationS3FormatCSVCommaSeparatedValues","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIP","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum","DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSON","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3FormatParquetColumnarStorage","DestinationS3FormatParquetColumnarStorageCompressionCodecEnum","DestinationS3FormatParquetColumnarStorageFormatTypeEnum","DestinationS3Glue","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3GlueS3BucketRegionEnum","DestinationS3GlueS3GlueEnum","DestinationS3GlueSerializationLibraryEnum","DestinationS3S3BucketRegionEnum","DestinationS3S3Enum","DestinationScylla","DestinationScyllaScyllaEnum","DestinationSftpJSON","DestinationSftpJSONSftpJSONEnum","DestinationSnowflake","DestinationSnowflakeCredentialsKeyPairAuthentication","DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum","DestinationSnowflakeCredentialsOAuth20","DestinationSnowflakeCredentialsOAuth20AuthTypeEnum","DestinationSnowflakeCredentialsUsernameAndPassword","DestinationSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","DestinationSnowflakeLoadingMethodAWSS3Staging","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum","DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum","DestinationSnowflakeLoadingMethodAzureBlobStorageStaging","DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging","DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodRecommendedInternalStaging","DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum","DestinationSnowflakeLoadingMethodSelectAnotherOption","DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum","DestinationSnowflakeSnowflakeEnum","DestinationTypesense","DestinationTypesenseTypesenseEnum","DestinationsResponse","GeographyEnumEnum","JobCreateRequest","JobResponse","JobStatusEnumEnum","JobTypeEnumEnum","JobsResponse","ScheduleTypeEnumEnum","ScheduleTypeWithBasicEnumEnum","Security","SourceAirtable","SourceAirtableAirtableEnum","SourceAirtableCredentialsOAuth20","SourceAirtableCredentialsOAuth20AuthMethodEnum","SourceAirtableCredentialsPersonalAccessToken","SourceAirtableCredentialsPersonalAccessTokenAuthMethodEnum","SourceAlloydb","SourceAlloydbAlloydbEnum","SourceAlloydbReplicationMethodStandard","SourceAlloydbReplicationMethodStandardMethodEnum","SourceAlloydbTunnelMethodNoTunnel","SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum","SourceAlloydbTunnelMethodPasswordAuthentication","SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceAlloydbTunnelMethodSSHKeyAuthentication","SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceAmazonAds","SourceAmazonAdsAmazonAdsEnum","SourceAmazonAdsAuthTypeEnum","SourceAmazonAdsRegionEnum","SourceAmazonAdsReportRecordTypesEnum","SourceAmazonAdsStateFilterEnum","SourceAmazonSellerPartner","SourceAmazonSellerPartnerAWSEnvironmentEnum","SourceAmazonSellerPartnerAWSRegionEnum","SourceAmazonSellerPartnerAmazonSellerPartnerEnum","SourceAmazonSellerPartnerAuthTypeEnum","SourceAmazonSqs","SourceAmazonSqsAWSRegionEnum","SourceAmazonSqsAmazonSqsEnum","SourceAmplitude","SourceAmplitudeAmplitudeEnum","SourceAmplitudeDataRegionEnum","SourceAmplitudeEventStreamTimeInterval","SourceAmplitudeEventStreamTimeIntervalEventsTimeIntervalSizeUnitEnum","SourceApifyDataset","SourceApifyDatasetApifyDatasetEnum","SourceAsana","SourceAsanaAsanaEnum","SourceAsanaCredentialsAuthenticateViaAsanaOauth","SourceAsanaCredentialsAuthenticateViaAsanaOauthCredentialsTitleEnum","SourceAsanaCredentialsAuthenticateWithPersonalAccessToken","SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum","SourceAuth0","SourceAuth0Auth0Enum","SourceAuth0CredentialsOAuth2AccessToken","SourceAuth0CredentialsOAuth2AccessTokenAuthenticationMethodEnum","SourceAuth0CredentialsOAuth2ConfidentialApplication","SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum","SourceAwsCloudtrail","SourceAwsCloudtrailAwsCloudtrailEnum","SourceAzureTable","SourceAzureTableAzureTableEnum","SourceBambooHr","SourceBambooHrBambooHrEnum","SourceBigcommerce","SourceBigcommerceBigcommerceEnum","SourceBigquery","SourceBigqueryBigqueryEnum","SourceBingAds","SourceBingAdsAuthMethodEnum","SourceBingAdsBingAdsEnum","SourceBraintree","SourceBraintreeBraintreeEnum","SourceBraintreeEnvironmentEnum","SourceBraze","SourceBrazeBrazeEnum","SourceChargebee","SourceChargebeeChargebeeEnum","SourceChargebeeProductCatalogEnum","SourceChartmogul","SourceChartmogulChartmogulEnum","SourceChartmogulIntervalEnum","SourceClickhouse","SourceClickhouseClickhouseEnum","SourceClickhouseTunnelMethodNoTunnel","SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum","SourceClickhouseTunnelMethodPasswordAuthentication","SourceClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceClickhouseTunnelMethodSSHKeyAuthentication","SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceClickupAPI","SourceClickupAPIClickupAPIEnum","SourceCloseCom","SourceCloseComCloseComEnum","SourceCoda","SourceCodaCodaEnum","SourceCoinAPI","SourceCoinAPICoinAPIEnum","SourceCoinAPIEnvironmentEnum","SourceCoinmarketcap","SourceCoinmarketcapCoinmarketcapEnum","SourceCoinmarketcapDataTypeEnum","SourceConfigcat","SourceConfigcatConfigcatEnum","SourceConfluence","SourceConfluenceConfluenceEnum","SourceCreateRequest","SourceDatascope","SourceDatascopeDatascopeEnum","SourceDelighted","SourceDelightedDelightedEnum","SourceDixa","SourceDixaDixaEnum","SourceDockerhub","SourceDockerhubDockerhubEnum","SourceDremio","SourceDremioDremioEnum","SourceDynamodb","SourceDynamodbDynamodbEnum","SourceDynamodbDynamodbRegionEnum","SourceE2eTestCloud","SourceE2eTestCloudE2eTestCloudEnum","SourceE2eTestCloudMockCatalogMultiSchema","SourceE2eTestCloudMockCatalogMultiSchemaTypeEnum","SourceE2eTestCloudMockCatalogSingleSchema","SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum","SourceE2eTestCloudTypeEnum","SourceEmailoctopus","SourceEmailoctopusEmailoctopusEnum","SourceExchangeRates","SourceExchangeRatesExchangeRatesEnum","SourceFacebookMarketing","SourceFacebookMarketingFacebookMarketingEnum","SourceFacebookMarketingInsightConfig","SourceFacebookMarketingInsightConfigLevelEnum","SourceFacebookMarketingInsightConfigValidActionBreakdownsEnum","SourceFacebookMarketingInsightConfigValidBreakdownsEnum","SourceFacebookMarketingInsightConfigValidEnumsEnum","SourceFacebookPages","SourceFacebookPagesFacebookPagesEnum","SourceFaker","SourceFakerFakerEnum","SourceFauna","SourceFaunaCollection","SourceFaunaCollectionDeletionsDisabled","SourceFaunaCollectionDeletionsDisabledDeletionModeEnum","SourceFaunaCollectionDeletionsEnabled","SourceFaunaCollectionDeletionsEnabledDeletionModeEnum","SourceFaunaFaunaEnum","SourceFileSecure","SourceFileSecureFileFormatEnum","SourceFileSecureFileSecureEnum","SourceFileSecureProviderAzBlobAzureBlobStorage","SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum","SourceFileSecureProviderGCSGoogleCloudStorage","SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum","SourceFileSecureProviderHTTPSPublicWeb","SourceFileSecureProviderHTTPSPublicWebStorageEnum","SourceFileSecureProviderS3AmazonWebServices","SourceFileSecureProviderS3AmazonWebServicesStorageEnum","SourceFileSecureProviderSCPSecureCopyProtocol","SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum","SourceFileSecureProviderSFTPSecureFileTransferProtocol","SourceFileSecureProviderSFTPSecureFileTransferProtocolStorageEnum","SourceFileSecureProviderSSHSecureShell","SourceFileSecureProviderSSHSecureShellStorageEnum","SourceFirebolt","SourceFireboltFireboltEnum","SourceFreshcaller","SourceFreshcallerFreshcallerEnum","SourceFreshdesk","SourceFreshdeskFreshdeskEnum","SourceFreshsales","SourceFreshsalesFreshsalesEnum","SourceGcs","SourceGcsGcsEnum","SourceGetlago","SourceGetlagoGetlagoEnum","SourceGithub","SourceGithubCredentialsOAuth","SourceGithubCredentialsOAuthOptionTitleEnum","SourceGithubCredentialsPersonalAccessToken","SourceGithubCredentialsPersonalAccessTokenOptionTitleEnum","SourceGithubGithubEnum","SourceGitlab","SourceGitlabCredentialsOAuth20","SourceGitlabCredentialsOAuth20AuthTypeEnum","SourceGitlabCredentialsPrivateToken","SourceGitlabCredentialsPrivateTokenAuthTypeEnum","SourceGitlabGitlabEnum","SourceGlassfrog","SourceGlassfrogGlassfrogEnum","SourceGnews","SourceGnewsCountryEnum","SourceGnewsGnewsEnum","SourceGnewsInEnum","SourceGnewsLanguageEnum","SourceGnewsNullableEnum","SourceGnewsSortByEnum","SourceGnewsTopHeadlinesTopicEnum","SourceGoogleAds","SourceGoogleAdsCustomQueries","SourceGoogleAdsGoogleAdsEnum","SourceGoogleAdsGoogleCredentials","SourceGoogleAnalyticsDataAPI","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum","SourceGoogleAnalyticsV4","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum","SourceGoogleDirectory","SourceGoogleDirectoryGoogleDirectoryEnum","SourceGoogleSearchConsole","SourceGoogleSearchConsoleAuthorizationOAuth","SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthentication","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSearchConsoleGoogleSearchConsoleEnum","SourceGoogleSheets","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuth","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum","SourceGoogleSheetsCredentialsServiceAccountKeyAuthentication","SourceGoogleSheetsCredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSheetsGoogleSheetsEnum","SourceGoogleWebfonts","SourceGoogleWebfontsGoogleWebfontsEnum","SourceGoogleWorkspaceAdminReports","SourceGoogleWorkspaceAdminReportsGoogleWorkspaceAdminReportsEnum","SourceGreenhouse","SourceGreenhouseGreenhouseEnum","SourceGridly","SourceGridlyGridlyEnum","SourceHarvest","SourceHarvestHarvestEnum","SourceHubplanner","SourceHubplannerHubplannerEnum","SourceHubspot","SourceHubspotCredentialsOAuth","SourceHubspotCredentialsOAuthCredentialsEnum","SourceHubspotCredentialsPrivateApp","SourceHubspotCredentialsPrivateAppCredentialsEnum","SourceHubspotHubspotEnum","SourceInsightly","SourceInsightlyInsightlyEnum","SourceInstagram","SourceInstagramInstagramEnum","SourceInstatus","SourceInstatusInstatusEnum","SourceIntercom","SourceIntercomIntercomEnum","SourceIp2whois","SourceIp2whoisIp2whoisEnum","SourceIterable","SourceIterableIterableEnum","SourceJira","SourceJiraJiraEnum","SourceK6Cloud","SourceK6CloudK6CloudEnum","SourceKlarna","SourceKlarnaKlarnaEnum","SourceKlarnaRegionEnum","SourceKlaviyo","SourceKlaviyoKlaviyoEnum","SourceKustomerSinger","SourceKustomerSingerKustomerSingerEnum","SourceLaunchdarkly","SourceLaunchdarklyLaunchdarklyEnum","SourceLemlist","SourceLemlistLemlistEnum","SourceLinkedinAds","SourceLinkedinAdsCredentialsAccessToken","SourceLinkedinAdsCredentialsAccessTokenAuthMethodEnum","SourceLinkedinAdsCredentialsOAuth20","SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum","SourceLinkedinAdsLinkedinAdsEnum","SourceLinkedinPages","SourceLinkedinPagesCredentialsAccessToken","SourceLinkedinPagesCredentialsAccessTokenAuthMethodEnum","SourceLinkedinPagesCredentialsOAuth20","SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum","SourceLinkedinPagesLinkedinPagesEnum","SourceLinnworks","SourceLinnworksLinnworksEnum","SourceLokalise","SourceLokaliseLokaliseEnum","SourceMailchimp","SourceMailchimpCredentialsAPIKey","SourceMailchimpCredentialsAPIKeyAuthTypeEnum","SourceMailchimpCredentialsOAuth20","SourceMailchimpCredentialsOAuth20AuthTypeEnum","SourceMailchimpMailchimpEnum","SourceMailgun","SourceMailgunMailgunEnum","SourceMailjetSms","SourceMailjetSmsMailjetSmsEnum","SourceMarketo","SourceMarketoMarketoEnum","SourceMetabase","SourceMetabaseMetabaseEnum","SourceMicrosoftTeams","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoft","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftAuthTypeEnum","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum","SourceMicrosoftTeamsMicrosoftTeamsEnum","SourceMixpanel","SourceMixpanelCredentialsProjectSecret","SourceMixpanelCredentialsProjectSecretOptionTitleEnum","SourceMixpanelCredentialsServiceAccount","SourceMixpanelCredentialsServiceAccountOptionTitleEnum","SourceMixpanelMixpanelEnum","SourceMixpanelRegionEnum","SourceMonday","SourceMondayCredentialsAPIToken","SourceMondayCredentialsAPITokenAuthTypeEnum","SourceMondayCredentialsOAuth20","SourceMondayCredentialsOAuth20AuthTypeEnum","SourceMondayMondayEnum","SourceMongodb","SourceMongodbInstanceTypeMongoDBAtlas","SourceMongodbInstanceTypeMongoDBAtlasInstanceEnum","SourceMongodbInstanceTypeReplicaSet","SourceMongodbInstanceTypeReplicaSetInstanceEnum","SourceMongodbInstanceTypeStandaloneMongoDbInstance","SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","SourceMongodbMongodbEnum","SourceMssql","SourceMssqlMssqlEnum","SourceMssqlReplicationMethodLogicalReplicationCDC","SourceMssqlReplicationMethodLogicalReplicationCDCDataToSyncEnum","SourceMssqlReplicationMethodLogicalReplicationCDCInitialSnapshotIsolationLevelEnum","SourceMssqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMssqlReplicationMethodStandard","SourceMssqlReplicationMethodStandardMethodEnum","SourceMssqlSslMethodEncryptedTrustServerCertificate","SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","SourceMssqlSslMethodEncryptedVerifyCertificate","SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","SourceMssqlTunnelMethodNoTunnel","SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMssqlTunnelMethodPasswordAuthentication","SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMssqlTunnelMethodSSHKeyAuthentication","SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceMyHours","SourceMyHoursMyHoursEnum","SourceMysql","SourceMysqlMysqlEnum","SourceMysqlReplicationMethodLogicalReplicationCDC","SourceMysqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMysqlReplicationMethodStandard","SourceMysqlReplicationMethodStandardMethodEnum","SourceMysqlSslModePreferred","SourceMysqlSslModePreferredModeEnum","SourceMysqlSslModeRequired","SourceMysqlSslModeRequiredModeEnum","SourceMysqlSslModeVerifyCA","SourceMysqlSslModeVerifyCAModeEnum","SourceMysqlSslModeVerifyIdentity","SourceMysqlSslModeVerifyIdentityModeEnum","SourceMysqlTunnelMethodNoTunnel","SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMysqlTunnelMethodPasswordAuthentication","SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMysqlTunnelMethodSSHKeyAuthentication","SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceNetsuite","SourceNetsuiteNetsuiteEnum","SourceNotion","SourceNotionCredentialsAccessToken","SourceNotionCredentialsAccessTokenAuthTypeEnum","SourceNotionCredentialsOAuth20","SourceNotionCredentialsOAuth20AuthTypeEnum","SourceNotionNotionEnum","SourceNytimes","SourceNytimesNytimesEnum","SourceNytimesPeriodUsedForMostPopularStreamsEnum","SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum","SourceOkta","SourceOktaCredentialsAPIToken","SourceOktaCredentialsAPITokenAuthTypeEnum","SourceOktaCredentialsOAuth20","SourceOktaCredentialsOAuth20AuthTypeEnum","SourceOktaOktaEnum","SourceOmnisend","SourceOmnisendOmnisendEnum","SourceOnesignal","SourceOnesignalApplications","SourceOnesignalOnesignalEnum","SourceOpenweather","SourceOpenweatherLanguageEnum","SourceOpenweatherOpenweatherEnum","SourceOpenweatherUnitsEnum","SourceOracle","SourceOracleConnectionDataServiceName","SourceOracleConnectionDataServiceNameConnectionTypeEnum","SourceOracleConnectionDataSystemIDSID","SourceOracleConnectionDataSystemIDSIDConnectionTypeEnum","SourceOracleEncryptionNativeNetworkEncryptionNNE","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionMethodEnum","SourceOracleEncryptionTLSEncryptedVerifyCertificate","SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum","SourceOracleOracleEnum","SourceOracleTunnelMethodNoTunnel","SourceOracleTunnelMethodNoTunnelTunnelMethodEnum","SourceOracleTunnelMethodPasswordAuthentication","SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceOracleTunnelMethodSSHKeyAuthentication","SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceOrb","SourceOrbOrbEnum","SourceOrbit","SourceOrbitOrbitEnum","SourceOutreach","SourceOutreachOutreachEnum","SourcePaypalTransaction","SourcePaypalTransactionPaypalTransactionEnum","SourcePaystack","SourcePaystackPaystackEnum","SourcePendo","SourcePendoPendoEnum","SourcePersistiq","SourcePersistiqPersistiqEnum","SourcePexelsAPI","SourcePexelsAPIPexelsAPIEnum","SourcePinterest","SourcePinterestCredentialsAccessToken","SourcePinterestCredentialsAccessTokenAuthMethodEnum","SourcePinterestCredentialsOAuth20","SourcePinterestCredentialsOAuth20AuthMethodEnum","SourcePinterestPinterestEnum","SourcePinterestStatusEnum","SourcePipedrive","SourcePipedriveAPIKeyAuthentication","SourcePipedriveAPIKeyAuthenticationAuthTypeEnum","SourcePipedrivePipedriveEnum","SourcePocket","SourcePocketContentTypeEnum","SourcePocketDetailTypeEnum","SourcePocketPocketEnum","SourcePocketSortByEnum","SourcePocketStateEnum","SourcePokeapi","SourcePokeapiPokeapiEnum","SourcePolygonStockAPI","SourcePolygonStockAPIPolygonStockAPIEnum","SourcePostgres","SourcePostgresPostgresEnum","SourcePostgresReplicationMethodStandard","SourcePostgresReplicationMethodStandardMethodEnum","SourcePostgresTunnelMethodNoTunnel","SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum","SourcePostgresTunnelMethodPasswordAuthentication","SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourcePostgresTunnelMethodSSHKeyAuthentication","SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourcePosthog","SourcePosthogPosthogEnum","SourcePostmarkapp","SourcePostmarkappPostmarkappEnum","SourcePrestashop","SourcePrestashopPrestashopEnum","SourcePublicApis","SourcePublicApisPublicApisEnum","SourcePunkAPI","SourcePunkAPIPunkAPIEnum","SourcePypi","SourcePypiPypiEnum","SourceQualaroo","SourceQualarooQualarooEnum","SourceRailz","SourceRailzRailzEnum","SourceRecharge","SourceRechargeRechargeEnum","SourceRecreation","SourceRecreationRecreationEnum","SourceRecruitee","SourceRecruiteeRecruiteeEnum","SourceRecurly","SourceRecurlyRecurlyEnum","SourceRedshift","SourceRedshiftRedshiftEnum","SourceResponse","SourceRetently","SourceRetentlyRetentlyEnum","SourceRkiCovid","SourceRkiCovidRkiCovidEnum","SourceRss","SourceRssRssEnum","SourceS3","SourceS3FormatAvro","SourceS3FormatAvroFiletypeEnum","SourceS3FormatCSV","SourceS3FormatCSVFiletypeEnum","SourceS3FormatJsonl","SourceS3FormatJsonlFiletypeEnum","SourceS3FormatJsonlUnexpectedFieldBehaviorEnum","SourceS3FormatParquet","SourceS3FormatParquetFiletypeEnum","SourceS3S3AmazonWebServices","SourceS3S3Enum","SourceSalesforce","SourceSalesforceAuthTypeEnum","SourceSalesforceSalesforceEnum","SourceSalesforceSinger","SourceSalesforceSingerAPITypeEnum","SourceSalesforceSingerSalesforceSingerEnum","SourceSalesforceStreamsCriteria","SourceSalesforceStreamsCriteriaSearchCriteriaEnum","SourceSalesloft","SourceSalesloftCredentialsAuthenticateViaAPIKey","SourceSalesloftCredentialsAuthenticateViaAPIKeyAuthTypeEnum","SourceSalesloftCredentialsAuthenticateViaOAuth","SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum","SourceSalesloftSalesloftEnum","SourceSapFieldglass","SourceSapFieldglassSapFieldglassEnum","SourceSecoda","SourceSecodaSecodaEnum","SourceSendgrid","SourceSendgridSendgridEnum","SourceSendinblue","SourceSendinblueSendinblueEnum","SourceSenseforce","SourceSenseforceSenseforceEnum","SourceSentry","SourceSentrySentryEnum","SourceSftp","SourceSftpBulk","SourceSftpBulkFileTypeEnum","SourceSftpBulkSftpBulkEnum","SourceSftpCredentialsPasswordAuthentication","SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum","SourceSftpCredentialsSSHKeyAuthentication","SourceSftpCredentialsSSHKeyAuthenticationAuthMethodEnum","SourceSftpSftpEnum","SourceShopify","SourceShopifyCredentialsAPIPassword","SourceShopifyCredentialsAPIPasswordAuthMethodEnum","SourceShopifyCredentialsOAuth20","SourceShopifyCredentialsOAuth20AuthMethodEnum","SourceShopifyShopifyEnum","SourceShortio","SourceShortioShortioEnum","SourceSlack","SourceSlackCredentialsAPIToken","SourceSlackCredentialsAPITokenOptionTitleEnum","SourceSlackCredentialsSignInViaSlackOAuth","SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum","SourceSlackSlackEnum","SourceSmaily","SourceSmailySmailyEnum","SourceSmartengage","SourceSmartengageSmartengageEnum","SourceSmartsheets","SourceSmartsheetsCredentialsAPIAccessToken","SourceSmartsheetsCredentialsAPIAccessTokenAuthTypeEnum","SourceSmartsheetsCredentialsOAuth20","SourceSmartsheetsCredentialsOAuth20AuthTypeEnum","SourceSmartsheetsSmartsheetsEnum","SourceSnapchatMarketing","SourceSnapchatMarketingSnapchatMarketingEnum","SourceSnowflake","SourceSnowflakeCredentialsOAuth20","SourceSnowflakeCredentialsOAuth20AuthTypeEnum","SourceSnowflakeCredentialsUsernameAndPassword","SourceSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","SourceSnowflakeSnowflakeEnum","SourceSonarCloud","SourceSonarCloudSonarCloudEnum","SourceSpacexAPI","SourceSpacexAPISpacexAPIEnum","SourceSquare","SourceSquareCredentialsAPIKey","SourceSquareCredentialsAPIKeyCredentialsTitleEnum","SourceSquareCredentialsOauthAuthentication","SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum","SourceSquareSquareEnum","SourceStrava","SourceStravaAuthTypeEnum","SourceStravaStravaEnum","SourceStripe","SourceStripeStripeEnum","SourceSurveySparrow","SourceSurveySparrowRegionEUBasedAccount","SourceSurveySparrowRegionEUBasedAccountURLBaseEnum","SourceSurveySparrowRegionGlobalAccount","SourceSurveySparrowRegionGlobalAccountURLBaseEnum","SourceSurveySparrowSurveySparrowEnum","SourceSurveymonkey","SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum","SourceSurveymonkeySurveyMonkeyAuthorizationMethod","SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum","SourceSurveymonkeySurveymonkeyEnum","SourceTempo","SourceTempoTempoEnum","SourceTheGuardianAPI","SourceTheGuardianAPITheGuardianAPIEnum","SourceTiktokMarketing","SourceTiktokMarketingCredentialsOAuth20","SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum","SourceTiktokMarketingCredentialsSandboxAccessToken","SourceTiktokMarketingCredentialsSandboxAccessTokenAuthTypeEnum","SourceTiktokMarketingReportAggregationGranularityEnum","SourceTiktokMarketingTiktokMarketingEnum","SourceTodoist","SourceTodoistTodoistEnum","SourceTrello","SourceTrelloTrelloEnum","SourceTrustpilot","SourceTrustpilotCredentialsAPIKey","SourceTrustpilotCredentialsAPIKeyAuthTypeEnum","SourceTrustpilotCredentialsOAuth20","SourceTrustpilotCredentialsOAuth20AuthTypeEnum","SourceTrustpilotTrustpilotEnum","SourceTvmazeSchedule","SourceTvmazeScheduleTvmazeScheduleEnum","SourceTwilio","SourceTwilioTaskrouter","SourceTwilioTaskrouterTwilioTaskrouterEnum","SourceTwilioTwilioEnum","SourceTwitter","SourceTwitterTwitterEnum","SourceTypeform","SourceTypeformTypeformEnum","SourceUsCensus","SourceUsCensusUsCensusEnum","SourceVantage","SourceVantageVantageEnum","SourceWebflow","SourceWebflowWebflowEnum","SourceWhiskyHunter","SourceWhiskyHunterWhiskyHunterEnum","SourceWikipediaPageviews","SourceWikipediaPageviewsWikipediaPageviewsEnum","SourceWoocommerce","SourceWoocommerceWoocommerceEnum","SourceXero","SourceXeroAuthenticateViaXeroOAuth","SourceXeroXeroEnum","SourceXkcd","SourceXkcdXkcdEnum","SourceYandexMetrica","SourceYandexMetricaYandexMetricaEnum","SourceYounium","SourceYouniumYouniumEnum","SourceYoutubeAnalytics","SourceYoutubeAnalyticsYoutubeAnalyticsEnum","SourceZendeskChat","SourceZendeskChatCredentialsAccessToken","SourceZendeskChatCredentialsAccessTokenCredentialsEnum","SourceZendeskChatCredentialsOAuth20","SourceZendeskChatCredentialsOAuth20CredentialsEnum","SourceZendeskChatZendeskChatEnum","SourceZendeskSunshine","SourceZendeskSunshineCredentialsAPIToken","SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum","SourceZendeskSunshineCredentialsOAuth20","SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum","SourceZendeskSunshineZendeskSunshineEnum","SourceZendeskSupport","SourceZendeskSupportZendeskSupportEnum","SourceZendeskTalk","SourceZendeskTalkZendeskTalkEnum","SourceZenloop","SourceZenloopZenloopEnum","SourceZohoCRMZohoCRMEditionEnum","SourceZohoCrm","SourceZohoCrmDataCenterLocationEnum","SourceZohoCrmEnvironmentEnum","SourceZohoCrmZohoCrmEnum","SourceZoom","SourceZoomZoomEnum","SourceZuora","SourceZuoraZuoraEnum","SourcesResponse","WorkspaceCreateRequest","WorkspaceResponse","WorkspacesResponse"]
+__all__ = ["ConnectionCreateRequest","ConnectionCreateRequestNamespaceDefinitionEnum","ConnectionResponse","ConnectionScheduleCreate","ConnectionScheduleResponse","ConnectionStatusEnumEnum","ConnectionSyncModeEnumEnum","ConnectionsResponse","DestinationAmazonSqs","DestinationAmazonSqsAWSRegionEnum","DestinationAmazonSqsAmazonSqsEnum","DestinationAwsDatalake","DestinationAwsDatalakeAwsDatalakeEnum","DestinationAwsDatalakeChooseHowToPartitionDataEnum","DestinationAwsDatalakeCredentialsIAMRole","DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum","DestinationAwsDatalakeCredentialsIAMUser","DestinationAwsDatalakeCredentialsIAMUserCredentialsTitleEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSON","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONFormatTypeWildcardEnum","DestinationAwsDatalakeFormatParquetColumnarStorage","DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatParquetColumnarStorageFormatTypeWildcardEnum","DestinationAwsDatalakeS3BucketRegionEnum","DestinationAzureBlobStorage","DestinationAzureBlobStorageAzureBlobStorageEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValues","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationBigquery","DestinationBigqueryBigqueryEnum","DestinationBigqueryDatasetLocationEnum","DestinationBigqueryDenormalized","DestinationBigqueryDenormalizedBigqueryDenormalizedEnum","DestinationBigqueryDenormalizedDatasetLocationEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStaging","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum","DestinationBigqueryDenormalizedLoadingMethodStandardInserts","DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryLoadingMethodGCSStaging","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryLoadingMethodGCSStagingMethodEnum","DestinationBigqueryLoadingMethodStandardInserts","DestinationBigqueryLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryTransformationQueryRunTypeEnum","DestinationCassandra","DestinationCassandraCassandraEnum","DestinationClickhouse","DestinationClickhouseClickhouseEnum","DestinationClickhouseTunnelMethodNoTunnel","DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum","DestinationClickhouseTunnelMethodPasswordAuthentication","DestinationClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationClickhouseTunnelMethodSSHKeyAuthentication","DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationConvex","DestinationConvexConvexEnum","DestinationCreateRequest","DestinationDatabend","DestinationDatabendDatabendEnum","DestinationDatabricks","DestinationDatabricksDataSourceAmazonS3","DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum","DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum","DestinationDatabricksDataSourceAzureBlobStorage","DestinationDatabricksDataSourceAzureBlobStorageDataSourceTypeEnum","DestinationDatabricksDataSourceRecommendedManagedTables","DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum","DestinationDatabricksDatabricksEnum","DestinationDynamodb","DestinationDynamodbDynamoDBRegionEnum","DestinationDynamodbDynamodbEnum","DestinationElasticsearch","DestinationElasticsearchAuthenticationMethodAPIKeySecret","DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum","DestinationElasticsearchAuthenticationMethodUsernamePassword","DestinationElasticsearchAuthenticationMethodUsernamePasswordMethodEnum","DestinationElasticsearchElasticsearchEnum","DestinationFirebolt","DestinationFireboltFireboltEnum","DestinationFireboltLoadingMethodExternalTableViaS3","DestinationFireboltLoadingMethodExternalTableViaS3MethodEnum","DestinationFireboltLoadingMethodSQLInserts","DestinationFireboltLoadingMethodSQLInsertsMethodEnum","DestinationFirestore","DestinationFirestoreFirestoreEnum","DestinationGCSGCSBucketRegionEnum","DestinationGcs","DestinationGcsCredentialHMACKey","DestinationGcsCredentialHMACKeyCredentialTypeEnum","DestinationGcsFormatAvroApacheAvro","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflate","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompression","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappy","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecXz","DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandard","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationGcsFormatAvroApacheAvroFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValues","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIP","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSON","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationGcsFormatParquetColumnarStorage","DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum","DestinationGcsFormatParquetColumnarStorageFormatTypeEnum","DestinationGcsGcsEnum","DestinationGoogleSheets","DestinationGoogleSheetsAuthenticationViaGoogleOAuth","DestinationGoogleSheetsGoogleSheetsEnum","DestinationKeen","DestinationKeenKeenEnum","DestinationKinesis","DestinationKinesisKinesisEnum","DestinationMariadbColumnstore","DestinationMariadbColumnstoreMariadbColumnstoreEnum","DestinationMariadbColumnstoreTunnelMethodNoTunnel","DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodPasswordAuthentication","DestinationMariadbColumnstoreTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthentication","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMeilisearch","DestinationMeilisearchMeilisearchEnum","DestinationMongodb","DestinationMongodbAuthTypeLoginPassword","DestinationMongodbAuthTypeLoginPasswordAuthorizationEnum","DestinationMongodbAuthTypeNone","DestinationMongodbAuthTypeNoneAuthorizationEnum","DestinationMongodbInstanceTypeMongoDBAtlas","DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum","DestinationMongodbInstanceTypeReplicaSet","DestinationMongodbInstanceTypeReplicaSetInstanceEnum","DestinationMongodbInstanceTypeStandaloneMongoDbInstance","DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","DestinationMongodbMongodbEnum","DestinationMongodbTunnelMethodNoTunnel","DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum","DestinationMongodbTunnelMethodPasswordAuthentication","DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMongodbTunnelMethodSSHKeyAuthentication","DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMssql","DestinationMssqlMssqlEnum","DestinationMssqlSslMethodEncryptedTrustServerCertificate","DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","DestinationMssqlSslMethodEncryptedVerifyCertificate","DestinationMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","DestinationMssqlTunnelMethodNoTunnel","DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMssqlTunnelMethodPasswordAuthentication","DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMssqlTunnelMethodSSHKeyAuthentication","DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMysql","DestinationMysqlMysqlEnum","DestinationMysqlTunnelMethodNoTunnel","DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMysqlTunnelMethodPasswordAuthentication","DestinationMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMysqlTunnelMethodSSHKeyAuthentication","DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationOracle","DestinationOracleOracleEnum","DestinationOracleTunnelMethodNoTunnel","DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum","DestinationOracleTunnelMethodPasswordAuthentication","DestinationOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationOracleTunnelMethodSSHKeyAuthentication","DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPostgres","DestinationPostgresPostgresEnum","DestinationPostgresSslModeAllow","DestinationPostgresSslModeAllowModeEnum","DestinationPostgresSslModeDisable","DestinationPostgresSslModeDisableModeEnum","DestinationPostgresSslModePrefer","DestinationPostgresSslModePreferModeEnum","DestinationPostgresSslModeRequire","DestinationPostgresSslModeRequireModeEnum","DestinationPostgresSslModeVerifyCa","DestinationPostgresSslModeVerifyCaModeEnum","DestinationPostgresSslModeVerifyFull","DestinationPostgresSslModeVerifyFullModeEnum","DestinationPostgresTunnelMethodNoTunnel","DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum","DestinationPostgresTunnelMethodPasswordAuthentication","DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationPostgresTunnelMethodSSHKeyAuthentication","DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPubsub","DestinationPubsubPubsubEnum","DestinationPulsar","DestinationPulsarCompressionTypeEnum","DestinationPulsarPulsarEnum","DestinationPulsarTopicTypeEnum","DestinationRabbitmq","DestinationRabbitmqRabbitmqEnum","DestinationRedis","DestinationRedisCacheTypeEnum","DestinationRedisRedisEnum","DestinationRedisSslModeDisable","DestinationRedisSslModeDisableModeEnum","DestinationRedisSslModeVerifyFull","DestinationRedisSslModeVerifyFullModeEnum","DestinationRedisTunnelMethodNoTunnel","DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedisTunnelMethodPasswordAuthentication","DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedisTunnelMethodSSHKeyAuthentication","DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshift","DestinationRedshiftRedshiftEnum","DestinationRedshiftTunnelMethodNoTunnel","DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedshiftTunnelMethodPasswordAuthentication","DestinationRedshiftTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedshiftTunnelMethodSSHKeyAuthentication","DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshiftUploadingMethodS3Staging","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingMethodEnum","DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum","DestinationRedshiftUploadingMethodStandard","DestinationRedshiftUploadingMethodStandardMethodEnum","DestinationResponse","DestinationRockset","DestinationRocksetRocksetEnum","DestinationS3","DestinationS3FormatAvroApacheAvro","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecDeflate","DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompression","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecSnappy","DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecXz","DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecZstandard","DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationS3FormatAvroApacheAvroFormatTypeEnum","DestinationS3FormatCSVCommaSeparatedValues","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIP","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum","DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSON","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3FormatParquetColumnarStorage","DestinationS3FormatParquetColumnarStorageCompressionCodecEnum","DestinationS3FormatParquetColumnarStorageFormatTypeEnum","DestinationS3Glue","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3GlueS3BucketRegionEnum","DestinationS3GlueS3GlueEnum","DestinationS3GlueSerializationLibraryEnum","DestinationS3S3BucketRegionEnum","DestinationS3S3Enum","DestinationScylla","DestinationScyllaScyllaEnum","DestinationSftpJSON","DestinationSftpJSONSftpJSONEnum","DestinationSnowflake","DestinationSnowflakeCredentialsKeyPairAuthentication","DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum","DestinationSnowflakeCredentialsOAuth20","DestinationSnowflakeCredentialsOAuth20AuthTypeEnum","DestinationSnowflakeCredentialsUsernameAndPassword","DestinationSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","DestinationSnowflakeLoadingMethodAWSS3Staging","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum","DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum","DestinationSnowflakeLoadingMethodAzureBlobStorageStaging","DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging","DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodRecommendedInternalStaging","DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum","DestinationSnowflakeLoadingMethodSelectAnotherOption","DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum","DestinationSnowflakeSnowflakeEnum","DestinationTypesense","DestinationTypesenseTypesenseEnum","DestinationsResponse","GeographyEnumEnum","JobCreateRequest","JobResponse","JobStatusEnumEnum","JobTypeEnumEnum","JobsResponse","ScheduleTypeEnumEnum","ScheduleTypeWithBasicEnumEnum","Security","SourceAirtable","SourceAirtableAirtableEnum","SourceAirtableCredentialsOAuth20","SourceAirtableCredentialsOAuth20AuthMethodEnum","SourceAirtableCredentialsPersonalAccessToken","SourceAirtableCredentialsPersonalAccessTokenAuthMethodEnum","SourceAlloydb","SourceAlloydbAlloydbEnum","SourceAlloydbReplicationMethodStandard","SourceAlloydbReplicationMethodStandardMethodEnum","SourceAlloydbTunnelMethodNoTunnel","SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum","SourceAlloydbTunnelMethodPasswordAuthentication","SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceAlloydbTunnelMethodSSHKeyAuthentication","SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceAmazonAds","SourceAmazonAdsAmazonAdsEnum","SourceAmazonAdsAuthTypeEnum","SourceAmazonAdsRegionEnum","SourceAmazonAdsReportRecordTypesEnum","SourceAmazonAdsStateFilterEnum","SourceAmazonSellerPartner","SourceAmazonSellerPartnerAWSEnvironmentEnum","SourceAmazonSellerPartnerAWSRegionEnum","SourceAmazonSellerPartnerAmazonSellerPartnerEnum","SourceAmazonSellerPartnerAuthTypeEnum","SourceAmazonSqs","SourceAmazonSqsAWSRegionEnum","SourceAmazonSqsAmazonSqsEnum","SourceAmplitude","SourceAmplitudeAmplitudeEnum","SourceAmplitudeDataRegionEnum","SourceApifyDataset","SourceApifyDatasetApifyDatasetEnum","SourceAsana","SourceAsanaAsanaEnum","SourceAsanaCredentialsAuthenticateViaAsanaOauth","SourceAsanaCredentialsAuthenticateViaAsanaOauthCredentialsTitleEnum","SourceAsanaCredentialsAuthenticateWithPersonalAccessToken","SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum","SourceAuth0","SourceAuth0Auth0Enum","SourceAuth0CredentialsOAuth2AccessToken","SourceAuth0CredentialsOAuth2AccessTokenAuthenticationMethodEnum","SourceAuth0CredentialsOAuth2ConfidentialApplication","SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum","SourceAwsCloudtrail","SourceAwsCloudtrailAwsCloudtrailEnum","SourceAzureBlobStorage","SourceAzureBlobStorageAzureBlobStorageEnum","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","SourceAzureTable","SourceAzureTableAzureTableEnum","SourceBambooHr","SourceBambooHrBambooHrEnum","SourceBigcommerce","SourceBigcommerceBigcommerceEnum","SourceBigquery","SourceBigqueryBigqueryEnum","SourceBingAds","SourceBingAdsAuthMethodEnum","SourceBingAdsBingAdsEnum","SourceBraintree","SourceBraintreeBraintreeEnum","SourceBraintreeEnvironmentEnum","SourceBraze","SourceBrazeBrazeEnum","SourceChargebee","SourceChargebeeChargebeeEnum","SourceChargebeeProductCatalogEnum","SourceChartmogul","SourceChartmogulChartmogulEnum","SourceChartmogulIntervalEnum","SourceClickhouse","SourceClickhouseClickhouseEnum","SourceClickhouseTunnelMethodNoTunnel","SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum","SourceClickhouseTunnelMethodPasswordAuthentication","SourceClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceClickhouseTunnelMethodSSHKeyAuthentication","SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceClickupAPI","SourceClickupAPIClickupAPIEnum","SourceCloseCom","SourceCloseComCloseComEnum","SourceCoda","SourceCodaCodaEnum","SourceCoinAPI","SourceCoinAPICoinAPIEnum","SourceCoinAPIEnvironmentEnum","SourceCoinmarketcap","SourceCoinmarketcapCoinmarketcapEnum","SourceCoinmarketcapDataTypeEnum","SourceConfigcat","SourceConfigcatConfigcatEnum","SourceConfluence","SourceConfluenceConfluenceEnum","SourceCreateRequest","SourceDatascope","SourceDatascopeDatascopeEnum","SourceDelighted","SourceDelightedDelightedEnum","SourceDixa","SourceDixaDixaEnum","SourceDockerhub","SourceDockerhubDockerhubEnum","SourceDremio","SourceDremioDremioEnum","SourceDynamodb","SourceDynamodbDynamodbEnum","SourceDynamodbDynamodbRegionEnum","SourceE2eTestCloud","SourceE2eTestCloudE2eTestCloudEnum","SourceE2eTestCloudMockCatalogMultiSchema","SourceE2eTestCloudMockCatalogMultiSchemaTypeEnum","SourceE2eTestCloudMockCatalogSingleSchema","SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum","SourceE2eTestCloudTypeEnum","SourceEmailoctopus","SourceEmailoctopusEmailoctopusEnum","SourceExchangeRates","SourceExchangeRatesExchangeRatesEnum","SourceFacebookMarketing","SourceFacebookMarketingFacebookMarketingEnum","SourceFacebookMarketingInsightConfig","SourceFacebookMarketingInsightConfigLevelEnum","SourceFacebookMarketingInsightConfigValidActionBreakdownsEnum","SourceFacebookMarketingInsightConfigValidBreakdownsEnum","SourceFacebookMarketingInsightConfigValidEnumsEnum","SourceFacebookPages","SourceFacebookPagesFacebookPagesEnum","SourceFaker","SourceFakerFakerEnum","SourceFauna","SourceFaunaCollection","SourceFaunaCollectionDeletionsDisabled","SourceFaunaCollectionDeletionsDisabledDeletionModeEnum","SourceFaunaCollectionDeletionsEnabled","SourceFaunaCollectionDeletionsEnabledDeletionModeEnum","SourceFaunaFaunaEnum","SourceFileSecure","SourceFileSecureFileFormatEnum","SourceFileSecureFileSecureEnum","SourceFileSecureProviderAzBlobAzureBlobStorage","SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum","SourceFileSecureProviderGCSGoogleCloudStorage","SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum","SourceFileSecureProviderHTTPSPublicWeb","SourceFileSecureProviderHTTPSPublicWebStorageEnum","SourceFileSecureProviderS3AmazonWebServices","SourceFileSecureProviderS3AmazonWebServicesStorageEnum","SourceFileSecureProviderSCPSecureCopyProtocol","SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum","SourceFileSecureProviderSFTPSecureFileTransferProtocol","SourceFileSecureProviderSFTPSecureFileTransferProtocolStorageEnum","SourceFileSecureProviderSSHSecureShell","SourceFileSecureProviderSSHSecureShellStorageEnum","SourceFirebolt","SourceFireboltFireboltEnum","SourceFreshcaller","SourceFreshcallerFreshcallerEnum","SourceFreshdesk","SourceFreshdeskFreshdeskEnum","SourceFreshsales","SourceFreshsalesFreshsalesEnum","SourceGcs","SourceGcsGcsEnum","SourceGetlago","SourceGetlagoGetlagoEnum","SourceGithub","SourceGithubCredentialsOAuth","SourceGithubCredentialsOAuthOptionTitleEnum","SourceGithubCredentialsPersonalAccessToken","SourceGithubCredentialsPersonalAccessTokenOptionTitleEnum","SourceGithubGithubEnum","SourceGitlab","SourceGitlabCredentialsOAuth20","SourceGitlabCredentialsOAuth20AuthTypeEnum","SourceGitlabCredentialsPrivateToken","SourceGitlabCredentialsPrivateTokenAuthTypeEnum","SourceGitlabGitlabEnum","SourceGlassfrog","SourceGlassfrogGlassfrogEnum","SourceGnews","SourceGnewsCountryEnum","SourceGnewsGnewsEnum","SourceGnewsInEnum","SourceGnewsLanguageEnum","SourceGnewsNullableEnum","SourceGnewsSortByEnum","SourceGnewsTopHeadlinesTopicEnum","SourceGoogleAds","SourceGoogleAdsCustomQueries","SourceGoogleAdsGoogleAdsEnum","SourceGoogleAdsGoogleCredentials","SourceGoogleAnalyticsDataAPI","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum","SourceGoogleAnalyticsV4","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum","SourceGoogleDirectory","SourceGoogleDirectoryGoogleDirectoryEnum","SourceGoogleSearchConsole","SourceGoogleSearchConsoleAuthorizationOAuth","SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthentication","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSearchConsoleGoogleSearchConsoleEnum","SourceGoogleSheets","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuth","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum","SourceGoogleSheetsCredentialsServiceAccountKeyAuthentication","SourceGoogleSheetsCredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSheetsGoogleSheetsEnum","SourceGoogleWebfonts","SourceGoogleWebfontsGoogleWebfontsEnum","SourceGoogleWorkspaceAdminReports","SourceGoogleWorkspaceAdminReportsGoogleWorkspaceAdminReportsEnum","SourceGreenhouse","SourceGreenhouseGreenhouseEnum","SourceGridly","SourceGridlyGridlyEnum","SourceHarvest","SourceHarvestHarvestEnum","SourceHubplanner","SourceHubplannerHubplannerEnum","SourceHubspot","SourceHubspotCredentialsOAuth","SourceHubspotCredentialsOAuthCredentialsEnum","SourceHubspotCredentialsPrivateApp","SourceHubspotCredentialsPrivateAppCredentialsEnum","SourceHubspotHubspotEnum","SourceInsightly","SourceInsightlyInsightlyEnum","SourceInstagram","SourceInstagramInstagramEnum","SourceInstatus","SourceInstatusInstatusEnum","SourceIntercom","SourceIntercomIntercomEnum","SourceIp2whois","SourceIp2whoisIp2whoisEnum","SourceIterable","SourceIterableIterableEnum","SourceJira","SourceJiraJiraEnum","SourceK6Cloud","SourceK6CloudK6CloudEnum","SourceKlarna","SourceKlarnaKlarnaEnum","SourceKlarnaRegionEnum","SourceKlaviyo","SourceKlaviyoKlaviyoEnum","SourceKustomerSinger","SourceKustomerSingerKustomerSingerEnum","SourceLaunchdarkly","SourceLaunchdarklyLaunchdarklyEnum","SourceLemlist","SourceLemlistLemlistEnum","SourceLinkedinAds","SourceLinkedinAdsCredentialsAccessToken","SourceLinkedinAdsCredentialsAccessTokenAuthMethodEnum","SourceLinkedinAdsCredentialsOAuth20","SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum","SourceLinkedinAdsLinkedinAdsEnum","SourceLinkedinPages","SourceLinkedinPagesCredentialsAccessToken","SourceLinkedinPagesCredentialsAccessTokenAuthMethodEnum","SourceLinkedinPagesCredentialsOAuth20","SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum","SourceLinkedinPagesLinkedinPagesEnum","SourceLinnworks","SourceLinnworksLinnworksEnum","SourceLokalise","SourceLokaliseLokaliseEnum","SourceMailchimp","SourceMailchimpCredentialsAPIKey","SourceMailchimpCredentialsAPIKeyAuthTypeEnum","SourceMailchimpCredentialsOAuth20","SourceMailchimpCredentialsOAuth20AuthTypeEnum","SourceMailchimpMailchimpEnum","SourceMailgun","SourceMailgunMailgunEnum","SourceMailjetSms","SourceMailjetSmsMailjetSmsEnum","SourceMarketo","SourceMarketoMarketoEnum","SourceMetabase","SourceMetabaseMetabaseEnum","SourceMicrosoftTeams","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoft","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftAuthTypeEnum","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum","SourceMicrosoftTeamsMicrosoftTeamsEnum","SourceMixpanel","SourceMixpanelCredentialsProjectSecret","SourceMixpanelCredentialsProjectSecretOptionTitleEnum","SourceMixpanelCredentialsServiceAccount","SourceMixpanelCredentialsServiceAccountOptionTitleEnum","SourceMixpanelMixpanelEnum","SourceMixpanelRegionEnum","SourceMonday","SourceMondayCredentialsAPIToken","SourceMondayCredentialsAPITokenAuthTypeEnum","SourceMondayCredentialsOAuth20","SourceMondayCredentialsOAuth20AuthTypeEnum","SourceMondayMondayEnum","SourceMongodb","SourceMongodbInstanceTypeMongoDBAtlas","SourceMongodbInstanceTypeMongoDBAtlasInstanceEnum","SourceMongodbInstanceTypeReplicaSet","SourceMongodbInstanceTypeReplicaSetInstanceEnum","SourceMongodbInstanceTypeStandaloneMongoDbInstance","SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","SourceMongodbMongodbEnum","SourceMssql","SourceMssqlMssqlEnum","SourceMssqlReplicationMethodLogicalReplicationCDC","SourceMssqlReplicationMethodLogicalReplicationCDCDataToSyncEnum","SourceMssqlReplicationMethodLogicalReplicationCDCInitialSnapshotIsolationLevelEnum","SourceMssqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMssqlReplicationMethodStandard","SourceMssqlReplicationMethodStandardMethodEnum","SourceMssqlSslMethodEncryptedTrustServerCertificate","SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","SourceMssqlSslMethodEncryptedVerifyCertificate","SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","SourceMssqlTunnelMethodNoTunnel","SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMssqlTunnelMethodPasswordAuthentication","SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMssqlTunnelMethodSSHKeyAuthentication","SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceMyHours","SourceMyHoursMyHoursEnum","SourceMysql","SourceMysqlMysqlEnum","SourceMysqlReplicationMethodLogicalReplicationCDC","SourceMysqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMysqlReplicationMethodStandard","SourceMysqlReplicationMethodStandardMethodEnum","SourceMysqlSslModePreferred","SourceMysqlSslModePreferredModeEnum","SourceMysqlSslModeRequired","SourceMysqlSslModeRequiredModeEnum","SourceMysqlSslModeVerifyCA","SourceMysqlSslModeVerifyCAModeEnum","SourceMysqlSslModeVerifyIdentity","SourceMysqlSslModeVerifyIdentityModeEnum","SourceMysqlTunnelMethodNoTunnel","SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMysqlTunnelMethodPasswordAuthentication","SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMysqlTunnelMethodSSHKeyAuthentication","SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceNetsuite","SourceNetsuiteNetsuiteEnum","SourceNotion","SourceNotionCredentialsAccessToken","SourceNotionCredentialsAccessTokenAuthTypeEnum","SourceNotionCredentialsOAuth20","SourceNotionCredentialsOAuth20AuthTypeEnum","SourceNotionNotionEnum","SourceNytimes","SourceNytimesNytimesEnum","SourceNytimesPeriodUsedForMostPopularStreamsEnum","SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum","SourceOkta","SourceOktaCredentialsAPIToken","SourceOktaCredentialsAPITokenAuthTypeEnum","SourceOktaCredentialsOAuth20","SourceOktaCredentialsOAuth20AuthTypeEnum","SourceOktaOktaEnum","SourceOmnisend","SourceOmnisendOmnisendEnum","SourceOnesignal","SourceOnesignalApplications","SourceOnesignalOnesignalEnum","SourceOpenweather","SourceOpenweatherLanguageEnum","SourceOpenweatherOpenweatherEnum","SourceOpenweatherUnitsEnum","SourceOracle","SourceOracleConnectionDataServiceName","SourceOracleConnectionDataServiceNameConnectionTypeEnum","SourceOracleConnectionDataSystemIDSID","SourceOracleConnectionDataSystemIDSIDConnectionTypeEnum","SourceOracleEncryptionNativeNetworkEncryptionNNE","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionMethodEnum","SourceOracleEncryptionTLSEncryptedVerifyCertificate","SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum","SourceOracleOracleEnum","SourceOracleTunnelMethodNoTunnel","SourceOracleTunnelMethodNoTunnelTunnelMethodEnum","SourceOracleTunnelMethodPasswordAuthentication","SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceOracleTunnelMethodSSHKeyAuthentication","SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceOrb","SourceOrbOrbEnum","SourceOrbit","SourceOrbitOrbitEnum","SourceOutreach","SourceOutreachOutreachEnum","SourcePaypalTransaction","SourcePaypalTransactionPaypalTransactionEnum","SourcePaystack","SourcePaystackPaystackEnum","SourcePendo","SourcePendoPendoEnum","SourcePersistiq","SourcePersistiqPersistiqEnum","SourcePexelsAPI","SourcePexelsAPIPexelsAPIEnum","SourcePinterest","SourcePinterestCredentialsAccessToken","SourcePinterestCredentialsAccessTokenAuthMethodEnum","SourcePinterestCredentialsOAuth20","SourcePinterestCredentialsOAuth20AuthMethodEnum","SourcePinterestPinterestEnum","SourcePinterestStatusEnum","SourcePipedrive","SourcePipedriveAPIKeyAuthentication","SourcePipedriveAPIKeyAuthenticationAuthTypeEnum","SourcePipedrivePipedriveEnum","SourcePocket","SourcePocketContentTypeEnum","SourcePocketDetailTypeEnum","SourcePocketPocketEnum","SourcePocketSortByEnum","SourcePocketStateEnum","SourcePokeapi","SourcePokeapiPokeapiEnum","SourcePolygonStockAPI","SourcePolygonStockAPIPolygonStockAPIEnum","SourcePostgres","SourcePostgresPostgresEnum","SourcePostgresReplicationMethodStandard","SourcePostgresReplicationMethodStandardMethodEnum","SourcePostgresTunnelMethodNoTunnel","SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum","SourcePostgresTunnelMethodPasswordAuthentication","SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourcePostgresTunnelMethodSSHKeyAuthentication","SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourcePosthog","SourcePosthogPosthogEnum","SourcePostmarkapp","SourcePostmarkappPostmarkappEnum","SourcePrestashop","SourcePrestashopPrestashopEnum","SourcePublicApis","SourcePublicApisPublicApisEnum","SourcePunkAPI","SourcePunkAPIPunkAPIEnum","SourcePypi","SourcePypiPypiEnum","SourceQualaroo","SourceQualarooQualarooEnum","SourceQuickbooks","SourceQuickbooksCredentialsOAuth20","SourceQuickbooksCredentialsOAuth20AuthTypeEnum","SourceQuickbooksQuickbooksEnum","SourceRailz","SourceRailzRailzEnum","SourceRecharge","SourceRechargeRechargeEnum","SourceRecreation","SourceRecreationRecreationEnum","SourceRecruitee","SourceRecruiteeRecruiteeEnum","SourceRecurly","SourceRecurlyRecurlyEnum","SourceRedshift","SourceRedshiftRedshiftEnum","SourceResponse","SourceRetently","SourceRetentlyRetentlyEnum","SourceRkiCovid","SourceRkiCovidRkiCovidEnum","SourceRss","SourceRssRssEnum","SourceS3","SourceS3FormatAvro","SourceS3FormatAvroFiletypeEnum","SourceS3FormatCSV","SourceS3FormatCSVFiletypeEnum","SourceS3FormatJsonl","SourceS3FormatJsonlFiletypeEnum","SourceS3FormatJsonlUnexpectedFieldBehaviorEnum","SourceS3FormatParquet","SourceS3FormatParquetFiletypeEnum","SourceS3S3AmazonWebServices","SourceS3S3Enum","SourceSalesforce","SourceSalesforceAuthTypeEnum","SourceSalesforceSalesforceEnum","SourceSalesforceSinger","SourceSalesforceSingerAPITypeEnum","SourceSalesforceSingerSalesforceSingerEnum","SourceSalesforceStreamsCriteria","SourceSalesforceStreamsCriteriaSearchCriteriaEnum","SourceSalesloft","SourceSalesloftCredentialsAuthenticateViaAPIKey","SourceSalesloftCredentialsAuthenticateViaAPIKeyAuthTypeEnum","SourceSalesloftCredentialsAuthenticateViaOAuth","SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum","SourceSalesloftSalesloftEnum","SourceSapFieldglass","SourceSapFieldglassSapFieldglassEnum","SourceSecoda","SourceSecodaSecodaEnum","SourceSendgrid","SourceSendgridSendgridEnum","SourceSendinblue","SourceSendinblueSendinblueEnum","SourceSenseforce","SourceSenseforceSenseforceEnum","SourceSentry","SourceSentrySentryEnum","SourceSftp","SourceSftpBulk","SourceSftpBulkFileTypeEnum","SourceSftpBulkSftpBulkEnum","SourceSftpCredentialsPasswordAuthentication","SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum","SourceSftpCredentialsSSHKeyAuthentication","SourceSftpCredentialsSSHKeyAuthenticationAuthMethodEnum","SourceSftpSftpEnum","SourceShopify","SourceShopifyCredentialsAPIPassword","SourceShopifyCredentialsAPIPasswordAuthMethodEnum","SourceShopifyCredentialsOAuth20","SourceShopifyCredentialsOAuth20AuthMethodEnum","SourceShopifyShopifyEnum","SourceShortio","SourceShortioShortioEnum","SourceSlack","SourceSlackCredentialsAPIToken","SourceSlackCredentialsAPITokenOptionTitleEnum","SourceSlackCredentialsSignInViaSlackOAuth","SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum","SourceSlackSlackEnum","SourceSmaily","SourceSmailySmailyEnum","SourceSmartengage","SourceSmartengageSmartengageEnum","SourceSmartsheets","SourceSmartsheetsCredentialsAPIAccessToken","SourceSmartsheetsCredentialsAPIAccessTokenAuthTypeEnum","SourceSmartsheetsCredentialsOAuth20","SourceSmartsheetsCredentialsOAuth20AuthTypeEnum","SourceSmartsheetsSmartsheetsEnum","SourceSnapchatMarketing","SourceSnapchatMarketingSnapchatMarketingEnum","SourceSnowflake","SourceSnowflakeCredentialsOAuth20","SourceSnowflakeCredentialsOAuth20AuthTypeEnum","SourceSnowflakeCredentialsUsernameAndPassword","SourceSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","SourceSnowflakeSnowflakeEnum","SourceSonarCloud","SourceSonarCloudSonarCloudEnum","SourceSpacexAPI","SourceSpacexAPISpacexAPIEnum","SourceSquare","SourceSquareCredentialsAPIKey","SourceSquareCredentialsAPIKeyCredentialsTitleEnum","SourceSquareCredentialsOauthAuthentication","SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum","SourceSquareSquareEnum","SourceStrava","SourceStravaAuthTypeEnum","SourceStravaStravaEnum","SourceStripe","SourceStripeStripeEnum","SourceSurveySparrow","SourceSurveySparrowRegionEUBasedAccount","SourceSurveySparrowRegionEUBasedAccountURLBaseEnum","SourceSurveySparrowRegionGlobalAccount","SourceSurveySparrowRegionGlobalAccountURLBaseEnum","SourceSurveySparrowSurveySparrowEnum","SourceSurveymonkey","SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum","SourceSurveymonkeySurveyMonkeyAuthorizationMethod","SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum","SourceSurveymonkeySurveymonkeyEnum","SourceTempo","SourceTempoTempoEnum","SourceTheGuardianAPI","SourceTheGuardianAPITheGuardianAPIEnum","SourceTiktokMarketing","SourceTiktokMarketingCredentialsOAuth20","SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum","SourceTiktokMarketingCredentialsSandboxAccessToken","SourceTiktokMarketingCredentialsSandboxAccessTokenAuthTypeEnum","SourceTiktokMarketingTiktokMarketingEnum","SourceTodoist","SourceTodoistTodoistEnum","SourceTrello","SourceTrelloTrelloEnum","SourceTrustpilot","SourceTrustpilotCredentialsAPIKey","SourceTrustpilotCredentialsAPIKeyAuthTypeEnum","SourceTrustpilotCredentialsOAuth20","SourceTrustpilotCredentialsOAuth20AuthTypeEnum","SourceTrustpilotTrustpilotEnum","SourceTvmazeSchedule","SourceTvmazeScheduleTvmazeScheduleEnum","SourceTwilio","SourceTwilioTaskrouter","SourceTwilioTaskrouterTwilioTaskrouterEnum","SourceTwilioTwilioEnum","SourceTwitter","SourceTwitterTwitterEnum","SourceTypeform","SourceTypeformTypeformEnum","SourceUsCensus","SourceUsCensusUsCensusEnum","SourceVantage","SourceVantageVantageEnum","SourceWebflow","SourceWebflowWebflowEnum","SourceWhiskyHunter","SourceWhiskyHunterWhiskyHunterEnum","SourceWikipediaPageviews","SourceWikipediaPageviewsWikipediaPageviewsEnum","SourceWoocommerce","SourceWoocommerceWoocommerceEnum","SourceXero","SourceXeroAuthenticateViaXeroOAuth","SourceXeroXeroEnum","SourceXkcd","SourceXkcdXkcdEnum","SourceYandexMetrica","SourceYandexMetricaYandexMetricaEnum","SourceYounium","SourceYouniumYouniumEnum","SourceYoutubeAnalytics","SourceYoutubeAnalyticsYoutubeAnalyticsEnum","SourceZendeskChat","SourceZendeskChatCredentialsAccessToken","SourceZendeskChatCredentialsAccessTokenCredentialsEnum","SourceZendeskChatCredentialsOAuth20","SourceZendeskChatCredentialsOAuth20CredentialsEnum","SourceZendeskChatZendeskChatEnum","SourceZendeskSunshine","SourceZendeskSunshineCredentialsAPIToken","SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum","SourceZendeskSunshineCredentialsOAuth20","SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum","SourceZendeskSunshineZendeskSunshineEnum","SourceZendeskSupport","SourceZendeskSupportZendeskSupportEnum","SourceZendeskTalk","SourceZendeskTalkZendeskTalkEnum","SourceZenloop","SourceZenloopZenloopEnum","SourceZohoCRMZohoCRMEditionEnum","SourceZohoCrm","SourceZohoCrmDataCenterLocationEnum","SourceZohoCrmEnvironmentEnum","SourceZohoCrmZohoCrmEnum","SourceZoom","SourceZoomZoomEnum","SourceZuora","SourceZuoraZuoraEnum","SourcesResponse","StreamConfiguration","StreamConfigurations","StreamProperties","WorkspaceCreateRequest","WorkspaceResponse","WorkspacesResponse"]
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/connectioncreaterequest.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_sftp_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import connectionschedulecreate as shared_connectionschedulecreate
-from ..shared import geographyenum_enum as shared_geographyenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Optional
 
+class DestinationSftpJSONSftpJSONEnum(str, Enum):
+    SFTP_JSON = 'sftp-json'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ConnectionCreateRequest:
+class DestinationSftpJSON:
+    r"""The values required to configure the destination."""
     
-    destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})  
-    source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})  
-    geography: Optional[shared_geographyenum_enum.GeographyEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('geography'), 'exclude': lambda f: f is None }})  
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Optional name of the connection"""  
-    schedule: Optional[shared_connectionschedulecreate.ConnectionScheduleCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schedule'), 'exclude': lambda f: f is None }})
-    r"""schedule for when the the connection should run, per the schedule type"""  
+    destination_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination_path') }})
+    r"""Path to the directory where json files will be written."""  
+    destination_type: DestinationSftpJSONSftpJSONEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})  
+    host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
+    r"""Hostname of the SFTP server."""  
+    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
+    r"""Password associated with the username."""  
+    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
+    r"""Username to use to access the SFTP server."""  
+    port: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
+    r"""Port of the SFTP server."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/connectionresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/connectionresponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectionResponse:
     r"""Provides details of a single connection."""
     
     connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})  
+    data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})  
     destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})  
-    geography: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('geography') }})  
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
     schedule: shared_connectionscheduleresponse.ConnectionScheduleResponse = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schedule') }})
     r"""schedule for when the the connection should run, per the schedule type"""  
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})  
     status: shared_connectionstatusenum_enum.ConnectionStatusEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
     workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/connectionschedulecreate.py` & `airbyte-1.2.0/src/airbyte/models/shared/connectionschedulecreate.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/connectionscheduleresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/connectionscheduleresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/connectionsresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/connectionsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_amazon_sqs.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_aws_datalake.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_aws_datalake.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_azure_blob_storage.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_bigquery.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,37 @@
     ASIA_NORTHEAST3 = 'asia-northeast3'
     ASIA_SOUTH1 = 'asia-south1'
     ASIA_SOUTH2 = 'asia-south2'
     ASIA_SOUTHEAST1 = 'asia-southeast1'
     ASIA_SOUTHEAST2 = 'asia-southeast2'
     AUSTRALIA_SOUTHEAST1 = 'australia-southeast1'
     AUSTRALIA_SOUTHEAST2 = 'australia-southeast2'
+    EUROPE_CENTRAL1 = 'europe-central1'
     EUROPE_CENTRAL2 = 'europe-central2'
     EUROPE_NORTH1 = 'europe-north1'
+    EUROPE_SOUTHWEST1 = 'europe-southwest1'
     EUROPE_WEST1 = 'europe-west1'
     EUROPE_WEST2 = 'europe-west2'
     EUROPE_WEST3 = 'europe-west3'
     EUROPE_WEST4 = 'europe-west4'
     EUROPE_WEST6 = 'europe-west6'
+    EUROPE_WEST7 = 'europe-west7'
+    EUROPE_WEST8 = 'europe-west8'
+    EUROPE_WEST9 = 'europe-west9'
+    ME_WEST1 = 'me-west1'
     NORTHAMERICA_NORTHEAST1 = 'northamerica-northeast1'
     NORTHAMERICA_NORTHEAST2 = 'northamerica-northeast2'
     SOUTHAMERICA_EAST1 = 'southamerica-east1'
     SOUTHAMERICA_WEST1 = 'southamerica-west1'
     US_CENTRAL1 = 'us-central1'
     US_EAST1 = 'us-east1'
+    US_EAST2 = 'us-east2'
+    US_EAST3 = 'us-east3'
     US_EAST4 = 'us-east4'
+    US_EAST5 = 'us-east5'
     US_WEST1 = 'us-west1'
     US_WEST2 = 'us-west2'
     US_WEST3 = 'us-west3'
     US_WEST4 = 'us-west4'
 
 class DestinationBigqueryBigqueryEnum(str, Enum):
     BIGQUERY = 'bigquery'
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_bigquery_denormalized.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_bigquery_denormalized.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,37 @@
     ASIA_NORTHEAST3 = 'asia-northeast3'
     ASIA_SOUTH1 = 'asia-south1'
     ASIA_SOUTH2 = 'asia-south2'
     ASIA_SOUTHEAST1 = 'asia-southeast1'
     ASIA_SOUTHEAST2 = 'asia-southeast2'
     AUSTRALIA_SOUTHEAST1 = 'australia-southeast1'
     AUSTRALIA_SOUTHEAST2 = 'australia-southeast2'
+    EUROPE_CENTRAL1 = 'europe-central1'
     EUROPE_CENTRAL2 = 'europe-central2'
     EUROPE_NORTH1 = 'europe-north1'
+    EUROPE_SOUTHWEST1 = 'europe-southwest1'
     EUROPE_WEST1 = 'europe-west1'
     EUROPE_WEST2 = 'europe-west2'
     EUROPE_WEST3 = 'europe-west3'
     EUROPE_WEST4 = 'europe-west4'
     EUROPE_WEST6 = 'europe-west6'
+    EUROPE_WEST7 = 'europe-west7'
+    EUROPE_WEST8 = 'europe-west8'
+    EUROPE_WEST9 = 'europe-west9'
+    ME_WEST1 = 'me-west1'
     NORTHAMERICA_NORTHEAST1 = 'northamerica-northeast1'
     NORTHAMERICA_NORTHEAST2 = 'northamerica-northeast2'
     SOUTHAMERICA_EAST1 = 'southamerica-east1'
     SOUTHAMERICA_WEST1 = 'southamerica-west1'
     US_CENTRAL1 = 'us-central1'
     US_EAST1 = 'us-east1'
+    US_EAST2 = 'us-east2'
+    US_EAST3 = 'us-east3'
     US_EAST4 = 'us-east4'
+    US_EAST5 = 'us-east5'
     US_WEST1 = 'us-west1'
     US_WEST2 = 'us-west2'
     US_WEST3 = 'us-west3'
     US_WEST4 = 'us-west4'
 
 class DestinationBigqueryDenormalizedBigqueryDenormalizedEnum(str, Enum):
     BIGQUERY_DENORMALIZED = 'bigquery-denormalized'
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_cassandra.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_cassandra.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_clickhouse.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_convex.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_convex.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_databend.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_databend.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_databricks.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_databricks.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_dynamodb.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_elasticsearch.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_firebolt.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_firestore.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_firestore.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_gcs.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_google_sheets.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_keen.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_keen.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_kinesis.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_kinesis.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_mariadb_columnstore.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_mariadb_columnstore.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_meilisearch.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_meilisearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_mongodb.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_mssql.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_mysql.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_oracle.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_postgres.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_pubsub.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_pubsub.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_pulsar.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_pulsar.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_rabbitmq.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_redis.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_redis.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_redshift.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_rockset.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_rockset.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_s3.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_s3.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_s3_glue.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_s3_glue.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,28 +28,33 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
     compression_type: Optional[DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})  
     
+class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum(str, Enum):
+    r"""Whether the input json data should be normalized (flattened) in the output JSON Lines. Please refer to docs for details."""
+    NO_FLATTENING = 'No flattening'
+    ROOT_LEVEL_FLATTENING = 'Root level flattening'
+
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum(str, Enum):
     JSONL = 'JSONL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON:
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     
     format_type: DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})  
     compression: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression'), 'exclude': lambda f: f is None }})
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""  
-    flatten_data: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flatten_data'), 'exclude': lambda f: f is None }})
-    r"""If true data will be flattened and won't be nested in the _airbyte_data field"""  
+    flattening: Optional[DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flattening'), 'exclude': lambda f: f is None }})
+    r"""Whether the input json data should be normalized (flattened) in the output JSON Lines. Please refer to docs for details."""  
     
 class DestinationS3GlueSerializationLibraryEnum(str, Enum):
     r"""The library that your query engine will use for reading and writing data in your lake."""
     ORG_OPENX_DATA_JSONSERDE_JSON_SER_DE = 'org.openx.data.jsonserde.JsonSerDe'
     ORG_APACHE_HIVE_HCATALOG_DATA_JSON_SER_DE = 'org.apache.hive.hcatalog.data.JsonSerDe'
 
 class DestinationS3GlueS3BucketRegionEnum(str, Enum):
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_scylla.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_scylla.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_sftp_json.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_shortio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from typing import Optional
 
-class DestinationSftpJSONSftpJSONEnum(str, Enum):
-    SFTP_JSON = 'sftp-json'
+class SourceShortioShortioEnum(str, Enum):
+    SHORTIO = 'shortio'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DestinationSftpJSON:
-    r"""The values required to configure the destination."""
+class SourceShortio:
+    r"""The values required to configure the source."""
     
-    destination_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination_path') }})
-    r"""Path to the directory where json files will be written."""  
-    destination_type: DestinationSftpJSONSftpJSONEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})  
-    host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-    r"""Hostname of the SFTP server."""  
-    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-    r"""Password associated with the username."""  
-    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-    r"""Username to use to access the SFTP server."""  
-    port: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-    r"""Port of the SFTP server."""  
+    domain_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_id') }})  
+    secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
+    r"""Short.io Secret Key"""  
+    source_type: SourceShortioShortioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
+    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_snowflake.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destination_typesense.py` & `airbyte-1.2.0/src/airbyte/models/shared/destination_typesense.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destinationcreaterequest.py` & `airbyte-1.2.0/src/airbyte/models/shared/destinationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destinationresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/destinationresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/destinationsresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/destinationsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/jobcreaterequest.py` & `airbyte-1.2.0/src/airbyte/models/shared/jobcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/jobresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/jobresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/jobsresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/jobsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_airtable.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_airtable.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_alloydb.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_alloydb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_amazon_ads.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_amazon_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_amazon_seller_partner.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_amazon_seller_partner.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_amazon_sqs.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_amplitude.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_amplitude.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,14 @@
 from typing import Optional
 
 class SourceAmplitudeDataRegionEnum(str, Enum):
     r"""Amplitude data region server"""
     STANDARD_SERVER = 'Standard Server'
     EU_RESIDENCY_SERVER = 'EU Residency Server'
 
-class SourceAmplitudeEventStreamTimeIntervalEventsTimeIntervalSizeUnitEnum(str, Enum):
-    r"""Amplitude event stream's interval size unit"""
-    DAYS = 'days'
-    HOURS = 'hours'
-    WEEKS = 'weeks'
-    MONTHS = 'months'
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SourceAmplitudeEventStreamTimeInterval:
-    r"""Amplitude event stream time interval"""
-    
-    size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size') }})
-    r"""Amplitude event stream's interval size unit"""  
-    size_unit: SourceAmplitudeEventStreamTimeIntervalEventsTimeIntervalSizeUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size_unit') }})
-    r"""Amplitude event stream's interval size unit"""  
-    
 class SourceAmplitudeAmplitudeEnum(str, Enum):
     AMPLITUDE = 'amplitude'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAmplitude:
@@ -44,10 +26,10 @@
     secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
     r"""Amplitude Secret Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/amplitude#setup-guide\\">setup guide</a> for more information on how to obtain this key."""  
     source_type: SourceAmplitudeAmplitudeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
     r"""UTC date and time in the format 2021-01-25T00:00:00Z. Any data before this date will not be replicated."""  
     data_region: Optional[SourceAmplitudeDataRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_region'), 'exclude': lambda f: f is None }})
     r"""Amplitude data region server"""  
-    event_time_interval: Optional[SourceAmplitudeEventStreamTimeInterval] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_time_interval'), 'exclude': lambda f: f is None }})
-    r"""Amplitude event stream time interval"""  
+    request_time_range: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('request_time_range'), 'exclude': lambda f: f is None }})
+    r"""According to <a href=\\"https://www.docs.developers.amplitude.com/analytics/apis/export-api/#considerations\\">Considerations</a> too big time range in request can cause a timeout error. In this case, set shorter time interval in hours."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_apify_dataset.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_apify_dataset.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_asana.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_asana.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_auth0.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_auth0.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_aws_cloudtrail.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_aws_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_azure_table.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_azure_table.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_bamboo_hr.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_bamboo_hr.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_bigcommerce.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_bigcommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_bigquery.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_bing_ads.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_bing_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_braintree.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_braintree.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_braze.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_braze.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_chargebee.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_chargebee.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_chartmogul.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_chartmogul.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_clickhouse.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_clickup_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_clickup_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_close_com.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_close_com.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_coda.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_coda.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_coin_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_coin_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_coinmarketcap.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_configcat.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_configcat.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_confluence.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_confluence.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_datascope.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_datascope.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_delighted.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_delighted.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_dixa.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_dixa.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_dockerhub.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_dockerhub.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_dremio.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_dremio.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_dynamodb.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_e2e_test_cloud.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_e2e_test_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_emailoctopus.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_emailoctopus.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_exchange_rates.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_exchange_rates.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_facebook_marketing.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_facebook_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_facebook_pages.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_facebook_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_faker.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_faker.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_fauna.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_fauna.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_file_secure.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_file_secure.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_firebolt.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_freshcaller.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_freshcaller.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_freshdesk.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_freshdesk.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_freshsales.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_freshsales.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_gcs.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_getlago.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_getlago.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_github.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_github.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_gitlab.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_gitlab.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_glassfrog.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_glassfrog.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_gnews.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_gnews.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_ads.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_analytics_data_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_analytics_data_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_analytics_v4.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_analytics_v4.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_directory.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_directory.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_search_console.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_search_console.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_sheets.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_webfonts.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_webfonts.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_google_workspace_admin_reports.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_greenhouse.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_greenhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_gridly.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_gridly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_harvest.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_paypal_transaction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from typing import Any, Optional
+from typing import Optional
 
-class SourceHarvestHarvestEnum(str, Enum):
-    HARVEST = 'harvest'
+class SourcePaypalTransactionPaypalTransactionEnum(str, Enum):
+    PAYPAL_TRANSACTION = 'paypal-transaction'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceHarvest:
+class SourcePaypalTransaction:
     r"""The values required to configure the source."""
     
-    account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
-    r"""Harvest account ID. Required for all Harvest requests in pair with Personal Access Token"""  
-    replication_start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_start_date') }})
-    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""  
-    source_type: SourceHarvestHarvestEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-    r"""Choose how to authenticate to Harvest."""  
-    replication_end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_end_date'), 'exclude': lambda f: f is None }})
-    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data after this date will not be replicated."""  
+    is_sandbox: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox') }})
+    r"""Determines whether to use the sandbox or production environment."""  
+    source_type: SourcePaypalTransactionPaypalTransactionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
+    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    r"""Start Date for data extraction in <a href=\\"https://datatracker.ietf.org/doc/html/rfc3339#section-5.6\\">ISO format</a>. Date must be in range from 3 years till 12 hrs before present time."""  
+    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
+    r"""The Client ID of your Paypal developer application."""  
+    client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
+    r"""The Client Secret of your Paypal developer application."""  
+    refresh_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token'), 'exclude': lambda f: f is None }})
+    r"""The key to refresh the expired access token."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_hubplanner.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_hubplanner.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_hubspot.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_hubspot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 from typing import Any
 
 class SourceHubspotCredentialsPrivateAppCredentialsEnum(str, Enum):
     r"""Name of the credentials set"""
     PRIVATE_APP_CREDENTIALS = 'Private App Credentials'
 
 
@@ -49,10 +52,10 @@
 @dataclasses.dataclass
 class SourceHubspot:
     r"""The values required to configure the source."""
     
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
     r"""Choose how to authenticate to HubSpot."""  
     source_type: SourceHubspotHubspotEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_insightly.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_insightly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_instagram.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_instagram.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_instatus.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_instatus.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_intercom.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_intercom.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_ip2whois.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_ip2whois.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_iterable.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_iterable.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_jira.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_jira.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 @dataclasses.dataclass
 class SourceJira:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
     r"""Jira API Token. See the <a href=\\"https://docs.airbyte.com/integrations/sources/jira\\">docs</a> for more information on how to generate this key."""  
     domain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain') }})
-    r"""The Domain for your Jira account, e.g. airbyteio.atlassian.net"""  
+    r"""The Domain for your Jira account, e.g. airbyteio.atlassian.net, airbyteio.jira.com, jira.your-domain.com"""  
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
     r"""The user email for your Jira account."""  
     source_type: SourceJiraJiraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
     enable_experimental_streams: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('enable_experimental_streams'), 'exclude': lambda f: f is None }})
     r"""Allow the use of experimental streams which rely on undocumented Jira API endpoints. See https://docs.airbyte.com/integrations/sources/jira#experimental-tables for more info."""  
     expand_issue_changelog: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expand_issue_changelog'), 'exclude': lambda f: f is None }})
     r"""Expand the changelog when replicating issues."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_k6_cloud.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_k6_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_klarna.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_klarna.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_klaviyo.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_klaviyo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_kustomer_singer.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_kustomer_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_launchdarkly.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_launchdarkly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_lemlist.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_lemlist.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_linkedin_ads.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_linkedin_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_linkedin_pages.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_linkedin_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_linnworks.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_linnworks.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_lokalise.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_lokalise.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_mailchimp.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_mailchimp.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_mailgun.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_mailgun.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_mailjet_sms.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_mailjet_sms.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_marketo.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_marketo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 
 class SourceMarketoMarketoEnum(str, Enum):
     MARKETO = 'marketo'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
@@ -18,10 +21,10 @@
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
     r"""The Client ID of your Marketo developer application. See <a href=\\"https://docs.airbyte.com/integrations/sources/marketo\\"> the docs </a> for info on how to obtain this."""  
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
     r"""The Client Secret of your Marketo developer application. See <a href=\\"https://docs.airbyte.com/integrations/sources/marketo\\"> the docs </a> for info on how to obtain this."""  
     domain_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_url') }})
     r"""Your Marketo Base URL. See <a href=\\"https://docs.airbyte.com/integrations/sources/marketo\\"> the docs </a> for info on how to obtain this."""  
     source_type: SourceMarketoMarketoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_metabase.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_metabase.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_microsoft_teams.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_mixpanel.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_mixpanel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 from typing import Any, Optional
 
 class SourceMixpanelCredentialsProjectSecretOptionTitleEnum(str, Enum):
     PROJECT_SECRET = 'Project Secret'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -52,20 +55,20 @@
     source_type: SourceMixpanelMixpanelEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
     attribution_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attribution_window'), 'exclude': lambda f: f is None }})
     r"""A period of time for attributing results to ads and the lookback period after those actions occur during which ad results are counted. Default attribution window is 5 days."""  
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
     r"""Choose how to authenticate to Mixpanel"""  
     date_window_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date_window_size'), 'exclude': lambda f: f is None }})
     r"""Defines window size in days, that used to slice through data. You can reduce it, if amount of data in each window is too big for your environment."""  
-    end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
+    end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     r"""The date in the format YYYY-MM-DD. Any data after this date will not be replicated. Left empty to always sync to most recent date"""  
     project_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id'), 'exclude': lambda f: f is None }})
     r"""Your project ID number. See the <a href=\\"https://help.mixpanel.com/hc/en-us/articles/115004490503-Project-Settings#project-id\\">docs</a> for more information on how to obtain this."""  
     project_timezone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_timezone'), 'exclude': lambda f: f is None }})
     r"""Time zone in which integer date times are stored. The project timezone may be found in the project settings in the <a href=\\"https://help.mixpanel.com/hc/en-us/articles/115004547203-Manage-Timezones-for-Projects-in-Mixpanel\\">Mixpanel console</a>."""  
     region: Optional[SourceMixpanelRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
     r"""The region of mixpanel domain instance either US or EU."""  
     select_properties_by_default: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('select_properties_by_default'), 'exclude': lambda f: f is None }})
     r"""Setting this config parameter to TRUE ensures that new properties on events and engage records are captured. Otherwise new properties will be ignored."""  
-    start_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'exclude': lambda f: f is None }})
+    start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     r"""The date in the format YYYY-MM-DD. Any data before this date will not be replicated. If this option is not set, the connector will replicate data from up to one year ago by default."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_monday.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_monday.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_mongodb.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_mssql.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_my_hours.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_my_hours.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_mysql.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_netsuite.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_netsuite.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_notion.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_notion.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_nytimes.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_nytimes.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_okta.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_okta.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_omnisend.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_omnisend.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_onesignal.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_onesignal.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_openweather.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_openweather.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_oracle.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_orb.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_orb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_orbit.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_orbit.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_outreach.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_outreach.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_paypal_transaction.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_twilio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 from typing import Optional
 
-class SourcePaypalTransactionPaypalTransactionEnum(str, Enum):
-    PAYPAL_TRANSACTION = 'paypal-transaction'
+class SourceTwilioTwilioEnum(str, Enum):
+    TWILIO = 'twilio'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcePaypalTransaction:
+class SourceTwilio:
     r"""The values required to configure the source."""
     
-    is_sandbox: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox') }})
-    r"""Determines whether to use the sandbox or production environment."""  
-    source_type: SourcePaypalTransactionPaypalTransactionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-    r"""Start Date for data extraction in <a href=\\"https://datatracker.ietf.org/doc/html/rfc3339#section-5.6\\">ISO format</a>. Date must be in range from 3 years till 12 hrs before present time."""  
-    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-    r"""The Client ID of your Paypal developer application."""  
-    client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-    r"""The Client Secret of your Paypal developer application."""  
-    refresh_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token'), 'exclude': lambda f: f is None }})
-    r"""The key to refresh the expired access token."""  
+    account_sid: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_sid') }})
+    r"""Twilio account SID"""  
+    auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
+    r"""Twilio Auth Token."""  
+    source_type: SourceTwilioTwilioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""UTC date and time in the format 2020-10-01T00:00:00Z. Any data before this date will not be replicated."""  
+    lookback_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback_window'), 'exclude': lambda f: f is None }})
+    r"""How far into the past to look for records. (in minutes)"""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_paystack.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_paystack.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_pendo.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_pendo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_persistiq.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_persistiq.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_pexels_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_pexels_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_pinterest.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_pinterest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_pipedrive.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_pipedrive.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_pocket.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_pocket.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_pokeapi.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_pokeapi.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_polygon_stock_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_polygon_stock_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_postgres.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_posthog.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_posthog.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_postmarkapp.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_postmarkapp.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_prestashop.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_prestashop.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_public_apis.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_public_apis.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_punk_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_punk_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_pypi.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_pypi.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_qualaroo.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_qualaroo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_railz.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_railz.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_recharge.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_recharge.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_recreation.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_recreation.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_recruitee.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_recruitee.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_recurly.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_recurly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_redshift.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_retently.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_retently.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_rki_covid.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_rki_covid.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_rss.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_rss.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_s3.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_s3.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_salesforce.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_salesforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_salesforce_singer.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_salesforce_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_salesloft.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_salesloft.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_sap_fieldglass.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_sap_fieldglass.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_secoda.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_secoda.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_sendgrid.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_sendgrid.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_sendinblue.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_sendinblue.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_senseforce.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_senseforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_sentry.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_sentry.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_sftp.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_sftp.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_sftp_bulk.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_sftp_bulk.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_shopify.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_shopify.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_shortio.py` & `airbyte-1.2.0/src/airbyte/models/shared/sourcecreaterequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-
-class SourceShortioShortioEnum(str, Enum):
-    SHORTIO = 'shortio'
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceShortio:
-    r"""The values required to configure the source."""
+class SourceCreateRequest:
     
-    domain_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_id') }})  
-    secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
-    r"""Short.io Secret Key"""  
-    source_type: SourceShortioShortioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""  
+    configuration: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configuration') }})
+    r"""The values required to configure the source."""  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})  
+    secret_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secretId'), 'exclude': lambda f: f is None }})
+    r"""Optional secretID obtained through the public API OAuth redirect flow."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_slack.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_slack.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_smaily.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_smaily.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_smartengage.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_smartengage.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_smartsheets.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_smartsheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_snapchat_marketing.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_snapchat_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_snowflake.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_sonar_cloud.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_spacex_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_spacex_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_square.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_square.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_strava.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_strava.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_stripe.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_stripe.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_survey_sparrow.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_survey_sparrow.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_surveymonkey.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_surveymonkey.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_tempo.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_tempo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_the_guardian_api.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_the_guardian_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_tiktok_marketing.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_tiktok_marketing.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,32 +39,26 @@
     r"""The Developer Application App ID."""  
     secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret') }})
     r"""The Developer Application Secret."""  
     advertiser_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('advertiser_id'), 'exclude': lambda f: f is None }})
     r"""The Advertiser ID to filter reports and streams. Let this empty to retrieve all."""  
     auth_type: Optional[SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})  
     
-class SourceTiktokMarketingReportAggregationGranularityEnum(str, Enum):
-    r"""The granularity used for aggregating performance data in reports. See <a href=\\"https://docs.airbyte.com/integrations/sources/tiktok-marketing/#report-aggregation\\">the docs</a>."""
-    LIFETIME = 'LIFETIME'
-    DAY = 'DAY'
-    HOUR = 'HOUR'
-
 class SourceTiktokMarketingTiktokMarketingEnum(str, Enum):
     TIKTOK_MARKETING = 'tiktok-marketing'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTiktokMarketing:
     r"""The values required to configure the source."""
     
     source_type: SourceTiktokMarketingTiktokMarketingEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
+    attribution_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attribution_window'), 'exclude': lambda f: f is None }})
+    r"""The attribution window in days."""  
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
     r"""Authentication method"""  
     end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     r"""The date until which you'd like to replicate data for all incremental streams, in the format YYYY-MM-DD. All data generated between start_date and this date will be replicated. Not setting this option will result in always syncing the data till the current date."""  
-    report_granularity: Optional[SourceTiktokMarketingReportAggregationGranularityEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('report_granularity'), 'exclude': lambda f: f is None }})
-    r"""The granularity used for aggregating performance data in reports. See <a href=\\"https://docs.airbyte.com/integrations/sources/tiktok-marketing/#report-aggregation\\">the docs</a>."""  
     start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     r"""The Start Date in format: YYYY-MM-DD. Any data before this date will not be replicated. If this parameter is not set, all data will be replicated."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_todoist.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_todoist.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_trello.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_trello.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_trustpilot.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_trustpilot.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_tvmaze_schedule.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_tvmaze_schedule.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_twilio.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_younium.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
-class SourceTwilioTwilioEnum(str, Enum):
-    TWILIO = 'twilio'
+class SourceYouniumYouniumEnum(str, Enum):
+    YOUNIUM = 'younium'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceTwilio:
+class SourceYounium:
     r"""The values required to configure the source."""
     
-    account_sid: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_sid') }})
-    r"""Twilio account SID"""  
-    auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
-    r"""Twilio Auth Token."""  
-    source_type: SourceTwilioTwilioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""UTC date and time in the format 2020-10-01T00:00:00Z. Any data before this date will not be replicated."""  
-    lookback_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback_window'), 'exclude': lambda f: f is None }})
-    r"""How far into the past to look for records. (in minutes)"""  
+    legal_entity: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('legal_entity') }})
+    r"""Legal Entity that data should be pulled from"""  
+    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
+    r"""Account password for younium account API key"""  
+    source_type: SourceYouniumYouniumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
+    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
+    r"""Username for Younium account"""  
+    playground: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('playground'), 'exclude': lambda f: f is None }})
+    r"""Property defining if connector is used against playground or production environment"""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_twilio_taskrouter.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_twilio_taskrouter.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_twitter.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_twitter.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_typeform.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_typeform.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_us_census.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_us_census.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_vantage.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_vantage.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_webflow.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_webflow.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_whisky_hunter.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_whisky_hunter.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_wikipedia_pageviews.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_wikipedia_pageviews.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_woocommerce.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_woocommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_xero.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_xero.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_xkcd.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_xkcd.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_yandex_metrica.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_yandex_metrica.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_younium.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zuora.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class SourceYouniumYouniumEnum(str, Enum):
-    YOUNIUM = 'younium'
+class SourceZuoraZuoraEnum(str, Enum):
+    ZUORA = 'zuora'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceYounium:
+class SourceZuora:
     r"""The values required to configure the source."""
     
-    legal_entity: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('legal_entity') }})
-    r"""Legal Entity that data should be pulled from"""  
-    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-    r"""Account password for younium account API key"""  
-    source_type: SourceYouniumYouniumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-    r"""Username for Younium account"""  
-    playground: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('playground'), 'exclude': lambda f: f is None }})
-    r"""Property defining if connector is used against playground or production environment"""  
+    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
+    r"""Client ID"""  
+    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
+    r"""Client Secret"""  
+    source_type: SourceZuoraZuoraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
+    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    r"""Start Date in format: YYYY-MM-DD"""  
+    is_sandbox: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox'), 'exclude': lambda f: f is None }})
+    r"""Defines whether use the SANDBOX or PRODUCTION environment."""  
+    window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
+    r"""The amount of days for each data-chunk begining from start_date. Bigger the value - faster the fetch. (Min=1, as for a Day; Max=364, as for a Year)."""
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_youtube_analytics.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_youtube_analytics.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_chat.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_chat.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_sunshine.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_sunshine.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_support.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_support.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zendesk_talk.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zendesk_talk.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zenloop.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zenloop.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zoho_crm.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zoho_crm.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zoom.py` & `airbyte-1.2.0/src/airbyte/models/shared/source_zoom.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/source_zuora.py` & `airbyte-1.2.0/src/airbyte/models/shared/streamproperties.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import connectionsyncmodeenum_enum as shared_connectionsyncmodeenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Optional
 
-class SourceZuoraZuoraEnum(str, Enum):
-    ZUORA = 'zuora'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceZuora:
-    r"""The values required to configure the source."""
+class StreamProperties:
+    r"""The stream properties associated with a connection."""
     
-    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-    r"""Client ID"""  
-    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-    r"""Client Secret"""  
-    source_type: SourceZuoraZuoraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})  
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-    r"""Start Date in format: YYYY-MM-DD"""  
-    is_sandbox: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox'), 'exclude': lambda f: f is None }})
-    r"""Defines whether use the SANDBOX or PRODUCTION environment."""  
-    window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
-    r"""The amount of days for each data-chunk begining from start_date. Bigger the value - faster the fetch. (Min=1, as for a Day; Max=364, as for a Year)."""  
+    default_cursor_field: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultCursorField'), 'exclude': lambda f: f is None }})  
+    property_fields: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('propertyFields'), 'exclude': lambda f: f is None }})  
+    source_defined_cursor_field: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedCursorField'), 'exclude': lambda f: f is None }})  
+    source_defined_primary_key: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedPrimaryKey'), 'exclude': lambda f: f is None }})  
+    stream_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamName'), 'exclude': lambda f: f is None }})  
+    sync_modes: Optional[list[shared_connectionsyncmodeenum_enum.ConnectionSyncModeEnumEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncModes'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/sourcecreaterequest.py` & `airbyte-1.2.0/src/airbyte/models/shared/streamconfigurations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import streamconfiguration as shared_streamconfiguration
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceCreateRequest:
+class StreamConfigurations:
+    r"""A list of configured stream options for a connection."""
     
-    configuration: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configuration') }})
-    r"""The values required to configure the source."""  
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})  
-    secret_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secretId'), 'exclude': lambda f: f is None }})
-    r"""Optional secretID obtained through the public API OAuth redirect flow."""  
+    streams: Optional[list[shared_streamconfiguration.StreamConfiguration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streams'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/sourceresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/sourceresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/sourcesresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/sourcesresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/workspaceresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/workspaceresponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class WorkspaceResponse:
     r"""Provides details of a single workspace."""
     
-    default_geography: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultGeography') }})  
+    data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})  
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
     workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
```

### Comparing `airbyte-1.1.1/src/airbyte/models/shared/workspacesresponse.py` & `airbyte-1.2.0/src/airbyte/models/shared/workspacesresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/sdk.py` & `airbyte-1.2.0/src/airbyte/sdk.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 import requests as requests_http
 from . import utils
 from .connections import Connections
 from .destinations import Destinations
 from .jobs import Jobs
 from .sources import Sources
+from .streams import Streams
 from .workspaces import Workspaces
 from airbyte.models import shared
 
 SERVERS = [
     "https://api.airbyte.com/v1/",
     r"""Airbyte API v1"""
 ]
 """Contains the list of servers available to the SDK"""
 
 class Airbyte:
     connections: Connections
     destinations: Destinations
     jobs: Jobs
     sources: Sources
+    streams: Streams
     workspaces: Workspaces
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.1.1"
-    _gen_version: str = "2.17.9"
+    _sdk_version: str = "1.2.0"
+    _gen_version: str = "2.18.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
@@ -95,14 +97,23 @@
             self._client,
             self._security_client,
             self._server_url,
             self._language,
             self._sdk_version,
             self._gen_version
         )
+        
+        self.streams = Streams(
+            self._client,
+            self._security_client,
+            self._server_url,
+            self._language,
+            self._sdk_version,
+            self._gen_version
+        )
         
         self.workspaces = Workspaces(
             self._client,
             self._security_client,
             self._server_url,
             self._language,
             self._sdk_version,
```

### Comparing `airbyte-1.1.1/src/airbyte/sources.py` & `airbyte-1.2.0/src/airbyte/sources.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,31 @@
                 out = utils.unmarshal_json(http_res.text, Optional[shared.SourceResponse])
                 res.source_response = out
         elif http_res.status_code in [400, 403]:
             pass
 
         return res
 
+    def delete_source(self, request: operations.DeleteSourceRequest) -> operations.DeleteSourceResponse:
+        r"""Get Connection details"""
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.DeleteSourceRequest, base_url, '/sources/{sourceId}', request)
+        
+        
+        client = self._security_client
+        
+        http_res = client.request('DELETE', url)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.DeleteSourceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+
+        return res
+
     def get_source(self, request: operations.GetSourceRequest) -> operations.GetSourceResponse:
         r"""Get Source details"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSourceRequest, base_url, '/sources/{sourceId}', request)
```

### Comparing `airbyte-1.1.1/src/airbyte/utils/retries.py` & `airbyte-1.2.0/src/airbyte/utils/retries.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte/utils/utils.py` & `airbyte-1.2.0/src/airbyte/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,70 +148,79 @@
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
 
-        if param_metadata.get('style', 'simple') == 'simple':
-            param = getattr(
-                path_params, field.name) if path_params is not None else None
-            param = _populate_from_globals(
-                field.name, param, 'pathParam', gbls)
-
-            if param is None:
-                continue
-
-            if isinstance(param, list):
-                pp_vals: list[str] = []
-                for pp_val in param:
-                    if pp_val is None:
-                        continue
-                    pp_vals.append(_val_to_string(pp_val))
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif isinstance(param, dict):
-                pp_vals: list[str] = []
-                for pp_key in param:
-                    if param[pp_key] is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{pp_key}={_val_to_string(param[pp_key])}")
-                    else:
-                        pp_vals.append(
-                            f"{pp_key},{_val_to_string(param[pp_key])}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif not isinstance(param, (str, int, float, complex, bool)):
-                pp_vals: list[str] = []
-                param_fields: Tuple[Field, ...] = fields(param)
-                for param_field in param_fields:
-                    param_value_metadata = param_field.metadata.get(
-                        'path_param')
-                    if not param_value_metadata:
-                        continue
-
-                    parm_name = param_value_metadata.get(
-                        'field_name', field.name)
-
-                    param_field_val = getattr(param, param_field.name)
-                    if param_field_val is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{parm_name}={_val_to_string(param_field_val)}")
-                    else:
-                        pp_vals.append(
-                            f"{parm_name},{_val_to_string(param_field_val)}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            else:
+        param = getattr(
+            path_params, field.name) if path_params is not None else None
+        param = _populate_from_globals(
+            field.name, param, 'pathParam', gbls)
+
+        if param is None:
+            continue
+
+        f_name = param_metadata.get("field_name", field.name)
+        serialization = param_metadata.get('serialization', '')
+        if serialization != '':
+            serialized_params = _get_serialized_params(
+                param_metadata, f_name, param)
+            for key, value in serialized_params.items():
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + key + '}', value, 1)
+        else:
+            if param_metadata.get('style', 'simple') == 'simple':
+                if isinstance(param, list):
+                    pp_vals: list[str] = []
+                    for pp_val in param:
+                        if pp_val is None:
+                            continue
+                        pp_vals.append(_val_to_string(pp_val))
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif isinstance(param, dict):
+                    pp_vals: list[str] = []
+                    for pp_key in param:
+                        if param[pp_key] is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        else:
+                            pp_vals.append(
+                                f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif not isinstance(param, (str, int, float, complex, bool)):
+                    pp_vals: list[str] = []
+                    param_fields: Tuple[Field, ...] = fields(param)
+                    for param_field in param_fields:
+                        param_value_metadata = param_field.metadata.get(
+                            'path_param')
+                        if not param_value_metadata:
+                            continue
+
+                        parm_name = param_value_metadata.get(
+                            'field_name', field.name)
+
+                        param_field_val = getattr(param, param_field.name)
+                        if param_field_val is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{parm_name}={_val_to_string(param_field_val)}")
+                        else:
+                            pp_vals.append(
+                                f"{parm_name},{_val_to_string(param_field_val)}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                else:
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -242,16 +251,20 @@
             query_params, param_name) if query_params is not None else None
 
         value = _populate_from_globals(param_name, value, 'queryParam', gbls)
 
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            params = params | _get_serialized_query_params(
-                metadata, f_name, value)
+            serialized_parms = _get_serialized_params(metadata, f_name, value)
+            for key, value in serialized_parms.items():
+                if key in params:
+                    params[key].extend(value)
+                else:
+                    params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
                 params = params | _get_form_query_params(
@@ -278,16 +291,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    params: dict[str, list[str]] = {}
+def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
+    params: dict[str, str] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
```

### Comparing `airbyte-1.1.1/src/airbyte/workspaces.py` & `airbyte-1.2.0/src/airbyte/workspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.1.1/src/airbyte.egg-info/SOURCES.txt` & `airbyte-1.2.0/src/airbyte.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,45 +3,51 @@
 setup.py
 src/airbyte/__init__.py
 src/airbyte/connections.py
 src/airbyte/destinations.py
 src/airbyte/jobs.py
 src/airbyte/sdk.py
 src/airbyte/sources.py
+src/airbyte/streams.py
 src/airbyte/workspaces.py
 src/airbyte.egg-info/PKG-INFO
 src/airbyte.egg-info/SOURCES.txt
 src/airbyte.egg-info/dependency_links.txt
 src/airbyte.egg-info/requires.txt
 src/airbyte.egg-info/top_level.txt
 src/airbyte/models/__init__.py
 src/airbyte/models/operations/__init__.py
 src/airbyte/models/operations/canceljob.py
 src/airbyte/models/operations/createconnection.py
 src/airbyte/models/operations/createdestination.py
 src/airbyte/models/operations/createjob.py
 src/airbyte/models/operations/createsource.py
 src/airbyte/models/operations/createworkspace.py
+src/airbyte/models/operations/deleteconnection.py
+src/airbyte/models/operations/deletedestination.py
+src/airbyte/models/operations/deletesource.py
 src/airbyte/models/operations/getconnection.py
 src/airbyte/models/operations/getdestination.py
 src/airbyte/models/operations/getjob.py
 src/airbyte/models/operations/getsource.py
+src/airbyte/models/operations/getstreamproperties.py
 src/airbyte/models/operations/getworkspace.py
 src/airbyte/models/operations/listconnections.py
 src/airbyte/models/operations/listdestinations.py
 src/airbyte/models/operations/listjobs.py
 src/airbyte/models/operations/listsources.py
 src/airbyte/models/operations/listworkspaces.py
 src/airbyte/models/shared/__init__.py
 src/airbyte/models/shared/connectioncreaterequest.py
 src/airbyte/models/shared/connectionresponse.py
 src/airbyte/models/shared/connectionschedulecreate.py
 src/airbyte/models/shared/connectionscheduleresponse.py
 src/airbyte/models/shared/connectionsresponse.py
 src/airbyte/models/shared/connectionstatusenum_enum.py
+src/airbyte/models/shared/connectionsyncmodeenum_enum.py
 src/airbyte/models/shared/destination_amazon_sqs.py
 src/airbyte/models/shared/destination_aws_datalake.py
 src/airbyte/models/shared/destination_azure_blob_storage.py
 src/airbyte/models/shared/destination_bigquery.py
 src/airbyte/models/shared/destination_bigquery_denormalized.py
 src/airbyte/models/shared/destination_cassandra.py
 src/airbyte/models/shared/destination_clickhouse.py
@@ -93,14 +99,15 @@
 src/airbyte/models/shared/source_amazon_seller_partner.py
 src/airbyte/models/shared/source_amazon_sqs.py
 src/airbyte/models/shared/source_amplitude.py
 src/airbyte/models/shared/source_apify_dataset.py
 src/airbyte/models/shared/source_asana.py
 src/airbyte/models/shared/source_auth0.py
 src/airbyte/models/shared/source_aws_cloudtrail.py
+src/airbyte/models/shared/source_azure_blob_storage.py
 src/airbyte/models/shared/source_azure_table.py
 src/airbyte/models/shared/source_bamboo_hr.py
 src/airbyte/models/shared/source_bigcommerce.py
 src/airbyte/models/shared/source_bigquery.py
 src/airbyte/models/shared/source_bing_ads.py
 src/airbyte/models/shared/source_braintree.py
 src/airbyte/models/shared/source_braze.py
@@ -205,14 +212,15 @@
 src/airbyte/models/shared/source_posthog.py
 src/airbyte/models/shared/source_postmarkapp.py
 src/airbyte/models/shared/source_prestashop.py
 src/airbyte/models/shared/source_public_apis.py
 src/airbyte/models/shared/source_punk_api.py
 src/airbyte/models/shared/source_pypi.py
 src/airbyte/models/shared/source_qualaroo.py
+src/airbyte/models/shared/source_quickbooks.py
 src/airbyte/models/shared/source_railz.py
 src/airbyte/models/shared/source_recharge.py
 src/airbyte/models/shared/source_recreation.py
 src/airbyte/models/shared/source_recruitee.py
 src/airbyte/models/shared/source_recurly.py
 src/airbyte/models/shared/source_redshift.py
 src/airbyte/models/shared/source_retently.py
@@ -274,13 +282,16 @@
 src/airbyte/models/shared/source_zenloop.py
 src/airbyte/models/shared/source_zoho_crm.py
 src/airbyte/models/shared/source_zoom.py
 src/airbyte/models/shared/source_zuora.py
 src/airbyte/models/shared/sourcecreaterequest.py
 src/airbyte/models/shared/sourceresponse.py
 src/airbyte/models/shared/sourcesresponse.py
+src/airbyte/models/shared/streamconfiguration.py
+src/airbyte/models/shared/streamconfigurations.py
+src/airbyte/models/shared/streamproperties.py
 src/airbyte/models/shared/workspacecreaterequest.py
 src/airbyte/models/shared/workspaceresponse.py
 src/airbyte/models/shared/workspacesresponse.py
 src/airbyte/utils/__init__.py
 src/airbyte/utils/retries.py
 src/airbyte/utils/utils.py
```

