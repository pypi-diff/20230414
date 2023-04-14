# Comparing `tmp/xmlschema-2.2.2.tar.gz` & `tmp/xmlschema-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlschema-2.2.2.tar", last modified: Sun Mar  5 21:10:04 2023, max compression
+gzip compressed data, was "xmlschema-2.2.3.tar", last modified: Fri Apr 14 13:52:42 2023, max compression
```

## Comparing `xmlschema-2.2.2.tar` & `xmlschema-2.2.3.tar`

### file list

```diff
@@ -1,486 +1,490 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.662572 xmlschema-2.2.2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 20:36:43.000000 xmlschema-2.2.2/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24632 2023-03-05 20:30:24.000000 xmlschema-2.2.2/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.2.2/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.2.2/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7326 2023-03-05 21:10:04.662572 xmlschema-2.2.2/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.2.2/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.554571 xmlschema-2.2.2/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.2.2/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.2.2/doc/api.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.2.2/doc/components.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-03-05 20:30:24.000000 xmlschema-2.2.2/doc/conf.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.2.2/doc/converters.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.2.2/doc/extras.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.2.2/doc/features.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.2.2/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.2.2/doc/intro.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.2.2/doc/testing.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.2.2/doc/usage.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.2.2/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-02-06 06:20:42.000000 xmlschema-2.2.2/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-03-05 21:10:04.663572 xmlschema-2.2.2/setup.cfg
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2714 2023-03-05 20:30:24.000000 xmlschema-2.2.2/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.559571 xmlschema-2.2.2/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.2.2/tests/__init__.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/check_memory.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.538571 xmlschema-2.2.2/tests/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.560571 xmlschema-2.2.2/tests/templates/demo/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/demo/demo_type_filter_test.jinja
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.562571 xmlschema-2.2.2/tests/templates/filters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/filters/name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/filters/namespace_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/filters/python_type_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/filters/qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/filters/sort_types_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.2.2/tests/templates/filters/type_name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/filters/type_qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/templates/filters/unknown_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.2.2/tests/templates/filters/wrong-template.jinja
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_all.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.562571 xmlschema-2.2.2/tests/test_cases/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.539571 xmlschema-2.2.2/tests/test_cases/examples/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.567571 xmlschema-2.2.2/tests/test_cases/examples/collection/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection-default.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-03-05 21:09:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection3bis.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection3bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection4.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.2.2/tests/test_cases/examples/collection/collection5.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.567571 xmlschema-2.2.2/tests/test_cases/examples/stockquote/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/examples/stockquote/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/examples/stockquote/stockquote.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.572571 xmlschema-2.2.2/tests/test_cases/examples/vehicles/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/bikes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/cars.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-1_error.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-3_errors.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-max.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles2.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles2.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.540571 xmlschema-2.2.2/tests/test_cases/features/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.572571 xmlschema-2.2.2/tests/test_cases/features/attributes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/attributes/default_attributes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.572571 xmlschema-2.2.2/tests/test_cases/features/builtins/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/builtins/builtins.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/builtins/builtins.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.574571 xmlschema-2.2.2/tests/test_cases/features/decoder/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.2.2/tests/test_cases/features/decoder/data.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/decoder/data2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.2.2/tests/test_cases/features/decoder/data3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/features/decoder/data4-mixed.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.2.2/tests/test_cases/features/decoder/long-sequence-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/features/decoder/mixed-content.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.2.2/tests/test_cases/features/decoder/simple-types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.576571 xmlschema-2.2.2/tests/test_cases/features/derivations/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/derivations/complex-extensions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2020-09-13 19:12:09.000000 xmlschema-2.2.2/tests/test_cases/features/derivations/invalid_enumeration_restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2020-08-14 19:07:25.000000 xmlschema-2.2.2/tests/test_cases/features/derivations/invalid_restrictions1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1718 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/derivations/invalid_restrictions2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/derivations/list_types.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/derivations/list_types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.577571 xmlschema-2.2.2/tests/test_cases/features/elements/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/elements/test_alternatives-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/elements/type_alternatives.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.581571 xmlschema-2.2.2/tests/test_cases/features/models/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/billion_laughs_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/circular_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/illegal-attributes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/illegal-declarations.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/illegal-occurs.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/invalid_models1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/invalid_models2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/model1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.2.2/tests/test_cases/features/models/models.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/other-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/models/recursive-groups.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.2.2/tests/test_cases/features/models/valid_model1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.589571 xmlschema-2.2.2/tests/test_cases/features/namespaces/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/chameleon1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/chameleon2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/chameleon3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/default_ns_invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/default_ns_valid1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/default_ns_valid2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case4-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case4-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case4a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case4b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case5a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case5b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case5c.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case1bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case2bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case5.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case6.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/included3-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/included4-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/included5-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/namespaces/included6-invalid.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.589571 xmlschema-2.2.2/tests/test_cases/features/patterns/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/features/patterns/patterns.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.2.2/tests/test_cases/features/patterns/patterns.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.592571 xmlschema-2.2.2/tests/test_cases/features/wsdl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2091 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.544571 xmlschema-2.2.2/tests/test_cases/issues/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.592571 xmlschema-2.2.2/tests/test_cases/issues/issue_008/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_008/issue_008.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_008/issue_008.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.592571 xmlschema-2.2.2/tests/test_cases/issues/issue_009/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_009/issue_009.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.594571 xmlschema-2.2.2/tests/test_cases/issues/issue_013/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_013/issue_013-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_013/issue_013-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_013/issue_013-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_013/issue_013.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_013/issue_013.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.594571 xmlschema-2.2.2/tests/test_cases/issues/issue_014/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_014/issue014.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.595571 xmlschema-2.2.2/tests/test_cases/issues/issue_018/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_018/issue_018-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_018/issue_018.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.596572 xmlschema-2.2.2/tests/test_cases/issues/issue_022/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_022/README.md
--rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_022/xml_string_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_022/xml_string_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_022/xsd_string.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.597571 xmlschema-2.2.2/tests/test_cases/issues/issue_026/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_026/issue_026-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_026/issue_026-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_026/issue_026-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_026/issue_026.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.598571 xmlschema-2.2.2/tests/test_cases/issues/issue_028/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_028/issue_028-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_028/issue_028-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_028/issue_028.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.599572 xmlschema-2.2.2/tests/test_cases/issues/issue_029/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_029/issue_029-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_029/issue_029-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_029/issue_029-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_029/issue_029.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.599572 xmlschema-2.2.2/tests/test_cases/issues/issue_035/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_035/dates.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_035/dates.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.600571 xmlschema-2.2.2/tests/test_cases/issues/issue_041/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_041/issue_041.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_041/issue_041.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.600571 xmlschema-2.2.2/tests/test_cases/issues/issue_045/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_045/issue_045.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.601571 xmlschema-2.2.2/tests/test_cases/issues/issue_046/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_046/issue_046.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_046/issue_046.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.602572 xmlschema-2.2.2/tests/test_cases/issues/issue_051/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_051/issue_051.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_051/issue_051.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.603572 xmlschema-2.2.2/tests/test_cases/issues/issue_073/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_073/issue_073-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_073/issue_073-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_073/issue_073.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.604571 xmlschema-2.2.2/tests/test_cases/issues/issue_086/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_086/issue_086-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_086/issue_086-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_086/issue_086.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.604571 xmlschema-2.2.2/tests/test_cases/issues/issue_105/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_105/issue_105.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.605572 xmlschema-2.2.2/tests/test_cases/issues/issue_111/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_111/issue_111.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.605572 xmlschema-2.2.2/tests/test_cases/issues/issue_115/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_115/Rotation.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.606572 xmlschema-2.2.2/tests/test_cases/issues/issue_171/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_171/issue_171.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_171/issue_171b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_171/issue_171c.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.606572 xmlschema-2.2.2/tests/test_cases/issues/issue_187/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_187/issue_187_1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_187/issue_187_2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.607571 xmlschema-2.2.2/tests/test_cases/issues/issue_190/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_190/issue_190.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_190/issue_190.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.608572 xmlschema-2.2.2/tests/test_cases/issues/issue_200/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_200/issue_200.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_200/issue_200.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.608572 xmlschema-2.2.2/tests/test_cases/issues/issue_203/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_203/issue_203.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_203/issue_203.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_203/issue_203alt.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.610571 xmlschema-2.2.2/tests/test_cases/issues/issue_204/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_204/issue_204.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_204/issue_204_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_204/issue_204_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_204/issue_204_3.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.610571 xmlschema-2.2.2/tests/test_cases/issues/issue_208/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_208/issue_208.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_208/issue_208.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.611571 xmlschema-2.2.2/tests/test_cases/issues/issue_222/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_222/issue_222.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_222/issue_222.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.611571 xmlschema-2.2.2/tests/test_cases/issues/issue_223/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_223/issue_223.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_223/issue_223.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.543571 xmlschema-2.2.2/tests/test_cases/issues/issue_237/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.612572 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.613572 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.614571 xmlschema-2.2.2/tests/test_cases/issues/issue_243/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_243/issue_243.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_243/issue_243.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.614571 xmlschema-2.2.2/tests/test_cases/issues/issue_245/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_245/issue_245-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_245/issue_245.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_245/issue_245.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.615572 xmlschema-2.2.2/tests/test_cases/issues/issue_259/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_259/issue_259-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_259/issue_259-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.616572 xmlschema-2.2.2/tests/test_cases/issues/issue_265/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_265/issue_265-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.618572 xmlschema-2.2.2/tests/test_cases/issues/issue_266/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266-2.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266b-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266b-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.618572 xmlschema-2.2.2/tests/test_cases/issues/issue_273/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_273/issue_273.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_273/issue_273.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.619572 xmlschema-2.2.2/tests/test_cases/issues/issue_276/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_276/dummy.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_276/schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.619572 xmlschema-2.2.2/tests/test_cases/issues/issue_298/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_298/issue_298-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_298/issue_298-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_298/issue_298.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.621572 xmlschema-2.2.2/tests/test_cases/issues/issue_306/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_306/issue_306-alt.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_306/issue_306-invalid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_306/issue_306-valid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_306/issue_306.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.621572 xmlschema-2.2.2/tests/test_cases/issues/issue_311/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_311/correct_no_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_311/incorrect_with_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.622572 xmlschema-2.2.2/tests/test_cases/issues/issue_314/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_314/issue_314.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_314/issue_314.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.624572 xmlschema-2.2.2/tests/test_cases/issues/issue_315/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315-3.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315-4.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315-5.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315_simple.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.624572 xmlschema-2.2.2/tests/test_cases/issues/issue_322/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_322/issue_322.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_322/issue_322.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.626572 xmlschema-2.2.2/tests/test_cases/issues/issue_324/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_324/issue_324-invalid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_324/issue_324-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_324/issue_324.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_324/issue_324a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_324/issue_324b.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.627572 xmlschema-2.2.2/tests/test_cases/issues/issue_334/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_334/issue_334.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_334/issue_334.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.2.2/tests/test_cases/issues/issue_334/issue_334.zip
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.628572 xmlschema-2.2.2/tests/test_cases/mypy/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.2.2/tests/test_cases/mypy/extra_validator.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2021-11-11 15:30:24.000000 xmlschema-2.2.2/tests/test_cases/mypy/schema_source.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.2.2/tests/test_cases/mypy/simple_types.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.630572 xmlschema-2.2.2/tests/test_cases/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/resources/dummy file #2.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/resources/dummy file.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/resources/malformed.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/resources/unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/resources/unused_external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.2.2/tests/test_cases/resources/unused_unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.2.2/tests/test_cases/resources/with_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     6165 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_cases/testfiles
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.2.2/tests/test_cli.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.2.2/tests/test_codegen.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.2.2/tests/test_converters.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.2.2/tests/test_dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24554 2023-02-06 06:20:42.000000 xmlschema-2.2.2/tests/test_documents.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.2.2/tests/test_files.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_helpers.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.2.2/tests/test_memory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.2.2/tests/test_namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 20:33:42.000000 xmlschema-2.2.2/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    70653 2023-02-06 06:20:42.000000 xmlschema-2.2.2/tests/test_resources.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.2.2/tests/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3600 2022-05-20 20:00:14.000000 xmlschema-2.2.2/tests/test_translations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2397 2022-05-20 16:16:20.000000 xmlschema-2.2.2/tests/test_typing.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.2.2/tests/test_validation.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    27317 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_w3c_suite.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    43436 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/test_wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.2.2/tests/test_xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.631572 xmlschema-2.2.2/tests/validation/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.2.2/tests/validation/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    62578 2023-02-11 10:41:50.000000 xmlschema-2.2.2/tests/validation/test_decoding.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validation/test_encoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16337 2022-10-01 13:42:01.000000 xmlschema-2.2.2/tests/validation/test_validation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.638572 xmlschema-2.2.2/tests/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.2.2/tests/validators/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.2.2/tests/validators/test_builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.2.2/tests/validators/test_complex_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.2.2/tests/validators/test_elements.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_exceptions.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_facets.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.2.2/tests/validators/test_global_maps.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    13430 2021-10-20 14:14:48.000000 xmlschema-2.2.2/tests/validators/test_groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.2.2/tests/validators/test_identities.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    53152 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_notations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41506 2022-10-01 13:42:01.000000 xmlschema-2.2.2/tests/validators/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_simple_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_wildcards.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.2.2/tests/validators/test_xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1571 2023-03-05 20:30:24.000000 xmlschema-2.2.2/tox.ini
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.642572 xmlschema-2.2.2/xmlschema/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-03-05 20:30:24.000000 xmlschema-2.2.2/xmlschema/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5515 2023-03-05 20:37:49.000000 xmlschema-2.2.2/xmlschema/aliases.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11662 2022-07-18 14:19:15.000000 xmlschema-2.2.2/xmlschema/cli.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.646572 xmlschema-2.2.2/xmlschema/converters/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.2.2/xmlschema/converters/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 20:40:13.000000 xmlschema-2.2.2/xmlschema/converters/abdera.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 20:38:30.000000 xmlschema-2.2.2/xmlschema/converters/badgerfish.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 20:40:12.000000 xmlschema-2.2.2/xmlschema/converters/columnar.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-03-05 20:40:11.000000 xmlschema-2.2.2/xmlschema/converters/default.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 20:40:12.000000 xmlschema-2.2.2/xmlschema/converters/jsonml.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 20:40:12.000000 xmlschema-2.2.2/xmlschema/converters/parker.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 20:40:12.000000 xmlschema-2.2.2/xmlschema/converters/unordered.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 20:39:06.000000 xmlschema-2.2.2/xmlschema/dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35488 2023-02-06 06:20:42.000000 xmlschema-2.2.2/xmlschema/documents.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.2.2/xmlschema/exceptions.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.647572 xmlschema-2.2.2/xmlschema/extras/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.2.2/xmlschema/extras/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    21923 2023-02-11 09:04:58.000000 xmlschema-2.2.2/xmlschema/extras/codegen.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.546571 xmlschema-2.2.2/xmlschema/extras/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.647572 xmlschema-2.2.2/xmlschema/extras/templates/python/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.2.2/xmlschema/extras/templates/python/bindings.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.2.2/xmlschema/extras/templates/python/sample.py.jinja
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    23802 2022-06-24 14:13:22.000000 xmlschema-2.2.2/xmlschema/extras/wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11097 2022-08-26 15:33:28.000000 xmlschema-2.2.2/xmlschema/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.2.2/xmlschema/limits.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.546571 xmlschema-2.2.2/xmlschema/locale/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.546571 xmlschema-2.2.2/xmlschema/locale/en/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.648572 xmlschema-2.2.2/xmlschema/locale/en/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.2.2/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.2.2/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.546571 xmlschema-2.2.2/xmlschema/locale/it/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.649572 xmlschema-2.2.2/xmlschema/locale/it/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.2.2/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.2.2/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.547571 xmlschema-2.2.2/xmlschema/locale/ru/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.649572 xmlschema-2.2.2/xmlschema/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.2.2/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.2.2/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8827 2020-12-23 12:38:37.000000 xmlschema-2.2.2/xmlschema/names.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.2.2/xmlschema/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.2.2/xmlschema/py.typed
--rw-r--r--   0 brunato   (1000) brunato   (1000)    55269 2023-02-11 10:41:50.000000 xmlschema-2.2.2/xmlschema/resources.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.548571 xmlschema-2.2.2/xmlschema/schemas/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.650572 xmlschema-2.2.2/xmlschema/schemas/HFP/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.650572 xmlschema-2.2.2/xmlschema/schemas/VC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/VC/XMLSchema-versioning.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.651572 xmlschema-2.2.2/xmlschema/schemas/WSDL/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/WSDL/soap-encoding.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/WSDL/soap-envelope.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/WSDL/wsdl-soap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/WSDL/wsdl.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.652572 xmlschema-2.2.2/xmlschema/schemas/XHTML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/XHTML/xhtml1-strict.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.652572 xmlschema-2.2.2/xmlschema/schemas/XLINK/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/XLINK/xlink.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.652572 xmlschema-2.2.2/xmlschema/schemas/XML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/XML/xml_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.653572 xmlschema-2.2.2/xmlschema/schemas/XSD_1.0/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.2.2/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/XSD_1.0/datatypes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.654572 xmlschema-2.2.2/xmlschema/schemas/XSD_1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.2.2/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/XSD_1.1/datatypes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.2.2/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.654572 xmlschema-2.2.2/xmlschema/schemas/XSI/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.2.2/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.656572 xmlschema-2.2.2/xmlschema/testing/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2109 2022-03-07 13:26:41.000000 xmlschema-2.2.2/xmlschema/testing/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    29735 2022-07-18 14:19:15.000000 xmlschema-2.2.2/xmlschema/testing/_builders.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7943 2022-07-18 14:19:15.000000 xmlschema-2.2.2/xmlschema/testing/_case_class.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     9436 2022-03-07 13:26:41.000000 xmlschema-2.2.2/xmlschema/testing/_factory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.2.2/xmlschema/testing/_helpers.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4884 2022-03-07 13:26:41.000000 xmlschema-2.2.2/xmlschema/testing/_observers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.2.2/xmlschema/translation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.662572 xmlschema-2.2.2/xmlschema/validators/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.2.2/xmlschema/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-03-05 20:40:29.000000 xmlschema-2.2.2/xmlschema/validators/assertions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.2.2/xmlschema/validators/attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.2.2/xmlschema/validators/builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-03-05 20:30:24.000000 xmlschema-2.2.2/xmlschema/validators/complex_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64166 2023-03-05 20:40:54.000000 xmlschema-2.2.2/xmlschema/validators/elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14970 2023-03-05 20:40:54.000000 xmlschema-2.2.2/xmlschema/validators/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-03-05 20:41:16.000000 xmlschema-2.2.2/xmlschema/validators/facets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33019 2023-03-05 20:30:24.000000 xmlschema-2.2.2/xmlschema/validators/global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64939 2023-03-05 20:41:28.000000 xmlschema-2.2.2/xmlschema/validators/groups.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.2.2/xmlschema/validators/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 20:41:54.000000 xmlschema-2.2.2/xmlschema/validators/identities.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    19493 2022-06-23 20:06:57.000000 xmlschema-2.2.2/xmlschema/validators/models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.2.2/xmlschema/validators/notations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6627 2022-09-08 10:16:11.000000 xmlschema-2.2.2/xmlschema/validators/particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)   103598 2023-02-06 06:20:42.000000 xmlschema-2.2.2/xmlschema/validators/schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    61468 2023-02-06 06:20:42.000000 xmlschema-2.2.2/xmlschema/validators/simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.2.2/xmlschema/validators/wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 20:42:55.000000 xmlschema-2.2.2/xmlschema/validators/xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.2.2/xmlschema/xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-03-05 21:10:04.644572 xmlschema-2.2.2/xmlschema.egg-info/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7326 2023-03-05 21:10:04.000000 xmlschema-2.2.2/xmlschema.egg-info/PKG-INFO
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    16790 2023-03-05 21:10:04.000000 xmlschema-2.2.2/xmlschema.egg-info/SOURCES.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-03-05 21:10:04.000000 xmlschema-2.2.2/xmlschema.egg-info/dependency_links.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-03-05 21:10:04.000000 xmlschema-2.2.2/xmlschema.egg-info/entry_points.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-03-05 21:10:04.000000 xmlschema-2.2.2/xmlschema.egg-info/requires.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-03-05 21:10:04.000000 xmlschema-2.2.2/xmlschema.egg-info/top_level.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.466140 xmlschema-2.2.3/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-2.2.3/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24835 2023-04-14 13:49:05.000000 xmlschema-2.2.3/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.2.3/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.2.3/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7377 2023-04-14 13:52:42.466140 xmlschema-2.2.3/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.2.3/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.390139 xmlschema-2.2.3/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.2.3/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.2.3/doc/api.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.2.3/doc/components.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-04-14 13:49:05.000000 xmlschema-2.2.3/doc/conf.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.2.3/doc/converters.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.2.3/doc/extras.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.2.3/doc/features.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.2.3/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.2.3/doc/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.2.3/doc/testing.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.2.3/doc/usage.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.2.3/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-02-06 06:20:42.000000 xmlschema-2.2.3/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-04-14 13:52:42.466140 xmlschema-2.2.3/setup.cfg
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2764 2023-04-14 13:49:05.000000 xmlschema-2.2.3/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.394140 xmlschema-2.2.3/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.2.3/tests/__init__.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/check_memory.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.377139 xmlschema-2.2.3/tests/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.395140 xmlschema-2.2.3/tests/templates/demo/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/demo/demo_type_filter_test.jinja
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.396139 xmlschema-2.2.3/tests/templates/filters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/namespace_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/python_type_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/sort_types_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.2.3/tests/templates/filters/type_name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/type_qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/templates/filters/unknown_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/wrong-template.jinja
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_all.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.396139 xmlschema-2.2.3/tests/test_cases/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.377139 xmlschema-2.2.3/tests/test_cases/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.399140 xmlschema-2.2.3/tests/test_cases/examples/collection/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection-default.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-04-14 13:51:59.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection5.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.399140 xmlschema-2.2.3/tests/test_cases/examples/stockquote/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.402140 xmlschema-2.2.3/tests/test_cases/examples/vehicles/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/bikes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/cars.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-1_error.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-3_errors.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-max.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles2.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.379140 xmlschema-2.2.3/tests/test_cases/features/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.402140 xmlschema-2.2.3/tests/test_cases/features/attributes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.403140 xmlschema-2.2.3/tests/test_cases/features/builtins/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.404140 xmlschema-2.2.3/tests/test_cases/features/decoder/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data4-mixed.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/long-sequence-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/mixed-content.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/simple-types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.405140 xmlschema-2.2.3/tests/test_cases/features/derivations/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/complex-extensions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2020-09-13 19:12:09.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_enumeration_restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1718 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/list_types.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/list_types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.406140 xmlschema-2.2.3/tests/test_cases/features/elements/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/elements/test_alternatives-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.409140 xmlschema-2.2.3/tests/test_cases/features/models/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/billion_laughs_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/circular_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/illegal-attributes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/illegal-declarations.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/illegal-occurs.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/invalid_models1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/invalid_models2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/model1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.2.3/tests/test_cases/features/models/models.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/other-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/recursive-groups.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.2.3/tests/test_cases/features/models/valid_model1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.414140 xmlschema-2.2.3/tests/test_cases/features/namespaces/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/chameleon1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/chameleon2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/chameleon3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/default_ns_invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/default_ns_valid1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/default_ns_valid2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case5a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case5b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case5c.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case1bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case5.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case6.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included3-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included4-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included5-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included6-invalid.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.414140 xmlschema-2.2.3/tests/test_cases/features/patterns/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.415140 xmlschema-2.2.3/tests/test_cases/features/wsdl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2091 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.383139 xmlschema-2.2.3/tests/test_cases/issues/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.416140 xmlschema-2.2.3/tests/test_cases/issues/issue_008/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_008/issue_008.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_008/issue_008.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.416140 xmlschema-2.2.3/tests/test_cases/issues/issue_009/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_009/issue_009.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.417140 xmlschema-2.2.3/tests/test_cases/issues/issue_013/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.417140 xmlschema-2.2.3/tests/test_cases/issues/issue_014/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_014/issue014.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.418140 xmlschema-2.2.3/tests/test_cases/issues/issue_018/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_018/issue_018-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_018/issue_018.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.419140 xmlschema-2.2.3/tests/test_cases/issues/issue_022/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/README.md
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/xml_string_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/xml_string_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/xsd_string.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.420140 xmlschema-2.2.3/tests/test_cases/issues/issue_026/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.420140 xmlschema-2.2.3/tests/test_cases/issues/issue_028/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_028/issue_028-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_028/issue_028-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_028/issue_028.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.421140 xmlschema-2.2.3/tests/test_cases/issues/issue_029/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.421140 xmlschema-2.2.3/tests/test_cases/issues/issue_035/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.422140 xmlschema-2.2.3/tests/test_cases/issues/issue_041/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_041/issue_041.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_041/issue_041.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.422140 xmlschema-2.2.3/tests/test_cases/issues/issue_045/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_045/issue_045.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.423140 xmlschema-2.2.3/tests/test_cases/issues/issue_046/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_046/issue_046.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_046/issue_046.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.423140 xmlschema-2.2.3/tests/test_cases/issues/issue_051/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_051/issue_051.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_051/issue_051.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.424140 xmlschema-2.2.3/tests/test_cases/issues/issue_073/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.424140 xmlschema-2.2.3/tests/test_cases/issues/issue_086/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.424140 xmlschema-2.2.3/tests/test_cases/issues/issue_105/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_105/issue_105.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.425140 xmlschema-2.2.3/tests/test_cases/issues/issue_111/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.425140 xmlschema-2.2.3/tests/test_cases/issues/issue_115/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_115/Rotation.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.426140 xmlschema-2.2.3/tests/test_cases/issues/issue_171/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171c.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.426140 xmlschema-2.2.3/tests/test_cases/issues/issue_187/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.427140 xmlschema-2.2.3/tests/test_cases/issues/issue_190/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_190/issue_190.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_190/issue_190.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.427140 xmlschema-2.2.3/tests/test_cases/issues/issue_200/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_200/issue_200.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_200/issue_200.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.428140 xmlschema-2.2.3/tests/test_cases/issues/issue_203/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203alt.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.429140 xmlschema-2.2.3/tests/test_cases/issues/issue_204/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204_3.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.429140 xmlschema-2.2.3/tests/test_cases/issues/issue_208/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_208/issue_208.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_208/issue_208.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.429140 xmlschema-2.2.3/tests/test_cases/issues/issue_222/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_222/issue_222.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_222/issue_222.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.430140 xmlschema-2.2.3/tests/test_cases/issues/issue_223/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_223/issue_223.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_223/issue_223.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.381139 xmlschema-2.2.3/tests/test_cases/issues/issue_237/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.430140 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.431140 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.431140 xmlschema-2.2.3/tests/test_cases/issues/issue_243/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_243/issue_243.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_243/issue_243.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.432140 xmlschema-2.2.3/tests/test_cases/issues/issue_245/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.432140 xmlschema-2.2.3/tests/test_cases/issues/issue_259/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.433140 xmlschema-2.2.3/tests/test_cases/issues/issue_265/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.434140 xmlschema-2.2.3/tests/test_cases/issues/issue_266/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-2.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.434140 xmlschema-2.2.3/tests/test_cases/issues/issue_273/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_273/issue_273.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_273/issue_273.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.435140 xmlschema-2.2.3/tests/test_cases/issues/issue_276/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_276/dummy.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_276/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.435140 xmlschema-2.2.3/tests/test_cases/issues/issue_298/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.436140 xmlschema-2.2.3/tests/test_cases/issues/issue_306/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-alt.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-invalid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-valid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.437140 xmlschema-2.2.3/tests/test_cases/issues/issue_311/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_311/correct_no_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_311/incorrect_with_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.437140 xmlschema-2.2.3/tests/test_cases/issues/issue_314/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_314/issue_314.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_314/issue_314.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.439140 xmlschema-2.2.3/tests/test_cases/issues/issue_315/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-3.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-4.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-5.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315_simple.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.439140 xmlschema-2.2.3/tests/test_cases/issues/issue_322/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_322/issue_322.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_322/issue_322.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.440140 xmlschema-2.2.3/tests/test_cases/issues/issue_324/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324-invalid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324b.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.441140 xmlschema-2.2.3/tests/test_cases/issues/issue_334/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.zip
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.442140 xmlschema-2.2.3/tests/test_cases/issues/issue_341/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341-ext.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.442140 xmlschema-2.2.3/tests/test_cases/mypy/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.2.3/tests/test_cases/mypy/extra_validator.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/mypy/schema_source.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/mypy/simple_types.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.444140 xmlschema-2.2.3/tests/test_cases/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/dummy file #2.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/dummy file.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/malformed.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/resources/unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/unused_external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/resources/unused_unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/with_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     6165 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/testfiles
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.2.3/tests/test_cli.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_codegen.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.2.3/tests/test_dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24554 2023-02-06 06:20:42.000000 xmlschema-2.2.3/tests/test_documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.2.3/tests/test_files.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_helpers.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.2.3/tests/test_memory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 21:16:57.000000 xmlschema-2.2.3/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    70653 2023-02-06 06:20:42.000000 xmlschema-2.2.3/tests/test_resources.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3600 2022-05-20 20:00:14.000000 xmlschema-2.2.3/tests/test_translations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2397 2022-05-20 16:16:20.000000 xmlschema-2.2.3/tests/test_typing.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_validation.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    27317 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_w3c_suite.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    43436 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.445140 xmlschema-2.2.3/tests/validation/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.2.3/tests/validation/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66088 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/validation/test_decoding.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validation/test_encoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16337 2022-10-01 13:42:01.000000 xmlschema-2.2.3/tests/validation/test_validation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.449140 xmlschema-2.2.3/tests/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.2.3/tests/validators/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.2.3/tests/validators/test_builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.2.3/tests/validators/test_complex_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/validators/test_elements.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_exceptions.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_facets.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.2.3/tests/validators/test_global_maps.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    13430 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/validators/test_groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.2.3/tests/validators/test_identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/validators/test_models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_notations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41506 2022-10-01 13:42:01.000000 xmlschema-2.2.3/tests/validators/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_simple_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_wildcards.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1632 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.451140 xmlschema-2.2.3/xmlschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5515 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/aliases.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11662 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/cli.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.454140 xmlschema-2.2.3/xmlschema/converters/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/converters/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/abdera.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/badgerfish.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/columnar.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/default.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/jsonml.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/parker.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/unordered.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35488 2023-02-06 06:20:42.000000 xmlschema-2.2.3/xmlschema/documents.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.2.3/xmlschema/exceptions.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.455140 xmlschema-2.2.3/xmlschema/extras/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.2.3/xmlschema/extras/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    21923 2023-02-11 09:04:58.000000 xmlschema-2.2.3/xmlschema/extras/codegen.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/extras/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.455140 xmlschema-2.2.3/xmlschema/extras/templates/python/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/extras/templates/python/bindings.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.2.3/xmlschema/extras/templates/python/sample.py.jinja
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    23802 2022-06-24 14:13:22.000000 xmlschema-2.2.3/xmlschema/extras/wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11097 2022-08-26 15:33:28.000000 xmlschema-2.2.3/xmlschema/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.2.3/xmlschema/limits.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/locale/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/locale/en/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.456140 xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/locale/it/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.456140 xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.385140 xmlschema-2.2.3/xmlschema/locale/ru/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.457140 xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8827 2020-12-23 12:38:37.000000 xmlschema-2.2.3/xmlschema/names.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.2.3/xmlschema/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.2.3/xmlschema/py.typed
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    55658 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/resources.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.386139 xmlschema-2.2.3/xmlschema/schemas/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.457140 xmlschema-2.2.3/xmlschema/schemas/HFP/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.457140 xmlschema-2.2.3/xmlschema/schemas/VC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/VC/XMLSchema-versioning.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.458140 xmlschema-2.2.3/xmlschema/schemas/WSDL/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-encoding.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-envelope.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl-soap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.458140 xmlschema-2.2.3/xmlschema/schemas/XHTML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XHTML/xhtml1-strict.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.459140 xmlschema-2.2.3/xmlschema/schemas/XLINK/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XLINK/xlink.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.459140 xmlschema-2.2.3/xmlschema/schemas/XML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XML/xml_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.459140 xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/datatypes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.460140 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/datatypes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.460140 xmlschema-2.2.3/xmlschema/schemas/XSI/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.462140 xmlschema-2.2.3/xmlschema/testing/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2109 2022-03-07 13:26:41.000000 xmlschema-2.2.3/xmlschema/testing/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    29735 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/testing/_builders.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7943 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/testing/_case_class.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     9436 2022-03-07 13:26:41.000000 xmlschema-2.2.3/xmlschema/testing/_factory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.2.3/xmlschema/testing/_helpers.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4884 2022-03-07 13:26:41.000000 xmlschema-2.2.3/xmlschema/testing/_observers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.2.3/xmlschema/translation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.465140 xmlschema-2.2.3/xmlschema/validators/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.2.3/xmlschema/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/assertions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.2.3/xmlschema/validators/attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.2.3/xmlschema/validators/builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-03-05 20:30:24.000000 xmlschema-2.2.3/xmlschema/validators/complex_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64166 2023-03-28 06:38:11.000000 xmlschema-2.2.3/xmlschema/validators/elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14970 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/facets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33050 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/validators/global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    61540 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/validators/groups.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.2.3/xmlschema/validators/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23474 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/validators/models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.2.3/xmlschema/validators/notations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6627 2022-09-08 10:16:11.000000 xmlschema-2.2.3/xmlschema/validators/particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)   103598 2023-02-06 06:20:42.000000 xmlschema-2.2.3/xmlschema/validators/schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    61468 2023-02-06 06:20:42.000000 xmlschema-2.2.3/xmlschema/validators/simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.2.3/xmlschema/validators/wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.2.3/xmlschema/xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.453140 xmlschema-2.2.3/xmlschema.egg-info/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7377 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/PKG-INFO
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    16938 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/entry_points.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/requires.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/top_level.txt
```

### Comparing `xmlschema-2.2.2/CHANGELOG.rst` & `xmlschema-2.2.3/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v2.2.3`_ (2023-04-14)
+======================
+* Add support for Python 3.12
+* Detach content iteration methods from ModelVisitor
+
 `v2.2.2`_ (2023-03-05)
 ======================
 * Fix mixed content extension with empty content (issue #337)
 * Fix lru_cache() usage on global maps caching
 
 `v2.2.1`_ (2023-02-11)
 ======================
@@ -606,7 +611,8 @@
 .. _v2.0.3: https://github.com/brunato/xmlschema/compare/v2.0.2...v2.0.3
 .. _v2.0.4: https://github.com/brunato/xmlschema/compare/v2.0.3...v2.0.4
 .. _v2.1.0: https://github.com/brunato/xmlschema/compare/v2.0.4...v2.1.0
 .. _v2.1.1: https://github.com/brunato/xmlschema/compare/v2.1.0...v2.1.1
 .. _v2.2.0: https://github.com/brunato/xmlschema/compare/v2.1.1...v2.2.0
 .. _v2.2.1: https://github.com/brunato/xmlschema/compare/v2.2.0...v2.2.1
 .. _v2.2.2: https://github.com/brunato/xmlschema/compare/v2.2.1...v2.2.2
+.. _v2.2.3: https://github.com/brunato/xmlschema/compare/v2.2.2...v2.2.3
```

