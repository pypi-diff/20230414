# Comparing `tmp/qilib-0.3.8.tar.gz` & `tmp/qilib-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qilib-0.3.8.tar", last modified: Tue Jun  1 13:43:06 2021, max compression
+gzip compressed data, was "dist\qilib-0.3.9.tar", last modified: Tue May 10 08:22:31 2022, max compression
```

## Comparing `qilib-0.3.8.tar` & `qilib-0.3.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:06.000000 qilib-0.3.8/
--rw-rw-rw-   0        0        0     1155 2021-06-01 06:56:01.000000 qilib-0.3.8/LICENSE.md
--rw-rw-rw-   0        0        0    11643 2021-06-01 13:43:06.000000 qilib-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    11068 2021-06-01 13:21:15.000000 qilib-0.3.8/README.md
--rw-rw-rw-   0        0        0       42 2021-06-01 13:43:06.000000 qilib-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     3051 2021-06-01 13:21:15.000000 qilib-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:05.000000 qilib-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib/
--rw-rw-rw-   0        0        0       39 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib/configuration_helper/
--rw-rw-rw-   0        0        0      737 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/
--rw-rw-rw-   0        0        0     1422 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/__init__.py
--rw-rw-rw-   0        0        0     3429 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/ami430_instrument_adapter.py
--rw-rw-rw-   0        0        0     4050 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/common_instrument_adapter.py
--rw-rw-rw-   0        0        0     3952 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/d5a_instrument_adapter.py
--rw-rw-rw-   0        0        0     2089 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/f1d_instrument_adapter.py
--rw-rw-rw-   0        0        0     2924 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/hdawg8_instrument_adapter.py
--rw-rw-rw-   0        0        0     2495 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/keithley_dmm6500_adapter.py
--rw-rw-rw-   0        0        0     2349 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/keysight_e8267d_instrument_adapter.py
--rw-rw-rw-   0        0        0     2089 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/m2j_instrument_adapter.py
--rw-rw-rw-   0        0        0     2345 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/m4i_instrument_adapter.py
--rw-rw-rw-   0        0        0     3571 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/read_only_configuration_instrument_adapter.py
--rw-rw-rw-   0        0        0     2089 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/s5i_instrument_adapter.py
--rw-rw-rw-   0        0        0     4804 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/spi_module_instrument_adapter.py
--rw-rw-rw-   0        0        0     2859 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/spi_rack_instrument_adapter.py
--rw-rw-rw-   0        0        0     2452 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/configuration_helper/adapters/uhfli_instrument_adapter.py
--rw-rw-rw-   0        0        0     5577 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/configuration_helper.py
--rw-rw-rw-   0        0        0       84 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/exceptions.py
--rw-rw-rw-   0        0        0     5910 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/instrument_adapter.py
--rw-rw-rw-   0        0        0     5616 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/instrument_adapter_factory.py
--rw-rw-rw-   0        0        0     7621 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/instrument_configuration.py
--rw-rw-rw-   0        0        0     6309 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/instrument_configuration_set.py
--rw-rw-rw-   0        0        0     3250 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/instrument_configuration_visitor.py
--rw-rw-rw-   0        0        0     3020 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/serial_port_resolver.py
--rw-rw-rw-   0        0        0     1464 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/configuration_helper/visitor.py
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib/data_set/
--rw-rw-rw-   0        0        0      381 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/__init__.py
--rw-rw-rw-   0        0        0     8447 2021-06-01 08:42:25.000000 qilib-0.3.8/src/qilib/data_set/data_array.py
--rw-rw-rw-   0        0        0    12197 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/data_set/data_set.py
--rw-rw-rw-   0        0        0     2427 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/data_set_io_reader.py
--rw-rw-rw-   0        0        0     2872 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/data_set_io_writer.py
--rw-rw-rw-   0        0        0     2065 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/memory_data_set_io_factory.py
--rw-rw-rw-   0        0        0     3496 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/memory_data_set_io_reader.py
--rw-rw-rw-   0        0        0     2617 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/memory_data_set_io_writer.py
--rw-rw-rw-   0        0        0     7393 2021-06-01 08:42:48.000000 qilib-0.3.8/src/qilib/data_set/mongo_data_set_io.py
--rw-rw-rw-   0        0        0    10119 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/mongo_data_set_io_reader.py
--rw-rw-rw-   0        0        0     4559 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/mongo_data_set_io_writer.py
--rw-rw-rw-   0        0        0      258 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/data_set/type_aliases.py
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:06.000000 qilib-0.3.8/src/qilib/utils/
--rw-rw-rw-   0        0        0       67 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/utils/__init__.py
--rw-rw-rw-   0        0        0     1914 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/utils/memory_storage_queue.py
--rw-rw-rw-   0        0        0     5264 2021-06-01 07:25:26.000000 qilib-0.3.8/src/qilib/utils/python_json_structure.py
--rw-rw-rw-   0        0        0    10902 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/utils/serialization.py
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:06.000000 qilib-0.3.8/src/qilib/utils/storage/
--rw-rw-rw-   0        0        0      108 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/utils/storage/__init__.py
--rw-rw-rw-   0        0        0     9713 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/utils/storage/interface.py
--rw-rw-rw-   0        0        0     7112 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/utils/storage/memory.py
--rw-rw-rw-   0        0        0    17661 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/utils/storage/mongo.py
--rw-rw-rw-   0        0        0      223 2021-06-01 06:56:01.000000 qilib-0.3.8/src/qilib/utils/type_aliases.py
--rw-rw-rw-   0        0        0       23 2021-06-01 13:21:15.000000 qilib-0.3.8/src/qilib/version.py
-drwxrwxrwx   0        0        0        0 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib.egg-info/
--rw-rw-rw-   0        0        0    11643 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2617 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-06-01 13:43:05.000000 qilib-0.3.8/src/qilib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.183054 qilib-0.3.9/
+-rw-rw-rw-   0        0        0     1167 2022-05-10 08:03:24.000000 qilib-0.3.9/LICENSE.md
+-rw-rw-rw-   0        0        0    11695 2022-05-10 08:22:31.182053 qilib-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11068 2022-05-10 07:29:21.000000 qilib-0.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-05-10 08:22:31.183054 qilib-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     3151 2022-05-10 08:03:24.000000 qilib-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.113053 qilib-0.3.9/src/
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.122057 qilib-0.3.9/src/qilib/
+-rw-rw-rw-   0        0        0       39 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.143056 qilib-0.3.9/src/qilib/configuration_helper/
+-rw-rw-rw-   0        0        0      737 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.158054 qilib-0.3.9/src/qilib/configuration_helper/adapters/
+-rw-rw-rw-   0        0        0     1470 2022-05-10 08:03:24.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/__init__.py
+-rw-rw-rw-   0        0        0     3429 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/ami430_instrument_adapter.py
+-rw-rw-rw-   0        0        0     4050 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/common_instrument_adapter.py
+-rw-rw-rw-   0        0        0     3952 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/d5a_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2089 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/f1d_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2924 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/hdawg8_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2495 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/keithley_dmm6500_adapter.py
+-rw-rw-rw-   0        0        0     2349 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/keysight_e8267d_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2089 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/m2j_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2345 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/m4i_instrument_adapter.py
+-rw-rw-rw-   0        0        0     3571 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/read_only_configuration_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2089 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/s5i_instrument_adapter.py
+-rw-rw-rw-   0        0        0     4804 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/spi_module_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2859 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/spi_rack_instrument_adapter.py
+-rw-rw-rw-   0        0        0     2452 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/adapters/uhfli_instrument_adapter.py
+-rw-rw-rw-   0        0        0     5577 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/configuration_helper.py
+-rw-rw-rw-   0        0        0       84 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/exceptions.py
+-rw-rw-rw-   0        0        0     5910 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/instrument_adapter.py
+-rw-rw-rw-   0        0        0     5616 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/instrument_adapter_factory.py
+-rw-rw-rw-   0        0        0     7621 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/instrument_configuration.py
+-rw-rw-rw-   0        0        0     6309 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/instrument_configuration_set.py
+-rw-rw-rw-   0        0        0     3250 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/instrument_configuration_visitor.py
+-rw-rw-rw-   0        0        0     3020 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/serial_port_resolver.py
+-rw-rw-rw-   0        0        0     1464 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/configuration_helper/visitor.py
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.172055 qilib-0.3.9/src/qilib/data_set/
+-rw-rw-rw-   0        0        0      381 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/__init__.py
+-rw-rw-rw-   0        0        0     8703 2022-05-10 08:03:24.000000 qilib-0.3.9/src/qilib/data_set/data_array.py
+-rw-rw-rw-   0        0        0    12197 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/data_set.py
+-rw-rw-rw-   0        0        0     2427 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/data_set_io_reader.py
+-rw-rw-rw-   0        0        0     2872 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/data_set_io_writer.py
+-rw-rw-rw-   0        0        0     2065 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/memory_data_set_io_factory.py
+-rw-rw-rw-   0        0        0     3496 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/memory_data_set_io_reader.py
+-rw-rw-rw-   0        0        0     2617 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/memory_data_set_io_writer.py
+-rw-rw-rw-   0        0        0     7553 2022-05-10 08:03:24.000000 qilib-0.3.9/src/qilib/data_set/mongo_data_set_io.py
+-rw-rw-rw-   0        0        0    10124 2022-05-10 08:03:24.000000 qilib-0.3.9/src/qilib/data_set/mongo_data_set_io_reader.py
+-rw-rw-rw-   0        0        0     4559 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/mongo_data_set_io_writer.py
+-rw-rw-rw-   0        0        0      258 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/data_set/type_aliases.py
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.178053 qilib-0.3.9/src/qilib/utils/
+-rw-rw-rw-   0        0        0       67 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/__init__.py
+-rw-rw-rw-   0        0        0     1914 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/memory_storage_queue.py
+-rw-rw-rw-   0        0        0     5264 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/python_json_structure.py
+-rw-rw-rw-   0        0        0    10902 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/serialization.py
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.181056 qilib-0.3.9/src/qilib/utils/storage/
+-rw-rw-rw-   0        0        0      108 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/storage/__init__.py
+-rw-rw-rw-   0        0        0     9713 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/storage/interface.py
+-rw-rw-rw-   0        0        0     7112 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/storage/memory.py
+-rw-rw-rw-   0        0        0    17960 2022-05-10 08:03:24.000000 qilib-0.3.9/src/qilib/utils/storage/mongo.py
+-rw-rw-rw-   0        0        0      223 2022-05-10 07:29:21.000000 qilib-0.3.9/src/qilib/utils/type_aliases.py
+-rw-rw-rw-   0        0        0       23 2022-05-10 08:03:24.000000 qilib-0.3.9/src/qilib/version.py
+drwxrwxrwx   0        0        0        0 2022-05-10 08:22:31.126053 qilib-0.3.9/src/qilib.egg-info/
+-rw-rw-rw-   0        0        0    11695 2022-05-10 08:22:31.000000 qilib-0.3.9/src/qilib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2617 2022-05-10 08:22:31.000000 qilib-0.3.9/src/qilib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-10 08:22:31.000000 qilib-0.3.9/src/qilib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2022-05-10 08:22:31.000000 qilib-0.3.9/src/qilib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-05-10 08:22:31.000000 qilib-0.3.9/src/qilib.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qilib-0.3.8/PKG-INFO` & `qilib-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: qilib
-Version: 0.3.8
+Version: 0.3.9
 Summary: Quantum Library for the Quantum Inspire platform
 Home-page: UNKNOWN
 Author: QuantumInspire
 License: Other/Proprietary License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 [![Coverage Status](https://coveralls.io/repos/github/QuTech-Delft/qilib/badge.svg?branch=dev)](https://coveralls.io/github/QuTech-Delft/qilib?branch=dev)
```

### Comparing `qilib-0.3.8/README.md` & `qilib-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/setup.py` & `qilib-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
       packages=['qilib', 'qilib.configuration_helper', 'qilib.configuration_helper.adapters',
                 'qilib.data_set', 'qilib.utils', 'qilib.utils.storage'],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9'],
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10'],
       license='Other/Proprietary License',
 
-      install_requires=['spirack>=0.1.8', 'numpy', 'serialize', 'zhinst', 'pymongo',
+      install_requires=['spirack>=0.1.8', 'numpy>=1.20', 'serialize', 'pymongo', 'zhinst;python_version<"3.10"', 
                         'requests', 'qcodes', 'qcodes_contrib_drivers', 'dataclasses-json'],
       extras_require={
-          'dev': ['pytest>=3.3.1', 'coverage>=4.5.1', 'mongomock==3.20.0', 'mypy', 'pylint'],
+          'dev': ['pytest>=3.3.1', 'coverage>=4.5.1', 'mongomock==3.20.0', 'mypy', 'pylint', 'types-requests'],
       })
```

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/__init__.py` & `qilib-0.3.9/src/qilib/configuration_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/__init__.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import sys
 from qilib.configuration_helper.adapters.common_instrument_adapter import CommonInstrumentAdapter
 from qilib.configuration_helper.adapters.read_only_configuration_instrument_adapter import ReadOnlyConfigurationInstrumentAdapter
 from qilib.configuration_helper.adapters.ami430_instrument_adapter import AMI430InstrumentAdapter
 from qilib.configuration_helper.adapters.keithley_dmm6500_adapter import Keithley6500InstrumentAdapter
 from qilib.configuration_helper.adapters.spi_rack_instrument_adapter import SpiRackInstrumentAdapter
 from qilib.configuration_helper.adapters.spi_module_instrument_adapter import SpiModuleInstrumentAdapter
 from qilib.configuration_helper.adapters.d5a_instrument_adapter import D5aInstrumentAdapter
 from qilib.configuration_helper.adapters.f1d_instrument_adapter import F1dInstrumentAdapter
 from qilib.configuration_helper.adapters.hdawg8_instrument_adapter import ZIHDAWG8InstrumentAdapter
 from qilib.configuration_helper.adapters.m2j_instrument_adapter import M2jInstrumentAdapter
 from qilib.configuration_helper.adapters.m4i_instrument_adapter import M4iInstrumentAdapter
 from qilib.configuration_helper.adapters.s5i_instrument_adapter import S5iInstrumentAdapter
-from qilib.configuration_helper.adapters.uhfli_instrument_adapter import ZIUHFLIInstrumentAdapter
+if sys.version_info < (3, 10):
+    from qilib.configuration_helper.adapters.uhfli_instrument_adapter import ZIUHFLIInstrumentAdapter
 from qilib.configuration_helper.adapters.keysight_e8267d_instrument_adapter import KeysightE8267DInstrumentAdapter
```

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/ami430_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/ami430_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/common_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/common_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/d5a_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/d5a_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/f1d_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/f1d_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/hdawg8_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/hdawg8_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/keithley_dmm6500_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/keithley_dmm6500_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/keysight_e8267d_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/keysight_e8267d_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/m2j_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/m2j_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/m4i_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/m4i_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/read_only_configuration_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/read_only_configuration_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/s5i_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/s5i_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/spi_module_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/spi_module_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/spi_rack_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/spi_rack_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/adapters/uhfli_instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/adapters/uhfli_instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/configuration_helper.py` & `qilib-0.3.9/src/qilib/configuration_helper/configuration_helper.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/instrument_adapter.py` & `qilib-0.3.9/src/qilib/configuration_helper/instrument_adapter.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/instrument_adapter_factory.py` & `qilib-0.3.9/src/qilib/configuration_helper/instrument_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/instrument_configuration.py` & `qilib-0.3.9/src/qilib/configuration_helper/instrument_configuration.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/instrument_configuration_set.py` & `qilib-0.3.9/src/qilib/configuration_helper/instrument_configuration_set.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/instrument_configuration_visitor.py` & `qilib-0.3.9/src/qilib/configuration_helper/instrument_configuration_visitor.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/serial_port_resolver.py` & `qilib-0.3.9/src/qilib/configuration_helper/serial_port_resolver.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/configuration_helper/visitor.py` & `qilib-0.3.9/src/qilib/configuration_helper/visitor.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/data_set/data_array.py` & `qilib-0.3.9/src/qilib/data_set/data_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,32 +15,36 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 import collections
 from copy import deepcopy
-from typing import Optional, Tuple, List, Union, Any, Set, Dict
+from typing import cast, Optional, Tuple, List, Union, Any, Set, Dict
 
 import numpy
 import numpy as np
+import numpy.typing as npt
+
+# type alias for numpy.ndarray
+numpy_ndarray_type = npt.NDArray[Any]
 
 
 class DataArray:
     """ A container for measurement data and setpoint arrays.
 
     All attributes/methods not defined in the DataArray are delegated to an underlying numpy array.
 
     The DataArray makes sure that the dimensions of the set arrays are correct with regards to the data array and vice
     versa (e.g., trying to set a 1D array of 10 elements as the data array with a 1D setpoint array of 8 elements will
     raise an error).
     """
 
     def __init__(self, name: str, label: str, unit: str = '', is_setpoint: bool = False,
-                 preset_data: Optional[numpy.ndarray] = None,
+                 preset_data: Optional[numpy_ndarray_type] = None,
                  set_arrays: Optional[Union[List['DataArray'], Tuple['DataArray', ...]]] = None,
                  shape: Optional[Tuple[int, ...]] = None) -> None:
         """
         Args:
             name:  Name for the data array
             label: Label, e.g. x-axis if it is a setpoint.
             unit: Unit for the measurement, or setpoint data.
@@ -51,62 +55,62 @@
             shape: Initialize with a shape rather than predefined data.
         """
 
         self._name: str = name
         self._label: str = label
         self._unit: str = unit
         self._is_setpoint: bool = is_setpoint
-        self._data: numpy.ndarray
+        self._data: numpy_ndarray_type
         if preset_data is not None:
             self._data = np.array(preset_data).copy()
         elif shape is not None:
             self._data = np.ndarray(shape) * np.NAN
         else:
             raise TypeError("Required arguments 'shape' or 'preset_data' not found")
         self._set_arrays = set_arrays if set_arrays is not None else []
         if len(self._set_arrays) > 0:
             self._verify_array_dimensions()
 
-    def __add__(self, other: Union[float, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __add__(self, other: Union[float, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__add__(other)
 
-    def __mul__(self, other: Union[float, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __mul__(self, other: Union[float, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__mul__(other)
 
-    def __matmul__(self, other: Union[List[Union[float, int]], 'DataArray', numpy.ndarray]) -> numpy.int64:
-        return self._data.__matmul__(other)
+    def __matmul__(self, other: Union[List[Union[float, int]], 'DataArray', numpy_ndarray_type]) -> numpy.int64:
+        return cast(numpy.int64, self._data.__matmul__(other))
 
-    def __pow__(self, other: Union[float, int]) -> numpy.ndarray:
+    def __pow__(self, other: Union[float, int]) -> numpy_ndarray_type:
         return self._data.__pow__(other)
 
-    def __sub__(self, other: Union[float, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __sub__(self, other: Union[float, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__sub__(other)
 
-    def __mod__(self, other: Union[float, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __mod__(self, other: Union[float, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__mod__(other)
 
-    def __floordiv__(self, other: Union[float, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __floordiv__(self, other: Union[float, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__floordiv__(other)
 
-    def __lshift__(self, other: Union[int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __lshift__(self, other: Union[int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__lshift__(other)
 
-    def __rshift__(self, other: Union[int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __rshift__(self, other: Union[int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__rshift__(other)
 
-    def __and__(self, other: Union[bool, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __and__(self, other: Union[bool, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__and__(other)
 
-    def __or__(self, other: Union[bool, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __or__(self, other: Union[bool, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__or__(other)
 
-    def __xor__(self, other: Union[bool, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __xor__(self, other: Union[bool, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__xor__(other)
 
-    def __truediv__(self, other: Union[float, int, 'DataArray', numpy.ndarray]) -> numpy.ndarray:
+    def __truediv__(self, other: Union[float, int, 'DataArray', numpy_ndarray_type]) -> numpy_ndarray_type:
         return self._data.__truediv__(other)
 
     def __getattr__(self, name: str) -> Any:
         if hasattr(np.ndarray, name):
             return getattr(self._data, name)
         raise AttributeError("DataArray has no attribute '{}'".format(name))
```

### Comparing `qilib-0.3.8/src/qilib/data_set/data_set.py` & `qilib-0.3.9/src/qilib/data_set/data_set.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/data_set/data_set_io_reader.py` & `qilib-0.3.9/src/qilib/data_set/data_set_io_reader.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/data_set/data_set_io_writer.py` & `qilib-0.3.9/src/qilib/data_set/data_set_io_writer.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/data_set/memory_data_set_io_factory.py` & `qilib-0.3.9/src/qilib/data_set/memory_data_set_io_factory.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/data_set/memory_data_set_io_reader.py` & `qilib-0.3.9/src/qilib/data_set/memory_data_set_io_reader.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/data_set/memory_data_set_io_writer.py` & `qilib-0.3.9/src/qilib/data_set/memory_data_set_io_writer.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/data_set/mongo_data_set_io.py` & `qilib-0.3.9/src/qilib/data_set/mongo_data_set_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 import base64
-from typing import Optional, Dict, Any, Union, List
+from typing import Optional, Dict, Any, Union, MutableMapping
 
 import numpy as np
-from bson import ObjectId
-from pymongo import MongoClient
+from bson.objectid import ObjectId
 from pymongo.change_stream import CollectionChangeStream
 from pymongo.errors import DuplicateKeyError
+from pymongo.mongo_client import MongoClient
 from qilib.data_set.type_aliases import EncodedNumpyArray
-from qilib.data_set.data_array import DataArray
+from qilib.data_set.data_array import DataArray, numpy_ndarray_type
 
 
 class DocumentNotFoundError(Exception):
     """ Error that is raised when document is not found."""
 
 
 class FieldNotUniqueError(Exception):
@@ -67,19 +67,19 @@
         Raises:
             DocumentNotFoundError: If document not found in database.
         """
 
         if name is None and document_id is None:
             raise DocumentNotFoundError("Neither 'name' nor 'document_id' were provided.")
 
-        self._client = MongoClient()
+        self._client = MongoClient()  # type: MongoClient[Any]
         self._db = self._client[database][collection]
         self._assert_name_field_is_unique()
 
-        query_dict = {}
+        query_dict: MutableMapping[str, Any] = {}
         if name is not None:
             query_dict['name'] = name
         if document_id is not None:
             query_dict['_id'] = ObjectId(document_id)
         document = self._db.find_one(query_dict)
         if document is None:
             if name is not None and document_id is None and create_if_not_found:
@@ -95,15 +95,15 @@
     def name(self) -> str:
         return self._name
 
     @property
     def id(self) -> str:
         return self._id
 
-    def watch(self) -> CollectionChangeStream:
+    def watch(self) -> CollectionChangeStream[Any]:
         """ Start watching the underlying document for updates.
 
         Returns:
             A blocking watch-cursor iterator that returns updates when available.
 
         """
         pipeline = [{'$match': {'fullDocument.name': self._name}}]
@@ -146,15 +146,15 @@
         self._db.update_one(
             {"name": self._name},
             {"$set": data,
              "$currentDate": {"lastModified": True}})
 
     @staticmethod
     def encode_numpy_array(
-            array: Union[np.ndarray, DataArray]) -> EncodedNumpyArray:
+            array: Union[numpy_ndarray_type, DataArray]) -> EncodedNumpyArray:
         """ Encode numpy array to store in database.
         Args:
             array: Numpy array to encode.
 
         Returns:
             The encoded array.
 
@@ -165,23 +165,24 @@
                 NumpyKeys.ARRAY: base64.b64encode(array.tobytes()).decode('ascii'),
                 NumpyKeys.DATA_TYPE: array.dtype.str,
                 NumpyKeys.SHAPE: list(array.shape),
             }
         }
 
     @staticmethod
-    def decode_numpy_array(encoded_array: Dict[str, Any]) -> np.ndarray:
+    def decode_numpy_array(encoded_array: Dict[str, Any]) -> numpy_ndarray_type:
         """ Decode a numpy array from database.
 
         Args:
             encoded_array: The encoded array to decode.
 
         Returns:
             The decoded array.
         """
+        array: numpy_ndarray_type
         content = encoded_array[NumpyKeys.CONTENT]
         array = np.frombuffer(base64.b64decode(content[NumpyKeys.ARRAY]),
                               dtype=np.dtype(content[NumpyKeys.DATA_TYPE])).reshape(content[NumpyKeys.SHAPE])
         # recreate the array to make it writable
         array = np.array(array)
 
         return array
```

### Comparing `qilib-0.3.8/src/qilib/data_set/mongo_data_set_io_reader.py` & `qilib-0.3.9/src/qilib/data_set/mongo_data_set_io_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,14 @@
         self._data_set.data_arrays[array['name']].label = array['label']
         self._data_set.data_arrays[array['name']].unit = array['unit']
 
         for i in range(len(np_array)):
             self._data_set.data_arrays[array['name']][i] = np_array[i]
 
     @staticmethod
-    def _update_worker(queue: Any, watcher: CollectionChangeStream) -> None:
+    def _update_worker(queue: Any, watcher: CollectionChangeStream[Any]) -> None:
         try:
             while True:
                 document = watcher.next()
                 queue.put(document)
         except (StopIteration, InvalidOperation, OperationFailure) as e:
             queue.put({MongoDataSetIOReader.THREAD_ERROR: e})
```

### Comparing `qilib-0.3.8/src/qilib/data_set/mongo_data_set_io_writer.py` & `qilib-0.3.9/src/qilib/data_set/mongo_data_set_io_writer.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/utils/memory_storage_queue.py` & `qilib-0.3.9/src/qilib/utils/memory_storage_queue.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/utils/python_json_structure.py` & `qilib-0.3.9/src/qilib/utils/python_json_structure.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/utils/serialization.py` & `qilib-0.3.9/src/qilib/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/utils/storage/interface.py` & `qilib-0.3.9/src/qilib/utils/storage/interface.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/utils/storage/memory.py` & `qilib-0.3.9/src/qilib/utils/storage/memory.py`

 * *Files identical despite different names*

### Comparing `qilib-0.3.8/src/qilib/utils/storage/mongo.py` & `qilib-0.3.9/src/qilib/utils/storage/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 from operator import itemgetter
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, cast
 
 import numpy as np
-from bson import ObjectId
 from bson.codec_options import TypeCodec, CodecOptions, TypeRegistry
-from pymongo import MongoClient
+from bson.objectid import ObjectId
+from pymongo.mongo_client import MongoClient
 from pymongo.errors import ServerSelectionTimeoutError
 
 from qilib.data_set.mongo_data_set_io import MongoDataSetIO, NumpyKeys
 from qilib.utils.serialization import Serializer, serializer as _serializer
 from qilib.utils.storage.interface import (NoDataAtKeyError,
                                            NodeAlreadyExistsError,
                                            StorageInterface,
                                            ConnectionTimeoutError)
 from qilib.utils.type_aliases import TagType
 
 
-class NumpyArrayCodec(TypeCodec):  # type: ignore
+class NumpyArrayCodec(TypeCodec):
 
     @property
     def python_type(self) -> Any:
         return np.ndarray
 
     def transform_python(self, value: Any) -> Any:
         return MongoDataSetIO.encode_numpy_array(value)
@@ -78,25 +78,31 @@
             connection_timeout: How long to try to connect to database before raising an error in milliseconds
         Raises:
             StorageTimeoutError: If connection to database has not been established before connection_timeout is reached
         """
         super().__init__(name)
 
         type_registry = TypeRegistry([NumpyArrayCodec()])
-        codec_options = CodecOptions(type_registry=type_registry)
-        self._client = MongoClient(host, port, serverSelectionTimeoutMS=connection_timeout)
+        codec_options = CodecOptions(type_registry=type_registry)  # type: CodecOptions[Any]
+        self._client = MongoClient(host, port, serverSelectionTimeoutMS=connection_timeout)  # type: MongoClient[Any]
         self._check_server_connection(connection_timeout)
         self._db = self._client.get_database(database or name, codec_options=codec_options)
         self._collection = self._db.get_collection('storage')
 
         if serializer is None:
             serializer = _serializer
         self._serialize = serializer.encode_data
         self._unserialize = serializer.decode_data
 
+    def __repr__(self) -> str:
+        return f'<{self.__class__.__name__} at 0x{id(self):x}: name {self._db.name}>'
+
+    def __str__(self) -> str:
+        return f'<{type(self).__name__}: name {self._db.name}>'
+
     def _check_server_connection(self, timeout: float) -> None:
         """ Check if connection has been established to database server."""
         try:
             self._client.server_info()
         except ServerSelectionTimeoutError as e:
             raise ConnectionTimeoutError(f'Failed to connect to Mongo database within {timeout} milliseconds') from e
 
@@ -106,17 +112,17 @@
         Returns:
             An ObjectID of the root node
         """
 
         node = self._collection.find_one({'tag': '', 'parent': {'$exists': False}})
 
         if node is not None:
-            return node['_id']
-        else:
-            return self._collection.insert_one({'tag': ''}).inserted_id
+            return cast(ObjectId, node['_id'])
+
+        return cast(ObjectId, self._collection.insert_one({'tag': ''}).inserted_id)
 
     def _retrieve_nodes_by_tag(self, tag: TagType, parent: ObjectId, document_limit: int = 0) -> TagType:
         """Traverse the tree and list the children of a given tag
 
         Args:
             tag: The node tag
             parent: The ObjectID of the node's parent
```

### Comparing `qilib-0.3.8/src/qilib.egg-info/PKG-INFO` & `qilib-0.3.9/src/qilib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: qilib
-Version: 0.3.8
+Version: 0.3.9
 Summary: Quantum Library for the Quantum Inspire platform
 Home-page: UNKNOWN
 Author: QuantumInspire
 License: Other/Proprietary License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 [![Coverage Status](https://coveralls.io/repos/github/QuTech-Delft/qilib/badge.svg?branch=dev)](https://coveralls.io/github/QuTech-Delft/qilib?branch=dev)
```

### Comparing `qilib-0.3.8/src/qilib.egg-info/SOURCES.txt` & `qilib-0.3.9/src/qilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

