# Comparing `tmp/dbt-iris-1.3.2b2.tar.gz` & `tmp/dbt-iris-1.3.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-iris-1.3.2b2.tar", last modified: Wed Feb  8 14:07:34 2023, max compression
+gzip compressed data, was "dbt-iris-1.3.2b3.tar", last modified: Fri Apr 14 14:31:25 2023, max compression
```

## Comparing `dbt-iris-1.3.2b2.tar` & `dbt-iris-1.3.2b3.tar`

### file list

```diff
@@ -1,132 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.078356 dbt-iris-1.3.2b2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-08 14:07:34.078356 dbt-iris-1.3.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.050356 dbt-iris-1.3.2b2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.050356 dbt-iris-1.3.2b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.058356 dbt-iris-1.3.2b2/dbt/adapters/iris/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/adapters/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/adapters/iris/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/adapters/iris/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/adapters/iris/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/adapters/iris/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/adapters/iris/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.054356 dbt-iris-1.3.2b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.058356 dbt-iris-1.3.2b2/dbt/include/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.058356 dbt-iris-1.3.2b2/dbt/include/iris/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.058356 dbt-iris-1.3.2b2/dbt/include/iris/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.058356 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.058356 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.058356 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.062356 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.062356 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/test/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/test/test.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.062356 dbt-iris-1.3.2b2/dbt/include/iris/macros/models/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/models/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.062356 dbt-iris-1.3.2b2/dbt/include/iris/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-08 14:07:13.000000 dbt-iris-1.3.2b2/dbt/include/iris/profile_iris.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.062356 dbt-iris-1.3.2b2/dbt_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/dbt_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-02-08 14:07:34.000000 dbt-iris-1.3.2b2/dbt_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/dbt_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/dbt_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/dbt_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.070356 dbt-iris-1.3.2b2/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20005 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      100 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       86 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3912 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1713 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.070356 dbt-iris-1.3.2b2/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    94357 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1437 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4233 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12186 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.070356 dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78424 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.074356 dbt-iris-1.3.2b2/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      325 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.074356 dbt-iris-1.3.2b2/intersystems_iris/sql/
--rw-rw-rw-   0 runner    (1001) docker     (123)      116 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/sql/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      225 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/sql/dataframe.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      474 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/intersystems_iris/sql/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.078356 dbt-iris-1.3.2b2/iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      815 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/iris/iris_site.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/iris/irisbuiltins.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/iris/irisloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:07:34.078356 dbt-iris-1.3.2b2/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-02-08 14:07:33.000000 dbt-iris-1.3.2b2/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 14:07:34.078356 dbt-iris-1.3.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-02-08 14:07:14.000000 dbt-iris-1.3.2b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.225136 dbt-iris-1.3.2b3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.225136 dbt-iris-1.3.2b3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/adapters/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/adapters/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/adapters/iris/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/adapters/iris/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/adapters/iris/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/adapters/iris/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/adapters/iris/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.225136 dbt-iris-1.3.2b3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/test/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/models/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt/include/iris/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 14:31:11.000000 dbt-iris-1.3.2b3/dbt/include/iris/profile_iris.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.229136 dbt-iris-1.3.2b3/dbt_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-14 14:31:25.000000 dbt-iris-1.3.2b3/dbt_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-14 14:31:25.000000 dbt-iris-1.3.2b3/dbt_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:31:25.000000 dbt-iris-1.3.2b3/dbt_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 14:31:25.000000 dbt-iris-1.3.2b3/dbt_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:31:25.000000 dbt-iris-1.3.2b3/dbt_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.233136 dbt-iris-1.3.2b3/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    94963 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78588 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/iris/iris_site.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/iris/irisbuiltins.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/iris/irisloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-14 14:31:24.000000 dbt-iris-1.3.2b3/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:31:25.237136 dbt-iris-1.3.2b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-14 14:31:12.000000 dbt-iris-1.3.2b3/setup.py
```

### Comparing `dbt-iris-1.3.2b2/PKG-INFO` & `dbt-iris-1.3.2b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-iris
-Version: 1.3.2b2
+Version: 1.3.2b3
 Summary: The InterSystems IRIS adapter plugin for dbt
 Home-page: https://github.com/caretdev/dbt-iris
 Author: CaretDev
 Author-email: info@caretdev.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt-iris-1.3.2b2/README.md` & `dbt-iris-1.3.2b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/adapters/iris/__init__.py` & `dbt-iris-1.3.2b3/dbt/adapters/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/adapters/iris/column.py` & `dbt-iris-1.3.2b3/dbt/adapters/iris/column.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/adapters/iris/connections.py` & `dbt-iris-1.3.2b3/dbt/adapters/iris/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,16 @@
 
         kwargs["hostname"] = credentials.hostname
         kwargs["port"] = credentials.port
         kwargs["namespace"] = credentials.database
         kwargs["username"] = credentials.username
         kwargs["password"] = credentials.password
 
+        kwargs["application_name"] = "dbt"
+
         try:
             connection.handle = dbapi.connect(**kwargs)
             connection.state = "open"
         except Exception as e:
             raise dbt.exceptions.FailedToConnectException(str(e))
 
         return connection
```

### Comparing `dbt-iris-1.3.2b2/dbt/adapters/iris/impl.py` & `dbt-iris-1.3.2b3/dbt/adapters/iris/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,43 +87,39 @@
                 return []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation}: {e.msg}")
                 return []
 
         relations = []
+        _database = schema_relation.database
         for row in results:
             if len(row) != 4:
                 raise RuntimeException(
                     "Invalid value from "
                     f'"iris__list_relations_without_caching({kwargs})", '
                     f"got {len(row)} values, expected 4"
                 )
             _, name, _schema, relation_type = row
-            relation = self.Relation.create(schema=_schema, identifier=name, type=relation_type)
+            relation = self.Relation.create(
+                database=_database, schema=_schema, identifier=name, type=relation_type
+            )
             relations.append(relation)
         return relations
 
     def get_rows_different_sql(
         self,
         relation_a: BaseRelation,
         relation_b: BaseRelation,
         column_names: Optional[List[str]] = None,
         except_operator: str = "EXCEPT",
     ) -> str:
         # TODO: IRIS does not support WITH and EXCEPT, no idea how to implement it, yet
         return "SELECT 0,0"
 
-    def get_relation(self, database: str, schema: str, identifier: str) -> Optional[IRISRelation]:  # type: ignore
-        if not self.Relation.include_policy.database:
-            database = None  # type: ignore
-
-        relation = super().get_relation(database, schema, identifier)
-        return relation
-
     def get_missing_columns(
         self, from_relation: IRISRelation, to_relation: IRISRelation
     ) -> List[IRISColumn]:
         """Returns a list of Columns in from_relation that are missing from
         to_relation.
         """
         if not isinstance(from_relation, self.Relation):