### Comparing `xmlschema-2.2.2/LICENSE` & `xmlschema-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/PKG-INFO` & `xmlschema-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.2.2
+Version: 2.2.3
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Provides-Extra: codegen
 Provides-Extra: dev
```

### Comparing `xmlschema-2.2.2/README.rst` & `xmlschema-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/Makefile` & `xmlschema-2.2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/api.rst` & `xmlschema-2.2.3/doc/api.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/components.rst` & `xmlschema-2.2.3/doc/components.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/conf.py` & `xmlschema-2.2.3/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '2.2'
 # The full version, including alpha/beta/rc tags.
-release = '2.2.2'
+release = '2.2.3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
```

### Comparing `xmlschema-2.2.2/doc/converters.rst` & `xmlschema-2.2.3/doc/converters.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/extras.rst` & `xmlschema-2.2.3/doc/extras.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/features.rst` & `xmlschema-2.2.3/doc/features.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/testing.rst` & `xmlschema-2.2.3/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/doc/usage.rst` & `xmlschema-2.2.3/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/setup.py` & `xmlschema-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with Path(__file__).parent.joinpath('README.rst').open() as readme:
     long_description = readme.read()
 
 
 setup(
     name='xmlschema',
-    version='2.2.2',
+    version='2.2.3',
     packages=find_packages(include=['xmlschema*']),
     package_data={
         'xmlschema': ['py.typed', 'locale/**/*.mo', 'locale/**/*.po', 'schemas/*/*.xsd'],
         'xmlschema.extras': ['templates/*/*.jinja'],
     },
     entry_points={
         'console_scripts': [
@@ -58,13 +58,14 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Libraries',
         'Topic :: Text Processing :: Markup :: XML',
     ]
 )
```

### Comparing `xmlschema-2.2.2/tests/check_memory.py` & `xmlschema-2.2.3/tests/check_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_all.py` & `xmlschema-2.2.3/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection-1_error.xml` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection-1_error.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection-default.xml` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection-default.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection.py` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection.xml` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection2.xml` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection2.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection3.xml` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection3.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection3bis.xml` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection3bis.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection4.xml` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection4.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/collection/collection5.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/collection/collection5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/stockquote/stockquote.wsdl` & `xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/stockquote/stockquote.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/stockquote/stockquoteservice.wsdl` & `xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/vehicles/invalid.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/vehicles/invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-max.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-max.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip` & `xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/examples/vehicles/vehicles.xsd` & `xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/attributes/default_attributes-missing_group.xsd` & `xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes-missing_group.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/attributes/default_attributes.xsd` & `xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/builtins/builtins.xml` & `xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/builtins/builtins.xsd` & `xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/decoder/data.xml` & `xmlschema-2.2.3/tests/test_cases/features/decoder/data.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/decoder/data2.xml` & `xmlschema-2.2.3/tests/test_cases/features/decoder/data2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/decoder/data3.xml` & `xmlschema-2.2.3/tests/test_cases/features/decoder/data3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/decoder/long-sequence-1.xsd` & `xmlschema-2.2.3/tests/test_cases/features/decoder/long-sequence-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/decoder/mixed-content.xsd` & `xmlschema-2.2.3/tests/test_cases/features/decoder/mixed-content.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/decoder/simple-types.xsd` & `xmlschema-2.2.3/tests/test_cases/features/decoder/simple-types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/derivations/complex-extensions.xsd` & `xmlschema-2.2.3/tests/test_cases/features/derivations/complex-extensions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd` & `xmlschema-2.2.3/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/derivations/invalid_enumeration_restriction.xsd` & `xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_enumeration_restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/derivations/invalid_restrictions1.xsd` & `xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/derivations/invalid_restrictions2.xsd` & `xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/derivations/list_types.xsd` & `xmlschema-2.2.3/tests/test_cases/features/derivations/list_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/elements/type_alternatives-no-ns.xsd` & `xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives-no-ns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/elements/type_alternatives.xsd` & `xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/billion_laughs_model.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/billion_laughs_model.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/illegal-declarations.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/illegal-declarations.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/illegal-occurs.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/illegal-occurs.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/invalid_models1.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/invalid_models1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/invalid_models2.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/invalid_models2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/models.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/models.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/recursive-groups.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/recursive-groups.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-2.2.3/tests/test_cases/features/models/valid_model1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case1.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case2.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case4a.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4a.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/import-case4b.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case2.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case2bis.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case3.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/namespaces/include-case5.xsd` & `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/patterns/patterns.xml` & `xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/patterns/patterns.xsd` & `xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example4.wsdl` & `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl` & `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example5.wsdl` & `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl` & `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl` & `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_008/issue_008.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_008/issue_008.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_013/issue_013-1.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_013/issue_013.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_014/issue014.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_014/issue014.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_018/issue_018.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_018/issue_018.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_022/README.md` & `xmlschema-2.2.3/tests/test_cases/issues/issue_022/README.md`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_022/xsd_string.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_022/xsd_string.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_026/issue_026.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_035/dates.xml` & `xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_035/dates.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_041/issue_041.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_041/issue_041.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_051/issue_051.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_051/issue_051.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_073/issue_073.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_086/issue_086.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_105/issue_105.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_105/issue_105.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_111/issue_111.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_115/Rotation.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_115/Rotation.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_171/issue_171.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_171/issue_171b.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_187/issue_187_1.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_187/issue_187_2.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_190/issue_190.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_190/issue_190.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_200/issue_200.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_200/issue_200.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_203/issue_203.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_203/issue_203alt.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_204/issue_204.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_208/issue_208.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_208/issue_208.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_222/issue_222.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_222/issue_222.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl` & `xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl` & `xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_237/dir2/stockquote.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_243/issue_243.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_243/issue_243.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_245/issue_245-valid.xml` & `xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245-valid.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_245/issue_245.xml` & `xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_245/issue_245.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_259/issue_259-1.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_259/issue_259-2.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_265/issue_265-1.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266-1.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266-2.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266b-1.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_266/issue_266b-2.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_273/issue_273.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_273/issue_273.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_298/issue_298.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_306/issue_306-alt.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_311/correct_no_list.xml` & `xmlschema-2.2.3/tests/test_cases/issues/issue_311/correct_no_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_311/incorrect_with_list.xml` & `xmlschema-2.2.3/tests/test_cases/issues/issue_311/incorrect_with_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_314/issue_314.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_314/issue_314.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_315/issue_315_mixed.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_324/issue_324.zip` & `xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_334/issue_334.xml` & `xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_334/issue_334.xsd` & `xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/issues/issue_334/issue_334.zip` & `xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/mypy/extra_validator.py` & `xmlschema-2.2.3/tests/test_cases/mypy/extra_validator.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/mypy/schema_source.py` & `xmlschema-2.2.3/tests/test_cases/mypy/schema_source.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/mypy/simple_types.py` & `xmlschema-2.2.3/tests/test_cases/mypy/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cases/testfiles` & `xmlschema-2.2.3/tests/test_cases/testfiles`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_cli.py` & `xmlschema-2.2.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_codegen.py` & `xmlschema-2.2.3/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_converters.py` & `xmlschema-2.2.3/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_dataobjects.py` & `xmlschema-2.2.3/tests/test_dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_documents.py` & `xmlschema-2.2.3/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_files.py` & `xmlschema-2.2.3/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_helpers.py` & `xmlschema-2.2.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_memory.py` & `xmlschema-2.2.3/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_namespaces.py` & `xmlschema-2.2.3/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_package.py` & `xmlschema-2.2.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_resources.py` & `xmlschema-2.2.3/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_schemas.py` & `xmlschema-2.2.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_translations.py` & `xmlschema-2.2.3/tests/test_translations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_typing.py` & `xmlschema-2.2.3/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_validation.py` & `xmlschema-2.2.3/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_w3c_suite.py` & `xmlschema-2.2.3/tests/test_w3c_suite.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_wsdl.py` & `xmlschema-2.2.3/tests/test_wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/test_xpath.py` & `xmlschema-2.2.3/tests/test_xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validation/test_decoding.py` & `xmlschema-2.2.3/tests/validation/test_decoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from elementpath import datatypes
 import xmlschema
 from xmlschema import XMLSchemaValidationError, ParkerConverter, BadgerFishConverter, \
     AbderaConverter, JsonMLConverter, ColumnarConverter, ElementData
 
 from xmlschema.names import XSD_STRING, XSI_NIL
 from xmlschema.converters import UnorderedConverter
-from xmlschema.validators import XMLSchema11
+from xmlschema.validators import XMLSchema11, ModelVisitor
 from xmlschema.testing import XsdValidatorTestCase, etree_elements_assert_equal
 
 VEHICLES_DICT = {
     '@xmlns:vh': 'http://example.com/vehicles',
     '@xmlns:xsi': 'http://www.w3.org/2001/XMLSchema-instance',
     '@xsi:schemaLocation': 'http://example.com/vehicles vehicles.xsd',
     'vh:cars': {
@@ -371,15 +371,17 @@
 
         xml_dict = self.vh_schema.to_dict(vh_xml_tree)
         self.assertNotEqual(xml_dict, VEHICLES_DICT)
 
         xml_dict = self.vh_schema.to_dict(vh_xml_tree, namespaces=self.vh_namespaces)
         self.assertEqual(xml_dict, VEHICLES_DICT)
 
-        xml_dict = xmlschema.to_dict(vh_xml_tree, self.vh_schema.url, namespaces=self.vh_namespaces)
+        xml_dict = xmlschema.to_dict(
+            vh_xml_tree, self.vh_schema.url, namespaces=self.vh_namespaces
+        )
         self.assertEqual(xml_dict, VEHICLES_DICT)
 
         xml_dict = self.col_schema.to_dict(col_xml_tree)
         self.assertNotEqual(xml_dict, COLLECTION_DICT)
 
         xml_dict = self.col_schema.to_dict(col_xml_tree, namespaces=self.col_namespaces)
         self.assertEqual(xml_dict, COLLECTION_DICT)
@@ -1371,14 +1373,100 @@
                     'To mitigate the risk, use the setHttpOnly(true) method.']
         self.assertListEqual(body_text, expected)
 
         result = xs.decode(xml_file, preserve_root=True)
         body_text = result['Demonstrative_Examples']['Demonstrative_Example'][0]['Body_Text']
         self.assertListEqual(body_text, expected)
 
+    def test_fill_missing_elements__issue_341(self):
+        xsd_file = self.casepath('issues/issue_341/issue_341.xsd')
+        xml_file = self.casepath('issues/issue_341/issue_341.xml')
+        schema = self.schema_class(xsd_file)
+
+        expected = {'TEST_EL': [
+            {'@Date': '2022-10-03',
+             'TEST_EL_2': {
+                 'exists_in_xml': {
+                     '@test_attr': 'test_value_attr', '@test_attr_2': None
+                 }
+             }}
+        ]}
+        xml_dict = schema.decode(xml_file, fill_missing=True)
+        self.assertDictEqual(xml_dict, expected)
+
+        def fill_missing_content(element_data: ElementData, _xsd_element, xsd_type):
+            group = xsd_type.model_group
+            if group is None:
+                return element_data  # an element with simple content
+
+            filled_content = []
+            model = ModelVisitor(group)
+            xsd_element = None
+            for name, value, xsd_element in element_data.content:
+                if isinstance(name, int) or xsd_element is None:
+                    filled_content.append((name, value, xsd_element))
+                    continue
+
+                while model.element is not None:
+                    if model.element is xsd_element:
+                        filled_content.append((name, value, xsd_element))
+                        for _err in model.advance(True):
+                            pass
+                        break
+
+                    if model.element.max_occurs != 0:
+                        filled_content.append((model.element.name, None, model.element))
+                    for _err in model.advance(False):
+                        pass
+                else:
+                    filled_content.append((name, value, xsd_element))
+
+            while model.element is not None:
+                if model.element is not xsd_element and model.element.max_occurs != 0:
+                    filled_content.append((model.element.name, None, model.element))
+                for _err in model.advance(False):
+                    pass
+
+            return ElementData(
+                element_data.tag,
+                element_data.text,
+                filled_content,
+                element_data.attributes
+            )
+
+        expected = {'TEST_EL': [
+            {'@Date': '2022-10-03',
+             'TEST_EL_2': {
+                 'exists_in_xml': {
+                     '@test_attr': 'test_value_attr', '@test_attr_2': None
+                 },
+                 'not_exists_in_xml': None
+             }}
+        ]}
+        xml_dict = schema.decode(xml_file, element_hook=fill_missing_content, fill_missing=True)
+        self.assertDictEqual(xml_dict, expected)
+
+        # Resolving more complex schemas requires more checks in hook function
+        xsd_file = self.casepath('issues/issue_341/issue_341-ext.xsd')
+        schema = self.schema_class(xsd_file)
+
+        expected = {'TEST_EL': [
+            {'@Date': '2022-10-03',
+             'TEST_EL_2': {
+                 'exists_in_xml': {
+                     '@test_attr': 'test_value_attr', '@test_attr_2': None
+                 },
+                 'not_exists_in_xml': None,
+                 'choice_elem1': None,
+                 'choice_elem2': None,  # this is wrong (at most one element for a choice)
+             }}
+        ]}
+        xml_dict = schema.decode(xml_file, element_hook=fill_missing_content, fill_missing=True)
+        self.assertDictEqual(xml_dict, expected)
+
 
 class TestDecoding11(TestDecoding):
     schema_class = XMLSchema11
 
     def test_datetime_types(self):
         xs = self.get_schema('<xs:element name="dt" type="xs:dateTime"/>')
         self.assertEqual(xs.decode('<dt>2019-01-01T13:40:00</dt>'), '2019-01-01T13:40:00')
```

### Comparing `xmlschema-2.2.2/tests/validation/test_encoding.py` & `xmlschema-2.2.3/tests/validation/test_encoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validation/test_validation.py` & `xmlschema-2.2.3/tests/validation/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_attributes.py` & `xmlschema-2.2.3/tests/validators/test_attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_builtins.py` & `xmlschema-2.2.3/tests/validators/test_builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_complex_types.py` & `xmlschema-2.2.3/tests/validators/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_elements.py` & `xmlschema-2.2.3/tests/validators/test_elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_exceptions.py` & `xmlschema-2.2.3/tests/validators/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_facets.py` & `xmlschema-2.2.3/tests/validators/test_facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_global_maps.py` & `xmlschema-2.2.3/tests/validators/test_global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_groups.py` & `xmlschema-2.2.3/tests/validators/test_groups.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_identities.py` & `xmlschema-2.2.3/tests/validators/test_identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_models.py` & `xmlschema-2.2.3/tests/validators/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from textwrap import dedent
 from typing import Any, Union, List, Optional
 
 from xmlschema import XMLSchema10, XMLSchema11
 from xmlschema.exceptions import XMLSchemaValueError
 from xmlschema.validators.exceptions import XMLSchemaValidationError
 from xmlschema.validators.particles import ParticleMixin
-from xmlschema.validators.models import distinguishable_paths, ModelVisitor
+from xmlschema.validators.models import distinguishable_paths, ModelVisitor, \
+    sort_content, iter_collapsed_content
 from xmlschema.validators.groups import XsdGroup
 from xmlschema.validators.elements import XsdElement
 from xmlschema.testing import XsdValidatorTestCase
 
 
 class ModelGroup(XsdGroup):
     """A subclass for testing XSD models, that disables element parsing and schema bindings."""
@@ -111,24 +112,24 @@
         group = ModelGroup('choice')
         group.append(ParticleMixin())
         group.append(ParticleMixin())
         group.append(ParticleMixin())
 
         model = ModelVisitor(group)
         model.occurs[group[1]] = 1
-        self.assertListEqual(list(model.items), group[1:])
+        self.assertEqual(list(model.items), group[1:])
 
         group = ModelGroup('all')
         group.append(ParticleMixin())
         group.append(ParticleMixin())
         group.append(ParticleMixin())
 
         model = ModelVisitor(group)
         model.occurs[group[1]] = 1
-        self.assertListEqual(list(model.items), group[2:])
+        self.assertEqual(list(model.items), group[2:])
 
     # --- Vehicles schema ---
 
     def test_vehicles_model(self):
         # Sequence with two not-emptiable single-occurs elements
         group = self.vh_schema.elements['vehicles'].type.content
 
@@ -981,85 +982,80 @@
                     <xs:element name="B1" type="xs:string"/>
                     <xs:element name="B2" type="xs:integer"/>
                     <xs:element name="B3" type="xs:boolean"/>
                 </xs:sequence>
             </xs:complexType>
             """)
 
-        model = ModelVisitor(schema.types['A_type'].content)
+        group = schema.types['A_type'].content
 
         self.assertListEqual(
-            model.sort_content([('B2', 10), ('B1', 'abc'), ('B3', True)], restart=False),
+            sort_content([('B2', 10), ('B1', 'abc'), ('B3', True)], group),
             [('B1', 'abc'), ('B2', 10), ('B3', True)]
         )
         self.assertListEqual(
-            model.sort_content([('B2', 10), ('B1', 'abc'), ('B3', True)]),
+            sort_content([('B3', True), ('B2', 10), ('B1', 'abc')], group),
             [('B1', 'abc'), ('B2', 10), ('B3', True)]
         )
         self.assertListEqual(
-            model.sort_content([('B2', 10), ('B1', 'abc'), ('B3', True)], restart=False),
-            [('B2', 10), ('B1', 'abc'), ('B3', True)]
-        )
-
-        self.assertListEqual(
-            model.sort_content([('B3', True), ('B2', 10), ('B1', 'abc')]),
-            [('B1', 'abc'), ('B2', 10), ('B3', True)]
-        )
-        self.assertListEqual(
-            model.sort_content([('B2', 10), ('B4', None), ('B1', 'abc'), ('B3', True)]),
+            sort_content([('B2', 10), ('B4', None), ('B1', 'abc'), ('B3', True)], group),
             [('B1', 'abc'), ('B2', 10), ('B3', True), ('B4', None)]
         )
 
         content = [('B2', 10), ('B4', None), ('B1', 'abc'), (1, 'hello'), ('B3', True)]
         self.assertListEqual(
-            model.sort_content(content),
+            sort_content(content, group),
             [(1, 'hello'), ('B1', 'abc'), ('B2', 10), ('B3', True), ('B4', None)]
         )
 
         content = [
             (2, 'world!'), ('B2', 10), ('B4', None), ('B1', 'abc'), (1, 'hello'), ('B3', True)
         ]
         self.assertListEqual(
-            model.sort_content(content),
+            sort_content(content, group),
             [(1, 'hello'), ('B1', 'abc'), (2, 'world!'), ('B2', 10), ('B3', True), ('B4', None)]
         )
 
         content = [
             ('B2', 10), ('B4', None), ('B1', 'abc'), ('B3', True), (6, 'six'),
             (5, 'five'), (4, 'four'), (2, 'two'), (3, 'three'), (1, 'one')
         ]
         self.assertListEqual(
-            model.sort_content(content),
+            sort_content(content, group),
             [(1, 'one'), ('B1', 'abc'), (2, 'two'), ('B2', 10), (3, 'three'),
              ('B3', True), (4, 'four'), ('B4', None), (5, 'five'), (6, 'six')]
         )
 
         # With a dict-type argument
         content = dict([('B2', [10]), ('B1', ['abc']), ('B3', [True])])
         self.assertListEqual(
-            model.sort_content(content), [('B1', 'abc'), ('B2', 10), ('B3', True)]
+            sort_content(content, group), [('B1', 'abc'), ('B2', 10), ('B3', True)]
         )
         content = dict([('B2', [10]), ('B1', ['abc']), ('B3', [True]), (1, 'hello')])
         self.assertListEqual(
-            model.sort_content(content), [(1, 'hello'), ('B1', 'abc'), ('B2', 10), ('B3', True)]
+            sort_content(content, group),
+            [(1, 'hello'), ('B1', 'abc'), ('B2', 10), ('B3', True)]
         )
 
         # With partial content
-        self.assertListEqual(model.sort_content([]), [])
-        self.assertListEqual(model.sort_content([('B1', 'abc')]), [('B1', 'abc')])
-        self.assertListEqual(model.sort_content([('B2', 10)]), [('B2', 10)])
-        self.assertListEqual(model.sort_content([('B3', True)]), [('B3', True)])
+        self.assertListEqual(sort_content([], group), [])
+        self.assertListEqual(sort_content([('B1', 'abc')], group), [('B1', 'abc')])
+        self.assertListEqual(sort_content([('B2', 10)], group), [('B2', 10)])
+        self.assertListEqual(sort_content([('B3', True)], group), [('B3', True)])
         self.assertListEqual(
-            model.sort_content([('B3', True), ('B1', 'abc')]), [('B1', 'abc'), ('B3', True)]
+            sort_content([('B3', True), ('B1', 'abc')], group),
+            [('B1', 'abc'), ('B3', True)]
         )
         self.assertListEqual(
-            model.sort_content([('B2', 10), ('B1', 'abc')]), [('B1', 'abc'), ('B2', 10)]
+            sort_content([('B2', 10), ('B1', 'abc')], group),
+            [('B1', 'abc'), ('B2', 10)]
         )
         self.assertListEqual(
-            model.sort_content([('B3', True), ('B2', 10)]), [('B2', 10), ('B3', True)]
+            sort_content([('B3', True), ('B2', 10)], group),
+            [('B2', 10), ('B3', True)]
         )
 
     def test_iter_collapsed_content_with_optional_elements(self):
         schema = self.get_schema("""
             <xs:element name="A" type="A_type" />
             <xs:complexType name="A_type">
                 <xs:sequence>
@@ -1070,27 +1066,34 @@
                     <xs:element name="B5" />
                     <xs:element name="B6" minOccurs="0" />
                     <xs:element name="B7" />
                 </xs:sequence>
             </xs:complexType>
             """)
 
-        model = ModelVisitor(schema.types['A_type'].content)
+        group = schema.types['A_type'].content
+        model = ModelVisitor(group)
 
         content = [('B3', 10), ('B4', None), ('B5', True), ('B6', 'alpha'), ('B7', 20)]
         model.restart()
         self.assertListEqual(
             list(model.iter_collapsed_content(content)), content
         )
+        self.assertListEqual(
+            list(iter_collapsed_content(content, group)), content
+        )
 
         content = [('B3', 10), ('B5', True), ('B6', 'alpha'), ('B7', 20)]  # Missing B4
         model.restart()
         self.assertListEqual(
             list(model.iter_collapsed_content(content)), content
         )
+        self.assertListEqual(
+            list(iter_collapsed_content(content, group)), content
+        )
 
     def test_iter_collapsed_content_with_repeated_elements(self):
         schema = self.get_schema("""
             <xs:element name="A" type="A_type" />
             <xs:complexType name="A_type">
                 <xs:sequence>
                     <xs:element name="B1" minOccurs="0" />
@@ -1100,79 +1103,66 @@
                     <xs:element name="B5" maxOccurs="unbounded" />
                     <xs:element name="B6" minOccurs="0" />
                     <xs:element name="B7" maxOccurs="unbounded" />
                 </xs:sequence>
             </xs:complexType>
             """)
 
-        model = ModelVisitor(schema.types['A_type'].content)
+        group = schema.types['A_type'].content
 
         content = [
             ('B3', 10), ('B4', None), ('B5', True), ('B5', False), ('B6', 'alpha'), ('B7', 20)
         ]
-        self.assertListEqual(
-            list(model.iter_collapsed_content(content)), content
-        )
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B3', 10), ('B3', 11), ('B3', 12), ('B4', None), ('B5', True),
                    ('B5', False), ('B6', 'alpha'), ('B7', 20), ('B7', 30)]
-        model.restart()
-        self.assertListEqual(
-            list(model.iter_collapsed_content(content)), content
-        )
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B3', 10), ('B3', 11), ('B3', 12), ('B4', None), ('B5', True), ('B5', False)]
-        model.restart()
-        self.assertListEqual(
-            list(model.iter_collapsed_content(content)), content
-        )
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
     def test_iter_collapsed_content_with_repeated_groups(self):
         schema = self.get_schema("""
             <xs:element name="A" type="A_type" />
             <xs:complexType name="A_type">
                 <xs:sequence minOccurs="1" maxOccurs="2">
                     <xs:element name="B1" minOccurs="0" />
                     <xs:element name="B2" minOccurs="0" />
                 </xs:sequence>
             </xs:complexType>
             """)
 
-        model = ModelVisitor(schema.types['A_type'].content)
+        group = schema.types['A_type'].content
 
         content = [('B1', 1), ('B1', 2), ('B2', 3), ('B2', 4)]
         self.assertListEqual(
-            list(model.iter_collapsed_content(content)),
+            list(iter_collapsed_content(content, group)),
             [('B1', 1), ('B2', 3), ('B1', 2), ('B2', 4)]
         )
 
         # Model broken by unknown element at start
         content = [('X', None), ('B1', 1), ('B1', 2), ('B2', 3), ('B2', 4)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B1', 1), ('X', None), ('B1', 2), ('B2', 3), ('B2', 4)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B1', 1), ('B1', 2), ('X', None), ('B2', 3), ('B2', 4)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B1', 1), ('B1', 2), ('B2', 3), ('X', None), ('B2', 4)]
-        model.restart()
         self.assertListEqual(
-            list(model.iter_collapsed_content(content)),
+            list(iter_collapsed_content(content, group)),
             [('B1', 1), ('B2', 3), ('B1', 2), ('X', None), ('B2', 4)]
         )
 
         content = [('B1', 1), ('B1', 2), ('B2', 3), ('B2', 4), ('X', None)]
-        model.restart()
         self.assertListEqual(
-            list(model.iter_collapsed_content(content)),
+            list(iter_collapsed_content(content, group)),
             [('B1', 1), ('B2', 3), ('B1', 2), ('B2', 4), ('X', None)]
         )
 
     def test_iter_collapsed_content_with_single_elements(self):
         schema = self.get_schema("""
             <xs:element name="A" type="A_type" />
             <xs:complexType name="A_type">
@@ -1180,42 +1170,36 @@
                     <xs:element name="B1" />
                     <xs:element name="B2" />
                     <xs:element name="B3" />
                 </xs:sequence>
             </xs:complexType>
             """)
 
-        model = ModelVisitor(schema.types['A_type'].content)
+        group = schema.types['A_type'].content
 
         content = [('B1', 'abc'), ('B2', 10), ('B3', False)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B3', False), ('B1', 'abc'), ('B2', 10)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B1', 'abc'), ('B3', False), ('B2', 10)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('B1', 'abc'), ('B1', 'def'), ('B2', 10), ('B3', False)]
-        model.restart()
         self.assertListEqual(
-            list(model.iter_collapsed_content(content)),
+            list(iter_collapsed_content(content, group)),
             [('B1', 'abc'), ('B2', 10), ('B3', False), ('B1', 'def')]
         )
 
         content = [('B1', 'abc'), ('B2', 10), ('X', None)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('X', None), ('B1', 'abc'), ('B2', 10), ('B3', False)]
-        model.restart()
-        self.assertListEqual(list(model.iter_collapsed_content(content)), content)
+        self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
 
 class TestModelPaths(unittest.TestCase):
 
     def test_distinguishable_paths_one_level(self):
         group = ModelGroup('sequence', min_occurs=0)
         group.append(ModelGroup('sequence'))
```

### Comparing `xmlschema-2.2.2/tests/validators/test_notations.py` & `xmlschema-2.2.3/tests/validators/test_notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_particles.py` & `xmlschema-2.2.3/tests/validators/test_particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_schemas.py` & `xmlschema-2.2.3/tests/validators/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_simple_types.py` & `xmlschema-2.2.3/tests/validators/test_simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_wildcards.py` & `xmlschema-2.2.3/tests/validators/test_wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tests/validators/test_xsdbase.py` & `xmlschema-2.2.3/tests/validators/test_xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/tox.ini` & `xmlschema-2.2.3/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 [tox]
-envlist = py{37,38,39,310,311}, pypy3, ep{40}, docs,
-    flake8, mypy-py{37,38,39,310,311}, coverage, pytest
+envlist = py{37,38,39,310,311,312,py3}, ep{40}, docs,
+    flake8, mypy-py{37,38,39,310,311,312,py3}, coverage, pytest
 skip_missing_interpreters = true
 work_dir = {tox_root}/../.tox/xmlschema
 
 [testenv]
 deps =
     elementpath>=4.0.0, <5.0.0
     lxml
     jinja2
     py{310,311}: memory_profiler
     docs: Sphinx
     docs: sphinx_rtd_theme
     coverage: coverage
 commands =
     python -m unittest
-allowlist_externals = make
 
-[testenv:pypy3]
-commands = python -m unittest
+[testenv:py312]
+deps =
+    elementpath>=4.0.0, <5.0.0
+    # lxml: skip for now
+    jinja2
 
 [testenv:ep40]
 deps =
     elementpath~=4.0.0
     lxml
 
 [testenv:docs]
 commands =
     make -C doc html SPHINXOPTS="-W -n"
     make -C doc latexpdf SPHINXOPTS="-W -n"
     make -C doc doctest SPHINXOPTS="-W -n"
     sphinx-build -W -n -T -b man doc build/sphinx/man
+allowlist_externals = make
 
 [flake8]
 max-line-length = 100
 
 [testenv:flake8]
 deps =
     flake8
 commands =
     flake8 xmlschema
     flake8 tests
 
 [testenv:mypy-py37]
 deps =
-    mypy==1.0.1
-    elementpath==4.0.1
+    mypy==1.2.0
+    elementpath==4.1.1
     lxml-stubs
     jinja2
 commands =
     mypy --config-file {toxinidir}/mypy.ini xmlschema
 
-[testenv:mypy-py{38,39,310,311}]
+[testenv:mypy-py{38,39,310,311,312,py3}]
 deps =
-    mypy==1.0.1
-    elementpath==4.0.1
+    mypy==1.2.0
+    elementpath==4.1.1
     lxml-stubs
     jinja2
 commands =
     mypy --config-file {toxinidir}/mypy.ini xmlschema
     python tests/test_typing.py
 
 [testenv:coverage]
@@ -70,15 +73,15 @@
 [testenv:pytest]
 deps =
     pytest
     pytest-randomly
     elementpath>=4.0.0, <5.0.0
     lxml
     jinja2
-    mypy==1.0.1
+    mypy==1.2.0
     lxml-stubs
 commands =
     pytest tests -ra
 
 [testenv:build]
 deps =
     setuptools
```

### Comparing `xmlschema-2.2.2/xmlschema/__init__.py` & `xmlschema-2.2.3/xmlschema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     XMLSchemaModelError, XMLSchemaModelDepthError, XMLSchemaValidationError,
     XMLSchemaDecodeError, XMLSchemaEncodeError, XMLSchemaChildrenValidationError,
     XMLSchemaIncludeWarning, XMLSchemaImportWarning, XMLSchemaTypeTableWarning,
     XsdGlobals, XMLSchemaBase, XMLSchema, XMLSchema10, XMLSchema11,
     XsdComponent, XsdType, XsdElement, XsdAttribute
 )
 
-__version__ = '2.2.2'
+__version__ = '2.2.3'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2016-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 __all__ = [
```

### Comparing `xmlschema-2.2.2/xmlschema/aliases.py` & `xmlschema-2.2.3/xmlschema/aliases.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/cli.py` & `xmlschema-2.2.3/xmlschema/cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/__init__.py` & `xmlschema-2.2.3/xmlschema/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/abdera.py` & `xmlschema-2.2.3/xmlschema/converters/abdera.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/badgerfish.py` & `xmlschema-2.2.3/xmlschema/converters/badgerfish.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/columnar.py` & `xmlschema-2.2.3/xmlschema/converters/columnar.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/default.py` & `xmlschema-2.2.3/xmlschema/converters/default.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/jsonml.py` & `xmlschema-2.2.3/xmlschema/converters/jsonml.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/parker.py` & `xmlschema-2.2.3/xmlschema/converters/parker.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/converters/unordered.py` & `xmlschema-2.2.3/xmlschema/converters/unordered.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/dataobjects.py` & `xmlschema-2.2.3/xmlschema/dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/documents.py` & `xmlschema-2.2.3/xmlschema/documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/exceptions.py` & `xmlschema-2.2.3/xmlschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/extras/codegen.py` & `xmlschema-2.2.3/xmlschema/extras/codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/extras/templates/python/bindings.py.jinja` & `xmlschema-2.2.3/xmlschema/extras/templates/python/bindings.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/extras/templates/python/sample.py.jinja` & `xmlschema-2.2.3/xmlschema/extras/templates/python/sample.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/extras/wsdl.py` & `xmlschema-2.2.3/xmlschema/extras/wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/helpers.py` & `xmlschema-2.2.3/xmlschema/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/limits.py` & `xmlschema-2.2.3/xmlschema/limits.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/locale/en/LC_MESSAGES/xmlschema.po` & `xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/locale/it/LC_MESSAGES/xmlschema.po` & `xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po` & `xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/names.py` & `xmlschema-2.2.3/xmlschema/names.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/namespaces.py` & `xmlschema-2.2.3/xmlschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/resources.py` & `xmlschema-2.2.3/xmlschema/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 import copy
 import os.path
+import ntpath
+import posixpath
 import platform
 import re
 import string
 from io import StringIO, BytesIO
 from pathlib import Path, PurePath, PurePosixPath, PureWindowsPath
 from typing import cast, Any, AnyStr, Dict, Optional, IO, Iterator, List, \
     MutableMapping, Union, Tuple
@@ -41,21 +43,20 @@
 ###
 # URL normalization (that fixes many headaches :)
 class _PurePath(PurePath):
     """
     A version of pathlib.PurePath adapted for managing the creation
     from URIs and the simple normalization of paths.
     """
-    _from_parts: Any
-    _flavour: Any
+    _path_module = os.path
 
     def __new__(cls, *args: str) -> '_PurePath':
         if cls is _PurePath:
             cls = _PureWindowsPath if os.name == 'nt' else _PurePosixPath
-        return cast('_PurePath', cls._from_parts(args))
+        return super().__new__(cls, *args)
 
     @classmethod
     def from_uri(cls, uri: str) -> '_PurePath':
         uri = uri.strip()
         if not uri:
             raise XMLSchemaValueError("Empty URI provided!")
 
@@ -94,37 +95,48 @@
 
         if '\\' in path:
             return _PureWindowsPath(unquote(path))
         return cls(unquote(path))
 
     def as_uri(self) -> str:
         if not self.is_absolute():
-            uri: str = self._flavour.make_uri(self)
-            while uri.startswith('file:/'):
-                uri = uri.replace('file:/', 'file:', 1)
-            return uri
+            # Converts relative paths to not RFC 8089 compliant relative
+            # file URIs because urlopen() doesn't accept simple paths
+            drive = self.drive
+            if len(drive) == 2 and drive[1] == ':':
+                prefix = 'file:' + drive
+                path = self.as_posix()[2:]
+            elif drive:
+                prefix = 'file:'
+                path = self.as_posix()
+            else:
+                prefix = 'file:'
+                path = str(self)
+            return prefix + quote_from_bytes(os.fsencode(path))
 
-        uri = cast(str, self._flavour.make_uri(self))
+        uri = super().as_uri()
         if isinstance(self, _PureWindowsPath) and str(self).startswith(r'\\'):
             # UNC format case: use the format where the host part is included
             # in the path part, to let urlopen() works.
             if not uri.startswith('file:////'):
                 return uri.replace('file://', 'file:////')
         return uri
 
     def normalize(self) -> '_PurePath':
-        normalized_path = self._flavour.pathmod.normpath(str(self))
-        return cast('_PurePath', self._from_parts((normalized_path,)))
+        normalized_path = self._path_module.normpath(str(self))
+        return self.__class__(normalized_path)
 
 
 class _PurePosixPath(_PurePath, PurePosixPath):
+    _path_module = posixpath
     __slots__ = ()
 
 
 class _PureWindowsPath(_PurePath, PureWindowsPath):
+    _path_module = ntpath
     __slots__ = ()
 
 
 def normalize_url(url: str, base_url: Optional[str] = None,
                   keep_relative: bool = False) -> str:
     """
     Returns a normalized URL eventually joining it to a base URL if it's a relative path.
```

### Comparing `xmlschema-2.2.2/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd` & `xmlschema-2.2.3/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/VC/XMLSchema-versioning.xsd` & `xmlschema-2.2.3/xmlschema/schemas/VC/XMLSchema-versioning.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/WSDL/soap-encoding.xsd` & `xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-encoding.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/WSDL/soap-envelope.xsd` & `xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/WSDL/wsdl-soap.xsd` & `xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl-soap.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/WSDL/wsdl.xsd` & `xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XHTML/xhtml1-strict.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XHTML/xhtml1-strict.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XLINK/xlink.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XLINK/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XML/xml_minimal.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XML/xml_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XSD_1.0/XMLSchema.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XSD_1.0/datatypes.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XSD_1.1/XMLSchema.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XSD_1.1/datatypes.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd` & `xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/testing/__init__.py` & `xmlschema-2.2.3/xmlschema/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/testing/_builders.py` & `xmlschema-2.2.3/xmlschema/testing/_builders.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/testing/_case_class.py` & `xmlschema-2.2.3/xmlschema/testing/_case_class.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/testing/_factory.py` & `xmlschema-2.2.3/xmlschema/testing/_factory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/testing/_helpers.py` & `xmlschema-2.2.3/xmlschema/testing/_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/testing/_observers.py` & `xmlschema-2.2.3/xmlschema/testing/_observers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/translation.py` & `xmlschema-2.2.3/xmlschema/translation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/__init__.py` & `xmlschema-2.2.3/xmlschema/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/assertions.py` & `xmlschema-2.2.3/xmlschema/validators/assertions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/attributes.py` & `xmlschema-2.2.3/xmlschema/validators/attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/builtins.py` & `xmlschema-2.2.3/xmlschema/validators/builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/complex_types.py` & `xmlschema-2.2.3/xmlschema/validators/complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/elements.py` & `xmlschema-2.2.3/xmlschema/validators/elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/exceptions.py` & `xmlschema-2.2.3/xmlschema/validators/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/facets.py` & `xmlschema-2.2.3/xmlschema/validators/facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/global_maps.py` & `xmlschema-2.2.3/xmlschema/validators/global_maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from ..namespaces import NamespaceResourcesMap
 from ..translation import gettext as _
 
 from .exceptions import XMLSchemaNotBuiltError, XMLSchemaModelError, XMLSchemaModelDepthError, \
     XMLSchemaParseError
 from .xsdbase import XsdValidator, XsdComponent
 from .builtins import xsd_builtin_types_factory
+from .models import check_model
 from . import XsdAttribute, XsdSimpleType, XsdComplexType, XsdElement, XsdAttributeGroup, \
     XsdGroup, XsdNotation, XsdIdentity, XsdAssert, XsdUnion, XsdAtomicRestriction
 
 
 #
 # Defines the load functions for XML Schema structures
 def create_load_function(tag: str) \
@@ -727,15 +728,15 @@
                             any_element=xsd_type.open_content.any_element
                         )
                         if not _group.is_restriction(base_type.content):
                             msg = _("restriction has an open content but base type has not")
                             _group.parse_error(msg, validation=validation)
 
                 try:
-                    xsd_type.content.check_model()
+                    check_model(xsd_type.content)
                 except XMLSchemaModelDepthError:
                     msg = _("can't verify the content model of {!r} "
                             "due to exceeding of maximum recursion depth")
                     xsd_type.schema.warnings.append(msg.format(xsd_type))
                     warnings.warn(msg, XMLSchemaWarning, stacklevel=4)
                 except XMLSchemaModelError as err:
                     if validation == 'strict':
```

### Comparing `xmlschema-2.2.2/xmlschema/validators/groups.py` & `xmlschema-2.2.3/xmlschema/validators/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from .exceptions import XMLSchemaModelError, XMLSchemaModelDepthError, \
     XMLSchemaValidationError, XMLSchemaChildrenValidationError, \
     XMLSchemaTypeTableWarning
 from .xsdbase import ValidationMixin, XsdComponent, XsdType
 from .particles import ParticleMixin, OccursCalculator
 from .elements import XsdElement, XsdAlternative
 from .wildcards import XsdAnyElement, Xsd11AnyElement
-from .models import ModelVisitor, distinguishable_paths
+from .models import ModelVisitor, iter_unordered_content, iter_collapsed_content
 
 if TYPE_CHECKING:
     from .complex_types import XsdComplexType
 
 ANY_ELEMENT = ElementTree.Element(
     XSD_ANY,
     attrib={
@@ -761,86 +761,14 @@
         if max_occurs is None:
             return self.max_occurs == 0
         elif self.max_occurs is None:
             return max_occurs == 0
         else:
             return other_max_occurs >= max_occurs * self.max_occurs
 
-    def check_model(self) -> None:
-        """
-        Checks if the model group is deterministic. Element Declarations Consistent and
-        Unique Particle Attribution constraints are checked.
-        :raises: an `XMLSchemaModelError` at first violated constraint.
-        """
-        def safe_iter_path() -> Iterator[SchemaElementType]:
-            iterators: List[Iterator[ModelParticleType]] = []
-            particles = iter(self)
-
-            while True:
-                for item in particles:
-                    if isinstance(item, XsdGroup):
-                        current_path.append(item)
-                        iterators.append(particles)
-                        particles = iter(item)
-                        if len(iterators) > limits.MAX_MODEL_DEPTH:
-                            raise XMLSchemaModelDepthError(self)
-                        break
-                    else:
-                        yield item
-                else:
-                    try:
-                        current_path.pop()
-                        particles = iterators.pop()
-                    except IndexError:
-                        return
-
-        paths: Any = {}
-        current_path: List[ModelParticleType] = [self]
-        try:
-            any_element = self.parent.open_content.any_element  # type: ignore[union-attr]
-        except AttributeError:
-            any_element = None
-
-        for e in safe_iter_path():
-
-            previous_path: List[ModelParticleType]
-            for pe, previous_path in paths.values():
-                # EDC check
-                if not e.is_consistent(pe) or any_element and not any_element.is_consistent(pe):
-                    msg = _("Element Declarations Consistent violation between {0!r} and {1!r}"
-                            ": match the same name but with different types").format(e, pe)
-                    raise XMLSchemaModelError(self, msg)
-
-                # UPA check
-                if pe is e or not pe.is_overlap(e):
-                    continue
-                elif pe.parent is e.parent:
-                    if pe.parent.model in {'all', 'choice'}:
-                        if isinstance(pe, Xsd11AnyElement) and not isinstance(e, XsdAnyElement):
-                            pe.add_precedence(e, self)
-                        elif isinstance(e, Xsd11AnyElement) and not isinstance(pe, XsdAnyElement):
-                            e.add_precedence(pe, self)
-                        else:
-                            msg = _("{0!r} and {1!r} overlap and are in the same {2!r} group")
-                            raise XMLSchemaModelError(self, msg.format(pe, e, pe.parent.model))
-                    elif pe.is_univocal():
-                        continue
-
-                if distinguishable_paths(previous_path + [pe], current_path + [e]):
-                    continue
-                elif isinstance(pe, Xsd11AnyElement) and not isinstance(e, XsdAnyElement):
-                    pe.add_precedence(e, self)
-                elif isinstance(e, Xsd11AnyElement) and not isinstance(pe, XsdAnyElement):
-                    e.add_precedence(pe, self)
-                else:
-                    msg = _("Unique Particle Attribution violation between {0!r} and {1!r}")
-                    raise XMLSchemaModelError(self, msg.format(pe, e))
-
-            paths[e.name] = e, current_path[:]
-
     def check_dynamic_context(self, elem: ElementType,
                               xsd_element: SchemaElementType,
                               model_element: SchemaElementType,
                               namespaces: NamespacesType) -> None:
 
         if model_element is not xsd_element and isinstance(model_element, XsdElement):
             if 'substitution' in model_element.block \
@@ -1133,32 +1061,28 @@
         wrong_content_type = False
         over_max_depth = 'max_depth' in kwargs and kwargs['max_depth'] <= level
 
         content: Iterable[Any]
         if not obj.content:
             content = []
         elif isinstance(obj.content, MutableMapping) or kwargs.get('unordered'):
-            content = ModelVisitor(self).iter_unordered_content(
-                obj.content, default_namespace
-            )
+            content = iter_unordered_content(obj.content, self, default_namespace)
         elif not isinstance(obj.content, MutableSequence):
             wrong_content_type = True
             content = []
         elif not isinstance(obj.content[0], tuple):
             if len(obj.content) > 1 or text is not None:
                 wrong_content_type = True
             else:
                 text = raw_xml_encode(obj.content[0])
             content = []
         elif converter.losslessly:
             content = obj.content
         else:
-            content = ModelVisitor(self).iter_collapsed_content(
-                obj.content, default_namespace
-            )
+            content = iter_collapsed_content(obj.content, self, default_namespace)
 
         for index, (name, value) in enumerate(content):
             if isinstance(name, int):
                 if not children:
                     text = padding + value if text is None else text + value + padding
                 elif children[-1].tail is None:
                     children[-1].tail = padding + value
```

### Comparing `xmlschema-2.2.2/xmlschema/validators/helpers.py` & `xmlschema-2.2.3/xmlschema/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/identities.py` & `xmlschema-2.2.3/xmlschema/validators/identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/models.py` & `xmlschema-2.2.3/xmlschema/validators/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 """
-This module contains a function and a class for validating XSD content models.
+This module contains a function and a class for validating XSD content models,
+plus a set of functions for manipulating encoded content.
 """
 from collections import defaultdict, deque
-from typing import Any, Counter, Dict, Iterable, Iterator, List, Optional, Tuple, Union
+from typing import Any, Counter, Dict, Iterable, Iterator, List, \
+    MutableMapping, MutableSequence, Optional, Tuple, Union
 
 from ..exceptions import XMLSchemaValueError
 from ..aliases import ModelGroupType, ModelParticleType, SchemaElementType
+from ..translation import gettext as _
+from .. import limits
+from .exceptions import XMLSchemaModelError, XMLSchemaModelDepthError
+from .wildcards import XsdAnyElement, Xsd11AnyElement
 from . import groups
 
 AdvanceYieldedType = Tuple[ModelParticleType, int, List[SchemaElementType]]
-EncodedContentType = Union[Dict[Union[int, str], List[Any]],
-                           List[Tuple[Union[int, str], List[Any]]]]
 ContentItemType = Tuple[Union[int, str], Any]
+EncodedContentType = Union[MutableMapping[Union[int, str], Any], Iterable[ContentItemType]]
 
 
 def distinguishable_paths(path1: List[ModelParticleType], path2: List[ModelParticleType]) -> bool:
     """
     Checks if two model paths are distinguishable in a deterministic way, without looking forward
     or backtracking. The arguments are lists containing paths from the base group of the model to
     a couple of leaf elements. Returns `True` if there is a deterministic separation between paths,
@@ -84,14 +89,89 @@
     elif path1[depth].max_occurs == 1:
         return before2 or (before1 or univocal1) and (path1[-1].is_univocal() or after1)
     else:
         return (before2 or (before1 or univocal1) and (path1[-1].is_univocal() or after1)) and \
                (before1 or (before2 or univocal2) and (path2[-1].is_univocal() or after2))
 
 
+def check_model(group: ModelGroupType) -> None:
+    """
+    Checks if the model group is deterministic. Element Declarations Consistent and
+    Unique Particle Attribution constraints are checked.
+
+    :param group: the model group to check.
+    :raises: an `XMLSchemaModelError` at first violated constraint.
+    """
+    def safe_iter_path() -> Iterator[SchemaElementType]:
+        iterators: List[Iterator[ModelParticleType]] = []
+        particles = iter(group)
+
+        while True:
+            for item in particles:
+                if isinstance(item, groups.XsdGroup):
+                    current_path.append(item)
+                    iterators.append(particles)
+                    particles = iter(item)
+                    if len(iterators) > limits.MAX_MODEL_DEPTH:
+                        raise XMLSchemaModelDepthError(group)
+                    break
+                else:
+                    yield item
+            else:
+                try:
+                    current_path.pop()
+                    particles = iterators.pop()
+                except IndexError:
+                    return
+
+    paths: Any = {}
+    current_path: List[ModelParticleType] = [group]
+    try:
+        any_element = group.parent.open_content.any_element  # type: ignore[union-attr]
+    except AttributeError:
+        any_element = None
+
+    for e in safe_iter_path():
+
+        previous_path: List[ModelParticleType]
+        for pe, previous_path in paths.values():
+            # EDC check
+            if not e.is_consistent(pe) or any_element and not any_element.is_consistent(pe):
+                msg = _("Element Declarations Consistent violation between {0!r} and {1!r}"
+                        ": match the same name but with different types").format(e, pe)
+                raise XMLSchemaModelError(group, msg)
+
+            # UPA check
+            if pe is e or not pe.is_overlap(e):
+                continue
+            elif pe.parent is e.parent:
+                if pe.parent.model in {'all', 'choice'}:
+                    if isinstance(pe, Xsd11AnyElement) and not isinstance(e, XsdAnyElement):
+                        pe.add_precedence(e, group)
+                    elif isinstance(e, Xsd11AnyElement) and not isinstance(pe, XsdAnyElement):
+                        e.add_precedence(pe, group)
+                    else:
+                        msg = _("{0!r} and {1!r} overlap and are in the same {2!r} group")
+                        raise XMLSchemaModelError(group, msg.format(pe, e, pe.parent.model))
+                elif pe.is_univocal():
+                    continue
+
+            if distinguishable_paths(previous_path + [pe], current_path + [e]):
+                continue
+            elif isinstance(pe, Xsd11AnyElement) and not isinstance(e, XsdAnyElement):
+                pe.add_precedence(e, group)
+            elif isinstance(e, Xsd11AnyElement) and not isinstance(pe, XsdAnyElement):
+                e.add_precedence(pe, group)
+            else:
+                msg = _("Unique Particle Attribution violation between {0!r} and {1!r}")
+                raise XMLSchemaModelError(group, msg.format(pe, e))
+
+        paths[e.name] = e, current_path[:]
+
+
 class ModelVisitor:
     """
     A visitor design pattern class that can be used for validating XML data related to an XSD
     model group. The visit of the model is done using an external match information,
     counting the occurrences and yielding tuples in case of model's item occurrence errors.
     Ends setting the current element to `None`.
 
@@ -101,14 +181,16 @@
     :ivar group: the current XSD model group, initialized to *root* argument.
     :ivar items: the current XSD group's items iterator.
     :ivar match: if the XSD group has an effective item match.
     """
     _groups: List[Tuple[ModelGroupType, Iterator[ModelParticleType], bool]]
     element: Optional[SchemaElementType]
 
+    __slots__ = '_groups', 'root', 'occurs', 'element', 'group', 'items', 'match'
+
     def __init__(self, root: ModelGroupType) -> None:
         self._groups = []
         self.root = root
         self.occurs = Counter[Union[ModelParticleType, Tuple[ModelParticleType]]]()
         self.element = None
         self.group = root
         self.items = self.iter_group()
@@ -242,45 +324,45 @@
                 for k, item2 in enumerate(self.group, start=1):  # pragma: no cover
                     item_occurs = occurs[item2]
                     if not item_occurs:
                         continue
 
                     item_max_occurs = occurs[(item2,)] or item_occurs
                     if item_max_occurs == 1 or any(not x.is_emptiable() for x in self.group[k:]):
-                        self.occurs[self.group] += 1
+                        occurs[self.group] += 1
                         break
 
                     min_group_occurs = max(1, item_occurs // (item2.max_occurs or item_occurs))
                     max_group_occurs = max(1, item_max_occurs // (item2.min_occurs or 1))
 
                     occurs[self.group] += min_group_occurs
                     occurs[(self.group,)] += max_group_occurs
                     break
 
             return item.is_missing(max(occurs[item], occurs[(item,)]))
 
-        element, occurs = self.element, self.occurs
-        if element is None:
+        occurs = self.occurs
+        if self.element is None:
             raise XMLSchemaValueError("cannot advance, %r is ended!" % self)
 
         if match:
-            occurs[element] += 1
+            occurs[self.element] += 1
             self.match = True
             if self.group.model == 'all':
                 self.items = (e for e in self.group.iter_elements() if not e.is_over(occurs[e]))
-            elif not element.is_over(occurs[element]):
+            elif not self.element.is_over(occurs[self.element]):
                 return
-            elif self.group.model == 'choice' and element.is_ambiguous():
+            elif self.group.model == 'choice' and self.element.is_ambiguous():
                 return
 
         obj = None
         try:
-            element_occurs = occurs[element]
-            if stop_item(element):
-                yield element, element_occurs, [element]
+            element_occurs = occurs[self.element]
+            if stop_item(self.element):
+                yield self.element, element_occurs, [self.element]
 
             while True:
                 while self.group.is_over(max(occurs[self.group], occurs[(self.group,)])):
                     stop_item(self.group)
 
                 obj = next(self.items, None)
                 if isinstance(obj, groups.XsdGroup):
@@ -329,135 +411,160 @@
                     if obj is not None:
                         yield self.group, occurs[self.group], self.expected
                 elif any(e.min_occurs > occurs[e] for e in self.group):
                     yield self.group, occurs[self.group], self.expected
             elif self.group.max_occurs is not None and self.group.max_occurs < occurs[self.group]:
                 yield self.group, occurs[self.group], self.expected
 
-    def sort_content(self, content: EncodedContentType, restart: bool = True) \
-            -> List[ContentItemType]:
-        if restart:
-            self.restart()
-        return [(name, value) for name, value in self.iter_unordered_content(content)]
-
+    # Kept for backward compatibility
     def iter_unordered_content(
             self, content: EncodedContentType,
             default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
-        """
-        Takes an unordered content stored in a dictionary of lists and yields the
-        content elements sorted with the ordering defined by the model. Character
-        data parts are yielded at start and between child elements.
-
-        Ordering is inferred from ModelVisitor instance with any elements that
-        don't fit the schema placed at the end of the returned sequence. Checking
-        the yielded content validity is the responsibility of method *iter_encode*
-        of class :class:`XsdGroup`.
-
-        :param content: a dictionary of element names to list of element contents \
-        or an iterable composed of couples of name and value. In case of a \
-        dictionary the values must be lists where each item is the content \
-        of a single element.
-        :param default_namespace: the default namespace to apply for matching names.
-        """
-        consumable_content: Dict[str, Any]
+        return iter_unordered_content(content, self.root, default_namespace)
 
-        if isinstance(content, dict):
-            cdata_content = sorted(
-                ((k, v) for k, v in content.items() if isinstance(k, int)), reverse=True
-            )
-            consumable_content = {k: deque(v) for k, v in content.items() if not isinstance(k, int)}
-        else:
-            cdata_content = sorted(((k, v) for k, v in content if isinstance(k, int)), reverse=True)
-            consumable_content = defaultdict(deque)
-            for k, v in content:
-                if isinstance(k, str):
-                    consumable_content[k].append(v)
-
-        if cdata_content:
-            yield cdata_content.pop()
-
-        while self.element is not None and consumable_content:  # pragma: no cover
-            for name in consumable_content:
-                if self.element.is_matching(name, default_namespace, group=self.group):
-                    yield name, consumable_content[name].popleft()
-                    if not consumable_content[name]:
-                        del consumable_content[name]
-                    for _ in self.advance(True):
-                        pass
-                    if cdata_content:
-                        yield cdata_content.pop()
-                    break
-            else:
-                # Consume the return of advance otherwise we get stuck in an infinite loop.
-                for _ in self.advance(False):
-                    pass
+    def iter_collapsed_content(
+            self, content: Iterable[ContentItemType],
+            default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
+        return iter_collapsed_content(content, self.root, default_namespace)
 
-        # Add the remaining consumable content onto the end of the data.
-        for name, values in consumable_content.items():
-            for v in values:
-                yield name, v
+
+#
+# Functions for manipulating encoded content
+
+def iter_unordered_content(
+        content: EncodedContentType,
+        group: ModelGroupType,
+        default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
+    """
+    Takes an unordered content stored in a dictionary of lists and yields the
+    content elements sorted with the ordering defined by the model group. Character
+    data parts are yielded at start and between child elements.
+
+    Ordering is inferred from ModelVisitor instance with any elements that
+    don't fit the schema placed at the end of the returned sequence. Checking
+    the yielded content validity is the responsibility of method *iter_encode*
+    of class :class:`XsdGroup`.
+
+    :param content: a dictionary of element names to list of element contents \
+    or an iterable composed of couples of name and value. In case of a \
+    dictionary the values must be lists where each item is the content \
+    of a single element.
+    :param group: the model group related to content.
+    :param default_namespace: the default namespace to apply for matching names.
+    """
+    consumable_content: Dict[str, Any]
+
+    if isinstance(content, MutableMapping):
+        cdata_content = sorted(
+            ((k, v) for k, v in content.items() if isinstance(k, int)), reverse=True
+        )
+        consumable_content = {
+            k: deque(v) if isinstance(v, MutableSequence) else deque([v])
+            for k, v in content.items() if not isinstance(k, int)
+        }
+    else:
+        cdata_content = sorted(((k, v) for k, v in content if isinstance(k, int)), reverse=True)
+        consumable_content = defaultdict(deque)
+        for k, v in content:
+            if isinstance(k, str):
+                consumable_content[k].append(v)
+
+    if cdata_content:
+        yield cdata_content.pop()
+
+    model = ModelVisitor(group)
+    while model.element is not None and consumable_content:  # pragma: no cover
+        for name in consumable_content:
+            if model.element.is_matching(name, default_namespace, group=group):
+                yield name, consumable_content[name].popleft()
+                if not consumable_content[name]:
+                    del consumable_content[name]
+                for _err in model.advance(True):
+                    pass
                 if cdata_content:
                     yield cdata_content.pop()
+                break
+        else:
+            # Consume the return of advance otherwise we get stuck in an infinite loop.
+            for _err in model.advance(False):
+                pass
 
-        while cdata_content:
-            yield cdata_content.pop()
-
-    def iter_collapsed_content(
-            self, content: Iterable[Tuple[Union[int, str], Any]],
-            default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
-        """
-        Iterates a content stored in a sequence of couples *(name, value)*, yielding
-        items in the same order of the sequence, except for repetitions of the same
-        tag that don't match with the current element of the :class:`ModelVisitor`
-        instance. These items are included in an unsorted buffer and yielded asap
-        when there is a match with the model's element or at the end of the iteration.
-
-        This iteration mode, in cooperation with the method *iter_encode* of the class
-        XsdGroup, facilitates the encoding of content formatted with a convention that
-        collapses the children with the same tag into a list (eg. BadgerFish).
+    # Add the remaining consumable content onto the end of the data.
+    for name, values in consumable_content.items():
+        for v in values:
+            yield name, v
+            if cdata_content:
+                yield cdata_content.pop()
+
+    while cdata_content:
+        yield cdata_content.pop()
+
+
+def sort_content(content: EncodedContentType,
+                 group: ModelGroupType,
+                 default_namespace: Optional[str] = None) -> List[ContentItemType]:
+    return [x for x in iter_unordered_content(content, group, default_namespace)]
+
+
+def iter_collapsed_content(
+        content: Iterable[ContentItemType],
+        group: ModelGroupType,
+        default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
+    """
+    Iterates a content stored in a sequence of couples *(name, value)*, yielding
+    items in the same order of the sequence, except for repetitions of the same
+    tag that don't match with the current element of the :class:`ModelVisitor`
+    instance. These items are included in an unsorted buffer and yielded asap
+    when there is a match with the model's element or at the end of the iteration.
+
+    This iteration mode, in cooperation with the method *iter_encode* of the class
+    XsdGroup, facilitates the encoding of content formatted with a convention that
+    collapses the children with the same tag into a list (eg. BadgerFish).
+
+    :param content: an iterable containing couples of names and values.
+    :param group: the model group related to content.
+    :param default_namespace: the default namespace to apply for matching names.
+    """
+    prev_name = None
+    unordered_content: Dict[str, Any] = defaultdict(deque)
 
-        :param content: an iterable containing couples of names and values.
-        :param default_namespace: the default namespace to apply for matching names.
-        """
-        prev_name = None
-        unordered_content: Dict[str, Any] = defaultdict(deque)
+    model = ModelVisitor(group)
+    for name, value in content:
+        if isinstance(name, int) or model.element is None:
+            yield name, value
+            continue
 
-        for name, value in content:
-            if isinstance(name, int) or self.element is None:
+        while model.element is not None:
+            if model.element.is_matching(name, default_namespace, group=group):
                 yield name, value
-                continue
+                prev_name = name
+                for _err in model.advance(True):
+                    pass
+                break
 
-            while self.element is not None:
-                if self.element.is_matching(name, default_namespace, group=self.group):
-                    yield name, value
-                    prev_name = name
-                    for _ in self.advance(True):
-                        pass
+            for key in unordered_content:
+                if model.element.is_matching(key, default_namespace, group=group):
+                    break
+            else:
+                if prev_name == name:
+                    unordered_content[name].append(value)
                     break
 
-                for key in unordered_content:
-                    if self.element.is_matching(key, default_namespace, group=self.group):
-                        break
-                else:
-                    if prev_name == name:
-                        unordered_content[name].append(value)
-                        break
-
-                    for _ in self.advance(False):
-                        pass
-                    continue
+                for _err in model.advance(False):
+                    pass
+                continue
 
-                try:
-                    yield key, unordered_content[key].popleft()
-                except IndexError:
-                    del unordered_content[key]
-                else:
-                    for _ in self.advance(True):
-                        pass
+            try:
+                yield key, unordered_content[key].popleft()
+            except IndexError:
+                del unordered_content[key]
             else:
-                yield name, value
-                prev_name = name
+                for _err in model.advance(True):
+                    pass
+        else:
+            yield name, value
+            prev_name = name
 
-        # Add the remaining consumable content onto the end of the data.
-        for name, values in unordered_content.items():
-            for v in values:
-                yield name, v
+    # Add the remaining consumable content onto the end of the data.
+    for name, values in unordered_content.items():
+        for v in values:
+            yield name, v
```

### Comparing `xmlschema-2.2.2/xmlschema/validators/notations.py` & `xmlschema-2.2.3/xmlschema/validators/notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/particles.py` & `xmlschema-2.2.3/xmlschema/validators/particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/schemas.py` & `xmlschema-2.2.3/xmlschema/validators/schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/simple_types.py` & `xmlschema-2.2.3/xmlschema/validators/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/wildcards.py` & `xmlschema-2.2.3/xmlschema/validators/wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/validators/xsdbase.py` & `xmlschema-2.2.3/xmlschema/validators/xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema/xpath.py` & `xmlschema-2.2.3/xmlschema/xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.2/xmlschema.egg-info/PKG-INFO` & `xmlschema-2.2.3/xmlschema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.2.2
+Version: 2.2.3
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Provides-Extra: codegen
 Provides-Extra: dev
```

### Comparing `xmlschema-2.2.2/xmlschema.egg-info/SOURCES.txt` & `xmlschema-2.2.3/xmlschema.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,17 @@
 tests/test_cases/issues/issue_324/issue_324-valid.xml
 tests/test_cases/issues/issue_324/issue_324.zip
 tests/test_cases/issues/issue_324/issue_324a.xsd
 tests/test_cases/issues/issue_324/issue_324b.xsd
 tests/test_cases/issues/issue_334/issue_334.xml
 tests/test_cases/issues/issue_334/issue_334.xsd
 tests/test_cases/issues/issue_334/issue_334.zip
+tests/test_cases/issues/issue_341/issue_341-ext.xsd
+tests/test_cases/issues/issue_341/issue_341.xml
+tests/test_cases/issues/issue_341/issue_341.xsd
 tests/test_cases/mypy/extra_validator.py
 tests/test_cases/mypy/schema_source.py
 tests/test_cases/mypy/simple_types.py
 tests/test_cases/resources/dummy file #2.txt
 tests/test_cases/resources/dummy file.txt
 tests/test_cases/resources/external_entity.xml
 tests/test_cases/resources/malformed.xml
```

