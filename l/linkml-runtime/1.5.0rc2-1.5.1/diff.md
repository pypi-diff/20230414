# Comparing `tmp/linkml_runtime-1.5.0rc2.tar.gz` & `tmp/linkml_runtime-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_runtime-1.5.0rc2.tar", max compression
+gzip compressed data, was "linkml_runtime-1.5.1.tar", max compression
```

## Comparing `linkml_runtime-1.5.0rc2.tar` & `linkml_runtime-1.5.1.tar`

### file list

```diff
@@ -1,141 +1,142 @@
--rw-r--r--   0        0        0     7048 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/LICENSE
--rw-r--r--   0        0        0     1990 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/README.md
--rw-r--r--   0        0        0     1179 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/__init__.py
--rw-r--r--   0        0        0      426 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/__init__.py
--rw-r--r--   0        0        0     1225 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/csv_dumper.py
--rw-r--r--   0        0        0      863 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/dumper_root.py
--rw-r--r--   0        0        0     3950 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/json_dumper.py
--rw-r--r--   0        0        0     3771 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/rdf_dumper.py
--rw-r--r--   0        0        0     7077 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/rdflib_dumper.py
--rw-r--r--   0        0        0      751 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/yaml_dumper.py
--rw-r--r--   0        0        0        0 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/index/__init__.py
--rw-r--r--   0        0        0     8875 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/index/object_index.py
--rw-r--r--   0        0        0      119 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/README.md
--rw-r--r--   0        0        0      738 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/__init__.py
--rw-r--r--   0        0        0     3240 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/annotations.py
--rw-r--r--   0        0        0     3333 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/extensions.py
--rw-r--r--   0        0        0      114 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/graphql/README.md
--rw-r--r--   0        0        0    30306 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/graphql/meta.graphql
--rw-r--r--   0        0        0      111 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/README.md
--rw-r--r--   0        0        0    11169 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/annotations.json
--rw-r--r--   0        0        0     9306 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/extensions.json
--rw-r--r--   0        0        0    12109 2023-03-17 17:01:23.498455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/mappings.json
--rw-r--r--   0        0        0   222072 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/meta.json
--rw-r--r--   0        0        0     6442 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/types.json
--rw-r--r--   0        0        0    22401 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/units.json
--rw-r--r--   0        0        0    14834 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/validation.json
--rw-r--r--   0        0        0      113 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/README.md
--rw-r--r--   0        0        0      648 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
--rw-r--r--   0        0        0      648 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
--rw-r--r--   0        0        0     7019 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/context.jsonld
--rw-r--r--   0        0        0      587 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
--rw-r--r--   0        0        0      587 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
--rw-r--r--   0        0        0     1615 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
--rw-r--r--   0        0        0     1615 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
--rw-r--r--   0        0        0    13814 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
--rw-r--r--   0        0        0    14266 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
--rw-r--r--   0        0        0      610 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/types.context.jsonld
--rw-r--r--   0        0        0      610 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
--rw-r--r--   0        0        0     2065 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/units.context.jsonld
--rw-r--r--   0        0        0     2065 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
--rw-r--r--   0        0        0     1910 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
--rw-r--r--   0        0        0     1910 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
--rw-r--r--   0        0        0      117 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/README.md
--rw-r--r--   0        0        0     4196 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
--rw-r--r--   0        0        0     1984 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
--rw-r--r--   0        0        0      297 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
--rw-r--r--   0        0        0   353208 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/meta.schema.json
--rw-r--r--   0        0        0      291 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/types.schema.json
--rw-r--r--   0        0        0     5621 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/units.schema.json
--rw-r--r--   0        0        0     2291 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/validation.schema.json
--rw-r--r--   0        0        0     7126 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/linkml_files.py
--rw-r--r--   0        0        0     1821 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/mappings.py
--rw-r--r--   0        0        0   249036 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/meta.py
--rw-r--r--   0        0        0      112 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/README.md
--rw-r--r--   0        0        0      118 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/docs/credits.md
--rw-r--r--   0        0        0      141 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/docs/home.md
--rw-r--r--   0        0        0        5 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/import_map.json
--rw-r--r--   0        0        0      119 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/README.md
--rw-r--r--   0        0        0      833 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/annotations.yaml
--rw-r--r--   0        0        0     1057 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/extensions.yaml
--rw-r--r--   0        0        0     2755 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/mappings.yaml
--rw-r--r--   0        0        0    89120 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/meta.yaml
--rw-r--r--   0        0        0     3880 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/types.yaml
--rw-r--r--   0        0        0     2776 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/units.yaml
--rw-r--r--   0        0        0     2953 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/validation.yaml
--rw-r--r--   0        0        0      110 2023-03-17 17:01:23.502455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/owl/README.md
--rw-r--r--   0        0        0   192274 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/owl/meta.owl.ttl
--rw-r--r--   0        0        0      110 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/README.md
--rw-r--r--   0        0        0    13054 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/annotations.model.ttl
--rw-r--r--   0        0        0    13054 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/annotations.ttl
--rw-r--r--   0        0        0    10932 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/extensions.model.ttl
--rw-r--r--   0        0        0    10932 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/extensions.ttl
--rw-r--r--   0        0        0    13825 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/mappings.model.ttl
--rw-r--r--   0        0        0    13825 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/mappings.ttl
--rw-r--r--   0        0        0   207795 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/meta.model.ttl
--rw-r--r--   0        0        0   207795 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/meta.ttl
--rw-r--r--   0        0        0     7565 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/types.model.ttl
--rw-r--r--   0        0        0     7565 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/types.ttl
--rw-r--r--   0        0        0    25276 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/units.model.ttl
--rw-r--r--   0        0        0    25276 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/units.ttl
--rw-r--r--   0        0        0    16810 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/validation.model.ttl
--rw-r--r--   0        0        0    16810 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/validation.ttl
--rw-r--r--   0        0        0      113 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/README.md
--rw-r--r--   0        0        0     1261 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/annotations.shex
--rw-r--r--   0        0        0     8918 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/annotations.shexj
--rw-r--r--   0        0        0      821 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/extensions.shex
--rw-r--r--   0        0        0     5303 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/extensions.shexj
--rw-r--r--   0        0        0      424 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/mappings.shex
--rw-r--r--   0        0        0     2568 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/mappings.shexj
--rw-r--r--   0        0        0    37441 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/meta.shex
--rw-r--r--   0        0        0   254576 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/meta.shexj
--rw-r--r--   0        0        0      459 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/types.shex
--rw-r--r--   0        0        0     2568 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/types.shexj
--rw-r--r--   0        0        0     1682 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/units.shex
--rw-r--r--   0        0        0    11643 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/units.shexj
--rw-r--r--   0        0        0     1519 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/validation.shex
--rw-r--r--   0        0        0     7343 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/validation.shexj
--rw-r--r--   0        0        0     4599 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/types.py
--rw-r--r--   0        0        0     3332 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/units.py
--rw-r--r--   0        0        0     6897 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/validation.py
--rw-r--r--   0        0        0      426 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/__init__.py
--rw-r--r--   0        0        0     1533 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/context_flattener.py
--rw-r--r--   0        0        0     1933 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/csv_loader.py
--rw-r--r--   0        0        0     1318 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/json_loader.py
--rw-r--r--   0        0        0     5199 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/loader_root.py
--rw-r--r--   0        0        0     4735 2023-03-17 17:01:23.506455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/rdf_loader.py
--rw-r--r--   0        0        0    14065 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/rdflib_loader.py
--rw-r--r--   0        0        0     1358 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/requests_ssl_patch.py
--rw-r--r--   0        0        0     1821 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/loaders/yaml_loader.py
--rw-r--r--   0        0        0    39671 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/processing/referencevalidator.py
--rw-r--r--   0        0        0    26951 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/processing/validation_datamodel.py
--rw-r--r--   0        0        0    10253 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/processing/validation_datamodel.yaml
--rw-r--r--   0        0        0        0 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/__init__.py
--rw-r--r--   0        0        0      850 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/comparefiles.py
--rw-r--r--   0        0        0     1972 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/compile_python.py
--rw-r--r--   0        0        0     3960 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/context_utils.py
--rw-r--r--   0        0        0     2389 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/csvutils.py
--rw-r--r--   0        0        0      486 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/curienamespace.py
--rw-r--r--   0        0        0     1325 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/dataclass_extensions_376.py
--rw-r--r--   0        0        0      433 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/dictutils.py
--rw-r--r--   0        0        0     2554 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/distroutils.py
--rw-r--r--   0        0        0     3683 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/enumerations.py
--rw-r--r--   0        0        0     6755 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/eval_utils.py
--rw-r--r--   0        0        0     6594 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/formatutils.py
--rw-r--r--   0        0        0     5672 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/inference_utils.py
--rw-r--r--   0        0        0     1976 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/introspection.py
--rw-r--r--   0        0        0    11551 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/metamodelcore.py
--rw-r--r--   0        0        0    10580 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/namespaces.py
--rw-r--r--   0        0        0     2870 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/pattern.py
--rw-r--r--   0        0        0     6697 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/permissiblevalueimpl.py
--rw-r--r--   0        0        0     4715 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/ruleutils.py
--rw-r--r--   0        0        0     2287 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/schema_as_dict.py
--rw-r--r--   0        0        0     2815 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/schemaops.py
--rw-r--r--   0        0        0    66368 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/schemaview.py
--rw-r--r--   0        0        0     4327 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/schemaview_cli.py
--rw-r--r--   0        0        0      368 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/slot.py
--rw-r--r--   0        0        0      641 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/strictness.py
--rw-r--r--   0        0        0     1405 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/walker_utils.py
--rw-r--r--   0        0        0    19743 2023-03-17 17:01:23.510455 linkml_runtime-1.5.0rc2/linkml_runtime/utils/yamlutils.py
--rw-r--r--   0        0        0     1829 2023-03-17 17:01:50.298216 linkml_runtime-1.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 linkml_runtime-1.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-04-14 20:04:34.213671 linkml_runtime-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1990 2023-04-14 20:04:34.213671 linkml_runtime-1.5.1/README.md
+-rw-r--r--   0        0        0     1179 2023-04-14 20:04:34.213671 linkml_runtime-1.5.1/linkml_runtime/__init__.py
+-rw-r--r--   0        0        0      426 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/csv_dumper.py
+-rw-r--r--   0        0        0      863 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/dumper_root.py
+-rw-r--r--   0        0        0     3950 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/json_dumper.py
+-rw-r--r--   0        0        0     3771 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/rdf_dumper.py
+-rw-r--r--   0        0        0     7077 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/rdflib_dumper.py
+-rw-r--r--   0        0        0      751 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/yaml_dumper.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/index/__init__.py
+-rw-r--r--   0        0        0     8875 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/index/object_index.py
+-rw-r--r--   0        0        0      119 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/README.md
+-rw-r--r--   0        0        0      738 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/__init__.py
+-rw-r--r--   0        0        0     3240 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/annotations.py
+-rw-r--r--   0        0        0     3333 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/extensions.py
+-rw-r--r--   0        0        0      114 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/graphql/README.md
+-rw-r--r--   0        0        0    30306 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/graphql/meta.graphql
+-rw-r--r--   0        0        0      111 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/README.md
+-rw-r--r--   0        0        0    11169 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/annotations.json
+-rw-r--r--   0        0        0     9306 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/extensions.json
+-rw-r--r--   0        0        0    12109 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/mappings.json
+-rw-r--r--   0        0        0   222072 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/meta.json
+-rw-r--r--   0        0        0     6442 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/types.json
+-rw-r--r--   0        0        0    22401 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/units.json
+-rw-r--r--   0        0        0    14834 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/validation.json
+-rw-r--r--   0        0        0      113 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/README.md
+-rw-r--r--   0        0        0      648 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
+-rw-r--r--   0        0        0      648 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
+-rw-r--r--   0        0        0     7019 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/context.jsonld
+-rw-r--r--   0        0        0      587 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
+-rw-r--r--   0        0        0      587 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
+-rw-r--r--   0        0        0    13814 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
+-rw-r--r--   0        0        0    14266 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
+-rw-r--r--   0        0        0      610 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.context.jsonld
+-rw-r--r--   0        0        0      610 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
+-rw-r--r--   0        0        0      117 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/README.md
+-rw-r--r--   0        0        0     4196 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
+-rw-r--r--   0        0        0     1984 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
+-rw-r--r--   0        0        0      297 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
+-rw-r--r--   0        0        0   353208 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/meta.schema.json
+-rw-r--r--   0        0        0      291 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/types.schema.json
+-rw-r--r--   0        0        0     5621 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/units.schema.json
+-rw-r--r--   0        0        0     2291 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/validation.schema.json
+-rw-r--r--   0        0        0     7126 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/linkml_files.py
+-rw-r--r--   0        0        0     1821 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/mappings.py
+-rw-r--r--   0        0        0   249036 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/meta.py
+-rw-r--r--   0        0        0      112 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/README.md
+-rw-r--r--   0        0        0      118 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/docs/credits.md
+-rw-r--r--   0        0        0      141 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/docs/home.md
+-rw-r--r--   0        0        0        5 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/import_map.json
+-rw-r--r--   0        0        0      119 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/README.md
+-rw-r--r--   0        0        0      833 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/annotations.yaml
+-rw-r--r--   0        0        0     1057 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/extensions.yaml
+-rw-r--r--   0        0        0     2755 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/mappings.yaml
+-rw-r--r--   0        0        0    89120 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/meta.yaml
+-rw-r--r--   0        0        0     3880 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/types.yaml
+-rw-r--r--   0        0        0     2776 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/units.yaml
+-rw-r--r--   0        0        0     2953 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/validation.yaml
+-rw-r--r--   0        0        0      110 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/owl/README.md
+-rw-r--r--   0        0        0   192274 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/owl/meta.owl.ttl
+-rw-r--r--   0        0        0      110 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/README.md
+-rw-r--r--   0        0        0    13054 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.model.ttl
+-rw-r--r--   0        0        0    13054 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.ttl
+-rw-r--r--   0        0        0    10932 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.model.ttl
+-rw-r--r--   0        0        0    10932 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.ttl
+-rw-r--r--   0        0        0    13825 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.model.ttl
+-rw-r--r--   0        0        0    13825 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.ttl
+-rw-r--r--   0        0        0   207795 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.model.ttl
+-rw-r--r--   0        0        0   207795 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.ttl
+-rw-r--r--   0        0        0     7565 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.model.ttl
+-rw-r--r--   0        0        0     7565 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.ttl
+-rw-r--r--   0        0        0    25276 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.model.ttl
+-rw-r--r--   0        0        0    25276 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.ttl
+-rw-r--r--   0        0        0    16810 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.model.ttl
+-rw-r--r--   0        0        0    16810 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.ttl
+-rw-r--r--   0        0        0      113 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/README.md
+-rw-r--r--   0        0        0     1261 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shex
+-rw-r--r--   0        0        0     8918 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shexj
+-rw-r--r--   0        0        0      821 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shex
+-rw-r--r--   0        0        0     5303 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shexj
+-rw-r--r--   0        0        0      424 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/mappings.shex
+-rw-r--r--   0        0        0     2568 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/mappings.shexj
+-rw-r--r--   0        0        0    37441 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shex
+-rw-r--r--   0        0        0   254576 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shexj
+-rw-r--r--   0        0        0      459 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/types.shex
+-rw-r--r--   0        0        0     2568 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/types.shexj
+-rw-r--r--   0        0        0     1682 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shex
+-rw-r--r--   0        0        0    11643 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shexj
+-rw-r--r--   0        0        0     1519 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shex
+-rw-r--r--   0        0        0     7343 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shexj
+-rw-r--r--   0        0        0     4599 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/types.py
+-rw-r--r--   0        0        0     3332 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/units.py
+-rw-r--r--   0        0        0     6897 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/validation.py
+-rw-r--r--   0        0        0      426 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/context_flattener.py
+-rw-r--r--   0        0        0     1933 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/csv_loader.py
+-rw-r--r--   0        0        0     1318 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/json_loader.py
+-rw-r--r--   0        0        0     5199 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/loader_root.py
+-rw-r--r--   0        0        0     4735 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/rdf_loader.py
+-rw-r--r--   0        0        0    14065 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/rdflib_loader.py
+-rw-r--r--   0        0        0     1358 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/requests_ssl_patch.py
+-rw-r--r--   0        0        0     1821 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/yaml_loader.py
+-rw-r--r--   0        0        0    42218 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/processing/referencevalidator.py
+-rw-r--r--   0        0        0    26951 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.py
+-rw-r--r--   0        0        0    10253 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.yaml
+-rw-r--r--   0        0        0        0 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/__init__.py
+-rw-r--r--   0        0        0      850 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/comparefiles.py
+-rw-r--r--   0        0        0     1972 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/compile_python.py
+-rw-r--r--   0        0        0     4034 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/context_utils.py
+-rw-r--r--   0        0        0     2389 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/csvutils.py
+-rw-r--r--   0        0        0      486 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/curienamespace.py
+-rw-r--r--   0        0        0     1325 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/dataclass_extensions_376.py
+-rw-r--r--   0        0        0      433 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/dictutils.py
+-rw-r--r--   0        0        0     2554 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/distroutils.py
+-rw-r--r--   0        0        0     3683 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/enumerations.py
+-rw-r--r--   0        0        0     6755 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/eval_utils.py
+-rw-r--r--   0        0        0     6594 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/formatutils.py
+-rw-r--r--   0        0        0     5672 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/inference_utils.py
+-rw-r--r--   0        0        0     1976 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/introspection.py
+-rw-r--r--   0        0        0    11553 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/metamodelcore.py
+-rw-r--r--   0        0        0    10580 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/namespaces.py
+-rw-r--r--   0        0        0     2870 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/pattern.py
+-rw-r--r--   0        0        0     6697 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/permissiblevalueimpl.py
+-rw-r--r--   0        0        0     4720 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/ruleutils.py
+-rw-r--r--   0        0        0     2287 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schema_as_dict.py
+-rw-r--r--   0        0        0     9312 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schema_builder.py
+-rw-r--r--   0        0        0     2815 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schemaops.py
+-rw-r--r--   0        0        0    66900 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schemaview.py
+-rw-r--r--   0        0        0     4327 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schemaview_cli.py
+-rw-r--r--   0        0        0      368 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/slot.py
+-rw-r--r--   0        0        0      641 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/strictness.py
+-rw-r--r--   0        0        0     1405 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/walker_utils.py
+-rw-r--r--   0        0        0    19743 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/yamlutils.py
+-rw-r--r--   0        0        0     1826 2023-04-14 20:04:54.545859 linkml_runtime-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 linkml_runtime-1.5.1/PKG-INFO
```

### Comparing `linkml_runtime-1.5.0rc2/LICENSE` & `linkml_runtime-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/README.md` & `linkml_runtime-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/__init__.py` & `linkml_runtime-1.5.1/linkml_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/csv_dumper.py` & `linkml_runtime-1.5.1/linkml_runtime/dumpers/csv_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/dumper_root.py` & `linkml_runtime-1.5.1/linkml_runtime/dumpers/dumper_root.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/json_dumper.py` & `linkml_runtime-1.5.1/linkml_runtime/dumpers/json_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/rdf_dumper.py` & `linkml_runtime-1.5.1/linkml_runtime/dumpers/rdf_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/rdflib_dumper.py` & `linkml_runtime-1.5.1/linkml_runtime/dumpers/rdflib_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/dumpers/yaml_dumper.py` & `linkml_runtime-1.5.1/linkml_runtime/dumpers/yaml_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/index/object_index.py` & `linkml_runtime-1.5.1/linkml_runtime/index/object_index.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/__init__.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/annotations.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/annotations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/extensions.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/extensions.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/graphql/meta.graphql` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/graphql/meta.graphql`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/annotations.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/annotations.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/extensions.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/extensions.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/mappings.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/mappings.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/meta.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/meta.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/types.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/types.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/units.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/units.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/json/validation.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/validation.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/meta.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/types.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/units.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/validation.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/annotations.schema.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/annotations.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/extensions.schema.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/extensions.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/meta.schema.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/meta.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/units.schema.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/units.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/jsonschema/validation.schema.json` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/validation.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/linkml_files.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/linkml_files.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/mappings.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/mappings.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/meta.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/meta.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/annotations.yaml` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/annotations.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/extensions.yaml` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/extensions.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/mappings.yaml` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/mappings.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/meta.yaml` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/meta.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/types.yaml` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/types.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/units.yaml` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/units.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/model/schema/validation.yaml` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/validation.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/owl/meta.owl.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/owl/meta.owl.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/annotations.model.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/annotations.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/extensions.model.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/extensions.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/mappings.model.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/mappings.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/meta.model.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/meta.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/types.model.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/types.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/units.model.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/units.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/validation.model.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/rdf/validation.ttl` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/annotations.shex` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/annotations.shexj` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/extensions.shex` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/extensions.shexj` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/mappings.shexj` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/mappings.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/meta.shex` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/meta.shexj` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/types.shexj` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/types.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/units.shex` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/units.shexj` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/validation.shex` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/shex/validation.shexj` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/types.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/types.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/units.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/units.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/linkml_model/validation.py` & `linkml_runtime-1.5.1/linkml_runtime/linkml_model/validation.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/context_flattener.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/context_flattener.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/csv_loader.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/json_loader.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/loader_root.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/loader_root.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/rdf_loader.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/rdf_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/rdflib_loader.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/rdflib_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/requests_ssl_patch.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/requests_ssl_patch.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/loaders/yaml_loader.py` & `linkml_runtime-1.5.1/linkml_runtime/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/processing/referencevalidator.py` & `linkml_runtime-1.5.1/linkml_runtime/processing/referencevalidator.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,23 +72,87 @@
     "xsd:decimal": Decimal,
     "xsd:dateTime": (str, datetime.datetime, datetime.time, XSDTime),
     "xsd:date": (str, datetime.date, XSDDate),
     "xsd:time": XSDTime,
 }
 
 
+def _is_list_of_lists(x: Any) -> bool:
+    """
+    True x is of the form `[[...`
+
+    >>> _is_list_of_lists([1])
+    False
+    >>> _is_list_of_lists([[1,2],[3,4]])
+    True
+    >>> _is_list_of_lists([[]])
+    True
+
+    :param x: element to be tested
+    :return: True if LoL
+    """
+    return x and isinstance(x, list) and isinstance(x[0], list)
+
+
+def linearize_nested_lists(nested_list: List, is_row_ordered=True):
+    """
+    Returns a linear sequence of elements corresponding to a nested list array representation
+
+    >>> linearize_nested_lists([[11,12,13],[21,22,23],[31,32,33]], is_row_ordered=True)
+    [11, 12, 13, 21, 22, 23, 31, 32, 33]
+
+    >>> linearize_nested_lists([[11,12,13],[21,22,23],[31,32,33]], is_row_ordered=False)
+    [11, 21, 31, 12, 22, 32, 13, 23, 33]
+
+    :param nested_list:
+    :param is_row_ordered:
+    :return:
+    """
+    if not is_row_ordered:
+        return _linearize_nested_list_column_order(nested_list)
+    # row-ordered
+    result = []
+    stack = [iter(nested_list)]
+    while stack:
+        try:
+            item = next(stack[-1])
+            if isinstance(item, list):
+                stack.append(iter(item))
+            else:
+                result.append(item)
+        except StopIteration:
+            stack.pop()
+    return result
+
+
+def _linearize_nested_list_column_order(nested_list):
+    result = []
+    if not nested_list:
+        return result
+
+    num_rows = len(nested_list)
+    max_row_len = max(len(row) for row in nested_list)
+
+    for col in range(max_row_len):
+        for row in range(num_rows):
+            if col < len(nested_list[row]):
+                result.append(nested_list[row][col])
+
+    return result
+
 class CollectionForm(Enum):
     """Form of a schema element.
     See Part 6 of the LinkML specification"""
 
     NonCollection = "NonCollection"
     ExpandedDict = "ExpandedDict"
     CompactDict = "CompactDict"
     SimpleDict = "SimpleDict"
     List = "List"
+    ListOfLists = "ListOfLists"
 
 
 COLLECTION_FORM_NORMALIZATION = Tuple[CollectionForm, CollectionForm]
 COLLECTION_FORM_ANNOTATION_KEY = "collection_form"
 
 
 @dataclass
@@ -323,15 +387,15 @@
         Create a parent slot that points at the target element.
 
         :param target:
         :param input_object:
         :return:
         """
         target = self._schema_root(target)
-        slot = SlotDefinition(name="temp", range=target)
+        slot = SlotDefinition(name="temp", range=target, inlined=True)
         if input_object is None or isinstance(input_object, dict):
             slot.inlined = True
         elif isinstance(input_object, list):
             slot.inlined = True
             slot.inlined_as_list = True
             slot.multivalued = True
         return slot
@@ -352,15 +416,15 @@
         pk_slot_name = None
         range_element = self._slot_range_element(parent_slot)
         # Infer collection form, and normalize to this form, if necessary
         form = self.infer_slot_collection_form(parent_slot)
         normalized_object = copy(input_object)
         if isinstance(range_element, ClassDefinition):
             pk_slot_name = self._identifier_slot_name(range_element)
-        normalized_object = self.normalize_to_collection_from(
+        normalized_object = self.normalize_to_collection_form(
             form, normalized_object, parent_slot, pk_slot_name, report
         )
         # Validate
         new_report = Report()
         if parent_slot.required and not normalized_object:
             report.add_problem(
                 ConstraintType.RequiredConstraint, parent_slot.range, str(input_object)
@@ -379,20 +443,23 @@
                     for k, v in normalized_object.items()
                 }
             else:
                 output_object = {
                     k: self.normalize_instance(v, simple_dict_value_slot, new_report)
                     for k, v in normalized_object.items()
                 }
+        elif _is_list_of_lists(normalized_object):
+            raise NotImplementedError(f"List of Lists: {normalized_object}")
         elif isinstance(normalized_object, list):
             output_object = [
                 self.normalize_instance(v, parent_slot, new_report)
                 for v in normalized_object
             ]
         else:
+            # normalize an instance
             output_object = self.normalize_instance(
                 normalized_object, parent_slot, new_report
             )
         report.combine(new_report)
         return output_object
 
     def _is_dict_collection(
@@ -428,22 +495,39 @@
         if (
             "expanded" in parent_slot.annotations
             and parent_slot.annotations["expanded"].value
         ):
             return CollectionForm.ExpandedDict
         return CollectionForm.CompactDict
 
-    def normalize_to_collection_from(
+    def normalize_to_collection_form(
         self,
         form: CollectionForm,
         input_object: Any,
         slot: SlotDefinition,
         pk_slot_name: SlotDefinitionName,
         report: Report,
     ) -> Any:
+        """
+        Normalizes the input object to a defined form
+
+        :param form:
+        :param input_object:
+        :param slot:
+        :param pk_slot_name:
+        :param report:
+        :return:
+        """
+        if _is_list_of_lists(input_object):
+            if form != CollectionForm.List:
+                return input_object
+            if not any(impl for impl in slot.implements if impl == "linkml:elements"):
+                return input_object
+            is_row_ordered = not any(impl for impl in slot.implements if impl == "linkml:ColumnOrderedArray")
+            input_object = linearize_nested_lists(input_object, is_row_ordered)
         if form == CollectionForm.NonCollection:
             return self.ensure_non_collection(input_object, slot, pk_slot_name, report)
         elif form == CollectionForm.List:
             return self.ensure_list(input_object, slot, pk_slot_name, report)
         elif form == CollectionForm.ExpandedDict:
             return self.ensure_expanded_dict(input_object, slot, pk_slot_name, report)
         elif form == CollectionForm.CompactDict:
@@ -659,24 +743,24 @@
             else:
                 return self.normalize_reference(input_object, range_element, report)
         elif isinstance(range_element, EnumDefinition):
             return self.normalize_enum(input_object, range_element, report)
         elif isinstance(range_element, TypeDefinition):
             return self.normalize_type(input_object, range_element, report, parent_slot)
         else:
-            raise ValueError(f"Cannot normalize: unknown range {parent_slot.range}")
+            return input_object
 
     def normalize_reference(
         self, input_object: dict, target: ClassDefinition, report: Report
     ) -> dict:
         pk_slot = self._identifier_slot(target)
         if pk_slot is None:
             raise AssertionError(f"Cannot normalize: no primary key for {target.name}")
         return self.normalize_type(
-            input_object, self.derived_schema.types[pk_slot.range], report
+            input_object, self.derived_schema.types.get(pk_slot.range, None), report
         )
 
     def normalize_object(
         self, input_object: dict, target: ClassDefinition, report: Report
     ) -> dict:
         if not isinstance(input_object, dict):
             raise AssertionError(
@@ -765,20 +849,22 @@
                 ConstraintType.PermissibleValueConstraint, target.name, input_object
             )
         return input_object
 
     def normalize_type(
         self,
         input_object: Any,
-        target: TypeDefinition,
+        target: Optional[TypeDefinition],
         report: Report,
         parent_slot: SlotDefinition = None,
     ) -> Any:
         if input_object is None:
             return None
+        if target is None:
+           return input_object
         output_value = input_object
         if target.base in XSD_OR_BASE_TO_PYTHON:
             expected_python_type = XSD_OR_BASE_TO_PYTHON[target.base]
         elif target.uri in XSD_OR_BASE_TO_PYTHON:
             expected_python_type = XSD_OR_BASE_TO_PYTHON[target.uri]
         else:
             report.add_problem(
@@ -866,25 +952,25 @@
                 return
 
     def subsumes(self, parent: ClassDefinition, child: ClassDefinition):
         return parent.name in self.schemaview.class_ancestors(
             child.name, reflexive=True
         )
 
-    def _slot_range_element(self, slot: SlotDefinition) -> Element:
+    def _slot_range_element(self, slot: SlotDefinition) -> Optional[Element]:
         ds = self.derived_schema
         sr = slot.range
         if sr in ds.classes:
             return ds.classes[sr]
         elif sr in ds.enums:
             return ds.enums[sr]
         elif sr in ds.types:
             return ds.types[sr]
         else:
-            raise ValueError(f"Undefined range {sr}")
+            return None
 
     def _slot_collection_form(self, slot: SlotDefinition) -> CollectionForm:
         if not slot.multivalued:
             return CollectionForm.NonCollection
         if slot.inlined_as_list:
             return CollectionForm.List
         if not slot.inlined:
```

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/processing/validation_datamodel.py` & `linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/processing/validation_datamodel.yaml` & `linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/comparefiles.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/comparefiles.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/compile_python.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/compile_python.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/context_utils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/context_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         JsonObj(**{"@context": context_list[0] if len(context_list) == 1 else context_list})
 
 
 def map_import(importmap: Dict[str, str], namespaces: Callable[[None], "Namespaces"], imp: Any) -> str:
     """
     lookup an import in an importmap.
 
+    An importmap is a dictionary that maps CURIEs or URIs to file paths.
+
     :param importmap:
     :param namespaces:
     :param imp:
     :return:
     """
     sname = str(imp)
     if ':' in sname:
```

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/csvutils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/csvutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/dataclass_extensions_376.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/dataclass_extensions_376.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/distroutils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/distroutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/enumerations.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/enumerations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/eval_utils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/formatutils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/formatutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/inference_utils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/introspection.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/metamodelcore.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/metamodelcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 
 class URI(URIorCURIE):
     """ A relative absolute URI
     """
     def __init__(self, v: str) -> None:
         if is_strict() and not URI.is_valid(v):
-            raise ValueError(f"{v}: is not a valid URI")
+            raise ValueError(f"'{v}': is not a valid URI")
         super().__init__(v)
 
     # this is more inclusive than the W3C specification
     #uri_re = re.compile("^[A-Za-z]\\S*$")
     uri_re = re.compile("^\\S+$")
 
     @classmethod
```

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/namespaces.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/pattern.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/pattern.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/permissiblevalueimpl.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/permissiblevalueimpl.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/ruleutils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/ruleutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             conjs.append(get_disjunction(slot.range_expression))
         else:
             logging.warning(f'Expected range_expression for {slot.name} to be a class expression, not {type(slot.range_expression)}')
     if len(conjs) == 0:
         if slot.range:
             conjs.append({slot.range})
         else:
-            logging.warning(f'No range for {slot}')
+            logging.warning(f'No range for {slot.name}')
     if len(conjs) > 1:
         raise Exception(f'Cannot determine range disjunction for {slot}, got conjunctions: {conjs}')
     if len(conjs) == 0:
         return None
     else:
         return conjs[0]
```

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/schema_as_dict.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/schema_as_dict.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/schemaops.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/schemaops.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/schemaview.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/schemaview.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,23 +64,37 @@
 
 def load_schema_wrap(path: str, **kwargs):
     # import here to avoid circular imports
     from linkml_runtime.loaders.yaml_loader import YAMLLoader
     yaml_loader = YAMLLoader()
     schema: SchemaDefinition
     schema = yaml_loader.load(path, target_class=SchemaDefinition, **kwargs)
-    if "\n" not in path and "://" not in path:
+    if "\n" not in path:
+    # if "\n" not in path and "://" not in path:
         # only set path if the input is not a yaml string or URL.
         # Setting the source path is necessary for relative imports;
         # while initializing a schema with a yaml string is possible, there
         # should be no expectation of relative imports working.
         schema.source_file = path
     return schema
 
 
+def is_absolute_path(path: str) -> bool:
+    if path.startswith("/"):
+        return True
+    # windows
+    if not os.path.isabs(path):
+        return False
+    norm_path = os.path.normpath(path)
+    if norm_path.startswith("\\\\") or ":" not in norm_path:
+        return False
+    drive, tail = os.path.splitdrive(norm_path)
+    return bool(drive and tail)
+
+
 @dataclass
 class SchemaUsage():
     """
     A usage of an element of a schema
     """
     used_by: ElementName
     slot: SlotDefinitionName
@@ -165,30 +179,35 @@
         import, in which case it is fetched from within the linkml_runtime package, where the yaml
         is distributed. This ensures that the version of the metamodel imported matches the version
         of the linkml_runtime package.
 
         In future, this mechanism may be extended to arbitrary modules, such that we avoid
         network dependence at runtime in general.
 
+        For local paths, the import is resolved relative to the directory containing the source file,
+        or the URL of the source file, if it is a URL.
+
         :param imp:
         :param from_schema:
         :return:
         """
         if from_schema is None:
             from_schema = self.schema
         from linkml_runtime import SCHEMA_DIRECTORY
         default_import_map = {
             "linkml:": str(SCHEMA_DIRECTORY)
         }
         importmap = {**default_import_map, **self.importmap}
         sname = map_import(importmap, self.namespaces, imp)
-        logging.info(f'Importing {imp} as {sname} from source {from_schema.source_file}')
-        schema = load_schema_wrap(sname + '.yaml',
-                                  base_dir=os.path.dirname(
-                                  from_schema.source_file) if from_schema.source_file else None)
+        if from_schema.source_file and not is_absolute_path(sname):
+            base_dir = os.path.dirname(from_schema.source_file)
+        else:
+            base_dir = None
+        logging.info(f'Importing {imp} as {sname} from source {from_schema.source_file}; base_dir={base_dir}')
+        schema = load_schema_wrap(sname + '.yaml', base_dir=base_dir)
         return schema
 
     @lru_cache()
     def imports_closure(self, imports: bool = True, traverse=True, inject_metadata=True) -> List[SchemaDefinitionName]:
         """
         Return all imports
 
@@ -1219,14 +1238,16 @@
             if v is None:
                 if metaslot_name == 'range':
                     v = self.schema.default_range
             if v is not None:
                 setattr(induced_slot, metaslot_name, v)
         if slot.inlined_as_list:
             slot.inlined = True
+        if slot.identifier or slot.key:
+            slot.required = True
         if mangle_name:
             mangled_name = f'{camelcase(class_name)}__{underscore(slot_name)}'
             induced_slot.name = mangled_name
         if not induced_slot.alias:
             induced_slot.alias = underscore(slot_name)
         for c in self.all_classes().values():
             if induced_slot.name in c.slots or induced_slot.name in c.attributes:
@@ -1449,29 +1470,28 @@
         for class_definition in self.all_classes().values():
             if class_definition.slot_usage:
                 for slot_definition in class_definition.slot_usage.values():
                     if slot_definition.range == enum_name:
                         enum_slots.append(slot_definition)
         return enum_slots
 
-    def get_classes_modifying_slot(self, slot_name: SLOT_NAME = None) -> List[ClassDefinition]:
+    def get_classes_modifying_slot(self, slot: SlotDefinition) -> List[ClassDefinition]:
         """Get all ClassDefinitions that modify a given slot.
 
         :param slot_name: slot in consideration
         :return: list of ClassDefinitions modifying the slot of interest
         """
-        # slot_classes = [c for c in self.all_classes().values() if c.slot_usage == slot_name]
-        # slot_classes = [c for c in self.all_classes().values()]
-        slot_classes = []
+        modifying_classes = []
         for class_definition in self.all_classes().values():
             if class_definition.slot_usage:
                 for slot_definition in class_definition.slot_usage.values():
-                    if slot_definition.name == slot_name:
-                        slot_classes.append(class_definition)
-        return slot_classes
+                    if slot_definition.name == slot.name:
+                        modifying_classes.append(class_definition.name)
+
+        return modifying_classes
 
     def is_slot_percent_encoded(self, slot: SlotDefinitionName) -> bool:
         """
         True if slot or its range is has a percent_encoded annotation.
 
         This is true for type fields that are the range of identifier columns,
         where the identifier is not guaranteed to be a valid URI or CURIE
@@ -1683,15 +1703,15 @@
 
             if class_definition.attributes:
                 for slot_definition in class_definition.attributes.values():
                     materialize_pattern_into_slot_definition(slot_definition)
 
     def materialize_derived_schema(self) -> SchemaDefinition:
         """ Materialize a schema view into a schema definition """
-        derived_schema = copy(self.schema)
+        derived_schema = deepcopy(self.schema)
         derived_schemaview = SchemaView(derived_schema)
         derived_schemaview.merge_imports()
         for typ in [deepcopy(t) for t in self.all_types().values()]:
             for typ_anc_name in self.type_ancestors(typ.name, reflexive=False):
                 a = derived_schema.types[typ_anc_name]
                 if not typ.uri:
                     typ.uri = a.uri
```

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/schemaview_cli.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/schemaview_cli.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/strictness.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/strictness.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/walker_utils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/walker_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/linkml_runtime/utils/yamlutils.py` & `linkml_runtime-1.5.1/linkml_runtime/utils/yamlutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.0rc2/pyproject.toml` & `linkml_runtime-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml-runtime"
-version = "v1.5.0rc2"
+version = "v1.5.1"
 description = "Runtime environment for LinkML, the Linked open data modeling language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sierra Moxon <smoxon@lbl.gov>",
     "Bill Duncan <wdduncan@gmail.com>",
     "Harshad Hegde <hhegde@lbl.gov>"
```

### Comparing `linkml_runtime-1.5.0rc2/PKG-INFO` & `linkml_runtime-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-runtime
-Version: 1.5.0rc2
+Version: 1.5.1
 Summary: Runtime environment for LinkML, the Linked open data modeling language
 Home-page: https://github.com/linkml/linkml-runtime
 Keywords: linkml,metamodel,schema visualization,rdf,owl,yaml
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