```

### Comparing `dbt-iris-1.3.2b2/dbt/adapters/iris/relation.py` & `dbt-iris-1.3.2b3/dbt/adapters/iris/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/adapters.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/catalog.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/helpers.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/incremental/incremental.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/seeds/helpers.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/helpers.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/snapshots/strategies.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/table.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/materializations/test/test.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt/include/iris/macros/models/merge.sql` & `dbt-iris-1.3.2b3/dbt/include/iris/macros/models/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/dbt_iris.egg-info/PKG-INFO` & `dbt-iris-1.3.2b3/dbt_iris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-iris
-Version: 1.3.2b2
+Version: 1.3.2b3
 Summary: The InterSystems IRIS adapter plugin for dbt
 Home-page: https://github.com/caretdev/dbt-iris
 Author: CaretDev
 Author-email: info@caretdev.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt-iris-1.3.2b2/dbt_iris.egg-info/SOURCES.txt` & `dbt-iris-1.3.2b3/dbt_iris.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,13 @@
 intersystems_iris/pex/_IRISBusinessService.py
 intersystems_iris/pex/_IRISInboundAdapter.py
 intersystems_iris/pex/_IRISOutboundAdapter.py
 intersystems_iris/pex/_InboundAdapter.py
 intersystems_iris/pex/_Message.py
 intersystems_iris/pex/_OutboundAdapter.py
 intersystems_iris/pex/__init__.py
-intersystems_iris/sql/__init__.py
-intersystems_iris/sql/dataframe.py
-intersystems_iris/sql/session.py
 iris/__init__.py
 iris/iris_site.py
 iris/irisbuiltins.py
 iris/irisloader.py
 irisnative/_IRISNative.py
 irisnative/__init__.py
