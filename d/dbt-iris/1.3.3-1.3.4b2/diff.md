# Comparing `tmp/dbt-iris-1.3.3.tar.gz` & `tmp/dbt-iris-1.3.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-iris-1.3.3.tar", last modified: Fri Apr 14 14:40:42 2023, max compression
+gzip compressed data, was "dbt-iris-1.3.4b2.tar", last modified: Fri Apr 14 15:56:21 2023, max compression
```

## Comparing `dbt-iris-1.3.3.tar` & `dbt-iris-1.3.4b2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.786319 dbt-iris-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 14:40:42.786319 dbt-iris-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.762318 dbt-iris-1.3.3/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.762318 dbt-iris-1.3.3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.766318 dbt-iris-1.3.3/dbt/adapters/iris/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/adapters/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/adapters/iris/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/adapters/iris/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/adapters/iris/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/adapters/iris/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/adapters/iris/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.762318 dbt-iris-1.3.3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.766318 dbt-iris-1.3.3/dbt/include/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.766318 dbt-iris-1.3.3/dbt/include/iris/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.766318 dbt-iris-1.3.3/dbt/include/iris/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/test/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/materializations/test/test.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt/include/iris/macros/models/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/models/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt/include/iris/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/dbt/include/iris/profile_iris.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.770318 dbt-iris-1.3.3/dbt_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/dbt_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/dbt_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/dbt_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/dbt_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/dbt_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.778318 dbt-iris-1.3.3/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.782318 dbt-iris-1.3.3/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    94963 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.782318 dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78588 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.786319 dbt-iris-1.3.3/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.786319 dbt-iris-1.3.3/iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/iris/iris_site.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/iris/irisbuiltins.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/iris/irisloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:40:42.786319 dbt-iris-1.3.3/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-14 14:40:42.000000 dbt-iris-1.3.3/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:40:42.786319 dbt-iris-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 14:40:26.000000 dbt-iris-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.424398 dbt-iris-1.3.4b2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-14 15:56:21.424398 dbt-iris-1.3.4b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.408397 dbt-iris-1.3.4b2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.408397 dbt-iris-1.3.4b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.412397 dbt-iris-1.3.4b2/dbt/adapters/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/adapters/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/adapters/iris/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/adapters/iris/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/adapters/iris/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/adapters/iris/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/adapters/iris/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.408397 dbt-iris-1.3.4b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.412397 dbt-iris-1.3.4b2/dbt/include/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.412397 dbt-iris-1.3.4b2/dbt/include/iris/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.412397 dbt-iris-1.3.4b2/dbt/include/iris/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.412397 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.412397 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.412397 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.416397 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.416397 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/test/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.416397 dbt-iris-1.3.4b2/dbt/include/iris/macros/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/models/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.416397 dbt-iris-1.3.4b2/dbt/include/iris/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/dbt/include/iris/profile_iris.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.416397 dbt-iris-1.3.4b2/dbt_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-14 15:56:21.000000 dbt-iris-1.3.4b2/dbt_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-14 15:56:21.000000 dbt-iris-1.3.4b2/dbt_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:56:21.000000 dbt-iris-1.3.4b2/dbt_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 15:56:21.000000 dbt-iris-1.3.4b2/dbt_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:56:21.000000 dbt-iris-1.3.4b2/dbt_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.420398 dbt-iris-1.3.4b2/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.420398 dbt-iris-1.3.4b2/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    94963 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.424398 dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78588 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.424398 dbt-iris-1.3.4b2/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.424398 dbt-iris-1.3.4b2/iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/iris/iris_site.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/iris/irisbuiltins.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/iris/irisloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:56:21.424398 dbt-iris-1.3.4b2/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-14 15:56:20.000000 dbt-iris-1.3.4b2/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:56:21.424398 dbt-iris-1.3.4b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-14 15:56:05.000000 dbt-iris-1.3.4b2/setup.py
```

### Comparing `dbt-iris-1.3.3/PKG-INFO` & `dbt-iris-1.3.4b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-iris
-Version: 1.3.3
+Version: 1.3.4b2
 Summary: The InterSystems IRIS adapter plugin for dbt
 Home-page: https://github.com/caretdev/dbt-iris
 Author: CaretDev
 Author-email: info@caretdev.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt-iris-1.3.3/README.md` & `dbt-iris-1.3.4b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/adapters/iris/__init__.py` & `dbt-iris-1.3.4b2/dbt/adapters/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/adapters/iris/column.py` & `dbt-iris-1.3.4b2/dbt/adapters/iris/column.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/adapters/iris/connections.py` & `dbt-iris-1.3.4b2/dbt/adapters/iris/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/adapters/iris/impl.py` & `dbt-iris-1.3.4b2/dbt/adapters/iris/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/adapters/iris/relation.py` & `dbt-iris-1.3.4b2/dbt/adapters/iris/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/adapters.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/catalog.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/helpers.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/materializations/incremental/incremental.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/materializations/seeds/helpers.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/helpers.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/materializations/snapshots/strategies.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/materializations/table.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/materializations/test/test.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt/include/iris/macros/models/merge.sql` & `dbt-iris-1.3.4b2/dbt/include/iris/macros/models/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/dbt_iris.egg-info/PKG-INFO` & `dbt-iris-1.3.4b2/dbt_iris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-iris