```

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_BufferWriter.py` & `dbt-iris-1.3.2b3/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_ConnectionInformation.py` & `dbt-iris-1.3.2b3/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_ConnectionParameters.py` & `dbt-iris-1.3.2b3/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_Constant.py` & `dbt-iris-1.3.2b3/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_DBList.py` & `dbt-iris-1.3.2b3/intersystems_iris/_DBList.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
     def _grab_oref_unicode(cls, buffer, offset, length, *args):
         return intersystems_iris._IRISOREF._IRISOREF(cls._grab_unicode_string(buffer, offset, length))
 
     @classmethod
     def _set(cls, buffer, offset, data, locale, is_unicode, compact_double):
         func = cls._set_switcher.get(type(data), None)
         if func is None:
-            raise Exception("Unsupported argument type: " + str(type(data)))
+            # raise Exception("Unsupported argument type: " + str(type(data)))
+            return cls._stuff_str(buffer, offset, str(data), locale, is_unicode, compact_double)
         else:
             return func(buffer, offset, data, locale, is_unicode, compact_double)
 
     @classmethod
     def _set_undefined(cls, buffer, offset):
         buffer[offset] = 1
         return offset + 1
```

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_Device.py` & `dbt-iris-1.3.2b3/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_GatewayContext.py` & `dbt-iris-1.3.2b3/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_GatewayUtility.py` & `dbt-iris-1.3.2b3/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRIS.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISConnection.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISEmbedded.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISGlobalNode.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISGlobalNodeView.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISIterator.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISList.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISNative.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISObject.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_IRISReference.py` & `dbt-iris-1.3.2b3/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_InStream.py` & `dbt-iris-1.3.2b3/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_LegacyIterator.py` & `dbt-iris-1.3.2b3/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_ListReader.py` & `dbt-iris-1.3.2b3/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_ListWriter.py` & `dbt-iris-1.3.2b3/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_LogFileStream.py` & `dbt-iris-1.3.2b3/intersystems_iris/_LogFileStream.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import io
-import os
-import datetime
-import threading
-import platform
-
-class _LogFileStream(object):
-
-    LOG_RECEIVED = 0
-    LOG_SENT = 1
-    LINE_SEPARATOR = '\n'
-    BUFFER_SIZE = io.DEFAULT_BUFFER_SIZE
-
-    def __init__(self, path):
-        b_new_file = False
-        if (path.startswith("+")):
-            b_new_file = True
-            path = path[1:]
-        if (path.startswith("-")):
-            self.b_skip_logging = True
-            path = path[1:]
-        if b_new_file and os.path.exists(path):
-            os.remove(path)
-        self.path = path
-        self.bytesPerLine = 14 if os.path.splitext(path)[0].endswith("14") else 16
-        self.__dump_start()
-    
-    def __dump_start(self):
-        with open(self.path, 'a') as f:
-            f.write(
-                self.LINE_SEPARATOR 
-                + "=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-")
-            f.write(
-                self.LINE_SEPARATOR 
-                + "\tStarted At:     " + datetime.datetime.now().strftime("%b %d, %Y %I:%M:%S %p"))
-            f.write(
-                self.LINE_SEPARATOR 
-                + "\tPython Version: " + platform.python_version())
-            f.write(
-                self.LINE_SEPARATOR 
-                + "=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-" 
-                + self.LINE_SEPARATOR)
-
-    def __dump_info(self, type, connection):
-        if type == self.LOG_SENT:
-            type_text = "Sent"
-        else:
-            type_text = "Received"
-        with open(self.path, 'a') as f:
-            f.write(
-                self.LINE_SEPARATOR + type_text + ": (" 
-                + datetime.datetime.now().strftime("%H:%M:%S:%f")[:-3] + ")"
-                + " [ThreadID = " + str(threading.get_ident()) + " ]"
-                + " [JobNumber = " + str(connection._connection_info._server_job_number) + " ]"
-                + " [DeviceID = " + str(id(connection._device)) + " ]"
-                + self.LINE_SEPARATOR)
-
-    def _logApi(self, text):
-        with open(self.path, 'a') as f:
-            f.write(self.LINE_SEPARATOR + text + self.LINE_SEPARATOR)
-
-    def _dump_header(self, buffer, type, connection):
-        if buffer is None:
-            return
-        self.__dump_info(type, connection)
-        line = "Header:"
-        self._dump(line, buffer, False)
-
-    def _dump_message(self, buffer):
-        if buffer is None:
-            return
-        line = "Message:"
-        self._dump(line, buffer, True)
-
-    def _dump(self, line, buffer, is_message):
-        asciistr = ""
-        i = 0
-        f = open(self.path, 'a')
-        while i < len(buffer):
-            if i % self.bytesPerLine == 0:
-                if i != 0:
-                    line += "     "
-                line += asciistr + self.LINE_SEPARATOR
-                asciistr = ""
-                line += _LogFileStream.__format_offset(i)
-            x = '{:02X}'.format(int(buffer[i]))
-            asciistr += _LogFileStream.__convert_to_ascii(int(buffer[i]))
-            line += " " + x + " "
-            if i % _LogFileStream.BUFFER_SIZE == 0:
-                f.write(line)
-                line = ""
-            i += 1
-        line += self.__format_last_line(i)
-        line += "     " + asciistr + self.LINE_SEPARATOR
-        if is_message:
-            line += self.LINE_SEPARATOR
-        f.write(line)
-        f.close()
-
-    @staticmethod
-    def __format_offset(value):
-        return '  {:04X}: '.format(value)
-
-    @staticmethod
-    def __convert_to_ascii(value):
-        if value >= 32 and value < 127:
-            return chr(value)
-        return "."
-
-    def __format_last_line(self, count):
-        spaces = ""
-        while count % self.bytesPerLine != 0:
-            spaces += "    "
-            count += 1
-        return spaces
+import io
+import os
+import datetime
+import threading
+import platform
+
+class _LogFileStream(object):
+
+    LOG_RECEIVED = 0
+    LOG_SENT = 1
+    LINE_SEPARATOR = '\n'
+    BUFFER_SIZE = io.DEFAULT_BUFFER_SIZE
+
+    def __init__(self, path):
+        b_new_file = False
+        if (path.startswith("+")):
+            b_new_file = True
+            path = path[1:]
+        if (path.startswith("-")):
+            self.b_skip_logging = True
+            path = path[1:]
+        if b_new_file and os.path.exists(path):
+            os.remove(path)
+        self.path = path
+        self.bytesPerLine = 14 if os.path.splitext(path)[0].endswith("14") else 16
+        self.__dump_start()
+    
+    def __dump_start(self):
+        with open(self.path, 'a') as f:
+            f.write(
+                self.LINE_SEPARATOR 
+                + "=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-")
+            f.write(
+                self.LINE_SEPARATOR 
+                + "\tStarted At:     " + datetime.datetime.now().strftime("%b %d, %Y %I:%M:%S %p"))
+            f.write(
+                self.LINE_SEPARATOR 
+                + "\tPython Version: " + platform.python_version())
+            f.write(
+                self.LINE_SEPARATOR 
+                + "=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-" 
+                + self.LINE_SEPARATOR)
+
+    def __dump_info(self, type, connection):
+        if type == self.LOG_SENT:
+            type_text = "Sent"
+        else:
+            type_text = "Received"
+        with open(self.path, 'a') as f:
+            f.write(
+                self.LINE_SEPARATOR + type_text + ": (" 
+                + datetime.datetime.now().strftime("%H:%M:%S:%f")[:-3] + ")"
+                + " [ThreadID = " + str(threading.get_ident()) + " ]"
+                + " [JobNumber = " + str(connection._connection_info._server_job_number) + " ]"
+                + " [DeviceID = " + str(id(connection._device)) + " ]"
+                + self.LINE_SEPARATOR)
+
+    def _logApi(self, text):
+        with open(self.path, 'a') as f:
+            f.write(self.LINE_SEPARATOR + text + self.LINE_SEPARATOR)
+
+    def _dump_header(self, buffer, type, connection):
+        if buffer is None:
+            return
+        self.__dump_info(type, connection)
+        line = "Header:"
+        self._dump(line, buffer, False)
+
+    def _dump_message(self, buffer):
+        if buffer is None:
+            return
+        line = "Message:"
+        self._dump(line, buffer, True)
+
+    def _dump(self, line, buffer, is_message):
+        asciistr = ""
+        i = 0
+        f = open(self.path, 'a')
+        while i < len(buffer):
+            if i % self.bytesPerLine == 0:
+                if i != 0:
+                    line += "     "
+                line += asciistr + self.LINE_SEPARATOR
+                asciistr = ""
+                line += _LogFileStream.__format_offset(i)
+            x = '{:02X}'.format(int(buffer[i]))
+            asciistr += _LogFileStream.__convert_to_ascii(int(buffer[i]))
+            line += " " + x + " "
+            if i % _LogFileStream.BUFFER_SIZE == 0:
+                f.write(line)
+                line = ""
+            i += 1
+        line += self.__format_last_line(i)
+        line += "     " + asciistr + self.LINE_SEPARATOR
+        if is_message:
+            line += self.LINE_SEPARATOR
+        f.write(line)
+        f.close()
+
+    @staticmethod
+    def __format_offset(value):
+        return '  {:04X}: '.format(value)
+
+    @staticmethod
+    def __convert_to_ascii(value):
+        if value >= 32 and value < 127:
+            return chr(value)
+        return "."
+
+    def __format_last_line(self, count):
+        spaces = ""
+        while count % self.bytesPerLine != 0:
+            spaces += "    "
+            count += 1
+        return spaces
```

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_OutStream.py` & `dbt-iris-1.3.2b3/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_PrintStream.py` & `dbt-iris-1.3.2b3/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_PythonGateway.py` & `dbt-iris-1.3.2b3/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/_SharedMemorySocket.py` & `dbt-iris-1.3.2b3/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/__init__.py` & `dbt-iris-1.3.2b3/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_Column.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_DBAPI.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_DBAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 
 def embedded_connect(*args, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
     connection = _IRISEmbedded()
     connection.connect(hostname, port,  namespace, username, password, **kw)
     return connection
 
 def connect(*args, embedded=False, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
-    if not embedded:
-        return native_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
-    else:
-        return embedded_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
-
+    try:
+        if not embedded:
+            return native_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
+        else:
+            return embedded_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
+    except Exception as e:
+        raise DatabaseError(e)
 
 class ServerReturnType(enum.IntEnum):
     NO_RETURN_VALUE = 0
     IGNORE_RETURN_VALUE = 1
     HAS_RETURN_VALUE = 2
     NULL_RETURN_VALUE = 3
 
@@ -56,14 +58,17 @@
 paramstyle = "qmark"
 
 class _BaseCursor:
     embedded = False
     def __init__(self, connection):
         self._connection = connection
         
+        self.statement = None
+        self._parsed_statement = None
+        
         self._columns = None
         self._rowcount = -1
         self.arraysize = 1
 
         self._result_set = None
 
         self._rsrow = None
@@ -81,14 +86,15 @@
         self._mrs_done = False
         self._has_return_value = 0
         self._cursor_type = 0
         self._parameter_list_mismatch_exception = False
         self._fetch_done = False
         self._output_parameter_list = None
 
+        self._sqlcode = None
         self._lastrowid = None
 
         self._closed = False
 
     def __enter__(self):
         return self
 
@@ -112,14 +118,20 @@
         return self._closed 
 
     def setinputsizes(self, sizes):
         raise NotImplementedErrorDBAPI()
 
     def setoutputsize(size, column = None):
         raise NotImplementedErrorDBAPI()
+    
+    @property
+    def sqlcode(self):
+        if self._closed:
+            raise InterfaceError("Cursor is closed")
+        return 0 if self._sqlcode is None else self._sqlcode
 
     def close(self):
         if self._closed:
             return
         self._columns = None
         self._rowcount = -1
         self.arraysize = 0
@@ -177,15 +189,23 @@
         self._rowcount = -1
         self._exec_params = None
         self._statementType = StatementType.UPDATE
         self.statementFeatureOption = 0
         self.maxRowItemCount = 0
         self._is_batch_update = False
 
+    def _is_alive(self):
+        if self._closed:
+            raise InterfaceError("Cursor is closed")
+        if self._connection == None or self._connection.isClosed():
+            raise InterfaceError("Connection not open")
+
     def direct_execute(self, operation, *params):
+        self._is_alive()
+
         self.statement = operation
         if len(params) == 1 and (isinstance(params[0], tuple) or isinstance(params[0], list)):
             self.params = params[0]
         else:
             self.params = params
         self._params.set_input_params(self.params)
 
@@ -193,14 +213,16 @@
         self._cleanup()
         self._preparse()
 
         self._execute()
         return self._rowcount
 
     def execute(self, operation, params=()):
+        self._is_alive()
+
         self.statement = operation
         if params and not isinstance(params, list) and not isinstance(params, tuple):
             params = (params, )
         self.params = params if params is not None else ()
         self._params.set_input_params(self.params)
 
         self._cleanup()
@@ -212,16 +234,15 @@
         else:
             self._cursor_type = CursorType.DEFAULT
 
         self._execute()
         return self._rowcount
 
     def add_batch(self):
-        if self._closed:
-            raise InterfaceError("Cursor is closed")
+        self._is_alive()
         
         if self._params._array_bound:
             if len(self._params._params_list) > 0:
                 cnt = 0
                 first = True
                 for i in range(self._params._user_parameters_size):
                     i = i + 1
@@ -242,19 +263,19 @@
                 if len(param._values) != self._parameter_sets:
                     if self._parameter_sets != 1:
                         if len(param._values) + 1 == self._parameter_sets:
                             param._values.append(param._values[len(param._values) - 1])
                             continue
 
     def executemany(self, operation, seq_of_params):
+        self._is_alive()
         self._rowcount = 0
-        if self._closed:
-            raise InterfaceError("Cursor is closed")
-        if self._connection == None or self._connection.isClosed():
-            raise InterfaceError("Connection not open")
+
+        if not isinstance(seq_of_params, tuple) and not isinstance(seq_of_params, list):
+            seq_of_params = tuple(seq_of_params)
 
         self.statement = operation
         self.params = seq_of_params
         self._params.set_input_params(self.params)
 
         self._cursor_type = CursorType.PREPARED
         self._cleanup()
@@ -278,14 +299,22 @@
             if mode == ParameterMode.INPUT_OUTPUT or mode == ParameterMode.OUTPUT:
                 raise ValueError("INOUT/OUT parameters not permitted")
 
         self._prepared_update_execute()
 
         return self._rowcount
 
+    def _process_sqlcode(self, sqlcode, message=None):
+        self._sqlcode = sqlcode
+        if sqlcode in [0, 100]:
+            return
+        if abs(sqlcode) in [108, 119, 121, 122]:
+            raise IntegrityError(message)
+        raise DatabaseError(message)
+
     def _preparse(self):
         csql = self._connection._pre_preparse_cache.get(self.statement)
         if csql != None:
             self._has_return_value = csql._has_return_value
             self._params = copy.deepcopy(csql._params)
             self._params.set_input_params(self.params)
             self._parsed_statement = csql._parsed_statement
@@ -298,15 +327,16 @@
             if isinstance(item, list) or isinstance(item, tuple):
                 if not self._is_batch_update:
                     raise TypeError("Unsupported argument type: " + str(type(item)))
                 for ele in item:
                     if intersystems_iris._DBList._DBList._set_switcher.get(type(ele), None) == None:
                         raise TypeError("Unsupported argument type: " + str(type(ele)))
             elif intersystems_iris._DBList._DBList._set_switcher.get(type(item), None) is None:
-                raise TypeError("Unsupported argument type: " + str(type(item)))
+                item = str(item)
+                # raise TypeError("Unsupported argument type: " + str(type(item)))
             if i == 0:
                 count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
             else:
                 curr_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
                 if count != curr_count:
                     raise Exception("Parameter count does not match")
 
@@ -357,15 +387,15 @@
                 elif item == '?':
                     unknown_count = unknown_count + 1
 
             if len(self.params) > 0:
                 item = self.params[0]
                 param_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else len(self.params)
                 if param_count != unknown_count:
-                    raise Exception("Parameter mismatch")
+                    raise Exception(f"Parameter mismatch: {param_count}/{unknown_count}")
         else:
             if self._cursor_type == CursorType.CALLABLE:
                 i = 0
                 for param in self._params._params_list:
                     if param.mode == ParameterMode.RETURN_VALUE:
                         continue
                     else:
@@ -388,15 +418,15 @@
                 for item in temp_list_data:
                     if item == 'c':
                         replaced_count = replaced_count + 1
                     elif item == '?':
                         unknown_count = unknown_count + 1
 
                 if unknown_count != len(self.params):
-                    raise Exception("Incorrect number of parameters")
+                    raise Exception(f"Incorrect number of parameters: {unknown_count}/{replaced_count}/{len(self.params)}")
 
     def _is_not_default_or_replaced(self, param):
         mode = param.mode
         if mode != ParameterMode.REPLACED_LITERAL and mode != ParameterMode.DEFAULT_PARAMETER and mode != ParameterMode.INPUT:
             raise Exception("Parameters not allowed in Cursor class")
 
     def _validate_parameters(self):
@@ -426,14 +456,15 @@
             raise InterfaceError("Cursor is closed")
         if self._connection == None or self._connection.isClosed():
             raise InterfaceError("Connection not open")
 
         exec_switcher = {
             StatementType.QUERY: self._execute_query,
             StatementType.CALL: self._execute_update,
+            StatementType.STMT_USE: self._execute_update,
             StatementType.UPDATE: self._execute_update,
             StatementType.DDL_OTHER: self._execute_update,
             StatementType.DDL_ALTER_DROP: self._execute_update
         }
         exec_func = exec_switcher.get(self._statementType, None)
         if exec_func is None:
             raise NotImplementedErrorDBAPI(f'StatementType {self._statementType.name} not implemented')
@@ -636,14 +667,19 @@
         self._fetch_done = False
         self._output_parameter_list = None
 
         self._lastrowid = None
 
         self._closed = False
 
+    def _process_sqlcode(self, sqlcode, message=None):
+        if sqlcode in [0, 100]:
+            return
+        super()._process_sqlcode(sqlcode, self._get_error_info(sqlcode))
+
     def _get_cached_info(self):
         if not self._connection._preparedCache or not hasattr(self._connection._preparedCache, '__iter__'):
             return False
         if self._parsed_statement in self._connection._preparedCache:
             self._prepare_cached(self._connection._preparedCache[self._parsed_statement])
             return True
         else:
@@ -723,15 +759,15 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
             sqlcode = self._in_message.wire.header._get_function_code()
             if sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(sqlcode))
+                raise DatabaseError(self._get_error_info(sqlcode))
 
         # process metadata
         try:
             if self._connection._isFastOption():
                 self._check_statement_feature(self._in_message.wire)
             else:
                 self.statementFeatureOption = Feature.optionNone
@@ -903,16 +939,15 @@
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [404, 100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
             self._handle_error_504(self._sqlcode)
             if self._sqlcode == 404:
                 return
-            if self._sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            self._process_sqlcode(self._sqlcode)
 
         self._current_wire = self._in_message.wire
         self._result_set = [self._current_wire]
         self._rs_index = 0
         
         self._rowcount = -1
 
@@ -937,15 +972,15 @@
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve metadata
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 sqlcode = self._in_message.wire.header._get_function_code()
                 if sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(sqlcode))
+                    raise DatabaseError(self._get_error_info(sqlcode))
 
                 self._process_stored_procedure_metadata(self._in_message.wire, True)
                 if self._multiple_result_sets:
                     # todo
                     return
 
                 self._cache_prepared_statement()
@@ -986,30 +1021,29 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve metadata
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 sqlcode = self._in_message.wire.header._get_function_code()
-                if sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(sqlcode))
+                self._process_sqlcode(sqlcode)
 
                 if self._connection._isFastOption():
                     self._check_statement_feature(self._in_message.wire)
                 else:
                     self.statementFeatureOption = Feature.optionNone
                 self._get_column_info(self._in_message.wire)
                 self._get_parameter_info(self._in_message.wire)
                 self._cache_prepared_statement()
 
                 # retrieve data
                 self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
                 if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))
+                    raise DatabaseError(self._get_error_info(self._sqlcode))
 
             except IndexError:
                 raise DatabaseError("Server response message terminated prematurely")
             except TypeError:
                 raise DatabaseError("Unexpected server response message format")
 
         self._current_wire = self._in_message.wire
@@ -1037,22 +1071,19 @@
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [404, 100])
-            sqlcode = self._in_message.wire.header._get_function_code()
-            if sqlcode == 404:
+            self._sqlcode = self._in_message.wire.header._get_function_code()
+            if self._sqlcode == 404:
                 self._update404()
                 return
-            if sqlcode == 119:
-                raise IntegrityError(self._get_error_info(sqlcode))
-            if sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(sqlcode))
+            self._process_sqlcode(self._sqlcode)
 
     def _send_direct_update_request(self):
         # send DU message
         with self._connection._lock:
             self._statement_id = self._connection._get_new_statement_id()
             # message header
             self._out_message.wire._write_header(_Message.DIRECT_UPDATE)
@@ -1070,17 +1101,16 @@
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve response
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
-                sqlcode = self._in_message.wire.header._get_function_code()
-                if sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(sqlcode))
+                self._sqlcode = self._in_message.wire.header._get_function_code()
+                self._process_sqlcode(self._sqlcode)
 
                 addToCache = self._get_parameter_info(self._in_message.wire)
                 
                 notDDL = bool(self._statementType != StatementType.DDL_ALTER_DROP 
                                   and self._statementType != StatementType.DDL_OTHER)
                 if notDDL and addToCache:
                     self._cache_prepared_statement()
@@ -1104,16 +1134,15 @@
             # send message
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
             sqlcode = self._in_message.wire.header._get_function_code()
-            if sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(sqlcode))
+            self._process_sqlcode(sqlcode)
 
             self._process_stored_procedure_metadata(self._in_message.wire, False)
             if self._multiple_result_sets:
                 return
         self._cache_prepared_statement()
         return
 
@@ -1269,16 +1298,15 @@
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [404, 100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
-            if self._sqlcode not in [0, 100,]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            self._process_sqlcode(self._sqlcode)
             if self._sqlcode == 404:
                 self._update404(404)
             else:
                 self._get_output_parameters(self._in_message.wire)
         return
 
     def _stored_procedure_query(self):
@@ -1308,14 +1336,15 @@
                 return
             elif self._sqlcode == 100:
                 self._handle_error_100(100)
                 return
             self._get_output_parameters(self._in_message.wire)
             self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
+            self._process_sqlcode(self._sqlcode)
             if self._sqlcode == 100:
                 self._handle_error_100(100)
 
             self._current_wire = self._in_message.wire
             self._result_set = [self._current_wire]
             self._rs_index = 0
 
@@ -1612,15 +1641,15 @@
         # with self._connection._lock:
         #     self._out_message.wire._write_header(_Message.GET_AUTO_GENERATED_KEYS)
         #     sequence_number = self._connection._get_new_sequence_number()
         #     self._out_message._send(sequence_number)
         #     self._in_message._read_message_sql(sequence_number)
         #     self._sqlcode = self._in_message.wire.header._get_function_code()
         #     if self._sqlcode != 100:
-        #         raise InterfaceError(self._get_error_info(self._sqlcode))
+        #         raise DatabaseError(self._get_error_info(self._sqlcode))
         #     self._get_column_info(self._in_message.wire)
         #     self._lastrowid = self._in_message.wire._get()
 
         self.execute('SELECT LAST_IDENTITY()')
         self._lastrowid = self.fetchone()[0]
         return self._lastrowid
 
@@ -1771,16 +1800,15 @@
                 intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
 
                 sequence_number = self._connection._get_new_sequence_number()
                 self._out_message._send(sequence_number)
 
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
-                if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))                
+                self._process_sqlcode(self._sqlcode)
             self._result_set.append(self._in_message.wire)
 
         if self._sqlcode == 404:
             self._query404()
             return
 
         if self._rs_index + 1 == len(self._result_set):
@@ -1885,23 +1913,24 @@
                 self._scroll_flag = False
             else:
                 if self.fetchone_helper():
                     retval = self._rsrow._offsets
 
         if retval is None:
             return retval
-        return retval[:]
+        return retval.as_tuple()
+        # return tuple(retval[:])
 
     def fetchmany(self, size = None):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
 
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
-                return None
+                return []
             if size is None:
                 size = self.arraysize
             if self._rs_index == 0:
                 if self._cursor_ptr < len(self._warehouse):
                     rows = []
                     for i in range(size):
                         row = self._warehouse[self._cursor_ptr]
@@ -1926,24 +1955,24 @@
             size = self.arraysize
 
         rows = []
         for i in range(size):
             row = self.fetchone()
             if row is None:
                 break
-            rows.append(row[:])
+            rows.append(row)
         return rows
 
     def fetchall(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
         
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
-                return None
+                return []
             if self._rs_index == 0:
                 if self._cursor_ptr < len(self._warehouse):
                     rows = []
                     while 1:
                         row = self._warehouse[self._cursor_ptr]
                         rows.append(row[:])
                         if self._cursor_ptr + 1 >= len(self._warehouse):
@@ -1962,15 +1991,16 @@
                     self._cursor_ptr += 1
                 return rows
         
         rows = []
         while self._current_wire is not None:
             row = self.fetchone()
             if not row: break
-            rows.append(row[:])
+            rows.append(row)
+        
         return rows
 
 class EmbdeddedCursor(_BaseCursor):
     embedded = True
     _result_set = None
 
     def __init__(self, connection: _IRISEmbedded) -> None:
@@ -2033,20 +2063,14 @@
                 _column_info.isHidden,
                 _column_info.isIdentity,
                 _column_info.isKeyColumn,
                 _column_info.isRowId,
             ]
             self._columns.append(intersystems_iris.dbapi._Column._Column(name, odbctype, precision, scale, nullable, label, tableName, schema, catalog, additionalData, slotPosition))
 
-    def _process_sqlcode(self, sqlcode, message):
-        if sqlcode == -119:
-            raise IntegrityError(message)
-        if sqlcode not in [0, 100]:
-            raise InterfaceError(message)
-
     @property
     def lastrowid(self):
         return self._lastrowid
 
     def _prepare_new(self):
         statement = self._parsed_statement
         sqlcode = 0
@@ -2150,33 +2174,34 @@
         return self._rowcount
         
     def fetchone(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
         
         try:
-            row = self._result_set.__next__()
+            values = self._result_set.__next__()
         except:
             return None
 
-        row = [None if v == '' else '' if v == '\x00' else v for v in row]
+        values = [None if v == '' else '' if v == '\x00' else v for v in values]
+        row = namedtuple('Row', [col.name for col in self._columns], rename=True)
 
         _types = {
             SQLType.BIGINT: int,
             SQLType.BINARY: bytes,
             SQLType.BIT: bool,
             SQLType.INTEGER: int,
             SQLType.VARCHAR: str,
             SQLType.LONGVARBINARY: IRISBinaryStream,
             SQLType.LONGVARCHAR: IRISStream,
         }
         
         if self._columns:
             for _column in self._columns:
-                value = row[_column.slotPosition - 1]
+                value = values[_column.slotPosition - 1]
 
                 ctype = _column.type
                 value_type = _types[ctype] if ctype in _types else None
                 try:
                     if type(value) == float:
                         value = decimal.Decimal(str(value))
                     elif not _column.tableName and not _column.schema:
@@ -2187,16 +2212,16 @@
                         stream = value_type(self._connection, value, embedded=True)
                         value = stream.fetch()
                     elif not isinstance(value, value_type):
                         value = value_type(value)
                 except Exception as ex:
                     raise ex
                     pass
-                row[_column.slotPosition - 1] = value
-        return row
+                values[_column.slotPosition - 1] = value
+        return row(*values)
 
     def fetchall(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
 
         rows = []
         while True:
```

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_IRISStream.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_Message.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_Message.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-def expect_response(message_type):
-    if message_type in NO_RESPONSE:
-        return False
-    return True
-
-HANDSHAKE = b'HS'
-CONNECT = b'CN'
-DISCONNECT = b'DC'
-PREPARE = b'PP'
-DIRECT_UPDATE = b'DU'
-DIRECT_QUERY = b'DQ'
-DIRECT_STORED_PROCEDURE = b'DS'
-PREPARE_DIALECT = b'PD'
-DIRECT_EXECUTE_DIALECT = b'DD'
-PREPARED_UPDATE_EXECUTE = b'PU'
-PREPARED_QUERY_EXECUTE = b'PQ'
-FETCH_DATA = b'FD'
-CLOSE_CURSOR = b'CC'
-PREPARE_STORED_PROCEDURE = b'SP'
-STORED_PROCEDURE_UPDATE_EXECUTE = b'SU'
-STORED_PROCEDURE_QUERY_EXECUTE = b'SQ'
-STORED_PROCEDURE_FETCH_DATA = b'SF'
-EXECUTE_MULTIPLE_RESULT_SETS = b'MS'
-MULTIPLE_RESULT_SETS_FETCH_DATA = b'MD'
-GET_MORE_RESULTS = b'MR'
-GET_STREAM_SIZE = b'SS'
-RETRIEVE_STREAM = b'RS'
-OPEN_STREAM = b'OS'
-READ_STREAM = b'JS'
-READ_STREAM_ODBC = b'AS'
-STORE_BINARY_STREAM = b'SB'
-STORE_CHARACTER_STREAM = b'SM'
-STREAM_GET_BYTES  = b'GB'
-STREAM_SET_BYTES  = b'SZ'
-STREAM_TRUNCATE  = b'SX'
-STREAM_GET_POSITION   = b'GP'
-CLOSE_STREAM   = b'CS'
-GET_RESULT_SET_OBJECT = b'FR'
-GET_STRUCT_OBJECT = b'FS'
-COMMIT = b'TC'
-ROLLBACK = b'TR'
-READ_COMMITTED = b'RC'
-READ_UNCOMMITTED = b'RU'
-ISOLATION_LEVEL = b'IL'
-AUTOCOMMIT_OFF = b'AF'
-AUTOCOMMIT_ON = b'AN'
-TOGGLE_SYNCHRONOUS_COMMIT = b'TS'
-GET_AUTO_GENERATED_KEYS = b'GG'
-IN_TRANSACTION = b'IT'
-JDBC_BESTROWID = b'BR'
-JDBC_CATALOGS = b'CA'
-JDBC_COLUMNPRIV = b'CP'
-JDBC_COLUMNS = b'CO'
-JDBC_CROSSREFERENCE = b'CR'
-JDBC_EXPORTEDKEYS = b'EK'
-JDBC_IMPORTEDKEYS = b'IK'
-JDBC_INDEXINFO = b'II'
-JDBC_PRIMARYKEYS = b'PK'
-JDBC_PROCEDURECOL = b'PC'
-JDBC_PROCEDURES = b'PR'
-JDBC_SCHEMAS = b'SC'
-JDBC_TABLEPRIV = b'TP'
-JDBC_TABLES = b'TA'
-JDBC_TABLETYPES = b'TT'
-JDBC_TYPEINFO = b'TI'
-JDBC_VERSIONCOL = b'VC'
-ODBC_BESTROWID = b'br'
-ODBC_CATALOGS = b'ca'
-ODBC_COLUMNPRIV = b'cp'
-ODBC_COLUMNS_35 = b'c3'
-ODBC_CROSSREFERENCE_35 = b'r3'
-ODBC_EXPORTEDKEYS_35 = b'e3'
-ODBC_IMPORTEDKEYS_35 = b'i3'
-ODBC_PROCEDURECOL_35 = b'p3'
-ODBC_TYPEINFO_35 = b't3'
-ODBC_COLUMNS = b'co'
-ODBC_CROSSREFERENCE = b'cr'
-ODBC_EXPORTEDKEYS = b'ek'
-ODBC_IMPORTEDKEYS = b'ik'
-ODBC_INDEXINFO = b'ii'
-ODBC_PRIMARYKEYS = b'pk'
-ODBC_PROCEDURECOL = b'pc'
-ODBC_PROCEDURES = b'pr'
-ODBC_SCHEMAS = b'sc'
-ODBC_STATISTICS = b'st'
-ODBC_TABLEPRIV = b'tp'
-ODBC_TABLES = b'ta'
-ODBC_TABLETYPES = b'tt'
-ODBC_TYPEINFO = b'ti'
-ODBC_VERSIONCOL = b'vc'
-JDBC_UDTS = b'UT'
-JDBC_SUPER_TYPES = b'SY'
-JDBC_SUPER_TABLES = b'SL'
-JDBC_GET_ATTRIBUTES = b'AT'
-JDBC_GET_FUNCTION_COLUMNS  = b'FC'
-JDBC_GET_FUNCTIONS  = b'FN'
-JDBC_CLIENT_INFO_PROPERTIES  = b'CF'
-SET_CLIENT_INFO_PROPERTIES   = b'CG'
-XA_START = b'XS'
-XA_END = b'XE'
-XA_FORGET = b'XF'
-XA_PREPARE = b'XP'
-XA_COMMIT = b'XC'
-XA_ROLLBACK = b'XR'
-XA_RECOVER = b'XV'
-EXECUTE_STATIC_CURSOR = b'EX'
-DIRECT_STATIC_CURSOR = b'DX'
-FETCH_STATIC_CURSOR = b'FX'
-UPDATE_CACHE = b'UC'
-RESET_CONNECTION = b'RN'
-GET_SERVER_ERROR = b'OE'
-EXECUTE_STATEMENT_BATCH = b'EB'
-CLOSE_STATEMENT = b'CU'
-QUICK_LOAD = b'QL'
-QUICK_CHILD_TABLE_LOAD = b'QZ'
-QUICK_CHILD_TABLE_CREATE = b'QX'
-QUICK_CHILD_TABLE_REMOVE = b'QK'
-QUICK_STORE = b'QS'
-QUICK_CREATE = b'QC'
-QUICK_REMOVE = b'QR'
-QUICK_FIND_ROWID_BY_PK = b'Q1'
-QUICK_FIND_ROWID_BY_CONSTRAINT = b'Q2'
-QUICK_FIND_PK_BY_CONSTRAINT = b'Q3'
-QUICK_REMOVE_BY_PK = b'Q4'
-QUICK_CREATE_BY_PK = b'Q5'
-QUICK_STORE_BY_PK = b'Q6'
-QUICK_LOAD_BY_PK = b'Q7'
-QUICK_CHILD_TABLE_REMOVE_BY_PK = b'Q8'
-QUICK_CHILD_TABLE_CREATE_BY_PK = b'Q9'
-QUICK_CHILD_TABLE_LOAD_BY_PK = b'QA'
-QUICK_GET_CHILDREN_PKS = b'QB'
-QUICK_GET_CHILDREN_PKS_BY_PK = b'QD'
-QUICK_FIND_PK_BY_ROWID = b'QE'
-QUICK_BULK_LOAD = b'QM'
-QUICK_BULK_CREATE = b'QN'
-QUICK_BULK_STORE = b'QO'
-QUICK_BULK_SAVE_BY_PK  = b'QW'
-QUICK_QUERY  = b'QQ'
-QUICK_JPA_FLUSH  = b'QF'
-GET_CACHE_INFO = b'CI'
-PING = b'PG'
-PING_TWO = b'P2'
-IS_TWO_FACTOR_ENABLED = b'2E'
-SEND_TWO_FACTOR_TOKEN = b'2F'
-STREAM_SET_PREFETCH_SIZE = b'SN'
-EXTERNAL_INTERUPT = b'EI'
-GET_NAMESPACES_MSG = b'CI'
-GATEWAY_INIT = b'GI'
-
-NO_RESPONSE = [AUTOCOMMIT_OFF,
-               AUTOCOMMIT_ON,
-               READ_COMMITTED,
-               READ_UNCOMMITTED,
-               CLOSE_CURSOR,
-               CLOSE_STREAM,
-               CLOSE_STATEMENT,
-               RESET_CONNECTION,
+def expect_response(message_type):
+    if message_type in NO_RESPONSE:
+        return False
+    return True
+
+HANDSHAKE = b'HS'
+CONNECT = b'CN'
+DISCONNECT = b'DC'
+PREPARE = b'PP'
+DIRECT_UPDATE = b'DU'
+DIRECT_QUERY = b'DQ'
+DIRECT_STORED_PROCEDURE = b'DS'
+PREPARE_DIALECT = b'PD'
+DIRECT_EXECUTE_DIALECT = b'DD'
+PREPARED_UPDATE_EXECUTE = b'PU'
+PREPARED_QUERY_EXECUTE = b'PQ'
+FETCH_DATA = b'FD'
+CLOSE_CURSOR = b'CC'
+PREPARE_STORED_PROCEDURE = b'SP'
+STORED_PROCEDURE_UPDATE_EXECUTE = b'SU'
+STORED_PROCEDURE_QUERY_EXECUTE = b'SQ'
+STORED_PROCEDURE_FETCH_DATA = b'SF'
+EXECUTE_MULTIPLE_RESULT_SETS = b'MS'
+MULTIPLE_RESULT_SETS_FETCH_DATA = b'MD'
+GET_MORE_RESULTS = b'MR'
+GET_STREAM_SIZE = b'SS'
+RETRIEVE_STREAM = b'RS'
+OPEN_STREAM = b'OS'
+READ_STREAM = b'JS'
+READ_STREAM_ODBC = b'AS'
+STORE_BINARY_STREAM = b'SB'
+STORE_CHARACTER_STREAM = b'SM'
+STREAM_GET_BYTES  = b'GB'
+STREAM_SET_BYTES  = b'SZ'
+STREAM_TRUNCATE  = b'SX'
+STREAM_GET_POSITION   = b'GP'
+CLOSE_STREAM   = b'CS'
+GET_RESULT_SET_OBJECT = b'FR'
+GET_STRUCT_OBJECT = b'FS'
+COMMIT = b'TC'
+ROLLBACK = b'TR'
+READ_COMMITTED = b'RC'
+READ_UNCOMMITTED = b'RU'
+ISOLATION_LEVEL = b'IL'
+AUTOCOMMIT_OFF = b'AF'
+AUTOCOMMIT_ON = b'AN'
+TOGGLE_SYNCHRONOUS_COMMIT = b'TS'
+GET_AUTO_GENERATED_KEYS = b'GG'
+IN_TRANSACTION = b'IT'
+JDBC_BESTROWID = b'BR'
+JDBC_CATALOGS = b'CA'
+JDBC_COLUMNPRIV = b'CP'
+JDBC_COLUMNS = b'CO'
+JDBC_CROSSREFERENCE = b'CR'
+JDBC_EXPORTEDKEYS = b'EK'
+JDBC_IMPORTEDKEYS = b'IK'
+JDBC_INDEXINFO = b'II'
+JDBC_PRIMARYKEYS = b'PK'
+JDBC_PROCEDURECOL = b'PC'
+JDBC_PROCEDURES = b'PR'
+JDBC_SCHEMAS = b'SC'
+JDBC_TABLEPRIV = b'TP'
+JDBC_TABLES = b'TA'
+JDBC_TABLETYPES = b'TT'
+JDBC_TYPEINFO = b'TI'
+JDBC_VERSIONCOL = b'VC'
+ODBC_BESTROWID = b'br'
+ODBC_CATALOGS = b'ca'
+ODBC_COLUMNPRIV = b'cp'
+ODBC_COLUMNS_35 = b'c3'
+ODBC_CROSSREFERENCE_35 = b'r3'
+ODBC_EXPORTEDKEYS_35 = b'e3'
+ODBC_IMPORTEDKEYS_35 = b'i3'
+ODBC_PROCEDURECOL_35 = b'p3'
+ODBC_TYPEINFO_35 = b't3'
+ODBC_COLUMNS = b'co'
+ODBC_CROSSREFERENCE = b'cr'
+ODBC_EXPORTEDKEYS = b'ek'
+ODBC_IMPORTEDKEYS = b'ik'
+ODBC_INDEXINFO = b'ii'
+ODBC_PRIMARYKEYS = b'pk'
+ODBC_PROCEDURECOL = b'pc'
+ODBC_PROCEDURES = b'pr'
+ODBC_SCHEMAS = b'sc'
+ODBC_STATISTICS = b'st'
+ODBC_TABLEPRIV = b'tp'
+ODBC_TABLES = b'ta'
+ODBC_TABLETYPES = b'tt'
+ODBC_TYPEINFO = b'ti'
+ODBC_VERSIONCOL = b'vc'
+JDBC_UDTS = b'UT'
+JDBC_SUPER_TYPES = b'SY'
+JDBC_SUPER_TABLES = b'SL'
+JDBC_GET_ATTRIBUTES = b'AT'
+JDBC_GET_FUNCTION_COLUMNS  = b'FC'
+JDBC_GET_FUNCTIONS  = b'FN'
+JDBC_CLIENT_INFO_PROPERTIES  = b'CF'
+SET_CLIENT_INFO_PROPERTIES   = b'CG'
+XA_START = b'XS'
+XA_END = b'XE'
+XA_FORGET = b'XF'
+XA_PREPARE = b'XP'
+XA_COMMIT = b'XC'
+XA_ROLLBACK = b'XR'
+XA_RECOVER = b'XV'
+EXECUTE_STATIC_CURSOR = b'EX'
+DIRECT_STATIC_CURSOR = b'DX'
+FETCH_STATIC_CURSOR = b'FX'
+UPDATE_CACHE = b'UC'
+RESET_CONNECTION = b'RN'
+GET_SERVER_ERROR = b'OE'
+EXECUTE_STATEMENT_BATCH = b'EB'
+CLOSE_STATEMENT = b'CU'
+QUICK_LOAD = b'QL'
+QUICK_CHILD_TABLE_LOAD = b'QZ'
+QUICK_CHILD_TABLE_CREATE = b'QX'
+QUICK_CHILD_TABLE_REMOVE = b'QK'
+QUICK_STORE = b'QS'
+QUICK_CREATE = b'QC'
+QUICK_REMOVE = b'QR'
+QUICK_FIND_ROWID_BY_PK = b'Q1'
+QUICK_FIND_ROWID_BY_CONSTRAINT = b'Q2'
+QUICK_FIND_PK_BY_CONSTRAINT = b'Q3'
+QUICK_REMOVE_BY_PK = b'Q4'
+QUICK_CREATE_BY_PK = b'Q5'
+QUICK_STORE_BY_PK = b'Q6'
+QUICK_LOAD_BY_PK = b'Q7'
+QUICK_CHILD_TABLE_REMOVE_BY_PK = b'Q8'
+QUICK_CHILD_TABLE_CREATE_BY_PK = b'Q9'
+QUICK_CHILD_TABLE_LOAD_BY_PK = b'QA'
+QUICK_GET_CHILDREN_PKS = b'QB'
+QUICK_GET_CHILDREN_PKS_BY_PK = b'QD'
+QUICK_FIND_PK_BY_ROWID = b'QE'
+QUICK_BULK_LOAD = b'QM'
+QUICK_BULK_CREATE = b'QN'
+QUICK_BULK_STORE = b'QO'
+QUICK_BULK_SAVE_BY_PK  = b'QW'
+QUICK_QUERY  = b'QQ'
+QUICK_JPA_FLUSH  = b'QF'
+GET_CACHE_INFO = b'CI'
+PING = b'PG'
+PING_TWO = b'P2'
+IS_TWO_FACTOR_ENABLED = b'2E'
+SEND_TWO_FACTOR_TOKEN = b'2F'
+STREAM_SET_PREFETCH_SIZE = b'SN'
+EXTERNAL_INTERUPT = b'EI'
+GET_NAMESPACES_MSG = b'CI'
+GATEWAY_INIT = b'GI'
+
+NO_RESPONSE = [AUTOCOMMIT_OFF,
+               AUTOCOMMIT_ON,
+               READ_COMMITTED,
+               READ_UNCOMMITTED,
+               CLOSE_CURSOR,
+               CLOSE_STREAM,
+               CLOSE_STATEMENT,
+               RESET_CONNECTION,
                DISCONNECT]
```

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_Parameter.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_ParameterCollection.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_ResultSetRow.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+from datetime import datetime
+from collections import namedtuple
 from ._SQLType import SQLType
 from .._DBList import _DBList
 from .._ListItem import _ListItem
 from ._IRISStream import IRISStream, IRISBinaryStream
 from ._Column import _Column
 
+def from_timestamp_posix(posix):
+    time = int(posix)
+    if time > 0:
+        time ^= 0x1000000000000000 
+    else:
+        time |= 0xF000000000000000 
+
+    time /= 1000000
+
+    value = datetime.utcfromtimestamp(time).replace(tzinfo=None)
+    return value
+
 class _ResultSetRow:
     _locale = "latin-1"
     _connection = None
 
     def __init__(self, connection, columns=None, rowcount=0, ):
         self._connection = connection
         # index from user-inputted columns to columns received from server
@@ -105,14 +119,19 @@
             self._locale = rsrow._locale
 
         def __getattr__(self, key):
             return self.__getitem__(key)
 
         def get(self):
             return self[:]
+        
+        def as_tuple(self):
+            row = namedtuple('Row', [col.name for col in self._columns], rename=True)
+            values = self[:]
+            return row(*values)
 
         def __getitem__(self, key):
             if isinstance(key, str):
                 key = key.lower()
                 if key not in self._name_dict_keys:
                     raise KeyError("Column '" + key + "' does not exist")
                 return self[self._name_dict[key][0] + 1]
@@ -134,14 +153,17 @@
                 self._list_item.next_offset = self._offsets[key]
                 _DBList._get_list_element(self._list_item)
                 item = _DBList._get(self._list_item, self._locale)
                 _column: _Column = self._columns[idx]
                 ctype = _column.type
                 value_type = self._types[ctype] if ctype in self._types else None
                 try:
+                    if ctype == SQLType.TIMESTAMP_POSIX:
+                        item = from_timestamp_posix(item)
+
                     if _column.tableName == 'None' and _column.schema == 'None':
                         # Ignore for anonymous tables
                         pass
                     elif item is None:
                         pass
                     elif issubclass(value_type, IRISStream):
                         stream = value_type(self._connection, item)
```

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/_SQLType.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_PreParser.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import functools
 import enum
 import intersystems_iris._IRISList
 import intersystems_iris.dbapi._DBAPI
 import intersystems_iris.dbapi._Parameter
 import intersystems_iris.dbapi.preparser._Token
 import intersystems_iris.dbapi.preparser._TokenList
@@ -753,15 +754,18 @@
         #  Do a table lookup to identify token
         if t_strIDUpper in self.s_KeywordTable:
             #  Found it, replace ID with specific type
             t_eToken = self.s_KeywordTable[t_strIDUpper]
             if (t_eToken == TOKEN.NOT):
                 t_strID = self.m_Scanner.checkForNotPredicates()
                 t_strIDUpper = t_strID.upper()
-        self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(t_eToken, t_strID, t_strIDUpper))
+        if t_strID == '%s':
+            self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(TOKEN.QUESTION_MARK, "?"))
+        else:
+            self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(t_eToken, t_strID, t_strIDUpper))
 
     # used for various operators
     def Tokenize_op(self, check_tokens = [ParseToken.tokEQUAL]):
         self.m_Scanner.BeginLexeme()
         if self.m_Scanner.PeekNextToken() in check_tokens:
             # Check for composite operators (e.g. <=, >=, !=, etc.)
             self.m_Scanner.NextToken()
```

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_Scanner.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_Token.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/dbapi/preparser/_TokenList.py` & `dbt-iris-1.3.2b3/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessHost.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessOperation.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessProcess.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_BusinessService.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_Common.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_Director.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_IRISBusinessService.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_IRISOutboundAdapter.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_InboundAdapter.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/_OutboundAdapter.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/intersystems_iris/pex/__init__.py` & `dbt-iris-1.3.2b3/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/iris/__init__.py` & `dbt-iris-1.3.2b3/iris/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from sys import path as __syspath
 import os
 
 # check for install dir in environment
 # environment to check is IRISINSTALLDIR
 # if not found, raise exception and exit
-installdir = os.environ.get('IRISINSTALLDIR')
+# ISC_PACKAGE_INSTALLDIR - defined by default in Docker images
+installdir = os.environ.get('IRISINSTALLDIR') or os.environ.get('ISC_PACKAGE_INSTALLDIR')
 if installdir is None:
         raise Exception("""Cannot find InterSystems IRIS installation directory
     Please set IRISINSTALLDIR environment variable to the InterSystems IRIS installation directory""")
 
 # join the install dir with the bin directory
 __syspath.append(os.path.join(installdir, 'bin'))
 # also append lib/python
```

### Comparing `dbt-iris-1.3.2b2/iris/irisbuiltins.py` & `dbt-iris-1.3.2b3/iris/irisbuiltins.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/iris/irisloader.py` & `dbt-iris-1.3.2b3/iris/irisloader.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/irisnative/_IRISNative.py` & `dbt-iris-1.3.2b3/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `dbt-iris-1.3.2b2/setup.py` & `dbt-iris-1.3.2b3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup
 import os
 
 package_name = "dbt-iris"
 # make sure this always matches dbt/adapters/{adapter}/__version__.py
-package_version = "1.3.2b2"
+package_version = "1.3.2b3"
 description = """The InterSystems IRIS adapter plugin for dbt"""
 
 thelibFolder = os.path.dirname(os.path.realpath(__file__))
 requirementPath = thelibFolder + "/requirements.txt"
 
 requirements = []
 if os.path.isfile(requirementPath):
```