-Version: 1.3.3
+Version: 1.3.4b2
 Summary: The InterSystems IRIS adapter plugin for dbt
 Home-page: https://github.com/caretdev/dbt-iris
 Author: CaretDev
 Author-email: info@caretdev.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt-iris-1.3.3/dbt_iris.egg-info/SOURCES.txt` & `dbt-iris-1.3.4b2/dbt_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_BufferWriter.py` & `dbt-iris-1.3.4b2/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_ConnectionInformation.py` & `dbt-iris-1.3.4b2/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_ConnectionParameters.py` & `dbt-iris-1.3.4b2/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_Constant.py` & `dbt-iris-1.3.4b2/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_DBList.py` & `dbt-iris-1.3.4b2/intersystems_iris/_DBList.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_Device.py` & `dbt-iris-1.3.4b2/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_GatewayContext.py` & `dbt-iris-1.3.4b2/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_GatewayUtility.py` & `dbt-iris-1.3.4b2/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRIS.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISConnection.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISEmbedded.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISGlobalNode.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISGlobalNodeView.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISIterator.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISList.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISNative.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISObject.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_IRISReference.py` & `dbt-iris-1.3.4b2/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_InStream.py` & `dbt-iris-1.3.4b2/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_LegacyIterator.py` & `dbt-iris-1.3.4b2/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_ListReader.py` & `dbt-iris-1.3.4b2/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_ListWriter.py` & `dbt-iris-1.3.4b2/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_LogFileStream.py` & `dbt-iris-1.3.4b2/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_MessageHeader.py` & `dbt-iris-1.3.4b2/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_OutStream.py` & `dbt-iris-1.3.4b2/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_PrintStream.py` & `dbt-iris-1.3.4b2/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_PythonGateway.py` & `dbt-iris-1.3.4b2/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/_SharedMemorySocket.py` & `dbt-iris-1.3.4b2/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/__init__.py` & `dbt-iris-1.3.4b2/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_Column.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_DBAPI.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_DBAPI.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_Descriptor.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_IRISStream.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_Message.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_Parameter.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_ParameterCollection.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_ResultSetRow.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/_SQLType.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_PreParser.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_Scanner.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_Token.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/dbapi/preparser/_TokenList.py` & `dbt-iris-1.3.4b2/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_BusinessHost.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_BusinessOperation.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_BusinessProcess.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_BusinessService.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_Common.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_Director.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_IRISBusinessService.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_IRISOutboundAdapter.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_InboundAdapter.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/_OutboundAdapter.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/intersystems_iris/pex/__init__.py` & `dbt-iris-1.3.4b2/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/iris/__init__.py` & `dbt-iris-1.3.4b2/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/iris/irisbuiltins.py` & `dbt-iris-1.3.4b2/iris/irisbuiltins.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/iris/irisloader.py` & `dbt-iris-1.3.4b2/iris/irisloader.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/irisnative/_IRISNative.py` & `dbt-iris-1.3.4b2/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.3/setup.py` & `dbt-iris-1.3.4b2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup
 import os
 
 package_name = "dbt-iris"
-# make sure this always matches dbt/adapters/{adapter}/__version__.py
-package_version = "1.3.3"
+package_version = "1.3.4b2"
 description = """The InterSystems IRIS adapter plugin for dbt"""
 
 thelibFolder = os.path.dirname(os.path.realpath(__file__))
 requirementPath = thelibFolder + "/requirements.txt"
 
 requirements = []
 if os.path.isfile(requirementPath):
```

