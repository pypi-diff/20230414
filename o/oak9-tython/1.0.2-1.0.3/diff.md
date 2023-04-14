# Comparing `tmp/oak9_tython-1.0.2.tar.gz` & `tmp/oak9_tython-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oak9_tython-1.0.2.tar", last modified: Tue Apr 11 17:57:06 2023, max compression
+gzip compressed data, was "oak9_tython-1.0.3.tar", last modified: Fri Apr 14 17:34:06 2023, max compression
```

## Comparing `oak9_tython-1.0.2.tar` & `oak9_tython-1.0.3.tar`

### file list

```diff
@@ -1,1167 +1,1167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.275495 oak9_tython-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 17:57:06.275495 oak9_tython-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.071495 oak9_tython-1.0.2/oak9/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.071495 oak9_tython-1.0.2/oak9/tython/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.071495 oak9_tython-1.0.2/oak9/tython/core/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.075495 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/blueprint_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_repo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.075495 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/empty_implements_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/no_implements_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/core/cf_types/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/cf_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/cf_types/capability.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/core/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/sdk/graph_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/sdk/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/sdk/resource_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/core/services/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/services/runner_input_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    31215 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/types_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.079495 oak9_tython-1.0.2/oak9/tython/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.159495 oak9_tython-1.0.2/oak9/tython/models/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_accessanalyzer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_accessanalyzer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_acmpca_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_acmpca_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_acmpca_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_alexa_ask_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_alexa_ask_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_amazonmq_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_amazonmq_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_amazonmq_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_amplify_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_amplify_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_amplify_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31462 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigateway_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    85923 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigateway_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigateway_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigatewayv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigatewayv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appconfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appconfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appconfig_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    88173 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appflow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationautoscaling_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationinsights_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationinsights_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    39964 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appmesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   115709 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appmesh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appmesh_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appsync_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41375 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appsync_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_appsync_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_athena_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_athena_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_athena_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscaling_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscaling_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscaling_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscalingplans_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscalingplans_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_backup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_budgets_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_budgets_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_budgets_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cassandra_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cassandra_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cassandra_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_certificatemanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_certificatemanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_chatbot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_chatbot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_chatbot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloud9_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloud9_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloud9_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudformation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudformation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudformation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudfront_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    68732 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudfront_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudfront_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudtrail_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudtrail_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudwatch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21664 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudwatch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codebuild_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38727 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codebuild_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codebuild_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codecommit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codecommit_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codecommit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codedeploy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codedeploy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codedeploy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codeguruprofiler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codegurureviewer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codegurureviewer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codepipeline_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codepipeline_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codepipeline_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarconnections_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarconnections_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarnotifications_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarnotifications_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29385 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cognito_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    87415 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cognito_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_cognito_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    46100 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_datapipeline_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_datapipeline_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_datapipeline_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_detective_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_detective_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_detective_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_directoryservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_directoryservice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_directoryservice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dlm_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dlm_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dlm_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    32336 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_docdb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_docdb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_docdb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    64868 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_instance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_networkacl_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    70103 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   219118 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_securitygroup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_subnet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_subnet_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecr_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecr_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29143 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    87498 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_efs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_efs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_efs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_eks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_eks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_eks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticbeanstalk_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    60919 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticsearch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticsearch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_emr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    85681 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_emr_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_emr_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_events_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_events_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_events_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_eventschemas_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_eventschemas_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_eventschemas_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_fms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_fms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_fms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_fsx_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_fsx_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_fsx_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_gamelift_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41568 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_gamelift_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_gamelift_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_globalaccelerator_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_globalaccelerator_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    35328 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_glue_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   104308 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_glue_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_glue_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    36639 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_greengrass_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   102539 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_greengrass_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_greengrass_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_groundstation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_groundstation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_groundstation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_guardduty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_guardduty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_guardduty_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iam_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_imagebuilder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33357 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_imagebuilder_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_inspector_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_inspector_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_inspector_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot1click_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot1click_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot1click_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57057 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotanalytics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    56169 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotanalytics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotevents_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39864 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotevents_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotevents_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesis_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalytics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20301 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    56745 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    60879 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisfirehose_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_kms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_lakeformation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_lakeformation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_lakeformation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_lambda_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38931 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_lambda_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_lambda_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_logs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_logs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_logs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_macie_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_macie_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_macie_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_managedblockchain_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_managedblockchain_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_mediaconvert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_mediaconvert_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_msk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_msk_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_msk_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_neptune_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_neptune_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_neptune_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_networkmanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_networkmanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_networkmanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19887 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    56713 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworkscm_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworkscm_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_qldb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_qldb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_qldb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ram_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ram_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ram_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38105 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbcluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbinstance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_redshift_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_redshift_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_redshift_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_resourcegroups_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_resourcegroups_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_robomaker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_robomaker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_robomaker_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53resolver_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53resolver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53resolver_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25507 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_s3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78676 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_s3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_s3_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22303 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sagemaker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    66680 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sagemaker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sagemaker_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sdb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sdb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sdb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_secretsmanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_secretsmanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_securityhub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_securityhub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_securityhub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicecatalog_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicecatalog_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicediscovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicediscovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sns_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sns_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sns_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sqs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sqs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sqs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ssm_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ssm_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_ssm_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sso_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sso_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_sso_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_stepfunctions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_stepfunctions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_synthetics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_synthetics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_synthetics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_transfer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_transfer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_transfer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_waf_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_waf_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_waf_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafregional_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafregional_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafregional_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   117299 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_workspaces_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_workspaces_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/aws/aws_workspaces_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.187495 oak9_tython-1.0.2/oak9/tython/models/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_aad_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_aad_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    49201 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   143537 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    71546 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30626 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cache_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cache_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    71498 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cdn_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    34710 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    67043 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47220 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   120178 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45682 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30190 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    84581 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerservice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_devices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39037 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_devices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    62661 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   158843 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_documentdb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_elastic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30105 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    47435 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40962 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_keyvault_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23604 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    63082 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    59960 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38521 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23525 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   101699 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   301469 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18672 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45382 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45963 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   131181 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31831 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40696 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    44588 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_servicebus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    63020 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    68845 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31681 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_storage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    91315 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_storage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    74260 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_web_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   226439 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_web_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.251495 oak9_tython-1.0.2/oak9/tython/models/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45414 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_access_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   115626 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_access_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_access_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_active_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_active_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_active_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apigee_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apigee_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apigee_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apikeys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apikeys_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30961 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    80283 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_artifact_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_artifact_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_artifact_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_assured_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_assured_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_assured_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigquery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   107299 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigquery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigtable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigtable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_billing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_billing_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_billing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_binary_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_binary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_binary_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_certificate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_certificate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_certificate_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    37530 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloud_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    96409 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloud_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloud_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudbuild_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_clouddeploy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudfunctions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudiot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudiot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_composer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_composer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_composer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_attached_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_attached_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_backend_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39586 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_backend_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_disk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_disk_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_external_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_external_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_firewall_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_forwarding_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_global_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_global_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ha_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ha_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_health_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_http_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_https_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_https_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_image_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    42340 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   110570 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_instance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_interconnect_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_managed_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_managed_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_node_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_node_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_packet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_packet_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_per_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_per_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_project_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    63992 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_region_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   170051 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_region_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_reservation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_router_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_router_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_security_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_security_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_shared_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_shared_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_snapshot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ssl_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_target_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_target_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    44049 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_url_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   112435 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_url_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_vpn_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    64469 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   166581 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_container_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_container_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    63657 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   146148 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_data_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataflow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataplex_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataplex_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    96272 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataproc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   222604 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataproc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_datastore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_datastore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_datastore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_deployment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_deployment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_deployment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27903 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dialogflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    76337 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dialogflow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dns_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dns_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dns_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_document_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_document_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_document_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_endpoints_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_endpoints_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_essential_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_essential_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_essential_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_eventarc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_eventarc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_filestore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_filestore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_filestore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firebaserules_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firebaserules_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firestore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firestore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firestore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_folder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_folder_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_folder_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_game_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25773 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_game_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_game_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_gke_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_gke_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_gke_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_container_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20029 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_healthcare_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_healthcare_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iam_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    55725 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iap_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iap_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_identity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27338 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_identity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_identity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_kms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25293 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_kms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_kms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_logging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41658 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_logging_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_logging_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_memcache_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_memcache_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_memcache_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_ml_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_ml_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32793 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    81993 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    62722 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_notebooks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57020 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_notebooks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_org_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_org_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_org_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_organization_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_organization_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_organization_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    39464 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_os_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    95395 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_os_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_os_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_privateca_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   110520 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_privateca_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_privateca_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_project_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_project_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_pubsub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41253 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_pubsub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_recaptcha_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_recaptcha_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_redis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_redis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_redis_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_resource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_scc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_scc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_scc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_secret_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_secret_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_secret_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sourcerepo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_spanner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_spanner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_spanner_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sql_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_storage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    66063 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_storage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_storage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tags_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tags_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tags_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tpu_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tpu_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tpu_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vertex_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vertex_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vertex_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vpc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vpc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_workflows_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_workflows_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_workflows_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50422 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.259495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33586 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   105265 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   323853 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.263495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33982 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25542 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.267495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30642 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38980 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    35874 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.271495 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apiserverinternal.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apps.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authorization.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.batch.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.certificates.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.coordination.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.core.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.discovery.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.events.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta3_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.node.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.policy.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.rbac.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.resource.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.scheduling.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1beta1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.apiextensionsapiserver.pkg.apis.apiextensions.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.api.resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.apis.meta.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.runtime_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.util.intstr_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io.k8s.kubeaggregator.pkg.apis.apiregistration.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.275495 oak9_tython-1.0.2/oak9/tython/models/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/shared/shared_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/shared/shared_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/oak9/tython/models/shared/shared_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-11 17:57:02.000000 oak9_tython-1.0.2/oak9/tython/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:57:06.275495 oak9_tython-1.0.2/oak9_tython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 17:57:05.000000 oak9_tython-1.0.2/oak9_tython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60432 2023-04-11 17:57:06.000000 oak9_tython-1.0.2/oak9_tython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:57:05.000000 oak9_tython-1.0.2/oak9_tython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 17:57:05.000000 oak9_tython-1.0.2/oak9_tython.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:57:06.275495 oak9_tython-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 17:57:03.000000 oak9_tython-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.810053 oak9_tython-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-14 17:34:06.810053 oak9_tython-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/blueprint_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_repo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.694052 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/empty_implements_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/no_implements_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.698052 oak9_tython-1.0.3/oak9/tython/core/cf_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/cf_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/cf_types/capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.698052 oak9_tython-1.0.3/oak9/tython/core/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/sdk/graph_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/sdk/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/sdk/resource_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.698052 oak9_tython-1.0.3/oak9/tython/core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/services/runner_input_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31216 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/types_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.698052 oak9_tython-1.0.3/oak9/tython/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.738052 oak9_tython-1.0.3/oak9/tython/models/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_accessanalyzer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_accessanalyzer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_acmpca_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_acmpca_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_acmpca_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_alexa_ask_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_alexa_ask_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_amazonmq_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_amazonmq_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_amazonmq_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_amplify_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_amplify_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_amplify_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31462 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigateway_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85923 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigateway_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigateway_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigatewayv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigatewayv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appconfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appconfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appconfig_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88173 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appflow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationautoscaling_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationinsights_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationinsights_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39964 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appmesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115709 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appmesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appmesh_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appsync_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41375 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appsync_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_appsync_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_athena_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_athena_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_athena_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscaling_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscaling_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscaling_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscalingplans_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscalingplans_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_budgets_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_budgets_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_budgets_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cassandra_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cassandra_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cassandra_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_certificatemanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_certificatemanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_chatbot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_chatbot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_chatbot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloud9_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloud9_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloud9_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudformation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudformation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudformation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudfront_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68732 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudfront_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudfront_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudtrail_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudtrail_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudwatch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21664 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudwatch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codebuild_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38727 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codebuild_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codebuild_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codecommit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codecommit_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codecommit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codedeploy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codedeploy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codedeploy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codeguruprofiler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codegurureviewer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codegurureviewer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codepipeline_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codepipeline_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codepipeline_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarconnections_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarconnections_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarnotifications_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarnotifications_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29385 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cognito_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87415 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cognito_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_cognito_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46100 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_datapipeline_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_datapipeline_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_datapipeline_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_detective_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_detective_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_detective_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_directoryservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_directoryservice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_directoryservice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dlm_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dlm_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dlm_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32336 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_docdb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_docdb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_docdb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64868 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_instance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_networkacl_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70103 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219118 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_securitygroup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_subnet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_subnet_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecr_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecr_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28648 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86946 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_efs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_efs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_efs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_eks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_eks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_eks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticbeanstalk_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60919 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticsearch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticsearch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_emr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85681 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_emr_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_emr_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_events_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_events_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_events_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_eventschemas_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_eventschemas_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_eventschemas_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_fms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_fms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_fms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_fsx_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_fsx_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_fsx_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_gamelift_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41568 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_gamelift_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_gamelift_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_globalaccelerator_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_globalaccelerator_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35328 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_glue_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104308 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_glue_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_glue_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36639 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_greengrass_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102539 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_greengrass_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_greengrass_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_groundstation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_groundstation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_groundstation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_guardduty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_guardduty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_guardduty_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iam_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_imagebuilder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33357 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_imagebuilder_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_inspector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_inspector_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_inspector_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot1click_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot1click_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot1click_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57057 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotanalytics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56169 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotanalytics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotevents_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39864 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotevents_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotevents_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesis_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalytics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20301 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56745 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60879 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisfirehose_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_kms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_lakeformation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_lakeformation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_lakeformation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_lambda_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38931 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_lambda_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_lambda_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_logs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_logs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_logs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_macie_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_macie_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_macie_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_managedblockchain_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_managedblockchain_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_mediaconvert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_mediaconvert_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_msk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_msk_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_msk_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_neptune_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_neptune_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_neptune_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_networkmanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_networkmanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_networkmanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19887 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56713 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworkscm_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworkscm_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_qldb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_qldb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_qldb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ram_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ram_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ram_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38105 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbcluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbinstance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_redshift_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_redshift_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_redshift_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_resourcegroups_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_resourcegroups_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_robomaker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_robomaker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_robomaker_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53resolver_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53resolver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53resolver_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25507 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_s3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78676 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_s3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_s3_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22303 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sagemaker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66680 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sagemaker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sagemaker_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sdb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sdb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sdb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_secretsmanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_secretsmanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_securityhub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_securityhub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_securityhub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicecatalog_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicecatalog_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicediscovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicediscovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sns_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sns_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sns_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sqs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sqs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sqs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ssm_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ssm_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_ssm_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sso_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sso_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_sso_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_stepfunctions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_stepfunctions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_synthetics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_synthetics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_synthetics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_transfer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_transfer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_transfer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_waf_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_waf_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_waf_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafregional_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafregional_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafregional_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117299 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_workspaces_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_workspaces_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/aws/aws_workspaces_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.754053 oak9_tython-1.0.3/oak9/tython/models/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_aad_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_aad_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49201 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143537 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71546 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30626 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cache_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cache_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71498 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cdn_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34710 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67043 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47220 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120178 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45682 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30190 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84581 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerservice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_devices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39037 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_devices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62661 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158843 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_documentdb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_elastic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30105 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47435 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40962 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_keyvault_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23604 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63082 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59960 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38521 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23525 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101699 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   301469 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18672 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45382 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45963 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131181 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31831 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40696 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44588 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_servicebus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63020 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68845 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31681 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_storage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91315 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_storage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75724 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_web_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   231864 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_web_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.794053 oak9_tython-1.0.3/oak9/tython/models/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45414 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_access_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115626 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_access_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_access_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_active_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_active_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_active_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apigee_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apigee_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apigee_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apikeys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apikeys_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30961 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80283 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_artifact_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_artifact_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_artifact_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_assured_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_assured_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_assured_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigquery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107299 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigquery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigtable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigtable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_billing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_billing_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_billing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_binary_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_binary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_binary_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_certificate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_certificate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_certificate_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37530 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96409 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloud_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloud_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudbuild_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_clouddeploy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudfunctions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudiot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudiot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_composer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_composer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_composer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_attached_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_attached_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_backend_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39586 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_backend_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_disk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_disk_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_external_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_external_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_firewall_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_forwarding_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_global_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_global_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ha_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ha_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_health_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_http_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_https_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_https_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_image_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42340 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110570 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_instance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_interconnect_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_managed_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_managed_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_node_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_node_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_packet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_packet_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_per_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_per_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_project_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63992 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_region_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170051 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_region_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_reservation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_router_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_router_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_security_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_security_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_shared_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_shared_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_snapshot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ssl_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_target_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_target_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44049 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_url_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112435 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_url_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_vpn_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64469 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166581 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_container_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_container_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63657 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146148 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataflow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataplex_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataplex_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96272 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataproc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222604 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataproc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_datastore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_datastore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_datastore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_deployment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_deployment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_deployment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27903 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dialogflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76337 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dialogflow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dns_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dns_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dns_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_document_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_document_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_document_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_endpoints_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_endpoints_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_essential_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_essential_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_essential_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_eventarc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_eventarc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_filestore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_filestore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_filestore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firebaserules_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firebaserules_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firestore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firestore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firestore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_folder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_folder_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_folder_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_game_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25773 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_game_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_game_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_gke_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_gke_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_gke_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_container_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20029 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_healthcare_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_healthcare_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iam_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55725 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iap_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iap_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_identity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27338 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_identity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_identity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_kms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25293 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_kms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_kms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_logging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41658 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_logging_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_logging_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_memcache_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_memcache_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_memcache_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_ml_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_ml_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32793 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81993 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62722 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_notebooks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57020 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_notebooks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_org_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_org_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_org_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_organization_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_organization_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_organization_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39464 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_os_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95395 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_os_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_os_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_privateca_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110520 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_privateca_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_privateca_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_project_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_project_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_pubsub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41253 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_pubsub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_recaptcha_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_recaptcha_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_redis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_redis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_redis_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_resource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_scc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_scc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_scc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_secret_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_secret_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_secret_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sourcerepo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_spanner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_spanner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_spanner_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_storage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66063 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_storage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_storage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tags_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tags_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tags_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tpu_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tpu_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tpu_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vertex_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vertex_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vertex_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vpc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vpc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_workflows_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_workflows_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_workflows_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50422 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.798053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33586 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105265 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   323853 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.802053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33982 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25542 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30642 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38980 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35874 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.806053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.810053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.810053 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apiserverinternal.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apps.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authorization.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.batch.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.certificates.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.coordination.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.core.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.discovery.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.events.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta3_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.node.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.policy.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.rbac.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.resource.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.scheduling.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1beta1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.apiextensionsapiserver.pkg.apis.apiextensions.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.api.resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.apis.meta.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.runtime_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.util.intstr_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io.k8s.kubeaggregator.pkg.apis.apiregistration.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.810053 oak9_tython-1.0.3/oak9/tython/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/shared/shared_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/shared/shared_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/models/shared/shared_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/oak9/tython/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:34:06.810053 oak9_tython-1.0.3/oak9_tython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-14 17:34:06.000000 oak9_tython-1.0.3/oak9_tython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60432 2023-04-14 17:34:06.000000 oak9_tython-1.0.3/oak9_tython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:34:06.000000 oak9_tython-1.0.3/oak9_tython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 17:34:06.000000 oak9_tython-1.0.3/oak9_tython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:34:06.810053 oak9_tython-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 17:34:04.000000 oak9_tython-1.0.3/setup.py
```

### Comparing `oak9_tython-1.0.2/LICENSE` & `oak9_tython-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/PKG-INFO` & `oak9_tython-1.0.3/oak9_tython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oak9_tython
-Version: 1.0.2
+Name: oak9-tython
+Version: 1.0.3
 Author: ['Claudio Balbin <cbalbin@oak9.io>', 'Brandon Nicoll <bnicoll@oak9.io>']
 Project-URL: Homepage, https://github.com/oak9io/tython
 Project-URL: Bug Tracker, https://github.com/oak9io/tython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `oak9_tython-1.0.2/README.md` & `oak9_tython-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/git_utils.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_repo.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_repo.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/policy_repo_test.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/policy_repo_test.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py` & `oak9_tython-1.0.3/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/exception.py` & `oak9_tython-1.0.3/oak9/tython/core/exception.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/logger.py` & `oak9_tython-1.0.3/oak9/tython/core/logger.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/sdk/graph_helper.py` & `oak9_tython-1.0.3/oak9/tython/core/sdk/graph_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,29 @@
 import core.sdk.helper as Helper
 
 class GraphHelper:
     '''
     Provides functions to handle graph data
     '''
     
-    
-    def filter_by_resource(graph: Graph, resource):
-        filtered_resource = []
+    def parse_resource(graph: Graph, resource):
+        parsed_resource = None
 
         for root_node in graph.root_nodes:
             mapped = grpc_type_map.get(root_node.node.resource.data.type_url)
             if mapped == resource:
-                # parse and add to the list
-                filtered_resource.append(Helper.unpack_grpc_resource(root_node.node.resource.data, mapped))
+                parsed_resource = Helper.unpack_grpc_resource(root_node.node.resource.data, mapped)
+                break
+
+        return parsed_resource
+    
+    
+    # def filter_by_resource(graph: Graph, resource):
+    #     filtered_resource = []
+
+    #     for root_node in graph.root_nodes:
+    #         mapped = grpc_type_map.get(root_node.node.resource.data.type_url)
+    #         if mapped == resource:
+    #             # parse and add to the list
+    #             filtered_resource.append(Helper.unpack_grpc_resource(root_node.node.resource.data, mapped))
 
-        return filtered_resource
+    #     return filtered_resource
```

### Comparing `oak9_tython-1.0.2/oak9/tython/core/sdk/helper.py` & `oak9_tython-1.0.3/oak9/tython/core/sdk/helper.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/sdk/resource_map.py` & `oak9_tython-1.0.3/oak9/tython/core/sdk/resource_map.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/tools.py` & `oak9_tython-1.0.3/oak9/tython/core/tools.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/types.py` & `oak9_tython-1.0.3/oak9/tython/core/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,15 +699,15 @@
         elif type(value) != str:
             self._preferred_value = str(value)
         else:
             self._preferred_value = value
 
     @property
     def additional_guidance(self):
-        return self.additional_guidance
+        return self._additional_guidance
 
     @additional_guidance.setter
     def additional_guidance(self, value):
         self._additional_guidance = value
 
     @property
     def severity(self) -> Severity:
```

### Comparing `oak9_tython-1.0.2/oak9/tython/core/types_tests.py` & `oak9_tython-1.0.3/oak9/tython/core/types_tests.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/core/utilities.py` & `oak9_tython-1.0.3/oak9/tython/core/utilities.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_accessanalyzer_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_accessanalyzer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_acmpca_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_acmpca_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_acmpca_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_acmpca_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_alexa_ask_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_alexa_ask_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_amazonmq_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_amazonmq_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_amazonmq_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_amazonmq_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_amplify_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_amplify_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_amplify_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_amplify_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigateway_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigateway_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigateway_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigateway_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigatewayv2_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigatewayv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appconfig_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appconfig_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appconfig_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appconfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appflow_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appflow_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appflow_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationinsights_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationinsights_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appmesh_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appmesh_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appmesh_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appmesh_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appsync_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appsync_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_appsync_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_appsync_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_athena_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_athena_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_athena_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_athena_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscaling_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscaling_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscaling_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscalingplans_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscalingplans_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_backup_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_backup_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_backup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_batch_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_batch_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_batch_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_budgets_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_budgets_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_budgets_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_budgets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cassandra_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cassandra_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cassandra_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cassandra_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_certificatemanager_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_certificatemanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_chatbot_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_chatbot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_chatbot_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_chatbot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloud9_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloud9_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloud9_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloud9_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudformation_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudformation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudformation_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudformation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudfront_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudfront_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudfront_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudfront_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudtrail_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudtrail_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudwatch_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudwatch_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codebuild_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codebuild_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codebuild_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codebuild_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codecommit_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codecommit_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codecommit_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codecommit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codedeploy_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codedeploy_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codedeploy_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codedeploy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codegurureviewer_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codegurureviewer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codepipeline_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codepipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codepipeline_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codepipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestar_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestar_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestar_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarconnections_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarconnections_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarnotifications_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarnotifications_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cognito_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cognito_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_cognito_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_cognito_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_config_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_config_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_config_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_datapipeline_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_datapipeline_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_datapipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_detective_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_detective_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_detective_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_detective_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_directoryservice_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_directoryservice_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_directoryservice_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_directoryservice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dlm_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dlm_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dlm_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dlm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dms_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dms_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_docdb_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_docdb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_docdb_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_docdb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_table_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_instance_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_route_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_route_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_route_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_subnet_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_subnet_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpc_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecr_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecr_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecr_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecr_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecs_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecs_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from oak9.tython.models.shared import shared_pb2 as shared_dot_shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x61ws/aws_ecs.proto\x12\x13oak9.tython.aws.ecs\x1a\x13shared/shared.proto\"\xc8\x01\n\x1e\x43\x61pacityProviderManagedScaling\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12!\n\x19minimum_scaling_step_size\x18\x02 \x01(\x05\x12!\n\x19maximum_scaling_step_size\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x17\n\x0ftarget_capacity\x18\x05 \x01(\x05\"\xf9\x01\n(CapacityProviderAutoScalingGroupProvider\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x1e\n\x16\x61uto_scaling_group_arn\x18\x02 \x01(\t\x12L\n\x0fmanaged_scaling\x18\x03 \x01(\x0b\x32\x33.oak9.tython.aws.ecs.CapacityProviderManagedScaling\x12&\n\x1emanaged_termination_protection\x18\x04 \x01(\t\"\xa9\x02\n\x10\x43\x61pacityProvider\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x62\n\x1b\x61uto_scaling_group_provider\x18\x02 \x01(\x0b\x32=.oak9.tython.aws.ecs.CapacityProviderAutoScalingGroupProvider\x12\x0c\n\x04name\x18\x03 \x01(\t\x12=\n\x04tags\x18\x04 \x03(\x0b\x32/.oak9.tython.aws.ecs.CapacityProvider.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd2\x02\n\x03\x45\x43S\x12@\n\x11\x63\x61pacity_provider\x18\x01 \x03(\x0b\x32%.oak9.tython.aws.ecs.CapacityProvider\x12-\n\x07\x63luster\x18\x02 \x01(\x0b\x32\x1c.oak9.tython.aws.ecs.Cluster\x12=\n\x10primary_task_set\x18\x03 \x01(\x0b\x32#.oak9.tython.aws.ecs.PrimaryTaskSet\x12-\n\x07service\x18\x04 \x03(\x0b\x32\x1c.oak9.tython.aws.ecs.Service\x12<\n\x0ftask_definition\x18\x05 \x03(\x0b\x32#.oak9.tython.aws.ecs.TaskDefinition\x12.\n\x08task_set\x18\x06 \x03(\x0b\x32\x1c.oak9.tython.aws.ecs.TaskSet\"n\n\x16\x43lusterClusterSettings\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x97\x01\n#ClusterCapacityProviderStrategyItem\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x19\n\x11\x63\x61pacity_provider\x18\x02 \x01(\t\x12\x0e\n\x06weight\x18\x03 \x01(\x05\x12\x0c\n\x04\x62\x61se\x18\x04 \x01(\x05\"\x84\x03\n\x07\x43luster\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x34\n\x04tags\x18\x02 \x03(\x0b\x32&.oak9.tython.aws.ecs.Cluster.TagsEntry\x12\x14\n\x0c\x63luster_name\x18\x03 \x01(\t\x12\x45\n\x10\x63luster_settings\x18\x04 \x03(\x0b\x32+.oak9.tython.aws.ecs.ClusterClusterSettings\x12\x1a\n\x12\x63\x61pacity_providers\x18\x05 \x03(\t\x12\x64\n\"default_capacity_provider_strategy\x18\x06 \x03(\x0b\x32\x38.oak9.tython.aws.ecs.ClusterCapacityProviderStrategyItem\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x80\x01\n\x0ePrimaryTaskSet\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63luster\x18\x02 \x01(\t\x12\x13\n\x0btask_set_id\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\"\x97\x01\n#ServiceCapacityProviderStrategyItem\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04\x62\x61se\x18\x02 \x01(\x05\x12\x19\n\x11\x63\x61pacity_provider\x18\x03 \x01(\t\x12\x0e\n\x06weight\x18\x04 \x01(\x05\"\x93\x01\n\x1eServiceDeploymentConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x17\n\x0fmaximum_percent\x18\x02 \x01(\x05\x12\x1f\n\x17minimum_healthy_percent\x18\x03 \x01(\x05\"V\n\x1bServiceDeploymentController\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\xb4\x01\n\x13ServiceLoadBalancer\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x1a\n\x12load_balancer_name\x18\x04 \x01(\t\x12\x18\n\x10target_group_arn\x18\x05 \x01(\t\"\x99\x01\n\x1aServiceAwsVpcConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x18\n\x10\x61ssign_public_ip\x18\x02 \x01(\t\x12\x17\n\x0fsecurity_groups\x18\x03 \x03(\t\x12\x0f\n\x07subnets\x18\x04 \x03(\t\"\xa6\x01\n\x1bServiceNetworkConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12N\n\x15\x61ws_vpc_configuration\x18\x02 \x01(\x0b\x32/.oak9.tython.aws.ecs.ServiceAwsVpcConfiguration\"i\n\x1aServicePlacementConstraint\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nexpression\x18\x02 \x01(\t\"b\n\x18ServicePlacementStrategy\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\r\n\x05\x66ield\x18\x02 \x01(\t\"\xa5\x01\n\x16ServiceServiceRegistry\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x0c\n\x04port\x18\x04 \x01(\x05\x12\x14\n\x0cregistry_arn\x18\x05 \x01(\t\"\xce\x08\n\x07Service\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x13\n\x0bservice_arn\x18\x02 \x01(\t\x12\\\n\x1a\x63\x61pacity_provider_strategy\x18\x03 \x03(\x0b\x32\x38.oak9.tython.aws.ecs.ServiceCapacityProviderStrategyItem\x12\x0f\n\x07\x63luster\x18\x04 \x01(\t\x12U\n\x18\x64\x65ployment_configuration\x18\x05 \x01(\x0b\x32\x33.oak9.tython.aws.ecs.ServiceDeploymentConfiguration\x12O\n\x15\x64\x65ployment_controller\x18\x06 \x01(\x0b\x32\x30.oak9.tython.aws.ecs.ServiceDeploymentController\x12\x15\n\rdesired_count\x18\x07 \x01(\x05\x12\x1f\n\x17\x65nable_ecs_managed_tags\x18\x08 \x01(\x08\x12)\n!health_check_grace_period_seconds\x18\t \x01(\x05\x12\x13\n\x0blaunch_type\x18\n \x01(\t\x12@\n\x0eload_balancers\x18\x0b \x03(\x0b\x32(.oak9.tython.aws.ecs.ServiceLoadBalancer\x12O\n\x15network_configuration\x18\x0c \x01(\x0b\x32\x30.oak9.tython.aws.ecs.ServiceNetworkConfiguration\x12N\n\x15placement_constraints\x18\r \x03(\x0b\x32/.oak9.tython.aws.ecs.ServicePlacementConstraint\x12K\n\x14placement_strategies\x18\x0e \x03(\x0b\x32-.oak9.tython.aws.ecs.ServicePlacementStrategy\x12\x18\n\x10platform_version\x18\x0f \x01(\t\x12\x16\n\x0epropagate_tags\x18\x10 \x01(\t\x12\x0c\n\x04role\x18\x11 \x01(\t\x12\x1b\n\x13scheduling_strategy\x18\x12 \x01(\t\x12\x14\n\x0cservice_name\x18\x13 \x01(\t\x12G\n\x12service_registries\x18\x14 \x03(\x0b\x32+.oak9.tython.aws.ecs.ServiceServiceRegistry\x12\x34\n\x04tags\x18\x15 \x03(\x0b\x32&.oak9.tython.aws.ecs.Service.TagsEntry\x12\x17\n\x0ftask_definition\x18\x16 \x01(\t\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x1aTaskDefinitionKeyValuePair\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"g\n\x1dTaskDefinitionEnvironmentFile\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\r\n\x05value\x18\x02 \x01(\t\"x\n\x17TaskDefinitionHostEntry\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x10\n\x08hostname\x18\x02 \x01(\t\x12\x12\n\nip_address\x18\x03 \x01(\t\"\xe6\x01\n#TaskDefinitionFirelensConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12V\n\x07options\x18\x02 \x03(\x0b\x32\x45.oak9.tython.aws.ecs.TaskDefinitionFirelensConfiguration.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaf\x01\n\x19TaskDefinitionHealthCheck\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63ommand\x18\x02 \x03(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12\x0f\n\x07retries\x18\x05 \x01(\x05\x12\x14\n\x0cstart_period\x18\x06 \x01(\x05\"v\n TaskDefinitionKernelCapabilities\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0b\n\x03\x61\x64\x64\x18\x02 \x03(\t\x12\x0c\n\x04\x64rop\x18\x03 \x03(\t\"\x8f\x01\n\x14TaskDefinitionDevice\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_path\x18\x02 \x01(\t\x12\x11\n\thost_path\x18\x03 \x01(\t\x12\x13\n\x0bpermissions\x18\x04 \x03(\t\"\x8b\x01\n\x13TaskDefinitionTmpfs\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_path\x18\x02 \x01(\t\x12\x15\n\rmount_options\x18\x03 \x03(\t\x12\x0c\n\x04size\x18\x04 \x01(\x05\"\xfa\x02\n\x1dTaskDefinitionLinuxParameters\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12K\n\x0c\x63\x61pabilities\x18\x02 \x01(\x0b\x32\x35.oak9.tython.aws.ecs.TaskDefinitionKernelCapabilities\x12:\n\x07\x64\x65vices\x18\x03 \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionDevice\x12\x1c\n\x14init_process_enabled\x18\x04 \x01(\x08\x12\x10\n\x08max_swap\x18\x05 \x01(\x05\x12\x1a\n\x12shared_memory_size\x18\x06 \x01(\x05\x12\x12\n\nswappiness\x18\x07 \x01(\x05\x12\x37\n\x05tmpfs\x18\x08 \x03(\x0b\x32(.oak9.tython.aws.ecs.TaskDefinitionTmpfs\"q\n\x14TaskDefinitionSecret\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nvalue_from\x18\x03 \x01(\t\"\xb3\x02\n\x1eTaskDefinitionLogConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nlog_driver\x18\x02 \x01(\t\x12Q\n\x07options\x18\x03 \x03(\x0b\x32@.oak9.tython.aws.ecs.TaskDefinitionLogConfiguration.OptionsEntry\x12\x41\n\x0esecret_options\x18\x04 \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionSecret\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x95\x01\n\x18TaskDefinitionMountPoint\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_path\x18\x02 \x01(\t\x12\x11\n\tread_only\x18\x03 \x01(\x08\x12\x15\n\rsource_volume\x18\x04 \x01(\t\"\x91\x01\n\x19TaskDefinitionPortMapping\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_port\x18\x02 \x01(\x05\x12\x11\n\thost_port\x18\x03 \x01(\x05\x12\x10\n\x08protocol\x18\x04 \x01(\t\"}\n#TaskDefinitionRepositoryCredentials\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x1d\n\x15\x63redentials_parameter\x18\x02 \x01(\t\"k\n!TaskDefinitionResourceRequirement\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\r\n\x05value\x18\x02 \x01(\t\"\x85\x01\n\x14TaskDefinitionUlimit\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nhard_limit\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nsoft_limit\x18\x04 \x01(\x05\"\x80\x01\n\x18TaskDefinitionVolumeFrom\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x11\n\tread_only\x18\x02 \x01(\x08\x12\x18\n\x10source_container\x18\x03 \x01(\t\"x\n\x1bTaskDefinitionSystemControl\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xa5\x0e\n!TaskDefinitionContainerDefinition\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63ommand\x18\x02 \x03(\t\x12\x0b\n\x03\x63pu\x18\x03 \x01(\x05\x12\x1a\n\x12\x64isable_networking\x18\x04 \x01(\x08\x12\x1a\n\x12\x64ns_search_domains\x18\x05 \x03(\t\x12\x13\n\x0b\x64ns_servers\x18\x06 \x03(\t\x12_\n\rdocker_labels\x18\x07 \x03(\x0b\x32H.oak9.tython.aws.ecs.TaskDefinitionContainerDefinition.DockerLabelsEntry\x12\x1f\n\x17\x64ocker_security_options\x18\x08 \x03(\t\x12\x13\n\x0b\x65ntry_point\x18\t \x03(\t\x12\x44\n\x0b\x65nvironment\x18\n \x03(\x0b\x32/.oak9.tython.aws.ecs.TaskDefinitionKeyValuePair\x12M\n\x11\x65nvironment_files\x18\x0b \x03(\x0b\x32\x32.oak9.tython.aws.ecs.TaskDefinitionEnvironmentFile\x12\x11\n\tessential\x18\x0c \x01(\x08\x12\x41\n\x0b\x65xtra_hosts\x18\r \x03(\x0b\x32,.oak9.tython.aws.ecs.TaskDefinitionHostEntry\x12X\n\x16\x66irelens_configuration\x18\x0e \x01(\x0b\x32\x38.oak9.tython.aws.ecs.TaskDefinitionFirelensConfiguration\x12\x44\n\x0chealth_check\x18\x0f \x01(\x0b\x32..oak9.tython.aws.ecs.TaskDefinitionHealthCheck\x12\x10\n\x08hostname\x18\x10 \x01(\t\x12\r\n\x05image\x18\x11 \x01(\t\x12\r\n\x05links\x18\x12 \x03(\t\x12L\n\x10linux_parameters\x18\x13 \x01(\x0b\x32\x32.oak9.tython.aws.ecs.TaskDefinitionLinuxParameters\x12N\n\x11log_configuration\x18\x14 \x01(\x0b\x32\x33.oak9.tython.aws.ecs.TaskDefinitionLogConfiguration\x12\x0e\n\x06memory\x18\x15 \x01(\x05\x12\x1a\n\x12memory_reservation\x18\x16 \x01(\x05\x12\x43\n\x0cmount_points\x18\x17 \x03(\x0b\x32-.oak9.tython.aws.ecs.TaskDefinitionMountPoint\x12\x0c\n\x04name\x18\x18 \x01(\t\x12\x45\n\rport_mappings\x18\x19 \x03(\x0b\x32..oak9.tython.aws.ecs.TaskDefinitionPortMapping\x12\x12\n\nprivileged\x18\x1a \x01(\x08\x12 \n\x18readonly_root_filesystem\x18\x1b \x01(\x08\x12X\n\x16repository_credentials\x18\x1c \x01(\x0b\x32\x38.oak9.tython.aws.ecs.TaskDefinitionRepositoryCredentials\x12U\n\x15resource_requirements\x18\x1d \x03(\x0b\x32\x36.oak9.tython.aws.ecs.TaskDefinitionResourceRequirement\x12:\n\x07secrets\x18\x1e \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionSecret\x12\x15\n\rstart_timeout\x18\x1f \x01(\x05\x12\x14\n\x0cstop_timeout\x18  \x01(\x05\x12:\n\x07ulimits\x18! \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionUlimit\x12\x0c\n\x04user\x18\" \x01(\t\x12\x43\n\x0cvolumes_from\x18# \x03(\x0b\x32-.oak9.tython.aws.ecs.TaskDefinitionVolumeFrom\x12\x19\n\x11working_directory\x18$ \x01(\t\x12\x13\n\x0binteractive\x18% \x01(\x08\x12\x17\n\x0fpseudo_terminal\x18& \x01(\x08\x12I\n\x0fsystem_controls\x18\' \x03(\x0b\x32\x30.oak9.tython.aws.ecs.TaskDefinitionSystemControl\x1a\x33\n\x11\x44ockerLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x01\n\"TaskDefinitionInferenceAccelerator\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x03 \x01(\t\"~\n/TaskDefinitionTaskDefinitionPlacementConstraint\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nexpression\x18\x02 \x01(\t\"\xcc\x01\n TaskDefinitionProxyConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12W\n\x1eproxy_configuration_properties\x18\x03 \x03(\x0b\x32/.oak9.tython.aws.ecs.TaskDefinitionKeyValuePair\"\xb7\x03\n\'TaskDefinitionDockerVolumeConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x15\n\rautoprovision\x18\x02 \x01(\x08\x12\x0e\n\x06\x64river\x18\x03 \x01(\t\x12\x61\n\x0b\x64river_opts\x18\x04 \x03(\x0b\x32L.oak9.tython.aws.ecs.TaskDefinitionDockerVolumeConfiguration.DriverOptsEntry\x12X\n\x06labels\x18\x05 \x03(\x0b\x32H.oak9.tython.aws.ecs.TaskDefinitionDockerVolumeConfiguration.LabelsEntry\x12\r\n\x05scope\x18\x06 \x01(\t\x1a\x31\n\x0f\x44riverOptsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xf9\x02\n$TaskDefinitionEFSVolumeConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x15\n\rfilesystem_id\x18\x02 \x01(\t\x12\x16\n\x0eroot_directory\x18\x03 \x01(\t\x12\x1a\n\x12transit_encryption\x18\x04 \x01(\t\x12\x1f\n\x17transit_encryption_port\x18\x05 \x01(\x05\x12p\n\x14\x61uthorization_config\x18\x06 \x03(\x0b\x32R.oak9.tython.aws.ecs.TaskDefinitionEFSVolumeConfiguration.AuthorizationConfigEntry\x1a:\n\x18\x41uthorizationConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\"TaskDefinitionHostVolumeProperties\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\"\xe4\x02\n\x14TaskDefinitionVolume\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x61\n\x1b\x64ocker_volume_configuration\x18\x02 \x01(\x0b\x32<.oak9.tython.aws.ecs.TaskDefinitionDockerVolumeConfiguration\x12[\n\x18\x65\x66s_volume_configuration\x18\x03 \x01(\x0b\x32\x39.oak9.tython.aws.ecs.TaskDefinitionEFSVolumeConfiguration\x12\x45\n\x04host\x18\x04 \x01(\x0b\x32\x37.oak9.tython.aws.ecs.TaskDefinitionHostVolumeProperties\x12\x0c\n\x04name\x18\x05 \x01(\t\"\x94\x06\n\x0eTaskDefinition\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0e\n\x06\x66\x61mily\x18\x02 \x01(\t\x12U\n\x15\x63ontainer_definitions\x18\x03 \x03(\x0b\x32\x36.oak9.tython.aws.ecs.TaskDefinitionContainerDefinition\x12\x0b\n\x03\x63pu\x18\x04 \x01(\t\x12\x1a\n\x12\x65xecution_role_arn\x18\x05 \x01(\t\x12W\n\x16inference_accelerators\x18\x06 \x03(\x0b\x32\x37.oak9.tython.aws.ecs.TaskDefinitionInferenceAccelerator\x12\x0e\n\x06memory\x18\x07 \x01(\t\x12\x14\n\x0cnetwork_mode\x18\x08 \x01(\t\x12\x63\n\x15placement_constraints\x18\t \x03(\x0b\x32\x44.oak9.tython.aws.ecs.TaskDefinitionTaskDefinitionPlacementConstraint\x12R\n\x13proxy_configuration\x18\n \x01(\x0b\x32\x35.oak9.tython.aws.ecs.TaskDefinitionProxyConfiguration\x12 \n\x18requires_compatibilities\x18\x0b \x03(\t\x12\x15\n\rtask_role_arn\x18\x0c \x01(\t\x12:\n\x07volumes\x18\r \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionVolume\x12\x10\n\x08pid_mode\x18\x0e \x01(\t\x12\x10\n\x08ipc_mode\x18\x0f \x01(\t\x12;\n\x04tags\x18\x10 \x03(\x0b\x32-.oak9.tython.aws.ecs.TaskDefinition.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb4\x01\n\x13TaskSetLoadBalancer\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x1a\n\x12load_balancer_name\x18\x04 \x01(\t\x12\x18\n\x10target_group_arn\x18\x05 \x01(\t\"\x99\x01\n\x1aTaskSetAwsVpcConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x18\n\x10\x61ssign_public_ip\x18\x02 \x01(\t\x12\x17\n\x0fsecurity_groups\x18\x03 \x03(\t\x12\x0f\n\x07subnets\x18\x04 \x03(\t\"\xa6\x01\n\x1bTaskSetNetworkConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12N\n\x15\x61ws_vpc_configuration\x18\x02 \x01(\x0b\x32/.oak9.tython.aws.ecs.TaskSetAwsVpcConfiguration\"d\n\x0cTaskSetScale\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"\xa5\x01\n\x16TaskSetServiceRegistry\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x0c\n\x04port\x18\x04 \x01(\x05\x12\x14\n\x0cregistry_arn\x18\x05 \x01(\t\"\xcf\x03\n\x07TaskSet\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63luster\x18\x02 \x01(\t\x12\x13\n\x0b\x65xternal_id\x18\x03 \x01(\t\x12\x13\n\x0blaunch_type\x18\x04 \x01(\t\x12@\n\x0eload_balancers\x18\x05 \x03(\x0b\x32(.oak9.tython.aws.ecs.TaskSetLoadBalancer\x12O\n\x15network_configuration\x18\x06 \x01(\x0b\x32\x30.oak9.tython.aws.ecs.TaskSetNetworkConfiguration\x12\x18\n\x10platform_version\x18\x07 \x01(\t\x12\x30\n\x05scale\x18\x08 \x01(\x0b\x32!.oak9.tython.aws.ecs.TaskSetScale\x12\x0f\n\x07service\x18\t \x01(\t\x12G\n\x12service_registries\x18\n \x03(\x0b\x32+.oak9.tython.aws.ecs.TaskSetServiceRegistry\x12\x17\n\x0ftask_definition\x18\x0b \x01(\t\"\x82\x01\n!TaskDefinitionAuthorizationConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0b\n\x03iam\x18\x02 \x01(\t\x12\x17\n\x0f\x61\x63\x63\x65ss_point_id\x18\x03 \x01(\t\"\x87\x01\n!TaskDefinitionContainerDependency\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x11\n\tcondition\x18\x03 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x61ws/aws_ecs.proto\x12\x13oak9.tython.aws.ecs\x1a\x13shared/shared.proto\"\xc8\x01\n\x1e\x43\x61pacityProviderManagedScaling\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12!\n\x19minimum_scaling_step_size\x18\x02 \x01(\x05\x12!\n\x19maximum_scaling_step_size\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x17\n\x0ftarget_capacity\x18\x05 \x01(\x05\"\xf9\x01\n(CapacityProviderAutoScalingGroupProvider\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x1e\n\x16\x61uto_scaling_group_arn\x18\x02 \x01(\t\x12L\n\x0fmanaged_scaling\x18\x03 \x01(\x0b\x32\x33.oak9.tython.aws.ecs.CapacityProviderManagedScaling\x12&\n\x1emanaged_termination_protection\x18\x04 \x01(\t\"\xa9\x02\n\x10\x43\x61pacityProvider\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x62\n\x1b\x61uto_scaling_group_provider\x18\x02 \x01(\x0b\x32=.oak9.tython.aws.ecs.CapacityProviderAutoScalingGroupProvider\x12\x0c\n\x04name\x18\x03 \x01(\t\x12=\n\x04tags\x18\x04 \x03(\x0b\x32/.oak9.tython.aws.ecs.CapacityProvider.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd2\x02\n\x03\x45\x43S\x12@\n\x11\x63\x61pacity_provider\x18\x01 \x03(\x0b\x32%.oak9.tython.aws.ecs.CapacityProvider\x12-\n\x07\x63luster\x18\x02 \x01(\x0b\x32\x1c.oak9.tython.aws.ecs.Cluster\x12=\n\x10primary_task_set\x18\x03 \x01(\x0b\x32#.oak9.tython.aws.ecs.PrimaryTaskSet\x12-\n\x07service\x18\x04 \x03(\x0b\x32\x1c.oak9.tython.aws.ecs.Service\x12<\n\x0ftask_definition\x18\x05 \x03(\x0b\x32#.oak9.tython.aws.ecs.TaskDefinition\x12.\n\x08task_set\x18\x06 \x03(\x0b\x32\x1c.oak9.tython.aws.ecs.TaskSet\"n\n\x16\x43lusterClusterSettings\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x97\x01\n#ClusterCapacityProviderStrategyItem\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x19\n\x11\x63\x61pacity_provider\x18\x02 \x01(\t\x12\x0e\n\x06weight\x18\x03 \x01(\x05\x12\x0c\n\x04\x62\x61se\x18\x04 \x01(\x05\"\x84\x03\n\x07\x43luster\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x34\n\x04tags\x18\x02 \x03(\x0b\x32&.oak9.tython.aws.ecs.Cluster.TagsEntry\x12\x14\n\x0c\x63luster_name\x18\x03 \x01(\t\x12\x45\n\x10\x63luster_settings\x18\x04 \x03(\x0b\x32+.oak9.tython.aws.ecs.ClusterClusterSettings\x12\x1a\n\x12\x63\x61pacity_providers\x18\x05 \x03(\t\x12\x64\n\"default_capacity_provider_strategy\x18\x06 \x03(\x0b\x32\x38.oak9.tython.aws.ecs.ClusterCapacityProviderStrategyItem\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x80\x01\n\x0ePrimaryTaskSet\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63luster\x18\x02 \x01(\t\x12\x13\n\x0btask_set_id\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\"\x97\x01\n#ServiceCapacityProviderStrategyItem\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04\x62\x61se\x18\x02 \x01(\x05\x12\x19\n\x11\x63\x61pacity_provider\x18\x03 \x01(\t\x12\x0e\n\x06weight\x18\x04 \x01(\x05\"\x93\x01\n\x1eServiceDeploymentConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x17\n\x0fmaximum_percent\x18\x02 \x01(\x05\x12\x1f\n\x17minimum_healthy_percent\x18\x03 \x01(\x05\"V\n\x1bServiceDeploymentController\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\xb4\x01\n\x13ServiceLoadBalancer\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x1a\n\x12load_balancer_name\x18\x04 \x01(\t\x12\x18\n\x10target_group_arn\x18\x05 \x01(\t\"\x99\x01\n\x1aServiceAwsVpcConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x18\n\x10\x61ssign_public_ip\x18\x02 \x01(\t\x12\x17\n\x0fsecurity_groups\x18\x03 \x03(\t\x12\x0f\n\x07subnets\x18\x04 \x03(\t\"\xa6\x01\n\x1bServiceNetworkConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12N\n\x15\x61ws_vpc_configuration\x18\x02 \x01(\x0b\x32/.oak9.tython.aws.ecs.ServiceAwsVpcConfiguration\"i\n\x1aServicePlacementConstraint\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nexpression\x18\x02 \x01(\t\"b\n\x18ServicePlacementStrategy\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\r\n\x05\x66ield\x18\x02 \x01(\t\"\xa5\x01\n\x16ServiceServiceRegistry\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x0c\n\x04port\x18\x04 \x01(\x05\x12\x14\n\x0cregistry_arn\x18\x05 \x01(\t\"\xce\x08\n\x07Service\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x13\n\x0bservice_arn\x18\x02 \x01(\t\x12\\\n\x1a\x63\x61pacity_provider_strategy\x18\x03 \x03(\x0b\x32\x38.oak9.tython.aws.ecs.ServiceCapacityProviderStrategyItem\x12\x0f\n\x07\x63luster\x18\x04 \x01(\t\x12U\n\x18\x64\x65ployment_configuration\x18\x05 \x01(\x0b\x32\x33.oak9.tython.aws.ecs.ServiceDeploymentConfiguration\x12O\n\x15\x64\x65ployment_controller\x18\x06 \x01(\x0b\x32\x30.oak9.tython.aws.ecs.ServiceDeploymentController\x12\x15\n\rdesired_count\x18\x07 \x01(\x05\x12\x1f\n\x17\x65nable_ecs_managed_tags\x18\x08 \x01(\x08\x12)\n!health_check_grace_period_seconds\x18\t \x01(\x05\x12\x13\n\x0blaunch_type\x18\n \x01(\t\x12@\n\x0eload_balancers\x18\x0b \x03(\x0b\x32(.oak9.tython.aws.ecs.ServiceLoadBalancer\x12O\n\x15network_configuration\x18\x0c \x01(\x0b\x32\x30.oak9.tython.aws.ecs.ServiceNetworkConfiguration\x12N\n\x15placement_constraints\x18\r \x03(\x0b\x32/.oak9.tython.aws.ecs.ServicePlacementConstraint\x12K\n\x14placement_strategies\x18\x0e \x03(\x0b\x32-.oak9.tython.aws.ecs.ServicePlacementStrategy\x12\x18\n\x10platform_version\x18\x0f \x01(\t\x12\x16\n\x0epropagate_tags\x18\x10 \x01(\t\x12\x0c\n\x04role\x18\x11 \x01(\t\x12\x1b\n\x13scheduling_strategy\x18\x12 \x01(\t\x12\x14\n\x0cservice_name\x18\x13 \x01(\t\x12G\n\x12service_registries\x18\x14 \x03(\x0b\x32+.oak9.tython.aws.ecs.ServiceServiceRegistry\x12\x34\n\x04tags\x18\x15 \x03(\x0b\x32&.oak9.tython.aws.ecs.Service.TagsEntry\x12\x17\n\x0ftask_definition\x18\x16 \x01(\t\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x1aTaskDefinitionKeyValuePair\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"g\n\x1dTaskDefinitionEnvironmentFile\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\r\n\x05value\x18\x02 \x01(\t\"x\n\x17TaskDefinitionHostEntry\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x10\n\x08hostname\x18\x02 \x01(\t\x12\x12\n\nip_address\x18\x03 \x01(\t\"\xe6\x01\n#TaskDefinitionFirelensConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12V\n\x07options\x18\x02 \x03(\x0b\x32\x45.oak9.tython.aws.ecs.TaskDefinitionFirelensConfiguration.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaf\x01\n\x19TaskDefinitionHealthCheck\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63ommand\x18\x02 \x03(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x05\x12\x0f\n\x07retries\x18\x05 \x01(\x05\x12\x14\n\x0cstart_period\x18\x06 \x01(\x05\"v\n TaskDefinitionKernelCapabilities\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0b\n\x03\x61\x64\x64\x18\x02 \x03(\t\x12\x0c\n\x04\x64rop\x18\x03 \x03(\t\"\x8f\x01\n\x14TaskDefinitionDevice\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_path\x18\x02 \x01(\t\x12\x11\n\thost_path\x18\x03 \x01(\t\x12\x13\n\x0bpermissions\x18\x04 \x03(\t\"\x8b\x01\n\x13TaskDefinitionTmpfs\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_path\x18\x02 \x01(\t\x12\x15\n\rmount_options\x18\x03 \x03(\t\x12\x0c\n\x04size\x18\x04 \x01(\x05\"\xfa\x02\n\x1dTaskDefinitionLinuxParameters\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12K\n\x0c\x63\x61pabilities\x18\x02 \x01(\x0b\x32\x35.oak9.tython.aws.ecs.TaskDefinitionKernelCapabilities\x12:\n\x07\x64\x65vices\x18\x03 \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionDevice\x12\x1c\n\x14init_process_enabled\x18\x04 \x01(\x08\x12\x10\n\x08max_swap\x18\x05 \x01(\x05\x12\x1a\n\x12shared_memory_size\x18\x06 \x01(\x05\x12\x12\n\nswappiness\x18\x07 \x01(\x05\x12\x37\n\x05tmpfs\x18\x08 \x03(\x0b\x32(.oak9.tython.aws.ecs.TaskDefinitionTmpfs\"q\n\x14TaskDefinitionSecret\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nvalue_from\x18\x03 \x01(\t\"\xb3\x02\n\x1eTaskDefinitionLogConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nlog_driver\x18\x02 \x01(\t\x12Q\n\x07options\x18\x03 \x03(\x0b\x32@.oak9.tython.aws.ecs.TaskDefinitionLogConfiguration.OptionsEntry\x12\x41\n\x0esecret_options\x18\x04 \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionSecret\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x95\x01\n\x18TaskDefinitionMountPoint\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_path\x18\x02 \x01(\t\x12\x11\n\tread_only\x18\x03 \x01(\x08\x12\x15\n\rsource_volume\x18\x04 \x01(\t\"\x91\x01\n\x19TaskDefinitionPortMapping\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_port\x18\x02 \x01(\x05\x12\x11\n\thost_port\x18\x03 \x01(\x05\x12\x10\n\x08protocol\x18\x04 \x01(\t\"}\n#TaskDefinitionRepositoryCredentials\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x1d\n\x15\x63redentials_parameter\x18\x02 \x01(\t\"k\n!TaskDefinitionResourceRequirement\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\r\n\x05value\x18\x02 \x01(\t\"\x85\x01\n\x14TaskDefinitionUlimit\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nhard_limit\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nsoft_limit\x18\x04 \x01(\x05\"\x80\x01\n\x18TaskDefinitionVolumeFrom\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x11\n\tread_only\x18\x02 \x01(\x08\x12\x18\n\x10source_container\x18\x03 \x01(\t\"x\n\x1bTaskDefinitionSystemControl\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xa5\x0e\n!TaskDefinitionContainerDefinition\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63ommand\x18\x02 \x03(\t\x12\x0b\n\x03\x63pu\x18\x03 \x01(\x05\x12\x1a\n\x12\x64isable_networking\x18\x04 \x01(\x08\x12\x1a\n\x12\x64ns_search_domains\x18\x05 \x03(\t\x12\x13\n\x0b\x64ns_servers\x18\x06 \x03(\t\x12_\n\rdocker_labels\x18\x07 \x03(\x0b\x32H.oak9.tython.aws.ecs.TaskDefinitionContainerDefinition.DockerLabelsEntry\x12\x1f\n\x17\x64ocker_security_options\x18\x08 \x03(\t\x12\x13\n\x0b\x65ntry_point\x18\t \x03(\t\x12\x44\n\x0b\x65nvironment\x18\n \x03(\x0b\x32/.oak9.tython.aws.ecs.TaskDefinitionKeyValuePair\x12M\n\x11\x65nvironment_files\x18\x0b \x03(\x0b\x32\x32.oak9.tython.aws.ecs.TaskDefinitionEnvironmentFile\x12\x11\n\tessential\x18\x0c \x01(\x08\x12\x41\n\x0b\x65xtra_hosts\x18\r \x03(\x0b\x32,.oak9.tython.aws.ecs.TaskDefinitionHostEntry\x12X\n\x16\x66irelens_configuration\x18\x0e \x01(\x0b\x32\x38.oak9.tython.aws.ecs.TaskDefinitionFirelensConfiguration\x12\x44\n\x0chealth_check\x18\x0f \x01(\x0b\x32..oak9.tython.aws.ecs.TaskDefinitionHealthCheck\x12\x10\n\x08hostname\x18\x10 \x01(\t\x12\r\n\x05image\x18\x11 \x01(\t\x12\r\n\x05links\x18\x12 \x03(\t\x12L\n\x10linux_parameters\x18\x13 \x01(\x0b\x32\x32.oak9.tython.aws.ecs.TaskDefinitionLinuxParameters\x12N\n\x11log_configuration\x18\x14 \x01(\x0b\x32\x33.oak9.tython.aws.ecs.TaskDefinitionLogConfiguration\x12\x0e\n\x06memory\x18\x15 \x01(\x05\x12\x1a\n\x12memory_reservation\x18\x16 \x01(\x05\x12\x43\n\x0cmount_points\x18\x17 \x03(\x0b\x32-.oak9.tython.aws.ecs.TaskDefinitionMountPoint\x12\x0c\n\x04name\x18\x18 \x01(\t\x12\x45\n\rport_mappings\x18\x19 \x03(\x0b\x32..oak9.tython.aws.ecs.TaskDefinitionPortMapping\x12\x12\n\nprivileged\x18\x1a \x01(\x08\x12 \n\x18readonly_root_filesystem\x18\x1b \x01(\x08\x12X\n\x16repository_credentials\x18\x1c \x01(\x0b\x32\x38.oak9.tython.aws.ecs.TaskDefinitionRepositoryCredentials\x12U\n\x15resource_requirements\x18\x1d \x03(\x0b\x32\x36.oak9.tython.aws.ecs.TaskDefinitionResourceRequirement\x12:\n\x07secrets\x18\x1e \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionSecret\x12\x15\n\rstart_timeout\x18\x1f \x01(\x05\x12\x14\n\x0cstop_timeout\x18  \x01(\x05\x12:\n\x07ulimits\x18! \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionUlimit\x12\x0c\n\x04user\x18\" \x01(\t\x12\x43\n\x0cvolumes_from\x18# \x03(\x0b\x32-.oak9.tython.aws.ecs.TaskDefinitionVolumeFrom\x12\x19\n\x11working_directory\x18$ \x01(\t\x12\x13\n\x0binteractive\x18% \x01(\x08\x12\x17\n\x0fpseudo_terminal\x18& \x01(\x08\x12I\n\x0fsystem_controls\x18\' \x03(\x0b\x32\x30.oak9.tython.aws.ecs.TaskDefinitionSystemControl\x1a\x33\n\x11\x44ockerLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x01\n\"TaskDefinitionInferenceAccelerator\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x03 \x01(\t\"~\n/TaskDefinitionTaskDefinitionPlacementConstraint\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nexpression\x18\x02 \x01(\t\"\xcc\x01\n TaskDefinitionProxyConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12W\n\x1eproxy_configuration_properties\x18\x03 \x03(\x0b\x32/.oak9.tython.aws.ecs.TaskDefinitionKeyValuePair\"\xb7\x03\n\'TaskDefinitionDockerVolumeConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x15\n\rautoprovision\x18\x02 \x01(\x08\x12\x0e\n\x06\x64river\x18\x03 \x01(\t\x12\x61\n\x0b\x64river_opts\x18\x04 \x03(\x0b\x32L.oak9.tython.aws.ecs.TaskDefinitionDockerVolumeConfiguration.DriverOptsEntry\x12X\n\x06labels\x18\x05 \x03(\x0b\x32H.oak9.tython.aws.ecs.TaskDefinitionDockerVolumeConfiguration.LabelsEntry\x12\r\n\x05scope\x18\x06 \x01(\t\x1a\x31\n\x0f\x44riverOptsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa1\x02\n$TaskDefinitionEFSVolumeConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x15\n\rfilesystem_id\x18\x02 \x01(\t\x12\x16\n\x0eroot_directory\x18\x03 \x01(\t\x12\x1a\n\x12transit_encryption\x18\x04 \x01(\t\x12\x1f\n\x17transit_encryption_port\x18\x05 \x01(\x05\x12T\n\x14\x61uthorization_config\x18\x06 \x01(\x0b\x32\x36.oak9.tython.aws.ecs.TaskDefinitionAuthorizationConfig\"r\n\"TaskDefinitionHostVolumeProperties\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\"\xe4\x02\n\x14TaskDefinitionVolume\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x61\n\x1b\x64ocker_volume_configuration\x18\x02 \x01(\x0b\x32<.oak9.tython.aws.ecs.TaskDefinitionDockerVolumeConfiguration\x12[\n\x18\x65\x66s_volume_configuration\x18\x03 \x01(\x0b\x32\x39.oak9.tython.aws.ecs.TaskDefinitionEFSVolumeConfiguration\x12\x45\n\x04host\x18\x04 \x01(\x0b\x32\x37.oak9.tython.aws.ecs.TaskDefinitionHostVolumeProperties\x12\x0c\n\x04name\x18\x05 \x01(\t\"\x94\x06\n\x0eTaskDefinition\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0e\n\x06\x66\x61mily\x18\x02 \x01(\t\x12U\n\x15\x63ontainer_definitions\x18\x03 \x03(\x0b\x32\x36.oak9.tython.aws.ecs.TaskDefinitionContainerDefinition\x12\x0b\n\x03\x63pu\x18\x04 \x01(\t\x12\x1a\n\x12\x65xecution_role_arn\x18\x05 \x01(\t\x12W\n\x16inference_accelerators\x18\x06 \x03(\x0b\x32\x37.oak9.tython.aws.ecs.TaskDefinitionInferenceAccelerator\x12\x0e\n\x06memory\x18\x07 \x01(\t\x12\x14\n\x0cnetwork_mode\x18\x08 \x01(\t\x12\x63\n\x15placement_constraints\x18\t \x03(\x0b\x32\x44.oak9.tython.aws.ecs.TaskDefinitionTaskDefinitionPlacementConstraint\x12R\n\x13proxy_configuration\x18\n \x01(\x0b\x32\x35.oak9.tython.aws.ecs.TaskDefinitionProxyConfiguration\x12 \n\x18requires_compatibilities\x18\x0b \x03(\t\x12\x15\n\rtask_role_arn\x18\x0c \x01(\t\x12:\n\x07volumes\x18\r \x03(\x0b\x32).oak9.tython.aws.ecs.TaskDefinitionVolume\x12\x10\n\x08pid_mode\x18\x0e \x01(\t\x12\x10\n\x08ipc_mode\x18\x0f \x01(\t\x12;\n\x04tags\x18\x10 \x03(\x0b\x32-.oak9.tython.aws.ecs.TaskDefinition.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb4\x01\n\x13TaskSetLoadBalancer\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x1a\n\x12load_balancer_name\x18\x04 \x01(\t\x12\x18\n\x10target_group_arn\x18\x05 \x01(\t\"\x99\x01\n\x1aTaskSetAwsVpcConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x18\n\x10\x61ssign_public_ip\x18\x02 \x01(\t\x12\x17\n\x0fsecurity_groups\x18\x03 \x03(\t\x12\x0f\n\x07subnets\x18\x04 \x03(\t\"\xa6\x01\n\x1bTaskSetNetworkConfiguration\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12N\n\x15\x61ws_vpc_configuration\x18\x02 \x01(\x0b\x32/.oak9.tython.aws.ecs.TaskSetAwsVpcConfiguration\"d\n\x0cTaskSetScale\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"\xa5\x01\n\x16TaskSetServiceRegistry\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_port\x18\x03 \x01(\x05\x12\x0c\n\x04port\x18\x04 \x01(\x05\x12\x14\n\x0cregistry_arn\x18\x05 \x01(\t\"\xcf\x03\n\x07TaskSet\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0f\n\x07\x63luster\x18\x02 \x01(\t\x12\x13\n\x0b\x65xternal_id\x18\x03 \x01(\t\x12\x13\n\x0blaunch_type\x18\x04 \x01(\t\x12@\n\x0eload_balancers\x18\x05 \x03(\x0b\x32(.oak9.tython.aws.ecs.TaskSetLoadBalancer\x12O\n\x15network_configuration\x18\x06 \x01(\x0b\x32\x30.oak9.tython.aws.ecs.TaskSetNetworkConfiguration\x12\x18\n\x10platform_version\x18\x07 \x01(\t\x12\x30\n\x05scale\x18\x08 \x01(\x0b\x32!.oak9.tython.aws.ecs.TaskSetScale\x12\x0f\n\x07service\x18\t \x01(\t\x12G\n\x12service_registries\x18\n \x03(\x0b\x32+.oak9.tython.aws.ecs.TaskSetServiceRegistry\x12\x17\n\x0ftask_definition\x18\x0b \x01(\t\"\x82\x01\n!TaskDefinitionAuthorizationConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0b\n\x03iam\x18\x02 \x01(\t\x12\x17\n\x0f\x61\x63\x63\x65ss_point_id\x18\x03 \x01(\t\"\x87\x01\n!TaskDefinitionContainerDependency\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x16\n\x0e\x63ontainer_name\x18\x02 \x01(\t\x12\x11\n\tcondition\x18\x03 \x01(\tb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aws.aws_ecs_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _CAPACITYPROVIDER_TAGSENTRY._options = None
@@ -33,16 +33,14 @@
   _TASKDEFINITIONLOGCONFIGURATION_OPTIONSENTRY._serialized_options = b'8\001'
   _TASKDEFINITIONCONTAINERDEFINITION_DOCKERLABELSENTRY._options = None
   _TASKDEFINITIONCONTAINERDEFINITION_DOCKERLABELSENTRY._serialized_options = b'8\001'
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_DRIVEROPTSENTRY._options = None
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_DRIVEROPTSENTRY._serialized_options = b'8\001'
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_LABELSENTRY._options = None
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_LABELSENTRY._serialized_options = b'8\001'
-  _TASKDEFINITIONEFSVOLUMECONFIGURATION_AUTHORIZATIONCONFIGENTRY._options = None
-  _TASKDEFINITIONEFSVOLUMECONFIGURATION_AUTHORIZATIONCONFIGENTRY._serialized_options = b'8\001'
   _TASKDEFINITION_TAGSENTRY._options = None
   _TASKDEFINITION_TAGSENTRY._serialized_options = b'8\001'
   _CAPACITYPROVIDERMANAGEDSCALING._serialized_start=64
   _CAPACITYPROVIDERMANAGEDSCALING._serialized_end=264
   _CAPACITYPROVIDERAUTOSCALINGGROUPPROVIDER._serialized_start=267
   _CAPACITYPROVIDERAUTOSCALINGGROUPPROVIDER._serialized_end=516
   _CAPACITYPROVIDER._serialized_start=519
@@ -136,35 +134,33 @@
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION._serialized_start=9526
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION._serialized_end=9965
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_DRIVEROPTSENTRY._serialized_start=9869
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_DRIVEROPTSENTRY._serialized_end=9918
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_LABELSENTRY._serialized_start=9920
   _TASKDEFINITIONDOCKERVOLUMECONFIGURATION_LABELSENTRY._serialized_end=9965
   _TASKDEFINITIONEFSVOLUMECONFIGURATION._serialized_start=9968
-  _TASKDEFINITIONEFSVOLUMECONFIGURATION._serialized_end=10345
-  _TASKDEFINITIONEFSVOLUMECONFIGURATION_AUTHORIZATIONCONFIGENTRY._serialized_start=10287
-  _TASKDEFINITIONEFSVOLUMECONFIGURATION_AUTHORIZATIONCONFIGENTRY._serialized_end=10345
-  _TASKDEFINITIONHOSTVOLUMEPROPERTIES._serialized_start=10347
-  _TASKDEFINITIONHOSTVOLUMEPROPERTIES._serialized_end=10461
-  _TASKDEFINITIONVOLUME._serialized_start=10464
-  _TASKDEFINITIONVOLUME._serialized_end=10820
-  _TASKDEFINITION._serialized_start=10823
-  _TASKDEFINITION._serialized_end=11611
+  _TASKDEFINITIONEFSVOLUMECONFIGURATION._serialized_end=10257
+  _TASKDEFINITIONHOSTVOLUMEPROPERTIES._serialized_start=10259
+  _TASKDEFINITIONHOSTVOLUMEPROPERTIES._serialized_end=10373
+  _TASKDEFINITIONVOLUME._serialized_start=10376
+  _TASKDEFINITIONVOLUME._serialized_end=10732
+  _TASKDEFINITION._serialized_start=10735
+  _TASKDEFINITION._serialized_end=11523
   _TASKDEFINITION_TAGSENTRY._serialized_start=773
   _TASKDEFINITION_TAGSENTRY._serialized_end=816
-  _TASKSETLOADBALANCER._serialized_start=11614
-  _TASKSETLOADBALANCER._serialized_end=11794
-  _TASKSETAWSVPCCONFIGURATION._serialized_start=11797
-  _TASKSETAWSVPCCONFIGURATION._serialized_end=11950
-  _TASKSETNETWORKCONFIGURATION._serialized_start=11953
-  _TASKSETNETWORKCONFIGURATION._serialized_end=12119
-  _TASKSETSCALE._serialized_start=12121
-  _TASKSETSCALE._serialized_end=12221
-  _TASKSETSERVICEREGISTRY._serialized_start=12224
-  _TASKSETSERVICEREGISTRY._serialized_end=12389
-  _TASKSET._serialized_start=12392
-  _TASKSET._serialized_end=12855
-  _TASKDEFINITIONAUTHORIZATIONCONFIG._serialized_start=12858
-  _TASKDEFINITIONAUTHORIZATIONCONFIG._serialized_end=12988
-  _TASKDEFINITIONCONTAINERDEPENDENCY._serialized_start=12991
-  _TASKDEFINITIONCONTAINERDEPENDENCY._serialized_end=13126
+  _TASKSETLOADBALANCER._serialized_start=11526
+  _TASKSETLOADBALANCER._serialized_end=11706
+  _TASKSETAWSVPCCONFIGURATION._serialized_start=11709
+  _TASKSETAWSVPCCONFIGURATION._serialized_end=11862
+  _TASKSETNETWORKCONFIGURATION._serialized_start=11865
+  _TASKSETNETWORKCONFIGURATION._serialized_end=12031
+  _TASKSETSCALE._serialized_start=12033
+  _TASKSETSCALE._serialized_end=12133
+  _TASKSETSERVICEREGISTRY._serialized_start=12136
+  _TASKSETSERVICEREGISTRY._serialized_end=12301
+  _TASKSET._serialized_start=12304
+  _TASKSET._serialized_end=12767
+  _TASKDEFINITIONAUTHORIZATIONCONFIG._serialized_start=12770
+  _TASKDEFINITIONAUTHORIZATIONCONFIG._serialized_end=12900
+  _TASKDEFINITIONCONTAINERDEPENDENCY._serialized_start=12903
+  _TASKDEFINITIONCONTAINERDEPENDENCY._serialized_end=13038
 # @@protoc_insertion_point(module_scope)
```

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ecs_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ecs_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1388,55 +1388,39 @@
 
 global___TaskDefinitionDockerVolumeConfiguration = TaskDefinitionDockerVolumeConfiguration
 
 @typing_extensions.final
 class TaskDefinitionEFSVolumeConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
-    class AuthorizationConfigEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
-
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
     FILESYSTEM_ID_FIELD_NUMBER: builtins.int
     ROOT_DIRECTORY_FIELD_NUMBER: builtins.int
     TRANSIT_ENCRYPTION_FIELD_NUMBER: builtins.int
     TRANSIT_ENCRYPTION_PORT_FIELD_NUMBER: builtins.int
     AUTHORIZATION_CONFIG_FIELD_NUMBER: builtins.int
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     filesystem_id: builtins.str
     root_directory: builtins.str
     transit_encryption: builtins.str
     transit_encryption_port: builtins.int
     @property
-    def authorization_config(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    def authorization_config(self) -> global___TaskDefinitionAuthorizationConfig: ...
     def __init__(
         self,
         *,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
         filesystem_id: builtins.str = ...,
         root_directory: builtins.str = ...,
         transit_encryption: builtins.str = ...,
         transit_encryption_port: builtins.int = ...,
-        authorization_config: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        authorization_config: global___TaskDefinitionAuthorizationConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def HasField(self, field_name: typing_extensions.Literal["authorization_config", b"authorization_config", "resource_info", b"resource_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["authorization_config", b"authorization_config", "filesystem_id", b"filesystem_id", "resource_info", b"resource_info", "root_directory", b"root_directory", "transit_encryption", b"transit_encryption", "transit_encryption_port", b"transit_encryption_port"]) -> None: ...
 
 global___TaskDefinitionEFSVolumeConfiguration = TaskDefinitionEFSVolumeConfiguration
 
 @typing_extensions.final
 class TaskDefinitionHostVolumeProperties(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_efs_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_efs_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_efs_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_efs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_eks_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_eks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_eks_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_eks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticsearch_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticsearch_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_emr_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_emr_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_emr_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_emr_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_events_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_events_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_events_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_eventschemas_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_eventschemas_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_eventschemas_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_eventschemas_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_fms_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_fms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_fms_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_fms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_fsx_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_fsx_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_fsx_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_fsx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_gamelift_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_gamelift_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_gamelift_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_gamelift_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_globalaccelerator_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_globalaccelerator_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_glue_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_glue_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_glue_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_glue_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_greengrass_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_greengrass_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_greengrass_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_greengrass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_groundstation_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_groundstation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_groundstation_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_groundstation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_guardduty_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_guardduty_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_guardduty_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_guardduty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iam_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iam_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iam_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_imagebuilder_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_imagebuilder_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_inspector_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_inspector_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_inspector_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_inspector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot1click_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot1click_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot1click_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot1click_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iot_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotanalytics_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotanalytics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotevents_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotevents_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_iotevents_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_iotevents_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesis_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesis_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesis_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kms_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_kms_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_kms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_lakeformation_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_lakeformation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_lakeformation_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_lakeformation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_lambda_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_lambda_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_lambda_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_lambda_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_logs_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_logs_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_logs_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_logs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_macie_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_macie_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_macie_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_macie_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_managedblockchain_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_managedblockchain_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_mediaconvert_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_mediaconvert_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_msk_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_msk_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_msk_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_msk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_neptune_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_neptune_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_neptune_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_neptune_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_networkmanager_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_networkmanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_networkmanager_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_networkmanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworks_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworks_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworkscm_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworkscm_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_qldb_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_qldb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_qldb_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_qldb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ram_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ram_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ram_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_rds_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_rds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_redshift_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_redshift_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_redshift_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_redshift_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_resourcegroups_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_resourcegroups_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_robomaker_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_robomaker_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_robomaker_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_robomaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53resolver_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53resolver_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_route53resolver_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_route53resolver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_s3_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_s3_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_s3_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_s3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sagemaker_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sagemaker_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sagemaker_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sagemaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sdb_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sdb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sdb_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sdb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_secretsmanager_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_secretsmanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_securityhub_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_securityhub_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_securityhub_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_securityhub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicecatalog_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicecatalog_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicediscovery_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicediscovery_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sns_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sns_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sns_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sns_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sqs_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sqs_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sqs_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sqs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ssm_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ssm_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_ssm_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_ssm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sso_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_sso_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_sso_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_stepfunctions_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_stepfunctions_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_synthetics_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_synthetics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_synthetics_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_synthetics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_transfer_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_transfer_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_waf_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_waf_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_waf_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_waf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafregional_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafregional_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafregional_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafregional_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafv2_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_wafv2_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_wafv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_workspaces_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_workspaces_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/aws/aws_workspaces_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/aws/aws_workspaces_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_aad_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_aad_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cache_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cache_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_devices_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_devices_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_storage_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_storage_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_web_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_web_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from oak9.tython.models.shared import shared_pb2 as shared_dot_shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x61zure/azure_microsoft_web.proto\x12\x1foak9.tython.azure.microsoft_web\x1a\x13shared/shared.proto\"\xd9\x05\n\rMicrosoft_Web\x12R\n\x14hosting_environments\x18\x01 \x01(\x0b\x32\x34.oak9.tython.azure.microsoft_web.HostingEnvironments\x12\x41\n\x0bserverfarms\x18\x02 \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.Serverfarms\x12\x87\x01\n0serverfarms_virtual_network_connections_gateways\x18\x03 \x03(\x0b\x32M.oak9.tython.azure.microsoft_web.ServerfarmsVirtualNetworkConnectionsGateways\x12\x83\x01\n.serverfarms_virtual_network_connections_routes\x18\x04 \x03(\x0b\x32K.oak9.tython.azure.microsoft_web.ServerfarmsVirtualNetworkConnectionsRoutes\x12\x35\n\x05sites\x18\x05 \x01(\x0b\x32&.oak9.tython.azure.microsoft_web.Sites\x12\x42\n\x0csites_config\x18\x06 \x03(\x0b\x32,.oak9.tython.azure.microsoft_web.SitesConfig\x12L\n\x11sites_deployments\x18\x07 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.SitesDeployments\x12X\n\x18sites_host_name_bindings\x18\x08 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.SitesHostNameBindings\"\xb9\x01\n#StaticSitesUserProvidedFunctionApps\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x66unction_app_region\x18\x04 \x01(\t\x12 \n\x18\x66unction_app_resource_id\x18\x05 \x01(\t\"\xe8\x01\n%StaticSitesPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"\x8a\x01\n\x18StaticSitesCustomDomains\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x19\n\x11validation_method\x18\x04 \x01(\t\"L\n\x11StaticSitesConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\xbf\x01\n)StaticSitesBuildsUserProvidedFunctionApps\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x66unction_app_region\x18\x04 \x01(\t\x12 \n\x18\x66unction_app_resource_id\x18\x05 \x01(\t\"R\n\x17StaticSitesBuildsConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\x83\t\n\x0bStaticSites\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12I\n\x08identity\x18\x02 \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.ManagedServiceIdentity\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12!\n\x19\x61llow_config_file_updates\x18\x06 \x01(\x08\x12\x0e\n\x06\x62ranch\x18\x07 \x01(\t\x12T\n\x10\x62uild_properties\x18\x08 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.StaticSiteBuildProperties\x12#\n\x1b\x65nterprise_grade_cdn_status\x18\t \x01(\t\x12\x10\n\x08provider\x18\n \x01(\t\x12\x18\n\x10repository_token\x18\x0b \x01(\t\x12\x16\n\x0erepository_url\x18\x0c \x01(\t\x12\"\n\x1astaging_environment_policy\x18\r \x01(\t\x12W\n\x13template_properties\x18\x0e \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.StaticSiteTemplateOptions\x12<\n\x03sku\x18\x0f \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\x12\x44\n\x04tags\x18\x10 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.StaticSites.TagsEntry\x12O\n\x13static_sites_config\x18\x11 \x03(\x0b\x32\x32.oak9.tython.azure.microsoft_web.StaticSitesConfig\x12^\n\x1bstatic_sites_custom_domains\x18\x12 \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.StaticSitesCustomDomains\x12y\n)static_sites_private_endpoint_connections\x18\x13 \x03(\x0b\x32\x46.oak9.tython.azure.microsoft_web.StaticSitesPrivateEndpointConnections\x12v\n(static_sites_user_provided_function_apps\x18\x14 \x03(\x0b\x32\x44.oak9.tython.azure.microsoft_web.StaticSitesUserProvidedFunctionApps\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x8d\x01\n\x19StaticSiteTemplateOptions\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x12\n\nis_private\x18\x02 \x01(\x08\x12\r\n\x05owner\x18\x03 \x01(\t\x12\x17\n\x0frepository_name\x18\x04 \x01(\t\x12\x1f\n\x17template_repository_url\x18\x05 \x01(\t\"\x91\x02\n\x19StaticSiteBuildProperties\x12\x19\n\x11\x61pi_build_command\x18\x01 \x01(\t\x12\x14\n\x0c\x61pi_location\x18\x02 \x01(\t\x12\x1d\n\x15\x61pp_artifact_location\x18\x03 \x01(\t\x12\x19\n\x11\x61pp_build_command\x18\x04 \x01(\t\x12\x14\n\x0c\x61pp_location\x18\x05 \x01(\t\x12*\n\"github_action_secret_name_override\x18\x06 \x01(\t\x12\x17\n\x0foutput_location\x18\x07 \x01(\t\x12.\n&skip_github_action_workflow_generation\x18\x08 \x01(\x08\"\xa9\x01\n&SitesVirtualNetworkConnectionsGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tvnet_name\x18\x04 \x01(\t\x12\x17\n\x0fvpn_package_uri\x18\x05 \x01(\t\"\xc6\x02\n\x1eSitesVirtualNetworkConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tcert_blob\x18\x04 \x01(\t\x12\x13\n\x0b\x64ns_servers\x18\x05 \x01(\t\x12\x10\n\x08is_swift\x18\x06 \x01(\x08\x12\x18\n\x10vnet_resource_id\x18\x07 \x01(\t\x12{\n*sites_virtual_network_connections_gateways\x18\x08 \x03(\x0b\x32G.oak9.tython.azure.microsoft_web.SitesVirtualNetworkConnectionsGateways\"\xe3\x02\n\x13SitesSourcecontrols\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\t\x12#\n\x1b\x64\x65ployment_rollback_enabled\x18\x05 \x01(\x08\x12`\n\x1cgit_hub_action_configuration\x18\x06 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.GitHubActionConfiguration\x12\x19\n\x11is_git_hub_action\x18\x07 \x01(\x08\x12\x1d\n\x15is_manual_integration\x18\x08 \x01(\x08\x12\x14\n\x0cis_mercurial\x18\t \x01(\x08\x12\x10\n\x08repo_url\x18\n \x01(\t\"\xae\x01\n+SitesSlotsVirtualNetworkConnectionsGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tvnet_name\x18\x04 \x01(\t\x12\x17\n\x0fvpn_package_uri\x18\x05 \x01(\t\"\xd7\x02\n#SitesSlotsVirtualNetworkConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tcert_blob\x18\x04 \x01(\t\x12\x13\n\x0b\x64ns_servers\x18\x05 \x01(\t\x12\x10\n\x08is_swift\x18\x06 \x01(\x08\x12\x18\n\x10vnet_resource_id\x18\x07 \x01(\t\x12\x86\x01\n0sites_slots_virtual_network_connections_gateways\x18\x08 \x03(\x0b\x32L.oak9.tython.azure.microsoft_web.SitesSlotsVirtualNetworkConnectionsGateways\"\xe8\x02\n\x18SitesSlotsSourcecontrols\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\t\x12#\n\x1b\x64\x65ployment_rollback_enabled\x18\x05 \x01(\x08\x12`\n\x1cgit_hub_action_configuration\x18\x06 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.GitHubActionConfiguration\x12\x19\n\x11is_git_hub_action\x18\x07 \x01(\x08\x12\x1d\n\x15is_manual_integration\x18\x08 \x01(\x08\x12\x14\n\x0cis_mercurial\x18\t \x01(\x08\x12\x10\n\x08repo_url\x18\n \x01(\t\"\x8f\x02\n\x19GitHubActionConfiguration\x12Z\n\x12\x63ode_configuration\x18\x01 \x01(\x0b\x32>.oak9.tython.azure.microsoft_web.GitHubActionCodeConfiguration\x12\x64\n\x17\x63ontainer_configuration\x18\x02 \x01(\x0b\x32\x43.oak9.tython.azure.microsoft_web.GitHubActionContainerConfiguration\x12\x1e\n\x16generate_workflow_file\x18\x03 \x01(\x08\x12\x10\n\x08is_linux\x18\x04 \x01(\x08\"p\n\"GitHubActionContainerConfiguration\x12\x12\n\nimage_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x12\n\nserver_url\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\"O\n\x1dGitHubActionCodeConfiguration\x12\x15\n\rruntime_stack\x18\x01 \x01(\t\x12\x17\n\x0fruntime_version\x18\x02 \x01(\t\"a\n\x18SitesSlotsSiteextensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xa6\x01\n\x1cSitesSlotsPublicCertificates\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x62lob\x18\x04 \x01(\t\x12#\n\x1bpublic_certificate_location\x18\x05 \x01(\t\"\xe7\x01\n$SitesSlotsPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"\xd7\x01\n\x17SitesSlotsPrivateAccess\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12V\n\x10virtual_networks\x18\x05 \x03(\x0b\x32<.oak9.tython.azure.microsoft_web.PrivateAccessVirtualNetwork\"\xe7\x02\n\x17SitesSlotsPremieraddons\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x19\n\x11marketplace_offer\x18\x05 \x01(\t\x12\x1d\n\x15marketplace_publisher\x18\x06 \x01(\t\x12\x0f\n\x07product\x18\x07 \x01(\t\x12\x0b\n\x03sku\x18\x08 \x01(\t\x12\x0e\n\x06vendor\x18\t \x01(\t\x12P\n\x04tags\x18\n \x03(\x0b\x32\x42.oak9.tython.azure.microsoft_web.SitesSlotsPremieraddons.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa3\x01\n\x17SitesSlotsNetworkConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12subnet_resource_id\x18\x04 \x01(\t\x12\x17\n\x0fswift_supported\x18\x05 \x01(\x08\"\xa7\x03\n\x1dSitesSlotsInstancesExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x61pp_offline\x18\x04 \x01(\x08\x12\x19\n\x11\x63onnection_string\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_type\x18\x06 \x01(\t\x12\x13\n\x0bpackage_uri\x18\x07 \x01(\t\x12i\n\x0eset_parameters\x18\x08 \x03(\x0b\x32Q.oak9.tython.azure.microsoft_web.SitesSlotsInstancesExtensions.SetParametersEntry\x12#\n\x1bset_parameters_xml_file_uri\x18\t \x01(\t\x12\x15\n\rskip_app_data\x18\n \x01(\x08\x1a\x34\n\x12SetParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb6\x02\n*SitesSlotsHybridConnectionNamespacesRelays\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08hostname\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x15\n\rrelay_arm_uri\x18\x06 \x01(\t\x12\x12\n\nrelay_name\x18\x07 \x01(\t\x12\x15\n\rsend_key_name\x18\x08 \x01(\t\x12\x16\n\x0esend_key_value\x18\t \x01(\t\x12\x1d\n\x15service_bus_namespace\x18\n \x01(\t\x12\x1a\n\x12service_bus_suffix\x18\x0b \x01(\t\"\x98\x02\n\x1aSitesSlotsHybridconnection\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x62iztalk_uri\x18\x04 \x01(\t\x12 \n\x18\x65ntity_connection_string\x18\x05 \x01(\t\x12\x13\n\x0b\x65ntity_name\x18\x06 \x01(\t\x12\x10\n\x08hostname\x18\x07 \x01(\t\x12\x0c\n\x04port\x18\x08 \x01(\x05\x12\"\n\x1aresource_connection_string\x18\t \x01(\t\x12\x15\n\rresource_type\x18\n \x01(\t\"\xba\x02\n\x1aSitesSlotsHostNameBindings\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x61zure_resource_name\x18\x04 \x01(\t\x12\x1b\n\x13\x61zure_resource_type\x18\x05 \x01(\t\x12(\n custom_host_name_dns_record_type\x18\x06 \x01(\t\x12\x11\n\tdomain_id\x18\x07 \x01(\t\x12\x16\n\x0ehost_name_type\x18\x08 \x01(\t\x12\x11\n\tsite_name\x18\t \x01(\t\x12\x11\n\tssl_state\x18\n \x01(\t\x12\x12\n\nthumbprint\x18\x0b \x01(\t\"o\n\x17SitesSlotsFunctionsKeys\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xc1\x05\n\x13SitesSlotsFunctions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12P\n\x06\x63onfig\x18\x04 \x03(\x0b\x32@.oak9.tython.azure.microsoft_web.SitesSlotsFunctions.ConfigEntry\x12\x13\n\x0b\x63onfig_href\x18\x05 \x01(\t\x12N\n\x05\x66iles\x18\x06 \x03(\x0b\x32?.oak9.tython.azure.microsoft_web.SitesSlotsFunctions.FilesEntry\x12\x17\n\x0f\x66unction_app_id\x18\x07 \x01(\t\x12\x0c\n\x04href\x18\x08 \x01(\t\x12\x1b\n\x13invoke_url_template\x18\t \x01(\t\x12\x13\n\x0bis_disabled\x18\n \x01(\x08\x12\x10\n\x08language\x18\x0b \x01(\t\x12\x13\n\x0bscript_href\x18\x0c \x01(\t\x12\x1d\n\x15script_root_path_href\x18\r \x01(\t\x12\x19\n\x11secrets_file_href\x18\x0e \x01(\t\x12\x11\n\ttest_data\x18\x0f \x01(\t\x12\x16\n\x0etest_data_href\x18\x10 \x01(\t\x12\\\n\x1asites_slots_functions_keys\x18\x11 \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsFunctionsKeys\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a,\n\nFilesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x95\x03\n\x14SitesSlotsExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x61pp_offline\x18\x04 \x01(\x08\x12\x19\n\x11\x63onnection_string\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_type\x18\x06 \x01(\t\x12\x13\n\x0bpackage_uri\x18\x07 \x01(\t\x12`\n\x0eset_parameters\x18\x08 \x03(\x0b\x32H.oak9.tython.azure.microsoft_web.SitesSlotsExtensions.SetParametersEntry\x12#\n\x1bset_parameters_xml_file_uri\x18\t \x01(\t\x12\x15\n\rskip_app_data\x18\n \x01(\x08\x1a\x34\n\x12SetParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x01\n$SitesSlotsDomainOwnershipIdentifiers\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\t\"\x8c\x02\n\x15SitesSlotsDeployments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x0e\n\x06\x61uthor\x18\x05 \x01(\t\x12\x14\n\x0c\x61uthor_email\x18\x06 \x01(\t\x12\x10\n\x08\x64\x65ployer\x18\x07 \x01(\t\x12\x0f\n\x07\x64\x65tails\x18\x08 \x01(\t\x12\x10\n\x08\x65nd_time\x18\t \x01(\t\x12\x0f\n\x07message\x18\n \x01(\t\x12\x12\n\nstart_time\x18\x0b \x01(\t\x12\x0e\n\x06status\x18\x0c \x01(\x05\"K\n\x10SitesSlotsConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"g\n,SitesSlotsBasicPublishingCredentialsPolicies\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\x94\x16\n\nSitesSlots\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12I\n\x08identity\x18\x03 \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.ManagedServiceIdentity\x12\x0c\n\x04kind\x18\x04 \x01(\t\x12\x10\n\x08location\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x1f\n\x17\x63lient_affinity_enabled\x18\x07 \x01(\x08\x12\x1b\n\x13\x63lient_cert_enabled\x18\x08 \x01(\x08\x12#\n\x1b\x63lient_cert_exclusion_paths\x18\t \x01(\t\x12\x18\n\x10\x63lient_cert_mode\x18\n \x01(\t\x12\x42\n\x0c\x63loning_info\x18\x0b \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.CloningInfo\x12\x16\n\x0e\x63ontainer_size\x18\x0c \x01(\x05\x12%\n\x1d\x63ustom_domain_verification_id\x18\r \x01(\t\x12\x1f\n\x17\x64\x61ily_memory_time_quota\x18\x0e \x01(\x05\x12\x0f\n\x07\x65nabled\x18\x0f \x01(\x08\x12_\n\x1bhosting_environment_profile\x18\x10 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.HostingEnvironmentProfile\x12\x1b\n\x13host_names_disabled\x18\x11 \x01(\x08\x12O\n\x14host_name_ssl_states\x18\x12 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.HostNameSslState\x12\x12\n\nhttps_only\x18\x13 \x01(\x08\x12\x0f\n\x07hyper_v\x18\x14 \x01(\x08\x12\x10\n\x08is_xenon\x18\x15 \x01(\x08\x12$\n\x1ckey_vault_reference_identity\x18\x16 \x01(\t\x12\x17\n\x0fredundancy_mode\x18\x17 \x01(\t\x12\x10\n\x08reserved\x18\x18 \x01(\x08\x12\x1d\n\x15scm_site_also_stopped\x18\x19 \x01(\x08\x12\x16\n\x0eserver_farm_id\x18\x1a \x01(\t\x12@\n\x0bsite_config\x18\x1b \x01(\x0b\x32+.oak9.tython.azure.microsoft_web.SiteConfig\x12 \n\x18storage_account_required\x18\x1c \x01(\x08\x12!\n\x19virtual_network_subnet_id\x18\x1d \x01(\t\x12\x43\n\x04tags\x18\x1e \x03(\x0b\x32\x35.oak9.tython.azure.microsoft_web.SitesSlots.TagsEntry\x12\x88\x01\n1sites_slots_basic_publishing_credentials_policies\x18\x1f \x03(\x0b\x32M.oak9.tython.azure.microsoft_web.SitesSlotsBasicPublishingCredentialsPolicies\x12M\n\x12sites_slots_config\x18  \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.SitesSlotsConfig\x12W\n\x17sites_slots_deployments\x18! \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.SitesSlotsDeployments\x12w\n(sites_slots_domain_ownership_identifiers\x18\" \x03(\x0b\x32\x45.oak9.tython.azure.microsoft_web.SitesSlotsDomainOwnershipIdentifiers\x12U\n\x16sites_slots_extensions\x18# \x03(\x0b\x32\x35.oak9.tython.azure.microsoft_web.SitesSlotsExtensions\x12S\n\x15sites_slots_functions\x18$ \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.SitesSlotsFunctions\x12\x63\n\x1esites_slots_host_name_bindings\x18% \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.SitesSlotsHostNameBindings\x12\x61\n\x1csites_slots_hybridconnection\x18& \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.SitesSlotsHybridconnection\x12\\\n\x1asites_slots_network_config\x18\' \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsNetworkConfig\x12[\n\x19sites_slots_premieraddons\x18( \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsPremieraddons\x12\\\n\x1asites_slots_private_access\x18) \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsPrivateAccess\x12w\n(sites_slots_private_endpoint_connections\x18* \x03(\x0b\x32\x45.oak9.tython.azure.microsoft_web.SitesSlotsPrivateEndpointConnections\x12\x66\n\x1fsites_slots_public_certificates\x18+ \x03(\x0b\x32=.oak9.tython.azure.microsoft_web.SitesSlotsPublicCertificates\x12]\n\x1asites_slots_siteextensions\x18, \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SitesSlotsSiteextensions\x12]\n\x1asites_slots_sourcecontrols\x18- \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SitesSlotsSourcecontrols\x12u\n\'sites_slots_virtual_network_connections\x18. \x03(\x0b\x32\x44.oak9.tython.azure.microsoft_web.SitesSlotsVirtualNetworkConnections\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\\\n\x13SitesSiteextensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xa1\x01\n\x17SitesPublicCertificates\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x62lob\x18\x04 \x01(\t\x12#\n\x1bpublic_certificate_location\x18\x05 \x01(\t\"\xe2\x01\n\x1fSitesPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"\xd2\x01\n\x12SitesPrivateAccess\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12V\n\x10virtual_networks\x18\x05 \x03(\x0b\x32<.oak9.tython.azure.microsoft_web.PrivateAccessVirtualNetwork\"\x94\x01\n\x1bPrivateAccessVirtualNetwork\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0bresource_id\x18\x03 \x01(\t\x12\x45\n\x07subnets\x18\x04 \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.PrivateAccessSubnet\"0\n\x13PrivateAccessSubnet\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xdd\x02\n\x12SitesPremieraddons\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x19\n\x11marketplace_offer\x18\x05 \x01(\t\x12\x1d\n\x15marketplace_publisher\x18\x06 \x01(\t\x12\x0f\n\x07product\x18\x07 \x01(\t\x12\x0b\n\x03sku\x18\x08 \x01(\t\x12\x0e\n\x06vendor\x18\t \x01(\t\x12K\n\x04tags\x18\n \x03(\x0b\x32=.oak9.tython.azure.microsoft_web.SitesPremieraddons.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9e\x01\n\x12SitesNetworkConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12subnet_resource_id\x18\x04 \x01(\t\x12\x17\n\x0fswift_supported\x18\x05 \x01(\x08\"\xec\x01\n\x0cSitesMigrate\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12$\n\x1c\x61zurefiles_connection_string\x18\x04 \x01(\t\x12\x18\n\x10\x61zurefiles_share\x18\x05 \x01(\t\x12\"\n\x1a\x62lock_write_access_to_site\x18\x06 \x01(\x08\x12#\n\x1bswitch_site_after_migration\x18\x07 \x01(\x08\"\x9d\x03\n\x18SitesInstancesExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x61pp_offline\x18\x04 \x01(\x08\x12\x19\n\x11\x63onnection_string\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_type\x18\x06 \x01(\t\x12\x13\n\x0bpackage_uri\x18\x07 \x01(\t\x12\x64\n\x0eset_parameters\x18\x08 \x03(\x0b\x32L.oak9.tython.azure.microsoft_web.SitesInstancesExtensions.SetParametersEntry\x12#\n\x1bset_parameters_xml_file_uri\x18\t \x01(\t\x12\x15\n\rskip_app_data\x18\n \x01(\x08\x1a\x34\n\x12SetParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb1\x02\n%SitesHybridConnectionNamespacesRelays\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08hostname\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x15\n\rrelay_arm_uri\x18\x06 \x01(\t\x12\x12\n\nrelay_name\x18\x07 \x01(\t\x12\x15\n\rsend_key_name\x18\x08 \x01(\t\x12\x16\n\x0esend_key_value\x18\t \x01(\t\x12\x1d\n\x15service_bus_namespace\x18\n \x01(\t\x12\x1a\n\x12service_bus_suffix\x18\x0b \x01(\t\"\x93\x02\n\x15SitesHybridconnection\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x62iztalk_uri\x18\x04 \x01(\t\x12 \n\x18\x65ntity_connection_string\x18\x05 \x01(\t\x12\x13\n\x0b\x65ntity_name\x18\x06 \x01(\t\x12\x10\n\x08hostname\x18\x07 \x01(\t\x12\x0c\n\x04port\x18\x08 \x01(\x05\x12\"\n\x1aresource_connection_string\x18\t \x01(\t\x12\x15\n\rresource_type\x18\n \x01(\t\"\xb5\x02\n\x15SitesHostNameBindings\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x61zure_resource_name\x18\x04 \x01(\t\x12\x1b\n\x13\x61zure_resource_type\x18\x05 \x01(\t\x12(\n custom_host_name_dns_record_type\x18\x06 \x01(\t\x12\x11\n\tdomain_id\x18\x07 \x01(\t\x12\x16\n\x0ehost_name_type\x18\x08 \x01(\t\x12\x11\n\tsite_name\x18\t \x01(\t\x12\x11\n\tssl_state\x18\n \x01(\t\x12\x12\n\nthumbprint\x18\x0b \x01(\t\"j\n\x12SitesFunctionsKeys\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xa7\x05\n\x0eSitesFunctions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12K\n\x06\x63onfig\x18\x04 \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.SitesFunctions.ConfigEntry\x12\x13\n\x0b\x63onfig_href\x18\x05 \x01(\t\x12I\n\x05\x66iles\x18\x06 \x03(\x0b\x32:.oak9.tython.azure.microsoft_web.SitesFunctions.FilesEntry\x12\x17\n\x0f\x66unction_app_id\x18\x07 \x01(\t\x12\x0c\n\x04href\x18\x08 \x01(\t\x12\x1b\n\x13invoke_url_template\x18\t \x01(\t\x12\x13\n\x0bis_disabled\x18\n \x01(\x08\x12\x10\n\x08language\x18\x0b \x01(\t\x12\x13\n\x0bscript_href\x18\x0c \x01(\t\x12\x1d\n\x15script_root_path_href\x18\r \x01(\t\x12\x19\n\x11secrets_file_href\x18\x0e \x01(\t\x12\x11\n\ttest_data\x18\x0f \x01(\t\x12\x16\n\x0etest_data_href\x18\x10 \x01(\t\x12Q\n\x14sites_functions_keys\x18\x11 \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesFunctionsKeys\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a,\n\nFilesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x8b\x03\n\x0fSitesExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x61pp_offline\x18\x04 \x01(\x08\x12\x19\n\x11\x63onnection_string\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_type\x18\x06 \x01(\t\x12\x13\n\x0bpackage_uri\x18\x07 \x01(\t\x12[\n\x0eset_parameters\x18\x08 \x03(\x0b\x32\x43.oak9.tython.azure.microsoft_web.SitesExtensions.SetParametersEntry\x12#\n\x1bset_parameters_xml_file_uri\x18\t \x01(\t\x12\x15\n\rskip_app_data\x18\n \x01(\x08\x1a\x34\n\x12SetParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x82\x01\n\x1fSitesDomainOwnershipIdentifiers\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\t\"\x87\x02\n\x10SitesDeployments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x0e\n\x06\x61uthor\x18\x05 \x01(\t\x12\x14\n\x0c\x61uthor_email\x18\x06 \x01(\t\x12\x10\n\x08\x64\x65ployer\x18\x07 \x01(\t\x12\x0f\n\x07\x64\x65tails\x18\x08 \x01(\t\x12\x10\n\x08\x65nd_time\x18\t \x01(\t\x12\x0f\n\x07message\x18\n \x01(\t\x12\x12\n\nstart_time\x18\x0b \x01(\t\x12\x0e\n\x06status\x18\x0c \x01(\x05\"\x94\x05\n\x0bSitesConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nftps_state\x18\x02 \x01(\t\x12\x19\n\x11health_check_path\x18\x03 \x01(\t\x12\x16\n\x0ehttp20_enabled\x18\x04 \x01(\t\x12\x1c\n\x14http_logging_enabled\x18\x05 \x01(\t\x12\x16\n\x0ejava_container\x18\x06 \x01(\t\x12\x1e\n\x16java_container_version\x18\x07 \x01(\t\x12\x14\n\x0cjava_version\x18\x08 \x01(\t\x12\x18\n\x10linux_fx_version\x18\t \x01(\t\x12\x16\n\x0eload_balancing\x18\n \x01(\t\x12!\n\x19logs_directory_size_limit\x18\x0b \x01(\t\x12\x1d\n\x15managed_pipeline_mode\x18\x0c \x01(\t\x12\x17\n\x0fmin_tls_version\x18\r \x01(\t\x12\x1d\n\x15net_framework_version\x18\x0e \x01(\t\x12\x14\n\x0cnode_version\x18\x0f \x01(\t\x12\x13\n\x0bphp_version\x18\x10 \x01(\t\x12\x1b\n\x13publishing_username\x18\x11 \x01(\t\x12\x16\n\x0epython_version\x18\x12 \x01(\t\x12 \n\x18remote_debugging_enabled\x18\x13 \x01(\t\x12 \n\x18remote_debugging_version\x18\x14 \x01(\t\x12-\n%scm_ip_security_restrictions_use_main\x18\x15 \x01(\t\x12\x1a\n\x12windows_fx_version\x18\x16 \x01(\t\"b\n\'SitesBasicPublishingCredentialsPolicies\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\xf5\x13\n\x05Sites\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12I\n\x08identity\x18\x03 \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.ManagedServiceIdentity\x12\x0c\n\x04kind\x18\x04 \x01(\t\x12\x10\n\x08location\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x1f\n\x17\x63lient_affinity_enabled\x18\x07 \x01(\x08\x12\x1b\n\x13\x63lient_cert_enabled\x18\x08 \x01(\x08\x12#\n\x1b\x63lient_cert_exclusion_paths\x18\t \x01(\t\x12\x18\n\x10\x63lient_cert_mode\x18\n \x01(\t\x12\x42\n\x0c\x63loning_info\x18\x0b \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.CloningInfo\x12\x16\n\x0e\x63ontainer_size\x18\x0c \x01(\x05\x12%\n\x1d\x63ustom_domain_verification_id\x18\r \x01(\t\x12\x1f\n\x17\x64\x61ily_memory_time_quota\x18\x0e \x01(\x05\x12\x0f\n\x07\x65nabled\x18\x0f \x01(\x08\x12_\n\x1bhosting_environment_profile\x18\x10 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.HostingEnvironmentProfile\x12\x1b\n\x13host_names_disabled\x18\x11 \x01(\x08\x12O\n\x14host_name_ssl_states\x18\x12 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.HostNameSslState\x12\x12\n\nhttps_only\x18\x13 \x01(\x08\x12\x0f\n\x07hyper_v\x18\x14 \x01(\x08\x12\x10\n\x08is_xenon\x18\x15 \x01(\x08\x12$\n\x1ckey_vault_reference_identity\x18\x16 \x01(\t\x12\x17\n\x0fredundancy_mode\x18\x17 \x01(\t\x12\x10\n\x08reserved\x18\x18 \x01(\x08\x12\x1d\n\x15scm_site_also_stopped\x18\x19 \x01(\x08\x12\x16\n\x0eserver_farm_id\x18\x1a \x01(\t\x12@\n\x0bsite_config\x18\x1b \x01(\x0b\x32+.oak9.tython.azure.microsoft_web.SiteConfig\x12 \n\x18storage_account_required\x18\x1c \x01(\x08\x12!\n\x19virtual_network_subnet_id\x18\x1d \x01(\t\x12>\n\x04tags\x18\x1e \x03(\x0b\x32\x30.oak9.tython.azure.microsoft_web.Sites.TagsEntry\x12}\n+sites_basic_publishing_credentials_policies\x18\x1f \x03(\x0b\x32H.oak9.tython.azure.microsoft_web.SitesBasicPublishingCredentialsPolicies\x12l\n\"sites_domain_ownership_identifiers\x18  \x03(\x0b\x32@.oak9.tython.azure.microsoft_web.SitesDomainOwnershipIdentifiers\x12J\n\x10sites_extensions\x18! \x03(\x0b\x32\x30.oak9.tython.azure.microsoft_web.SitesExtensions\x12H\n\x0fsites_functions\x18\" \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.SitesFunctions\x12V\n\x16sites_hybridconnection\x18# \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.SitesHybridconnection\x12\x44\n\rsites_migrate\x18$ \x03(\x0b\x32-.oak9.tython.azure.microsoft_web.SitesMigrate\x12Q\n\x14sites_network_config\x18% \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesNetworkConfig\x12P\n\x13sites_premieraddons\x18& \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesPremieraddons\x12Q\n\x14sites_private_access\x18\' \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesPrivateAccess\x12l\n\"sites_private_endpoint_connections\x18( \x03(\x0b\x32@.oak9.tython.azure.microsoft_web.SitesPrivateEndpointConnections\x12[\n\x19sites_public_certificates\x18) \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesPublicCertificates\x12R\n\x14sites_siteextensions\x18* \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.SitesSiteextensions\x12@\n\x0bsites_slots\x18+ \x03(\x0b\x32+.oak9.tython.azure.microsoft_web.SitesSlots\x12R\n\x14sites_sourcecontrols\x18, \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.SitesSourcecontrols\x12j\n!sites_virtual_network_connections\x18- \x03(\x0b\x32?.oak9.tython.azure.microsoft_web.SitesVirtualNetworkConnections\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa1\x15\n\nSiteConfig\x12&\n\x1e\x61\x63r_use_managed_identity_creds\x18\x01 \x01(\x08\x12$\n\x1c\x61\x63r_user_managed_identity_id\x18\x02 \x01(\t\x12\x11\n\talways_on\x18\x03 \x01(\x08\x12J\n\x0e\x61pi_definition\x18\x04 \x01(\x0b\x32\x32.oak9.tython.azure.microsoft_web.ApiDefinitionInfo\x12S\n\x15\x61pi_management_config\x18\x05 \x01(\x0b\x32\x34.oak9.tython.azure.microsoft_web.ApiManagementConfig\x12\x18\n\x10\x61pp_command_line\x18\x06 \x01(\t\x12\x44\n\x0c\x61pp_settings\x18\x07 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.NameValuePair\x12\x19\n\x11\x61uto_heal_enabled\x18\x08 \x01(\x08\x12G\n\x0f\x61uto_heal_rules\x18\t \x01(\x0b\x32..oak9.tython.azure.microsoft_web.AutoHealRules\x12\x1b\n\x13\x61uto_swap_slot_name\x18\n \x01(\t\x12\x65\n\x16\x61zure_storage_accounts\x18\x0b \x03(\x0b\x32\x45.oak9.tython.azure.microsoft_web.SiteConfig.AzureStorageAccountsEntry\x12K\n\x12\x63onnection_strings\x18\x0c \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.ConnStringInfo\x12;\n\x04\x63ors\x18\r \x01(\x0b\x32-.oak9.tython.azure.microsoft_web.CorsSettings\x12\x19\n\x11\x64\x65\x66\x61ult_documents\x18\x0e \x03(\t\x12&\n\x1e\x64\x65tailed_error_logging_enabled\x18\x0f \x01(\x08\x12\x15\n\rdocument_root\x18\x10 \x01(\t\x12\x41\n\x0b\x65xperiments\x18\x11 \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.Experiments\x12\x12\n\nftps_state\x18\x12 \x01(\t\x12 \n\x18\x66unction_app_scale_limit\x18\x13 \x01(\x05\x12\x32\n*functions_runtime_scale_monitoring_enabled\x18\x14 \x01(\x08\x12I\n\x10handler_mappings\x18\x15 \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.HandlerMapping\x12\x19\n\x11health_check_path\x18\x16 \x01(\t\x12\x16\n\x0ehttp20_enabled\x18\x17 \x01(\x08\x12\x1c\n\x14http_logging_enabled\x18\x18 \x01(\x08\x12X\n\x18ip_security_restrictions\x18\x19 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.IpSecurityRestriction\x12\x16\n\x0ejava_container\x18\x1a \x01(\t\x12\x1e\n\x16java_container_version\x18\x1b \x01(\t\x12\x14\n\x0cjava_version\x18\x1c \x01(\t\x12$\n\x1ckey_vault_reference_identity\x18\x1d \x01(\t\x12;\n\x06limits\x18\x1e \x01(\x0b\x32+.oak9.tython.azure.microsoft_web.SiteLimits\x12\x18\n\x10linux_fx_version\x18\x1f \x01(\t\x12\x16\n\x0eload_balancing\x18  \x01(\t\x12\x1c\n\x14local_my_sql_enabled\x18! \x01(\x08\x12!\n\x19logs_directory_size_limit\x18\" \x01(\x05\x12\x1d\n\x15managed_pipeline_mode\x18# \x01(\t\x12#\n\x1bmanaged_service_identity_id\x18$ \x01(\x05\x12&\n\x1eminimum_elastic_instance_count\x18% \x01(\x05\x12\x17\n\x0fmin_tls_version\x18& \x01(\t\x12\x1d\n\x15net_framework_version\x18\' \x01(\t\x12\x14\n\x0cnode_version\x18( \x01(\t\x12\x19\n\x11number_of_workers\x18) \x01(\x05\x12\x13\n\x0bphp_version\x18* \x01(\t\x12\x1b\n\x13power_shell_version\x18+ \x01(\t\x12!\n\x19pre_warmed_instance_count\x18, \x01(\x05\x12\x1d\n\x15public_network_access\x18- \x01(\t\x12\x1b\n\x13publishing_username\x18. \x01(\t\x12;\n\x04push\x18/ \x01(\x0b\x32-.oak9.tython.azure.microsoft_web.PushSettings\x12\x16\n\x0epython_version\x18\x30 \x01(\t\x12 \n\x18remote_debugging_enabled\x18\x31 \x01(\x08\x12 \n\x18remote_debugging_version\x18\x32 \x01(\t\x12\x1f\n\x17request_tracing_enabled\x18\x33 \x01(\x08\x12\'\n\x1frequest_tracing_expiration_time\x18\x34 \x01(\t\x12\\\n\x1cscm_ip_security_restrictions\x18\x35 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.IpSecurityRestriction\x12-\n%scm_ip_security_restrictions_use_main\x18\x36 \x01(\x08\x12\x1b\n\x13scm_min_tls_version\x18\x37 \x01(\t\x12\x10\n\x08scm_type\x18\x38 \x01(\t\x12\x17\n\x0ftracing_options\x18\x39 \x01(\t\x12 \n\x18use32_bit_worker_process\x18: \x01(\x08\x12Q\n\x14virtual_applications\x18; \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.VirtualApplication\x12\x11\n\tvnet_name\x18< \x01(\t\x12 \n\x18vnet_private_ports_count\x18= \x01(\x05\x12\x1e\n\x16vnet_route_all_enabled\x18> \x01(\x08\x12\x19\n\x11website_time_zone\x18? \x01(\t\x12\x1b\n\x13web_sockets_enabled\x18@ \x01(\x08\x12\x1a\n\x12windows_fx_version\x18\x41 \x01(\t\x12%\n\x1dx_managed_service_identity_id\x18\x42 \x01(\x05\x1a;\n\x19\x41zureStorageAccountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x12VirtualApplication\x12\x15\n\rphysical_path\x18\x01 \x01(\t\x12\x17\n\x0fpreload_enabled\x18\x02 \x01(\x08\x12N\n\x13virtual_directories\x18\x03 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.VirtualDirectory\x12\x14\n\x0cvirtual_path\x18\x04 \x01(\t\"?\n\x10VirtualDirectory\x12\x15\n\rphysical_path\x18\x01 \x01(\t\x12\x14\n\x0cvirtual_path\x18\x02 \x01(\t\"\x89\x01\n\x0cPushSettings\x12\x0c\n\x04kind\x18\x01 \x01(\t\x12\x19\n\x11\x64ynamic_tags_json\x18\x02 \x01(\t\x12\x17\n\x0fis_push_enabled\x18\x03 \x01(\x08\x12\x1b\n\x13tags_requiring_auth\x18\x04 \x01(\t\x12\x1a\n\x12tag_whitelist_json\x18\x05 \x01(\t\"_\n\nSiteLimits\x12\x1b\n\x13max_disk_size_in_mb\x18\x01 \x01(\x05\x12\x18\n\x10max_memory_in_mb\x18\x02 \x01(\x05\x12\x1a\n\x12max_percentage_cpu\x18\x03 \x01(\x01\"\xef\x02\n\x15IpSecurityRestriction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12T\n\x07headers\x18\x03 \x03(\x0b\x32\x43.oak9.tython.azure.microsoft_web.IpSecurityRestriction.HeadersEntry\x12\x12\n\nip_address\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\x05\x12\x13\n\x0bsubnet_mask\x18\x07 \x01(\t\x12\x1a\n\x12subnet_traffic_tag\x18\x08 \x01(\x05\x12\x0b\n\x03tag\x18\t \x01(\t\x12\x1f\n\x17vnet_subnet_resource_id\x18\n \x01(\t\x12\x18\n\x10vnet_traffic_tag\x18\x0b \x01(\x05\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"P\n\x0eHandlerMapping\x12\x11\n\targuments\x18\x01 \x01(\t\x12\x11\n\textension\x18\x02 \x01(\t\x12\x18\n\x10script_processor\x18\x03 \x01(\t\"Q\n\x0b\x45xperiments\x12\x42\n\rramp_up_rules\x18\x01 \x03(\x0b\x32+.oak9.tython.azure.microsoft_web.RampUpRule\"\xef\x01\n\nRampUpRule\x12\x18\n\x10\x61\x63tion_host_name\x18\x01 \x01(\t\x12$\n\x1c\x63hange_decision_callback_url\x18\x02 \x01(\t\x12\"\n\x1a\x63hange_interval_in_minutes\x18\x03 \x01(\x05\x12\x13\n\x0b\x63hange_step\x18\x04 \x01(\x01\x12\x1e\n\x16max_reroute_percentage\x18\x05 \x01(\x01\x12\x1e\n\x16min_reroute_percentage\x18\x06 \x01(\x01\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x1a\n\x12reroute_percentage\x18\x08 \x01(\x01\"D\n\x0c\x43orsSettings\x12\x17\n\x0f\x61llowed_origins\x18\x01 \x03(\t\x12\x1b\n\x13support_credentials\x18\x02 \x01(\x08\"G\n\x0e\x43onnStringInfo\x12\x19\n\x11\x63onnection_string\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\"\x97\x01\n\rAutoHealRules\x12\x41\n\x07\x61\x63tions\x18\x01 \x01(\x0b\x32\x30.oak9.tython.azure.microsoft_web.AutoHealActions\x12\x43\n\x08triggers\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.AutoHealTriggers\"\xd1\x03\n\x10\x41utoHealTriggers\x12\x1b\n\x13private_bytes_in_kb\x18\x01 \x01(\x05\x12G\n\x08requests\x18\x02 \x01(\x0b\x32\x35.oak9.tython.azure.microsoft_web.RequestsBasedTrigger\x12P\n\rslow_requests\x18\x03 \x01(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SlowRequestsBasedTrigger\x12Z\n\x17slow_requests_with_path\x18\x04 \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SlowRequestsBasedTrigger\x12N\n\x0cstatus_codes\x18\x05 \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.StatusCodesBasedTrigger\x12Y\n\x12status_codes_range\x18\x06 \x03(\x0b\x32=.oak9.tython.azure.microsoft_web.StatusCodesRangeBasedTrigger\"h\n\x1cStatusCodesRangeBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x14\n\x0cstatus_codes\x18\x03 \x01(\t\x12\x15\n\rtime_interval\x18\x04 \x01(\t\"\x87\x01\n\x17StatusCodesBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\x05\x12\x12\n\nsub_status\x18\x04 \x01(\x05\x12\x15\n\rtime_interval\x18\x05 \x01(\t\x12\x14\n\x0cwin32_status\x18\x06 \x01(\x05\"b\n\x18SlowRequestsBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x15\n\rtime_interval\x18\x03 \x01(\t\x12\x12\n\ntime_taken\x18\x04 \x01(\t\"<\n\x14RequestsBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x15\n\rtime_interval\x18\x02 \x01(\t\"\x98\x01\n\x0f\x41utoHealActions\x12\x13\n\x0b\x61\x63tion_type\x18\x01 \x01(\t\x12L\n\rcustom_action\x18\x02 \x01(\x0b\x32\x35.oak9.tython.azure.microsoft_web.AutoHealCustomAction\x12\"\n\x1amin_process_execution_time\x18\x03 \x01(\t\"7\n\x14\x41utoHealCustomAction\x12\x0b\n\x03\x65xe\x18\x01 \x01(\t\x12\x12\n\nparameters\x18\x02 \x01(\t\"!\n\x13\x41piManagementConfig\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x11\x41piDefinitionInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x81\x01\n\x10HostNameSslState\x12\x11\n\thost_type\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tssl_state\x18\x03 \x01(\t\x12\x12\n\nthumbprint\x18\x04 \x01(\t\x12\x11\n\tto_update\x18\x05 \x01(\x08\x12\x12\n\nvirtual_ip\x18\x06 \x01(\t\"\xe1\x03\n\x0b\x43loningInfo\x12\x66\n\x16\x61pp_settings_overrides\x18\x01 \x03(\x0b\x32\x46.oak9.tython.azure.microsoft_web.CloningInfo.AppSettingsOverridesEntry\x12\x1f\n\x17\x63lone_custom_host_names\x18\x02 \x01(\x08\x12\x1c\n\x14\x63lone_source_control\x18\x03 \x01(\x08\x12 \n\x18\x63onfigure_load_balancing\x18\x04 \x01(\x08\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12\x1b\n\x13hosting_environment\x18\x06 \x01(\t\x12\x11\n\toverwrite\x18\x07 \x01(\x08\x12\x19\n\x11source_web_app_id\x18\x08 \x01(\t\x12\x1f\n\x17source_web_app_location\x18\t \x01(\t\x12\"\n\x1atraffic_manager_profile_id\x18\n \x01(\t\x12$\n\x1ctraffic_manager_profile_name\x18\x0b \x01(\t\x1a;\n\x19\x41ppSettingsOverridesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xdc\x01\n\x16ManagedServiceIdentity\x12\x0c\n\x04type\x18\x01 \x01(\t\x12u\n\x18user_assigned_identities\x18\x02 \x03(\x0b\x32S.oak9.tython.azure.microsoft_web.ManagedServiceIdentity.UserAssignedIdentitiesEntry\x1a=\n\x1bUserAssignedIdentitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc1\x01\n*ServerfarmsVirtualNetworkConnectionsRoutes\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x65nd_address\x18\x04 \x01(\t\x12\x12\n\nroute_type\x18\x05 \x01(\t\x12\x15\n\rstart_address\x18\x06 \x01(\t\"\xaf\x01\n,ServerfarmsVirtualNetworkConnectionsGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tvnet_name\x18\x04 \x01(\t\x12\x17\n\x0fvpn_package_uri\x18\x05 \x01(\t\"\x84\x07\n\x0bServerfarms\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1d\n\x15\x65lastic_scale_enabled\x18\x06 \x01(\x08\x12\"\n\x1a\x66ree_offer_expiration_time\x18\x07 \x01(\t\x12_\n\x1bhosting_environment_profile\x18\x08 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.HostingEnvironmentProfile\x12\x0f\n\x07hyper_v\x18\t \x01(\x08\x12\x0f\n\x07is_spot\x18\n \x01(\x08\x12\x10\n\x08is_xenon\x18\x0b \x01(\x08\x12Y\n\x18kube_environment_profile\x18\x0c \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.KubeEnvironmentProfile\x12$\n\x1cmaximum_elastic_worker_count\x18\r \x01(\x05\x12\x18\n\x10per_site_scaling\x18\x0e \x01(\x08\x12\x10\n\x08reserved\x18\x0f \x01(\x08\x12\x1c\n\x14spot_expiration_time\x18\x10 \x01(\t\x12\x1b\n\x13target_worker_count\x18\x11 \x01(\x05\x12\x1d\n\x15target_worker_size_id\x18\x12 \x01(\x05\x12\x18\n\x10worker_tier_name\x18\x13 \x01(\t\x12\x16\n\x0ezone_redundant\x18\x14 \x01(\x08\x12<\n\x03sku\x18\x15 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\x12\x44\n\x04tags\x18\x16 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.Serverfarms.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"$\n\x16KubeEnvironmentProfile\x12\n\n\x02id\x18\x01 \x01(\t\"\'\n\x19HostingEnvironmentProfile\x12\n\n\x02id\x18\x01 \x01(\t\"\xb5\x05\n\x10KubeEnvironments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x17\n\x0f\x61ks_resource_id\x18\x06 \x01(\t\x12U\n\x16\x61pp_logs_configuration\x18\x07 \x01(\x0b\x32\x35.oak9.tython.azure.microsoft_web.AppLogsConfiguration\x12L\n\x11\x61rc_configuration\x18\x08 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ArcConfiguration\x12\x61\n\x1c\x63ontainer_apps_configuration\x18\t \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.ContainerAppsConfiguration\x12\x18\n\x10\x65nvironment_type\x18\n \x01(\t\x12&\n\x1einternal_load_balancer_enabled\x18\x0b \x01(\x08\x12\x11\n\tstatic_ip\x18\x0c \x01(\t\x12I\n\x04tags\x18\r \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.KubeEnvironments.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xea\x01\n\x1a\x43ontainerAppsConfiguration\x12\x1e\n\x16\x61pp_subnet_resource_id\x18\x01 \x01(\t\x12(\n control_plane_subnet_resource_id\x18\x02 \x01(\t\x12$\n\x1c\x64\x61pr_a_i_instrumentation_key\x18\x03 \x01(\t\x12\x1a\n\x12\x64ocker_bridge_cidr\x18\x04 \x01(\t\x12\x1e\n\x16platform_reserved_cidr\x18\x05 \x01(\t\x12 \n\x18platform_reserved_dns_ip\x18\x06 \x01(\t\"\xbc\x02\n\x10\x41rcConfiguration\x12\x1e\n\x16\x61rtifacts_storage_type\x18\x01 \x01(\t\x12$\n\x1c\x61rtifact_storage_access_mode\x18\x02 \x01(\t\x12#\n\x1b\x61rtifact_storage_class_name\x18\x03 \x01(\t\x12#\n\x1b\x61rtifact_storage_mount_path\x18\x04 \x01(\t\x12\"\n\x1a\x61rtifact_storage_node_name\x18\x05 \x01(\t\x12_\n\x1f\x66ront_end_service_configuration\x18\x06 \x01(\x0b\x32\x36.oak9.tython.azure.microsoft_web.FrontEndConfiguration\x12\x13\n\x0bkube_config\x18\x07 \x01(\t\"%\n\x15\x46rontEndConfiguration\x12\x0c\n\x04kind\x18\x01 \x01(\t\"\x8c\x01\n\x14\x41ppLogsConfiguration\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12_\n\x1blog_analytics_configuration\x18\x02 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.LogAnalyticsConfiguration\"D\n\x19LogAnalyticsConfiguration\x12\x13\n\x0b\x63ustomer_id\x18\x01 \x01(\t\x12\x12\n\nshared_key\x18\x02 \x01(\t\" \n\x10\x45xtendedLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x8c\x02\n\x1eHostingEnvironmentsWorkerPools\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ompute_mode\x18\x04 \x01(\t\x12\x14\n\x0cworker_count\x18\x05 \x01(\x05\x12\x13\n\x0bworker_size\x18\x06 \x01(\t\x12\x16\n\x0eworker_size_id\x18\x07 \x01(\x05\x12<\n\x03sku\x18\x08 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\"\xf0\x01\n-HostingEnvironmentsPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"[\n\x1aPrivateLinkConnectionState\x12\x18\n\x10\x61\x63tions_required\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\"\x8f\x02\n!HostingEnvironmentsMultiRolePools\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ompute_mode\x18\x04 \x01(\t\x12\x14\n\x0cworker_count\x18\x05 \x01(\x05\x12\x13\n\x0bworker_size\x18\x06 \x01(\t\x12\x16\n\x0eworker_size_id\x18\x07 \x01(\x05\x12<\n\x03sku\x18\x08 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\"\xf6\x01\n\x0eSkuDescription\x12\x41\n\x0c\x63\x61pabilities\x18\x01 \x03(\x0b\x32+.oak9.tython.azure.microsoft_web.Capability\x12\x10\n\x08\x63\x61pacity\x18\x02 \x01(\x05\x12\x0e\n\x06\x66\x61mily\x18\x03 \x01(\t\x12\x11\n\tlocations\x18\x04 \x03(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x0c\n\x04size\x18\x06 \x01(\t\x12\x42\n\x0csku_capacity\x18\x07 \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.SkuCapacity\x12\x0c\n\x04tier\x18\x08 \x01(\t\"m\n\x0bSkuCapacity\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x01 \x01(\x05\x12\x17\n\x0f\x65lastic_maximum\x18\x02 \x01(\x05\x12\x0f\n\x07maximum\x18\x03 \x01(\x05\x12\x0f\n\x07minimum\x18\x04 \x01(\x05\x12\x12\n\nscale_type\x18\x05 \x01(\t\"9\n\nCapability\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xa8\x01\n!HostingEnvironmentsConfigurations\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12.\n&allow_new_private_endpoint_connections\x18\x04 \x01(\x08\"\xd3\x08\n\x13HostingEnvironments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12H\n\x10\x63luster_settings\x18\x05 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.NameValuePair\x12\x1c\n\x14\x64\x65\x64icated_host_count\x18\x06 \x01(\x05\x12\x12\n\ndns_suffix\x18\x07 \x01(\t\x12\x1e\n\x16\x66ront_end_scale_factor\x18\x08 \x01(\x05\x12$\n\x1cinternal_load_balancing_mode\x18\t \x01(\t\x12\x1b\n\x13ipssl_address_count\x18\n \x01(\x05\x12\x12\n\nmulti_size\x18\x0b \x01(\t\x12\"\n\x1auser_whitelisted_ip_ranges\x18\x0c \x03(\t\x12O\n\x0fvirtual_network\x18\r \x01(\x0b\x32\x36.oak9.tython.azure.microsoft_web.VirtualNetworkProfile\x12\x16\n\x0ezone_redundant\x18\x0e \x01(\x08\x12L\n\x04tags\x18\x0f \x03(\x0b\x32>.oak9.tython.azure.microsoft_web.HostingEnvironments.TagsEntry\x12o\n#hosting_environments_configurations\x18\x10 \x03(\x0b\x32\x42.oak9.tython.azure.microsoft_web.HostingEnvironmentsConfigurations\x12q\n%hosting_environments_multi_role_pools\x18\x11 \x03(\x0b\x32\x42.oak9.tython.azure.microsoft_web.HostingEnvironmentsMultiRolePools\x12\x89\x01\n1hosting_environments_private_endpoint_connections\x18\x12 \x03(\x0b\x32N.oak9.tython.azure.microsoft_web.HostingEnvironmentsPrivateEndpointConnections\x12j\n!hosting_environments_worker_pools\x18\x13 \x03(\x0b\x32?.oak9.tython.azure.microsoft_web.HostingEnvironmentsWorkerPools\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"3\n\x15VirtualNetworkProfile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06subnet\x18\x02 \x01(\t\",\n\rNameValuePair\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x8c\x03\n\rContainerApps\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x45\n\rconfiguration\x18\x05 \x01(\x0b\x32..oak9.tython.azure.microsoft_web.Configuration\x12\x1b\n\x13kube_environment_id\x18\x06 \x01(\t\x12;\n\x08template\x18\x07 \x01(\x0b\x32).oak9.tython.azure.microsoft_web.Template\x12\x46\n\x04tags\x18\x08 \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.ContainerApps.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xcf\x01\n\x08Template\x12>\n\ncontainers\x18\x01 \x03(\x0b\x32*.oak9.tython.azure.microsoft_web.Container\x12\x33\n\x04\x64\x61pr\x18\x02 \x01(\x0b\x32%.oak9.tython.azure.microsoft_web.Dapr\x12\x17\n\x0frevision_suffix\x18\x03 \x01(\t\x12\x35\n\x05scale\x18\x04 \x01(\x0b\x32&.oak9.tython.azure.microsoft_web.Scale\"n\n\x05Scale\x12\x14\n\x0cmax_replicas\x18\x01 \x01(\x05\x12\x14\n\x0cmin_replicas\x18\x02 \x01(\x05\x12\x39\n\x05rules\x18\x03 \x03(\x0b\x32*.oak9.tython.azure.microsoft_web.ScaleRule\"\xdf\x01\n\tScaleRule\x12\x44\n\x0b\x61zure_queue\x18\x01 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.QueueScaleRule\x12@\n\x06\x63ustom\x18\x02 \x01(\x0b\x32\x30.oak9.tython.azure.microsoft_web.CustomScaleRule\x12<\n\x04http\x18\x03 \x01(\x0b\x32..oak9.tython.azure.microsoft_web.HttpScaleRule\x12\x0c\n\x04name\x18\x04 \x01(\t\"\xce\x01\n\rHttpScaleRule\x12<\n\x04\x61uth\x18\x01 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.ScaleRuleAuth\x12N\n\x08metadata\x18\x02 \x03(\x0b\x32<.oak9.tython.azure.microsoft_web.HttpScaleRule.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe0\x01\n\x0f\x43ustomScaleRule\x12<\n\x04\x61uth\x18\x01 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.ScaleRuleAuth\x12P\n\x08metadata\x18\x02 \x03(\x0b\x32>.oak9.tython.azure.microsoft_web.CustomScaleRule.MetadataEntry\x12\x0c\n\x04type\x18\x03 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"x\n\x0eQueueScaleRule\x12<\n\x04\x61uth\x18\x01 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.ScaleRuleAuth\x12\x14\n\x0cqueue_length\x18\x02 \x01(\x05\x12\x12\n\nqueue_name\x18\x03 \x01(\t\">\n\rScaleRuleAuth\x12\x12\n\nsecret_ref\x18\x01 \x01(\t\x12\x19\n\x11trigger_parameter\x18\x02 \x01(\t\"}\n\x04\x44\x61pr\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x10\n\x08\x61pp_port\x18\x02 \x01(\x05\x12\x42\n\ncomponents\x18\x03 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.DaprComponent\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\"}\n\rDaprComponent\x12?\n\x08metadata\x18\x01 \x03(\x0b\x32-.oak9.tython.azure.microsoft_web.DaprMetadata\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"?\n\x0c\x44\x61prMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsecret_ref\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x85\x01\n\tContainer\x12\x0c\n\x04\x61rgs\x18\x01 \x03(\t\x12\x0f\n\x07\x63ommand\x18\x02 \x03(\t\x12<\n\x03\x65nv\x18\x03 \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.EnvironmentVar\x12\r\n\x05image\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\"A\n\x0e\x45nvironmentVar\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsecret_ref\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xed\x01\n\rConfiguration\x12\x1d\n\x15\x61\x63tive_revisions_mode\x18\x01 \x01(\t\x12\x39\n\x07ingress\x18\x02 \x01(\x0b\x32(.oak9.tython.azure.microsoft_web.Ingress\x12H\n\nregistries\x18\x03 \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.RegistryCredentials\x12\x38\n\x07secrets\x18\x04 \x03(\x0b\x32\'.oak9.tython.azure.microsoft_web.Secret\"%\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"T\n\x13RegistryCredentials\x12\x1b\n\x13password_secret_ref\x18\x01 \x01(\t\x12\x0e\n\x06server\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\"\x9c\x01\n\x07Ingress\x12\x16\n\x0e\x61llow_insecure\x18\x01 \x01(\x08\x12\x10\n\x08\x65xternal\x18\x02 \x01(\x08\x12\x13\n\x0btarget_port\x18\x03 \x01(\x05\x12?\n\x07traffic\x18\x04 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.TrafficWeight\x12\x11\n\ttransport\x18\x05 \x01(\t\"O\n\rTrafficWeight\x12\x17\n\x0flatest_revision\x18\x01 \x01(\x08\x12\x15\n\rrevision_name\x18\x02 \x01(\t\x12\x0e\n\x06weight\x18\x03 \x01(\x05\"\xa8\x03\n\x0c\x43\x65rtificates\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x16\n\x0e\x63\x61nonical_name\x18\x05 \x01(\t\x12 \n\x18\x64omain_validation_method\x18\x06 \x01(\t\x12\x12\n\nhost_names\x18\x07 \x03(\t\x12\x14\n\x0ckey_vault_id\x18\x08 \x01(\t\x12\x1d\n\x15key_vault_secret_name\x18\t \x01(\t\x12\x10\n\x08password\x18\n \x01(\t\x12\x10\n\x08pfx_blob\x18\x0b \x01(\t\x12\x16\n\x0eserver_farm_id\x18\x0c \x01(\t\x12\x45\n\x04tags\x18\r \x03(\x0b\x32\x37.oak9.tython.azure.microsoft_web.Certificates.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x61zure/azure_microsoft_web.proto\x12\x1foak9.tython.azure.microsoft_web\x1a\x13shared/shared.proto\"\xd8\x05\n\rMicrosoft_Web\x12R\n\x14hosting_environments\x18\x01 \x01(\x0b\x32\x34.oak9.tython.azure.microsoft_web.HostingEnvironments\x12\x41\n\x0bserverfarms\x18\x02 \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.Serverfarms\x12\x87\x01\n0serverfarms_virtual_network_connections_gateways\x18\x03 \x03(\x0b\x32M.oak9.tython.azure.microsoft_web.ServerfarmsVirtualNetworkConnectionsGateways\x12\x83\x01\n.serverfarms_virtual_network_connections_routes\x18\x04 \x03(\x0b\x32K.oak9.tython.azure.microsoft_web.ServerfarmsVirtualNetworkConnectionsRoutes\x12\x35\n\x05sites\x18\x05 \x01(\x0b\x32&.oak9.tython.azure.microsoft_web.Sites\x12\x41\n\x0csites_config\x18\x06 \x03(\x0b\x32+.oak9.tython.azure.microsoft_web.SiteConfig\x12L\n\x11sites_deployments\x18\x07 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.SitesDeployments\x12X\n\x18sites_host_name_bindings\x18\x08 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.SitesHostNameBindings\"\xb9\x01\n#StaticSitesUserProvidedFunctionApps\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x66unction_app_region\x18\x04 \x01(\t\x12 \n\x18\x66unction_app_resource_id\x18\x05 \x01(\t\"\xe8\x01\n%StaticSitesPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"\x9d\x01\n\x19StaticSitesLinkedBackends\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x62\x61\x63kend_resource_id\x18\x04 \x01(\t\x12\x0e\n\x06region\x18\x05 \x01(\t\"\x8a\x01\n\x18StaticSitesCustomDomains\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x19\n\x11validation_method\x18\x04 \x01(\t\"L\n\x11StaticSitesConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\xbf\x01\n)StaticSitesBuildsUserProvidedFunctionApps\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x66unction_app_region\x18\x04 \x01(\t\x12 \n\x18\x66unction_app_resource_id\x18\x05 \x01(\t\"\xa3\x01\n\x1fStaticSitesBuildsLinkedBackends\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x62\x61\x63kend_resource_id\x18\x04 \x01(\t\x12\x0e\n\x06region\x18\x05 \x01(\t\"R\n\x17StaticSitesBuildsConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\x84\n\n\x0bStaticSites\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12I\n\x08identity\x18\x02 \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.ManagedServiceIdentity\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12!\n\x19\x61llow_config_file_updates\x18\x06 \x01(\x08\x12\x0e\n\x06\x62ranch\x18\x07 \x01(\t\x12T\n\x10\x62uild_properties\x18\x08 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.StaticSiteBuildProperties\x12#\n\x1b\x65nterprise_grade_cdn_status\x18\t \x01(\t\x12\x10\n\x08provider\x18\n \x01(\t\x12\x1d\n\x15public_network_access\x18\x0b \x01(\t\x12\x18\n\x10repository_token\x18\x0c \x01(\t\x12\x16\n\x0erepository_url\x18\r \x01(\t\x12\"\n\x1astaging_environment_policy\x18\x0e \x01(\t\x12W\n\x13template_properties\x18\x0f \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.StaticSiteTemplateOptions\x12<\n\x03sku\x18\x10 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\x12\x44\n\x04tags\x18\x11 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.StaticSites.TagsEntry\x12O\n\x13static_sites_config\x18\x12 \x03(\x0b\x32\x32.oak9.tython.azure.microsoft_web.StaticSitesConfig\x12^\n\x1bstatic_sites_custom_domains\x18\x13 \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.StaticSitesCustomDomains\x12y\n)static_sites_private_endpoint_connections\x18\x14 \x03(\x0b\x32\x46.oak9.tython.azure.microsoft_web.StaticSitesPrivateEndpointConnections\x12v\n(static_sites_user_provided_function_apps\x18\x15 \x03(\x0b\x32\x44.oak9.tython.azure.microsoft_web.StaticSitesUserProvidedFunctionApps\x12`\n\x1cstatic_sites_linked_backends\x18\x16 \x03(\x0b\x32:.oak9.tython.azure.microsoft_web.StaticSitesLinkedBackends\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x8d\x01\n\x19StaticSiteTemplateOptions\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x12\n\nis_private\x18\x02 \x01(\x08\x12\r\n\x05owner\x18\x03 \x01(\t\x12\x17\n\x0frepository_name\x18\x04 \x01(\t\x12\x1f\n\x17template_repository_url\x18\x05 \x01(\t\"\x91\x02\n\x19StaticSiteBuildProperties\x12\x19\n\x11\x61pi_build_command\x18\x01 \x01(\t\x12\x14\n\x0c\x61pi_location\x18\x02 \x01(\t\x12\x1d\n\x15\x61pp_artifact_location\x18\x03 \x01(\t\x12\x19\n\x11\x61pp_build_command\x18\x04 \x01(\t\x12\x14\n\x0c\x61pp_location\x18\x05 \x01(\t\x12*\n\"github_action_secret_name_override\x18\x06 \x01(\t\x12\x17\n\x0foutput_location\x18\x07 \x01(\t\x12.\n&skip_github_action_workflow_generation\x18\x08 \x01(\x08\"\xa9\x01\n&SitesVirtualNetworkConnectionsGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tvnet_name\x18\x04 \x01(\t\x12\x17\n\x0fvpn_package_uri\x18\x05 \x01(\t\"\xc6\x02\n\x1eSitesVirtualNetworkConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tcert_blob\x18\x04 \x01(\t\x12\x13\n\x0b\x64ns_servers\x18\x05 \x01(\t\x12\x10\n\x08is_swift\x18\x06 \x01(\x08\x12\x18\n\x10vnet_resource_id\x18\x07 \x01(\t\x12{\n*sites_virtual_network_connections_gateways\x18\x08 \x03(\x0b\x32G.oak9.tython.azure.microsoft_web.SitesVirtualNetworkConnectionsGateways\"\xe3\x02\n\x13SitesSourcecontrols\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\t\x12#\n\x1b\x64\x65ployment_rollback_enabled\x18\x05 \x01(\x08\x12`\n\x1cgit_hub_action_configuration\x18\x06 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.GitHubActionConfiguration\x12\x19\n\x11is_git_hub_action\x18\x07 \x01(\x08\x12\x1d\n\x15is_manual_integration\x18\x08 \x01(\x08\x12\x14\n\x0cis_mercurial\x18\t \x01(\x08\x12\x10\n\x08repo_url\x18\n \x01(\t\"\xae\x01\n+SitesSlotsVirtualNetworkConnectionsGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tvnet_name\x18\x04 \x01(\t\x12\x17\n\x0fvpn_package_uri\x18\x05 \x01(\t\"\xd7\x02\n#SitesSlotsVirtualNetworkConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tcert_blob\x18\x04 \x01(\t\x12\x13\n\x0b\x64ns_servers\x18\x05 \x01(\t\x12\x10\n\x08is_swift\x18\x06 \x01(\x08\x12\x18\n\x10vnet_resource_id\x18\x07 \x01(\t\x12\x86\x01\n0sites_slots_virtual_network_connections_gateways\x18\x08 \x03(\x0b\x32L.oak9.tython.azure.microsoft_web.SitesSlotsVirtualNetworkConnectionsGateways\"\xe8\x02\n\x18SitesSlotsSourcecontrols\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\t\x12#\n\x1b\x64\x65ployment_rollback_enabled\x18\x05 \x01(\x08\x12`\n\x1cgit_hub_action_configuration\x18\x06 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.GitHubActionConfiguration\x12\x19\n\x11is_git_hub_action\x18\x07 \x01(\x08\x12\x1d\n\x15is_manual_integration\x18\x08 \x01(\x08\x12\x14\n\x0cis_mercurial\x18\t \x01(\x08\x12\x10\n\x08repo_url\x18\n \x01(\t\"\x8f\x02\n\x19GitHubActionConfiguration\x12Z\n\x12\x63ode_configuration\x18\x01 \x01(\x0b\x32>.oak9.tython.azure.microsoft_web.GitHubActionCodeConfiguration\x12\x64\n\x17\x63ontainer_configuration\x18\x02 \x01(\x0b\x32\x43.oak9.tython.azure.microsoft_web.GitHubActionContainerConfiguration\x12\x1e\n\x16generate_workflow_file\x18\x03 \x01(\x08\x12\x10\n\x08is_linux\x18\x04 \x01(\x08\"p\n\"GitHubActionContainerConfiguration\x12\x12\n\nimage_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x12\n\nserver_url\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\"O\n\x1dGitHubActionCodeConfiguration\x12\x15\n\rruntime_stack\x18\x01 \x01(\t\x12\x17\n\x0fruntime_version\x18\x02 \x01(\t\"a\n\x18SitesSlotsSiteextensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xa6\x01\n\x1cSitesSlotsPublicCertificates\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x62lob\x18\x04 \x01(\t\x12#\n\x1bpublic_certificate_location\x18\x05 \x01(\t\"\xe7\x01\n$SitesSlotsPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"\xd7\x01\n\x17SitesSlotsPrivateAccess\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12V\n\x10virtual_networks\x18\x05 \x03(\x0b\x32<.oak9.tython.azure.microsoft_web.PrivateAccessVirtualNetwork\"\xe7\x02\n\x17SitesSlotsPremieraddons\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x19\n\x11marketplace_offer\x18\x05 \x01(\t\x12\x1d\n\x15marketplace_publisher\x18\x06 \x01(\t\x12\x0f\n\x07product\x18\x07 \x01(\t\x12\x0b\n\x03sku\x18\x08 \x01(\t\x12\x0e\n\x06vendor\x18\t \x01(\t\x12P\n\x04tags\x18\n \x03(\x0b\x32\x42.oak9.tython.azure.microsoft_web.SitesSlotsPremieraddons.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa3\x01\n\x17SitesSlotsNetworkConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12subnet_resource_id\x18\x04 \x01(\t\x12\x17\n\x0fswift_supported\x18\x05 \x01(\x08\"\xa7\x03\n\x1dSitesSlotsInstancesExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x61pp_offline\x18\x04 \x01(\x08\x12\x19\n\x11\x63onnection_string\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_type\x18\x06 \x01(\t\x12\x13\n\x0bpackage_uri\x18\x07 \x01(\t\x12i\n\x0eset_parameters\x18\x08 \x03(\x0b\x32Q.oak9.tython.azure.microsoft_web.SitesSlotsInstancesExtensions.SetParametersEntry\x12#\n\x1bset_parameters_xml_file_uri\x18\t \x01(\t\x12\x15\n\rskip_app_data\x18\n \x01(\x08\x1a\x34\n\x12SetParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb6\x02\n*SitesSlotsHybridConnectionNamespacesRelays\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08hostname\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x15\n\rrelay_arm_uri\x18\x06 \x01(\t\x12\x12\n\nrelay_name\x18\x07 \x01(\t\x12\x15\n\rsend_key_name\x18\x08 \x01(\t\x12\x16\n\x0esend_key_value\x18\t \x01(\t\x12\x1d\n\x15service_bus_namespace\x18\n \x01(\t\x12\x1a\n\x12service_bus_suffix\x18\x0b \x01(\t\"\x98\x02\n\x1aSitesSlotsHybridconnection\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x62iztalk_uri\x18\x04 \x01(\t\x12 \n\x18\x65ntity_connection_string\x18\x05 \x01(\t\x12\x13\n\x0b\x65ntity_name\x18\x06 \x01(\t\x12\x10\n\x08hostname\x18\x07 \x01(\t\x12\x0c\n\x04port\x18\x08 \x01(\x05\x12\"\n\x1aresource_connection_string\x18\t \x01(\t\x12\x15\n\rresource_type\x18\n \x01(\t\"\xba\x02\n\x1aSitesSlotsHostNameBindings\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x61zure_resource_name\x18\x04 \x01(\t\x12\x1b\n\x13\x61zure_resource_type\x18\x05 \x01(\t\x12(\n custom_host_name_dns_record_type\x18\x06 \x01(\t\x12\x11\n\tdomain_id\x18\x07 \x01(\t\x12\x16\n\x0ehost_name_type\x18\x08 \x01(\t\x12\x11\n\tsite_name\x18\t \x01(\t\x12\x11\n\tssl_state\x18\n \x01(\t\x12\x12\n\nthumbprint\x18\x0b \x01(\t\"o\n\x17SitesSlotsFunctionsKeys\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xc1\x05\n\x13SitesSlotsFunctions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12P\n\x06\x63onfig\x18\x04 \x03(\x0b\x32@.oak9.tython.azure.microsoft_web.SitesSlotsFunctions.ConfigEntry\x12\x13\n\x0b\x63onfig_href\x18\x05 \x01(\t\x12N\n\x05\x66iles\x18\x06 \x03(\x0b\x32?.oak9.tython.azure.microsoft_web.SitesSlotsFunctions.FilesEntry\x12\x17\n\x0f\x66unction_app_id\x18\x07 \x01(\t\x12\x0c\n\x04href\x18\x08 \x01(\t\x12\x1b\n\x13invoke_url_template\x18\t \x01(\t\x12\x13\n\x0bis_disabled\x18\n \x01(\x08\x12\x10\n\x08language\x18\x0b \x01(\t\x12\x13\n\x0bscript_href\x18\x0c \x01(\t\x12\x1d\n\x15script_root_path_href\x18\r \x01(\t\x12\x19\n\x11secrets_file_href\x18\x0e \x01(\t\x12\x11\n\ttest_data\x18\x0f \x01(\t\x12\x16\n\x0etest_data_href\x18\x10 \x01(\t\x12\\\n\x1asites_slots_functions_keys\x18\x11 \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsFunctionsKeys\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a,\n\nFilesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x95\x03\n\x14SitesSlotsExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x61pp_offline\x18\x04 \x01(\x08\x12\x19\n\x11\x63onnection_string\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_type\x18\x06 \x01(\t\x12\x13\n\x0bpackage_uri\x18\x07 \x01(\t\x12`\n\x0eset_parameters\x18\x08 \x03(\x0b\x32H.oak9.tython.azure.microsoft_web.SitesSlotsExtensions.SetParametersEntry\x12#\n\x1bset_parameters_xml_file_uri\x18\t \x01(\t\x12\x15\n\rskip_app_data\x18\n \x01(\x08\x1a\x34\n\x12SetParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x01\n$SitesSlotsDomainOwnershipIdentifiers\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\t\"\x8c\x02\n\x15SitesSlotsDeployments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x0e\n\x06\x61uthor\x18\x05 \x01(\t\x12\x14\n\x0c\x61uthor_email\x18\x06 \x01(\t\x12\x10\n\x08\x64\x65ployer\x18\x07 \x01(\t\x12\x0f\n\x07\x64\x65tails\x18\x08 \x01(\t\x12\x10\n\x08\x65nd_time\x18\t \x01(\t\x12\x0f\n\x07message\x18\n \x01(\t\x12\x12\n\nstart_time\x18\x0b \x01(\t\x12\x0e\n\x06status\x18\x0c \x01(\x05\"K\n\x10SitesSlotsConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"g\n,SitesSlotsBasicPublishingCredentialsPolicies\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\x98\x17\n\nSitesSlots\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12I\n\x08identity\x18\x03 \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.ManagedServiceIdentity\x12\x0c\n\x04kind\x18\x04 \x01(\t\x12\x10\n\x08location\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x1f\n\x17\x63lient_affinity_enabled\x18\x07 \x01(\x08\x12\x1b\n\x13\x63lient_cert_enabled\x18\x08 \x01(\x08\x12#\n\x1b\x63lient_cert_exclusion_paths\x18\t \x01(\t\x12\x18\n\x10\x63lient_cert_mode\x18\n \x01(\t\x12\x42\n\x0c\x63loning_info\x18\x0b \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.CloningInfo\x12\x16\n\x0e\x63ontainer_size\x18\x0c \x01(\x05\x12%\n\x1d\x63ustom_domain_verification_id\x18\r \x01(\t\x12\x1f\n\x17\x64\x61ily_memory_time_quota\x18\x0e \x01(\x05\x12\x0f\n\x07\x65nabled\x18\x0f \x01(\x08\x12_\n\x1bhosting_environment_profile\x18\x10 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.HostingEnvironmentProfile\x12\x1b\n\x13host_names_disabled\x18\x11 \x01(\x08\x12O\n\x14host_name_ssl_states\x18\x12 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.HostNameSslState\x12\x12\n\nhttps_only\x18\x13 \x01(\x08\x12\x0f\n\x07hyper_v\x18\x14 \x01(\x08\x12\x10\n\x08is_xenon\x18\x15 \x01(\x08\x12$\n\x1ckey_vault_reference_identity\x18\x16 \x01(\t\x12\x1d\n\x15public_network_access\x18\x17 \x01(\t\x12\x17\n\x0fredundancy_mode\x18\x18 \x01(\t\x12\x10\n\x08reserved\x18\x19 \x01(\x08\x12\x1d\n\x15scm_site_also_stopped\x18\x1a \x01(\x08\x12\x16\n\x0eserver_farm_id\x18\x1b \x01(\t\x12@\n\x0bsite_config\x18\x1c \x01(\x0b\x32+.oak9.tython.azure.microsoft_web.SiteConfig\x12 \n\x18storage_account_required\x18\x1d \x01(\x08\x12!\n\x19virtual_network_subnet_id\x18\x1e \x01(\t\x12\"\n\x1avnet_content_share_enabled\x18\x1f \x01(\x08\x12\x1f\n\x17vnet_image_pull_enabled\x18  \x01(\x08\x12\x1e\n\x16vnet_route_all_enabled\x18! \x01(\x08\x12\x43\n\x04tags\x18\" \x03(\x0b\x32\x35.oak9.tython.azure.microsoft_web.SitesSlots.TagsEntry\x12\x88\x01\n1sites_slots_basic_publishing_credentials_policies\x18# \x03(\x0b\x32M.oak9.tython.azure.microsoft_web.SitesSlotsBasicPublishingCredentialsPolicies\x12M\n\x12sites_slots_config\x18$ \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.SitesSlotsConfig\x12W\n\x17sites_slots_deployments\x18% \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.SitesSlotsDeployments\x12w\n(sites_slots_domain_ownership_identifiers\x18& \x03(\x0b\x32\x45.oak9.tython.azure.microsoft_web.SitesSlotsDomainOwnershipIdentifiers\x12U\n\x16sites_slots_extensions\x18\' \x03(\x0b\x32\x35.oak9.tython.azure.microsoft_web.SitesSlotsExtensions\x12S\n\x15sites_slots_functions\x18( \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.SitesSlotsFunctions\x12\x63\n\x1esites_slots_host_name_bindings\x18) \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.SitesSlotsHostNameBindings\x12\x61\n\x1csites_slots_hybridconnection\x18* \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.SitesSlotsHybridconnection\x12\\\n\x1asites_slots_network_config\x18+ \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsNetworkConfig\x12[\n\x19sites_slots_premieraddons\x18, \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsPremieraddons\x12\\\n\x1asites_slots_private_access\x18- \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesSlotsPrivateAccess\x12w\n(sites_slots_private_endpoint_connections\x18. \x03(\x0b\x32\x45.oak9.tython.azure.microsoft_web.SitesSlotsPrivateEndpointConnections\x12\x66\n\x1fsites_slots_public_certificates\x18/ \x03(\x0b\x32=.oak9.tython.azure.microsoft_web.SitesSlotsPublicCertificates\x12]\n\x1asites_slots_siteextensions\x18\x30 \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SitesSlotsSiteextensions\x12]\n\x1asites_slots_sourcecontrols\x18\x31 \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SitesSlotsSourcecontrols\x12u\n\'sites_slots_virtual_network_connections\x18\x32 \x03(\x0b\x32\x44.oak9.tython.azure.microsoft_web.SitesSlotsVirtualNetworkConnections\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\\\n\x13SitesSiteextensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xa1\x01\n\x17SitesPublicCertificates\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x62lob\x18\x04 \x01(\t\x12#\n\x1bpublic_certificate_location\x18\x05 \x01(\t\"\xe2\x01\n\x1fSitesPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"\xd2\x01\n\x12SitesPrivateAccess\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12V\n\x10virtual_networks\x18\x05 \x03(\x0b\x32<.oak9.tython.azure.microsoft_web.PrivateAccessVirtualNetwork\"\x94\x01\n\x1bPrivateAccessVirtualNetwork\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0bresource_id\x18\x03 \x01(\t\x12\x45\n\x07subnets\x18\x04 \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.PrivateAccessSubnet\"0\n\x13PrivateAccessSubnet\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xdd\x02\n\x12SitesPremieraddons\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x19\n\x11marketplace_offer\x18\x05 \x01(\t\x12\x1d\n\x15marketplace_publisher\x18\x06 \x01(\t\x12\x0f\n\x07product\x18\x07 \x01(\t\x12\x0b\n\x03sku\x18\x08 \x01(\t\x12\x0e\n\x06vendor\x18\t \x01(\t\x12K\n\x04tags\x18\n \x03(\x0b\x32=.oak9.tython.azure.microsoft_web.SitesPremieraddons.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9e\x01\n\x12SitesNetworkConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12subnet_resource_id\x18\x04 \x01(\t\x12\x17\n\x0fswift_supported\x18\x05 \x01(\x08\"\xec\x01\n\x0cSitesMigrate\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12$\n\x1c\x61zurefiles_connection_string\x18\x04 \x01(\t\x12\x18\n\x10\x61zurefiles_share\x18\x05 \x01(\t\x12\"\n\x1a\x62lock_write_access_to_site\x18\x06 \x01(\x08\x12#\n\x1bswitch_site_after_migration\x18\x07 \x01(\x08\"\x9d\x03\n\x18SitesInstancesExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x61pp_offline\x18\x04 \x01(\x08\x12\x19\n\x11\x63onnection_string\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_type\x18\x06 \x01(\t\x12\x13\n\x0bpackage_uri\x18\x07 \x01(\t\x12\x64\n\x0eset_parameters\x18\x08 \x03(\x0b\x32L.oak9.tython.azure.microsoft_web.SitesInstancesExtensions.SetParametersEntry\x12#\n\x1bset_parameters_xml_file_uri\x18\t \x01(\t\x12\x15\n\rskip_app_data\x18\n \x01(\x08\x1a\x34\n\x12SetParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb1\x02\n%SitesHybridConnectionNamespacesRelays\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08hostname\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x15\n\rrelay_arm_uri\x18\x06 \x01(\t\x12\x12\n\nrelay_name\x18\x07 \x01(\t\x12\x15\n\rsend_key_name\x18\x08 \x01(\t\x12\x16\n\x0esend_key_value\x18\t \x01(\t\x12\x1d\n\x15service_bus_namespace\x18\n \x01(\t\x12\x1a\n\x12service_bus_suffix\x18\x0b \x01(\t\"\x93\x02\n\x15SitesHybridconnection\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x62iztalk_uri\x18\x04 \x01(\t\x12 \n\x18\x65ntity_connection_string\x18\x05 \x01(\t\x12\x13\n\x0b\x65ntity_name\x18\x06 \x01(\t\x12\x10\n\x08hostname\x18\x07 \x01(\t\x12\x0c\n\x04port\x18\x08 \x01(\x05\x12\"\n\x1aresource_connection_string\x18\t \x01(\t\x12\x15\n\rresource_type\x18\n \x01(\t\"\xb5\x02\n\x15SitesHostNameBindings\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1b\n\x13\x61zure_resource_name\x18\x04 \x01(\t\x12\x1b\n\x13\x61zure_resource_type\x18\x05 \x01(\t\x12(\n custom_host_name_dns_record_type\x18\x06 \x01(\t\x12\x11\n\tdomain_id\x18\x07 \x01(\t\x12\x16\n\x0ehost_name_type\x18\x08 \x01(\t\x12\x11\n\tsite_name\x18\t \x01(\t\x12\x11\n\tssl_state\x18\n \x01(\t\x12\x12\n\nthumbprint\x18\x0b \x01(\t\"j\n\x12SitesFunctionsKeys\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xa7\x05\n\x0eSitesFunctions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12K\n\x06\x63onfig\x18\x04 \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.SitesFunctions.ConfigEntry\x12\x13\n\x0b\x63onfig_href\x18\x05 \x01(\t\x12I\n\x05\x66iles\x18\x06 \x03(\x0b\x32:.oak9.tython.azure.microsoft_web.SitesFunctions.FilesEntry\x12\x17\n\x0f\x66unction_app_id\x18\x07 \x01(\t\x12\x0c\n\x04href\x18\x08 \x01(\t\x12\x1b\n\x13invoke_url_template\x18\t \x01(\t\x12\x13\n\x0bis_disabled\x18\n \x01(\x08\x12\x10\n\x08language\x18\x0b \x01(\t\x12\x13\n\x0bscript_href\x18\x0c \x01(\t\x12\x1d\n\x15script_root_path_href\x18\r \x01(\t\x12\x19\n\x11secrets_file_href\x18\x0e \x01(\t\x12\x11\n\ttest_data\x18\x0f \x01(\t\x12\x16\n\x0etest_data_href\x18\x10 \x01(\t\x12Q\n\x14sites_functions_keys\x18\x11 \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesFunctionsKeys\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a,\n\nFilesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"J\n\x0fSitesExtensions\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\x82\x01\n\x1fSitesDomainOwnershipIdentifiers\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\t\"\x87\x02\n\x10SitesDeployments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x0e\n\x06\x61uthor\x18\x05 \x01(\t\x12\x14\n\x0c\x61uthor_email\x18\x06 \x01(\t\x12\x10\n\x08\x64\x65ployer\x18\x07 \x01(\t\x12\x0f\n\x07\x64\x65tails\x18\x08 \x01(\t\x12\x10\n\x08\x65nd_time\x18\t \x01(\t\x12\x0f\n\x07message\x18\n \x01(\t\x12\x12\n\nstart_time\x18\x0b \x01(\t\x12\x0e\n\x06status\x18\x0c \x01(\x05\"\x94\x05\n\x0bSitesConfig\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x12\n\nftps_state\x18\x02 \x01(\t\x12\x19\n\x11health_check_path\x18\x03 \x01(\t\x12\x16\n\x0ehttp20_enabled\x18\x04 \x01(\t\x12\x1c\n\x14http_logging_enabled\x18\x05 \x01(\t\x12\x16\n\x0ejava_container\x18\x06 \x01(\t\x12\x1e\n\x16java_container_version\x18\x07 \x01(\t\x12\x14\n\x0cjava_version\x18\x08 \x01(\t\x12\x18\n\x10linux_fx_version\x18\t \x01(\t\x12\x16\n\x0eload_balancing\x18\n \x01(\t\x12!\n\x19logs_directory_size_limit\x18\x0b \x01(\t\x12\x1d\n\x15managed_pipeline_mode\x18\x0c \x01(\t\x12\x17\n\x0fmin_tls_version\x18\r \x01(\t\x12\x1d\n\x15net_framework_version\x18\x0e \x01(\t\x12\x14\n\x0cnode_version\x18\x0f \x01(\t\x12\x13\n\x0bphp_version\x18\x10 \x01(\t\x12\x1b\n\x13publishing_username\x18\x11 \x01(\t\x12\x16\n\x0epython_version\x18\x12 \x01(\t\x12 \n\x18remote_debugging_enabled\x18\x13 \x01(\t\x12 \n\x18remote_debugging_version\x18\x14 \x01(\t\x12-\n%scm_ip_security_restrictions_use_main\x18\x15 \x01(\t\x12\x1a\n\x12windows_fx_version\x18\x16 \x01(\t\"b\n\'SitesBasicPublishingCredentialsPolicies\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\xf9\x14\n\x05Sites\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12I\n\x08identity\x18\x03 \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.ManagedServiceIdentity\x12\x0c\n\x04kind\x18\x04 \x01(\t\x12\x10\n\x08location\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x1f\n\x17\x63lient_affinity_enabled\x18\x07 \x01(\x08\x12\x1b\n\x13\x63lient_cert_enabled\x18\x08 \x01(\x08\x12#\n\x1b\x63lient_cert_exclusion_paths\x18\t \x01(\t\x12\x18\n\x10\x63lient_cert_mode\x18\n \x01(\t\x12\x42\n\x0c\x63loning_info\x18\x0b \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.CloningInfo\x12\x16\n\x0e\x63ontainer_size\x18\x0c \x01(\x05\x12%\n\x1d\x63ustom_domain_verification_id\x18\r \x01(\t\x12\x1f\n\x17\x64\x61ily_memory_time_quota\x18\x0e \x01(\x05\x12\x0f\n\x07\x65nabled\x18\x0f \x01(\x08\x12_\n\x1bhosting_environment_profile\x18\x10 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.HostingEnvironmentProfile\x12\x1b\n\x13host_names_disabled\x18\x11 \x01(\x08\x12O\n\x14host_name_ssl_states\x18\x12 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.HostNameSslState\x12\x12\n\nhttps_only\x18\x13 \x01(\x08\x12\x0f\n\x07hyper_v\x18\x14 \x01(\x08\x12\x10\n\x08is_xenon\x18\x15 \x01(\x08\x12$\n\x1ckey_vault_reference_identity\x18\x16 \x01(\t\x12\x1d\n\x15public_network_access\x18\x17 \x01(\t\x12\x17\n\x0fredundancy_mode\x18\x18 \x01(\t\x12\x10\n\x08reserved\x18\x19 \x01(\x08\x12\x1d\n\x15scm_site_also_stopped\x18\x1a \x01(\x08\x12\x16\n\x0eserver_farm_id\x18\x1b \x01(\t\x12@\n\x0bsite_config\x18\x1c \x01(\x0b\x32+.oak9.tython.azure.microsoft_web.SiteConfig\x12 \n\x18storage_account_required\x18\x1d \x01(\x08\x12!\n\x19virtual_network_subnet_id\x18\x1e \x01(\t\x12\"\n\x1avnet_content_share_enabled\x18\x1f \x01(\x08\x12\x1f\n\x17vnet_image_pull_enabled\x18  \x01(\x08\x12\x1e\n\x16vnet_route_all_enabled\x18! \x01(\x08\x12>\n\x04tags\x18\" \x03(\x0b\x32\x30.oak9.tython.azure.microsoft_web.Sites.TagsEntry\x12}\n+sites_basic_publishing_credentials_policies\x18# \x03(\x0b\x32H.oak9.tython.azure.microsoft_web.SitesBasicPublishingCredentialsPolicies\x12l\n\"sites_domain_ownership_identifiers\x18$ \x03(\x0b\x32@.oak9.tython.azure.microsoft_web.SitesDomainOwnershipIdentifiers\x12J\n\x10sites_extensions\x18% \x03(\x0b\x32\x30.oak9.tython.azure.microsoft_web.SitesExtensions\x12H\n\x0fsites_functions\x18& \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.SitesFunctions\x12V\n\x16sites_hybridconnection\x18\' \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.SitesHybridconnection\x12\x44\n\rsites_migrate\x18( \x03(\x0b\x32-.oak9.tython.azure.microsoft_web.SitesMigrate\x12Q\n\x14sites_network_config\x18) \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesNetworkConfig\x12P\n\x13sites_premieraddons\x18* \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesPremieraddons\x12Q\n\x14sites_private_access\x18+ \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.SitesPrivateAccess\x12l\n\"sites_private_endpoint_connections\x18, \x03(\x0b\x32@.oak9.tython.azure.microsoft_web.SitesPrivateEndpointConnections\x12[\n\x19sites_public_certificates\x18- \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.SitesPublicCertificates\x12R\n\x14sites_siteextensions\x18. \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.SitesSiteextensions\x12@\n\x0bsites_slots\x18/ \x03(\x0b\x32+.oak9.tython.azure.microsoft_web.SitesSlots\x12R\n\x14sites_sourcecontrols\x18\x30 \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.SitesSourcecontrols\x12j\n!sites_virtual_network_connections\x18\x31 \x03(\x0b\x32?.oak9.tython.azure.microsoft_web.SitesVirtualNetworkConnections\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa1\x15\n\nSiteConfig\x12&\n\x1e\x61\x63r_use_managed_identity_creds\x18\x01 \x01(\x08\x12$\n\x1c\x61\x63r_user_managed_identity_id\x18\x02 \x01(\t\x12\x11\n\talways_on\x18\x03 \x01(\x08\x12J\n\x0e\x61pi_definition\x18\x04 \x01(\x0b\x32\x32.oak9.tython.azure.microsoft_web.ApiDefinitionInfo\x12S\n\x15\x61pi_management_config\x18\x05 \x01(\x0b\x32\x34.oak9.tython.azure.microsoft_web.ApiManagementConfig\x12\x18\n\x10\x61pp_command_line\x18\x06 \x01(\t\x12\x44\n\x0c\x61pp_settings\x18\x07 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.NameValuePair\x12\x19\n\x11\x61uto_heal_enabled\x18\x08 \x01(\x08\x12G\n\x0f\x61uto_heal_rules\x18\t \x01(\x0b\x32..oak9.tython.azure.microsoft_web.AutoHealRules\x12\x1b\n\x13\x61uto_swap_slot_name\x18\n \x01(\t\x12\x65\n\x16\x61zure_storage_accounts\x18\x0b \x03(\x0b\x32\x45.oak9.tython.azure.microsoft_web.SiteConfig.AzureStorageAccountsEntry\x12K\n\x12\x63onnection_strings\x18\x0c \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.ConnStringInfo\x12;\n\x04\x63ors\x18\r \x01(\x0b\x32-.oak9.tython.azure.microsoft_web.CorsSettings\x12\x19\n\x11\x64\x65\x66\x61ult_documents\x18\x0e \x03(\t\x12&\n\x1e\x64\x65tailed_error_logging_enabled\x18\x0f \x01(\x08\x12\x15\n\rdocument_root\x18\x10 \x01(\t\x12\x41\n\x0b\x65xperiments\x18\x11 \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.Experiments\x12\x12\n\nftps_state\x18\x12 \x01(\t\x12 \n\x18\x66unction_app_scale_limit\x18\x13 \x01(\x05\x12\x32\n*functions_runtime_scale_monitoring_enabled\x18\x14 \x01(\x08\x12I\n\x10handler_mappings\x18\x15 \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.HandlerMapping\x12\x19\n\x11health_check_path\x18\x16 \x01(\t\x12\x16\n\x0ehttp20_enabled\x18\x17 \x01(\x08\x12\x1c\n\x14http_logging_enabled\x18\x18 \x01(\x08\x12X\n\x18ip_security_restrictions\x18\x19 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.IpSecurityRestriction\x12\x16\n\x0ejava_container\x18\x1a \x01(\t\x12\x1e\n\x16java_container_version\x18\x1b \x01(\t\x12\x14\n\x0cjava_version\x18\x1c \x01(\t\x12$\n\x1ckey_vault_reference_identity\x18\x1d \x01(\t\x12;\n\x06limits\x18\x1e \x01(\x0b\x32+.oak9.tython.azure.microsoft_web.SiteLimits\x12\x18\n\x10linux_fx_version\x18\x1f \x01(\t\x12\x16\n\x0eload_balancing\x18  \x01(\t\x12\x1c\n\x14local_my_sql_enabled\x18! \x01(\x08\x12!\n\x19logs_directory_size_limit\x18\" \x01(\x05\x12\x1d\n\x15managed_pipeline_mode\x18# \x01(\t\x12#\n\x1bmanaged_service_identity_id\x18$ \x01(\x05\x12&\n\x1eminimum_elastic_instance_count\x18% \x01(\x05\x12\x17\n\x0fmin_tls_version\x18& \x01(\t\x12\x1d\n\x15net_framework_version\x18\' \x01(\t\x12\x14\n\x0cnode_version\x18( \x01(\t\x12\x19\n\x11number_of_workers\x18) \x01(\x05\x12\x13\n\x0bphp_version\x18* \x01(\t\x12\x1b\n\x13power_shell_version\x18+ \x01(\t\x12!\n\x19pre_warmed_instance_count\x18, \x01(\x05\x12\x1d\n\x15public_network_access\x18- \x01(\t\x12\x1b\n\x13publishing_username\x18. \x01(\t\x12;\n\x04push\x18/ \x01(\x0b\x32-.oak9.tython.azure.microsoft_web.PushSettings\x12\x16\n\x0epython_version\x18\x30 \x01(\t\x12 \n\x18remote_debugging_enabled\x18\x31 \x01(\x08\x12 \n\x18remote_debugging_version\x18\x32 \x01(\t\x12\x1f\n\x17request_tracing_enabled\x18\x33 \x01(\x08\x12\'\n\x1frequest_tracing_expiration_time\x18\x34 \x01(\t\x12\\\n\x1cscm_ip_security_restrictions\x18\x35 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.IpSecurityRestriction\x12-\n%scm_ip_security_restrictions_use_main\x18\x36 \x01(\x08\x12\x1b\n\x13scm_min_tls_version\x18\x37 \x01(\t\x12\x10\n\x08scm_type\x18\x38 \x01(\t\x12\x17\n\x0ftracing_options\x18\x39 \x01(\t\x12 \n\x18use32_bit_worker_process\x18: \x01(\x08\x12Q\n\x14virtual_applications\x18; \x03(\x0b\x32\x33.oak9.tython.azure.microsoft_web.VirtualApplication\x12\x11\n\tvnet_name\x18< \x01(\t\x12 \n\x18vnet_private_ports_count\x18= \x01(\x05\x12\x1e\n\x16vnet_route_all_enabled\x18> \x01(\x08\x12\x19\n\x11website_time_zone\x18? \x01(\t\x12\x1b\n\x13web_sockets_enabled\x18@ \x01(\x08\x12\x1a\n\x12windows_fx_version\x18\x41 \x01(\t\x12%\n\x1dx_managed_service_identity_id\x18\x42 \x01(\x05\x1a;\n\x19\x41zureStorageAccountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x12VirtualApplication\x12\x15\n\rphysical_path\x18\x01 \x01(\t\x12\x17\n\x0fpreload_enabled\x18\x02 \x01(\x08\x12N\n\x13virtual_directories\x18\x03 \x03(\x0b\x32\x31.oak9.tython.azure.microsoft_web.VirtualDirectory\x12\x14\n\x0cvirtual_path\x18\x04 \x01(\t\"?\n\x10VirtualDirectory\x12\x15\n\rphysical_path\x18\x01 \x01(\t\x12\x14\n\x0cvirtual_path\x18\x02 \x01(\t\"\x89\x01\n\x0cPushSettings\x12\x0c\n\x04kind\x18\x01 \x01(\t\x12\x19\n\x11\x64ynamic_tags_json\x18\x02 \x01(\t\x12\x17\n\x0fis_push_enabled\x18\x03 \x01(\x08\x12\x1b\n\x13tags_requiring_auth\x18\x04 \x01(\t\x12\x1a\n\x12tag_whitelist_json\x18\x05 \x01(\t\"_\n\nSiteLimits\x12\x1b\n\x13max_disk_size_in_mb\x18\x01 \x01(\x05\x12\x18\n\x10max_memory_in_mb\x18\x02 \x01(\x05\x12\x1a\n\x12max_percentage_cpu\x18\x03 \x01(\x01\"\xef\x02\n\x15IpSecurityRestriction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12T\n\x07headers\x18\x03 \x03(\x0b\x32\x43.oak9.tython.azure.microsoft_web.IpSecurityRestriction.HeadersEntry\x12\x12\n\nip_address\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\x05\x12\x13\n\x0bsubnet_mask\x18\x07 \x01(\t\x12\x1a\n\x12subnet_traffic_tag\x18\x08 \x01(\x05\x12\x0b\n\x03tag\x18\t \x01(\t\x12\x1f\n\x17vnet_subnet_resource_id\x18\n \x01(\t\x12\x18\n\x10vnet_traffic_tag\x18\x0b \x01(\x05\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"P\n\x0eHandlerMapping\x12\x11\n\targuments\x18\x01 \x01(\t\x12\x11\n\textension\x18\x02 \x01(\t\x12\x18\n\x10script_processor\x18\x03 \x01(\t\"Q\n\x0b\x45xperiments\x12\x42\n\rramp_up_rules\x18\x01 \x03(\x0b\x32+.oak9.tython.azure.microsoft_web.RampUpRule\"\xef\x01\n\nRampUpRule\x12\x18\n\x10\x61\x63tion_host_name\x18\x01 \x01(\t\x12$\n\x1c\x63hange_decision_callback_url\x18\x02 \x01(\t\x12\"\n\x1a\x63hange_interval_in_minutes\x18\x03 \x01(\x05\x12\x13\n\x0b\x63hange_step\x18\x04 \x01(\x01\x12\x1e\n\x16max_reroute_percentage\x18\x05 \x01(\x01\x12\x1e\n\x16min_reroute_percentage\x18\x06 \x01(\x01\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x1a\n\x12reroute_percentage\x18\x08 \x01(\x01\"D\n\x0c\x43orsSettings\x12\x17\n\x0f\x61llowed_origins\x18\x01 \x03(\t\x12\x1b\n\x13support_credentials\x18\x02 \x01(\x08\"G\n\x0e\x43onnStringInfo\x12\x19\n\x11\x63onnection_string\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\"\x97\x01\n\rAutoHealRules\x12\x41\n\x07\x61\x63tions\x18\x01 \x01(\x0b\x32\x30.oak9.tython.azure.microsoft_web.AutoHealActions\x12\x43\n\x08triggers\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.AutoHealTriggers\"\xd1\x03\n\x10\x41utoHealTriggers\x12\x1b\n\x13private_bytes_in_kb\x18\x01 \x01(\x05\x12G\n\x08requests\x18\x02 \x01(\x0b\x32\x35.oak9.tython.azure.microsoft_web.RequestsBasedTrigger\x12P\n\rslow_requests\x18\x03 \x01(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SlowRequestsBasedTrigger\x12Z\n\x17slow_requests_with_path\x18\x04 \x03(\x0b\x32\x39.oak9.tython.azure.microsoft_web.SlowRequestsBasedTrigger\x12N\n\x0cstatus_codes\x18\x05 \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.StatusCodesBasedTrigger\x12Y\n\x12status_codes_range\x18\x06 \x03(\x0b\x32=.oak9.tython.azure.microsoft_web.StatusCodesRangeBasedTrigger\"h\n\x1cStatusCodesRangeBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x14\n\x0cstatus_codes\x18\x03 \x01(\t\x12\x15\n\rtime_interval\x18\x04 \x01(\t\"\x87\x01\n\x17StatusCodesBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\x05\x12\x12\n\nsub_status\x18\x04 \x01(\x05\x12\x15\n\rtime_interval\x18\x05 \x01(\t\x12\x14\n\x0cwin32_status\x18\x06 \x01(\x05\"b\n\x18SlowRequestsBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x15\n\rtime_interval\x18\x03 \x01(\t\x12\x12\n\ntime_taken\x18\x04 \x01(\t\"<\n\x14RequestsBasedTrigger\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x15\n\rtime_interval\x18\x02 \x01(\t\"\x98\x01\n\x0f\x41utoHealActions\x12\x13\n\x0b\x61\x63tion_type\x18\x01 \x01(\t\x12L\n\rcustom_action\x18\x02 \x01(\x0b\x32\x35.oak9.tython.azure.microsoft_web.AutoHealCustomAction\x12\"\n\x1amin_process_execution_time\x18\x03 \x01(\t\"7\n\x14\x41utoHealCustomAction\x12\x0b\n\x03\x65xe\x18\x01 \x01(\t\x12\x12\n\nparameters\x18\x02 \x01(\t\"!\n\x13\x41piManagementConfig\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x11\x41piDefinitionInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x81\x01\n\x10HostNameSslState\x12\x11\n\thost_type\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tssl_state\x18\x03 \x01(\t\x12\x12\n\nthumbprint\x18\x04 \x01(\t\x12\x11\n\tto_update\x18\x05 \x01(\x08\x12\x12\n\nvirtual_ip\x18\x06 \x01(\t\"\xe1\x03\n\x0b\x43loningInfo\x12\x66\n\x16\x61pp_settings_overrides\x18\x01 \x03(\x0b\x32\x46.oak9.tython.azure.microsoft_web.CloningInfo.AppSettingsOverridesEntry\x12\x1f\n\x17\x63lone_custom_host_names\x18\x02 \x01(\x08\x12\x1c\n\x14\x63lone_source_control\x18\x03 \x01(\x08\x12 \n\x18\x63onfigure_load_balancing\x18\x04 \x01(\x08\x12\x16\n\x0e\x63orrelation_id\x18\x05 \x01(\t\x12\x1b\n\x13hosting_environment\x18\x06 \x01(\t\x12\x11\n\toverwrite\x18\x07 \x01(\x08\x12\x19\n\x11source_web_app_id\x18\x08 \x01(\t\x12\x1f\n\x17source_web_app_location\x18\t \x01(\t\x12\"\n\x1atraffic_manager_profile_id\x18\n \x01(\t\x12$\n\x1ctraffic_manager_profile_name\x18\x0b \x01(\t\x1a;\n\x19\x41ppSettingsOverridesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xdc\x01\n\x16ManagedServiceIdentity\x12\x0c\n\x04type\x18\x01 \x01(\t\x12u\n\x18user_assigned_identities\x18\x02 \x03(\x0b\x32S.oak9.tython.azure.microsoft_web.ManagedServiceIdentity.UserAssignedIdentitiesEntry\x1a=\n\x1bUserAssignedIdentitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc1\x01\n*ServerfarmsVirtualNetworkConnectionsRoutes\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x65nd_address\x18\x04 \x01(\t\x12\x12\n\nroute_type\x18\x05 \x01(\t\x12\x15\n\rstart_address\x18\x06 \x01(\t\"\xaf\x01\n,ServerfarmsVirtualNetworkConnectionsGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x11\n\tvnet_name\x18\x04 \x01(\t\x12\x17\n\x0fvpn_package_uri\x18\x05 \x01(\t\"\x84\x07\n\x0bServerfarms\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1d\n\x15\x65lastic_scale_enabled\x18\x06 \x01(\x08\x12\"\n\x1a\x66ree_offer_expiration_time\x18\x07 \x01(\t\x12_\n\x1bhosting_environment_profile\x18\x08 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.HostingEnvironmentProfile\x12\x0f\n\x07hyper_v\x18\t \x01(\x08\x12\x0f\n\x07is_spot\x18\n \x01(\x08\x12\x10\n\x08is_xenon\x18\x0b \x01(\x08\x12Y\n\x18kube_environment_profile\x18\x0c \x01(\x0b\x32\x37.oak9.tython.azure.microsoft_web.KubeEnvironmentProfile\x12$\n\x1cmaximum_elastic_worker_count\x18\r \x01(\x05\x12\x18\n\x10per_site_scaling\x18\x0e \x01(\x08\x12\x10\n\x08reserved\x18\x0f \x01(\x08\x12\x1c\n\x14spot_expiration_time\x18\x10 \x01(\t\x12\x1b\n\x13target_worker_count\x18\x11 \x01(\x05\x12\x1d\n\x15target_worker_size_id\x18\x12 \x01(\x05\x12\x18\n\x10worker_tier_name\x18\x13 \x01(\t\x12\x16\n\x0ezone_redundant\x18\x14 \x01(\x08\x12<\n\x03sku\x18\x15 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\x12\x44\n\x04tags\x18\x16 \x03(\x0b\x32\x36.oak9.tython.azure.microsoft_web.Serverfarms.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"$\n\x16KubeEnvironmentProfile\x12\n\n\x02id\x18\x01 \x01(\t\"\'\n\x19HostingEnvironmentProfile\x12\n\n\x02id\x18\x01 \x01(\t\"\xb5\x05\n\x10KubeEnvironments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12L\n\x11\x65xtended_location\x18\x02 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ExtendedLocation\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x17\n\x0f\x61ks_resource_id\x18\x06 \x01(\t\x12U\n\x16\x61pp_logs_configuration\x18\x07 \x01(\x0b\x32\x35.oak9.tython.azure.microsoft_web.AppLogsConfiguration\x12L\n\x11\x61rc_configuration\x18\x08 \x01(\x0b\x32\x31.oak9.tython.azure.microsoft_web.ArcConfiguration\x12\x61\n\x1c\x63ontainer_apps_configuration\x18\t \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.ContainerAppsConfiguration\x12\x18\n\x10\x65nvironment_type\x18\n \x01(\t\x12&\n\x1einternal_load_balancer_enabled\x18\x0b \x01(\x08\x12\x11\n\tstatic_ip\x18\x0c \x01(\t\x12I\n\x04tags\x18\r \x03(\x0b\x32;.oak9.tython.azure.microsoft_web.KubeEnvironments.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xea\x01\n\x1a\x43ontainerAppsConfiguration\x12\x1e\n\x16\x61pp_subnet_resource_id\x18\x01 \x01(\t\x12(\n control_plane_subnet_resource_id\x18\x02 \x01(\t\x12$\n\x1c\x64\x61pr_a_i_instrumentation_key\x18\x03 \x01(\t\x12\x1a\n\x12\x64ocker_bridge_cidr\x18\x04 \x01(\t\x12\x1e\n\x16platform_reserved_cidr\x18\x05 \x01(\t\x12 \n\x18platform_reserved_dns_ip\x18\x06 \x01(\t\"\xbc\x02\n\x10\x41rcConfiguration\x12\x1e\n\x16\x61rtifacts_storage_type\x18\x01 \x01(\t\x12$\n\x1c\x61rtifact_storage_access_mode\x18\x02 \x01(\t\x12#\n\x1b\x61rtifact_storage_class_name\x18\x03 \x01(\t\x12#\n\x1b\x61rtifact_storage_mount_path\x18\x04 \x01(\t\x12\"\n\x1a\x61rtifact_storage_node_name\x18\x05 \x01(\t\x12_\n\x1f\x66ront_end_service_configuration\x18\x06 \x01(\x0b\x32\x36.oak9.tython.azure.microsoft_web.FrontEndConfiguration\x12\x13\n\x0bkube_config\x18\x07 \x01(\t\"%\n\x15\x46rontEndConfiguration\x12\x0c\n\x04kind\x18\x01 \x01(\t\"\x8c\x01\n\x14\x41ppLogsConfiguration\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12_\n\x1blog_analytics_configuration\x18\x02 \x01(\x0b\x32:.oak9.tython.azure.microsoft_web.LogAnalyticsConfiguration\"D\n\x19LogAnalyticsConfiguration\x12\x13\n\x0b\x63ustomer_id\x18\x01 \x01(\t\x12\x12\n\nshared_key\x18\x02 \x01(\t\" \n\x10\x45xtendedLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x8c\x02\n\x1eHostingEnvironmentsWorkerPools\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ompute_mode\x18\x04 \x01(\t\x12\x14\n\x0cworker_count\x18\x05 \x01(\x05\x12\x13\n\x0bworker_size\x18\x06 \x01(\t\x12\x16\n\x0eworker_size_id\x18\x07 \x01(\x05\x12<\n\x03sku\x18\x08 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\"\xf0\x01\n-HostingEnvironmentsPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12j\n%private_link_service_connection_state\x18\x04 \x01(\x0b\x32;.oak9.tython.azure.microsoft_web.PrivateLinkConnectionState\"[\n\x1aPrivateLinkConnectionState\x12\x18\n\x10\x61\x63tions_required\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\"\x8f\x02\n!HostingEnvironmentsMultiRolePools\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ompute_mode\x18\x04 \x01(\t\x12\x14\n\x0cworker_count\x18\x05 \x01(\x05\x12\x13\n\x0bworker_size\x18\x06 \x01(\t\x12\x16\n\x0eworker_size_id\x18\x07 \x01(\x05\x12<\n\x03sku\x18\x08 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.SkuDescription\"\xf6\x01\n\x0eSkuDescription\x12\x41\n\x0c\x63\x61pabilities\x18\x01 \x03(\x0b\x32+.oak9.tython.azure.microsoft_web.Capability\x12\x10\n\x08\x63\x61pacity\x18\x02 \x01(\x05\x12\x0e\n\x06\x66\x61mily\x18\x03 \x01(\t\x12\x11\n\tlocations\x18\x04 \x03(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x0c\n\x04size\x18\x06 \x01(\t\x12\x42\n\x0csku_capacity\x18\x07 \x01(\x0b\x32,.oak9.tython.azure.microsoft_web.SkuCapacity\x12\x0c\n\x04tier\x18\x08 \x01(\t\"m\n\x0bSkuCapacity\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x01 \x01(\x05\x12\x17\n\x0f\x65lastic_maximum\x18\x02 \x01(\x05\x12\x0f\n\x07maximum\x18\x03 \x01(\x05\x12\x0f\n\x07minimum\x18\x04 \x01(\x05\x12\x12\n\nscale_type\x18\x05 \x01(\t\"9\n\nCapability\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\\\n!HostingEnvironmentsConfigurations\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\"\xb8\n\n\x13HostingEnvironments\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12H\n\x10\x63luster_settings\x18\x05 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.NameValuePair\x12\x66\n\x1f\x63ustom_dns_suffix_configuration\x18\x06 \x01(\x0b\x32=.oak9.tython.azure.microsoft_web.CustomDnsSuffixConfiguration\x12\x1c\n\x14\x64\x65\x64icated_host_count\x18\x07 \x01(\x05\x12\x12\n\ndns_suffix\x18\x08 \x01(\t\x12\x1e\n\x16\x66ront_end_scale_factor\x18\t \x01(\x05\x12$\n\x1cinternal_load_balancing_mode\x18\n \x01(\t\x12\x1b\n\x13ipssl_address_count\x18\x0b \x01(\x05\x12\x12\n\nmulti_size\x18\x0c \x01(\t\x12_\n\x18networking_configuration\x18\r \x01(\x0b\x32=.oak9.tython.azure.microsoft_web.AseV3NetworkingConfiguration\x12\x1a\n\x12upgrade_preference\x18\x0e \x01(\t\x12\"\n\x1auser_whitelisted_ip_ranges\x18\x0f \x03(\t\x12O\n\x0fvirtual_network\x18\x10 \x01(\x0b\x32\x36.oak9.tython.azure.microsoft_web.VirtualNetworkProfile\x12\x16\n\x0ezone_redundant\x18\x11 \x01(\x08\x12L\n\x04tags\x18\x12 \x03(\x0b\x32>.oak9.tython.azure.microsoft_web.HostingEnvironments.TagsEntry\x12o\n#hosting_environments_configurations\x18\x13 \x03(\x0b\x32\x42.oak9.tython.azure.microsoft_web.HostingEnvironmentsConfigurations\x12q\n%hosting_environments_multi_role_pools\x18\x14 \x03(\x0b\x32\x42.oak9.tython.azure.microsoft_web.HostingEnvironmentsMultiRolePools\x12\x89\x01\n1hosting_environments_private_endpoint_connections\x18\x15 \x03(\x0b\x32N.oak9.tython.azure.microsoft_web.HostingEnvironmentsPrivateEndpointConnections\x12j\n!hosting_environments_worker_pools\x18\x16 \x03(\x0b\x32?.oak9.tython.azure.microsoft_web.HostingEnvironmentsWorkerPools\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"3\n\x15VirtualNetworkProfile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06subnet\x18\x02 \x01(\t\"\xb4\x01\n\x1c\x41seV3NetworkingConfiguration\x12\x0c\n\x04kind\x18\x01 \x01(\t\x12.\n&allow_new_private_endpoint_connections\x18\x02 \x01(\x08\x12\x13\n\x0b\x66tp_enabled\x18\x03 \x01(\x08\x12#\n\x1binbound_ip_address_override\x18\x04 \x01(\t\x12\x1c\n\x14remote_debug_enabled\x18\x05 \x01(\x08\"\x7f\n\x1c\x43ustomDnsSuffixConfiguration\x12\x0c\n\x04kind\x18\x01 \x01(\t\x12\x17\n\x0f\x63\x65rtificate_url\x18\x02 \x01(\t\x12\x12\n\ndns_suffix\x18\x03 \x01(\t\x12$\n\x1ckey_vault_reference_identity\x18\x04 \x01(\t\",\n\rNameValuePair\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x8c\x03\n\rContainerApps\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x45\n\rconfiguration\x18\x05 \x01(\x0b\x32..oak9.tython.azure.microsoft_web.Configuration\x12\x1b\n\x13kube_environment_id\x18\x06 \x01(\t\x12;\n\x08template\x18\x07 \x01(\x0b\x32).oak9.tython.azure.microsoft_web.Template\x12\x46\n\x04tags\x18\x08 \x03(\x0b\x32\x38.oak9.tython.azure.microsoft_web.ContainerApps.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xcf\x01\n\x08Template\x12>\n\ncontainers\x18\x01 \x03(\x0b\x32*.oak9.tython.azure.microsoft_web.Container\x12\x33\n\x04\x64\x61pr\x18\x02 \x01(\x0b\x32%.oak9.tython.azure.microsoft_web.Dapr\x12\x17\n\x0frevision_suffix\x18\x03 \x01(\t\x12\x35\n\x05scale\x18\x04 \x01(\x0b\x32&.oak9.tython.azure.microsoft_web.Scale\"n\n\x05Scale\x12\x14\n\x0cmax_replicas\x18\x01 \x01(\x05\x12\x14\n\x0cmin_replicas\x18\x02 \x01(\x05\x12\x39\n\x05rules\x18\x03 \x03(\x0b\x32*.oak9.tython.azure.microsoft_web.ScaleRule\"\xdf\x01\n\tScaleRule\x12\x44\n\x0b\x61zure_queue\x18\x01 \x01(\x0b\x32/.oak9.tython.azure.microsoft_web.QueueScaleRule\x12@\n\x06\x63ustom\x18\x02 \x01(\x0b\x32\x30.oak9.tython.azure.microsoft_web.CustomScaleRule\x12<\n\x04http\x18\x03 \x01(\x0b\x32..oak9.tython.azure.microsoft_web.HttpScaleRule\x12\x0c\n\x04name\x18\x04 \x01(\t\"\xce\x01\n\rHttpScaleRule\x12<\n\x04\x61uth\x18\x01 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.ScaleRuleAuth\x12N\n\x08metadata\x18\x02 \x03(\x0b\x32<.oak9.tython.azure.microsoft_web.HttpScaleRule.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe0\x01\n\x0f\x43ustomScaleRule\x12<\n\x04\x61uth\x18\x01 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.ScaleRuleAuth\x12P\n\x08metadata\x18\x02 \x03(\x0b\x32>.oak9.tython.azure.microsoft_web.CustomScaleRule.MetadataEntry\x12\x0c\n\x04type\x18\x03 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"x\n\x0eQueueScaleRule\x12<\n\x04\x61uth\x18\x01 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.ScaleRuleAuth\x12\x14\n\x0cqueue_length\x18\x02 \x01(\x05\x12\x12\n\nqueue_name\x18\x03 \x01(\t\">\n\rScaleRuleAuth\x12\x12\n\nsecret_ref\x18\x01 \x01(\t\x12\x19\n\x11trigger_parameter\x18\x02 \x01(\t\"}\n\x04\x44\x61pr\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x10\n\x08\x61pp_port\x18\x02 \x01(\x05\x12\x42\n\ncomponents\x18\x03 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.DaprComponent\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\"}\n\rDaprComponent\x12?\n\x08metadata\x18\x01 \x03(\x0b\x32-.oak9.tython.azure.microsoft_web.DaprMetadata\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"?\n\x0c\x44\x61prMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsecret_ref\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x85\x01\n\tContainer\x12\x0c\n\x04\x61rgs\x18\x01 \x03(\t\x12\x0f\n\x07\x63ommand\x18\x02 \x03(\t\x12<\n\x03\x65nv\x18\x03 \x03(\x0b\x32/.oak9.tython.azure.microsoft_web.EnvironmentVar\x12\r\n\x05image\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\"A\n\x0e\x45nvironmentVar\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsecret_ref\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xed\x01\n\rConfiguration\x12\x1d\n\x15\x61\x63tive_revisions_mode\x18\x01 \x01(\t\x12\x39\n\x07ingress\x18\x02 \x01(\x0b\x32(.oak9.tython.azure.microsoft_web.Ingress\x12H\n\nregistries\x18\x03 \x03(\x0b\x32\x34.oak9.tython.azure.microsoft_web.RegistryCredentials\x12\x38\n\x07secrets\x18\x04 \x03(\x0b\x32\'.oak9.tython.azure.microsoft_web.Secret\"%\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"T\n\x13RegistryCredentials\x12\x1b\n\x13password_secret_ref\x18\x01 \x01(\t\x12\x0e\n\x06server\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\"\x9c\x01\n\x07Ingress\x12\x16\n\x0e\x61llow_insecure\x18\x01 \x01(\x08\x12\x10\n\x08\x65xternal\x18\x02 \x01(\x08\x12\x13\n\x0btarget_port\x18\x03 \x01(\x05\x12?\n\x07traffic\x18\x04 \x03(\x0b\x32..oak9.tython.azure.microsoft_web.TrafficWeight\x12\x11\n\ttransport\x18\x05 \x01(\t\"O\n\rTrafficWeight\x12\x17\n\x0flatest_revision\x18\x01 \x01(\x08\x12\x15\n\rrevision_name\x18\x02 \x01(\t\x12\x0e\n\x06weight\x18\x03 \x01(\x05\"\xa8\x03\n\x0c\x43\x65rtificates\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04kind\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x16\n\x0e\x63\x61nonical_name\x18\x05 \x01(\t\x12 \n\x18\x64omain_validation_method\x18\x06 \x01(\t\x12\x12\n\nhost_names\x18\x07 \x03(\t\x12\x14\n\x0ckey_vault_id\x18\x08 \x01(\t\x12\x1d\n\x15key_vault_secret_name\x18\t \x01(\t\x12\x10\n\x08password\x18\n \x01(\t\x12\x10\n\x08pfx_blob\x18\x0b \x01(\t\x12\x16\n\x0eserver_farm_id\x18\x0c \x01(\t\x12\x45\n\x04tags\x18\r \x03(\x0b\x32\x37.oak9.tython.azure.microsoft_web.Certificates.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'azure.azure_microsoft_web_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _STATICSITES_TAGSENTRY._options = None
@@ -39,16 +39,14 @@
   _SITESPREMIERADDONS_TAGSENTRY._serialized_options = b'8\001'
   _SITESINSTANCESEXTENSIONS_SETPARAMETERSENTRY._options = None
   _SITESINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_options = b'8\001'
   _SITESFUNCTIONS_CONFIGENTRY._options = None
   _SITESFUNCTIONS_CONFIGENTRY._serialized_options = b'8\001'
   _SITESFUNCTIONS_FILESENTRY._options = None
   _SITESFUNCTIONS_FILESENTRY._serialized_options = b'8\001'
-  _SITESEXTENSIONS_SETPARAMETERSENTRY._options = None
-  _SITESEXTENSIONS_SETPARAMETERSENTRY._serialized_options = b'8\001'
   _SITES_TAGSENTRY._options = None
   _SITES_TAGSENTRY._serialized_options = b'8\001'
   _SITECONFIG_AZURESTORAGEACCOUNTSENTRY._options = None
   _SITECONFIG_AZURESTORAGEACCOUNTSENTRY._serialized_options = b'8\001'
   _IPSECURITYRESTRICTION_HEADERSENTRY._options = None
   _IPSECURITYRESTRICTION_HEADERSENTRY._serialized_options = b'8\001'
   _CLONINGINFO_APPSETTINGSOVERRIDESENTRY._options = None
@@ -66,303 +64,309 @@
   _HTTPSCALERULE_METADATAENTRY._options = None
   _HTTPSCALERULE_METADATAENTRY._serialized_options = b'8\001'
   _CUSTOMSCALERULE_METADATAENTRY._options = None
   _CUSTOMSCALERULE_METADATAENTRY._serialized_options = b'8\001'
   _CERTIFICATES_TAGSENTRY._options = None
   _CERTIFICATES_TAGSENTRY._serialized_options = b'8\001'
   _MICROSOFT_WEB._serialized_start=90
-  _MICROSOFT_WEB._serialized_end=819
-  _STATICSITESUSERPROVIDEDFUNCTIONAPPS._serialized_start=822
-  _STATICSITESUSERPROVIDEDFUNCTIONAPPS._serialized_end=1007
-  _STATICSITESPRIVATEENDPOINTCONNECTIONS._serialized_start=1010
-  _STATICSITESPRIVATEENDPOINTCONNECTIONS._serialized_end=1242
-  _STATICSITESCUSTOMDOMAINS._serialized_start=1245
-  _STATICSITESCUSTOMDOMAINS._serialized_end=1383
-  _STATICSITESCONFIG._serialized_start=1385
-  _STATICSITESCONFIG._serialized_end=1461
-  _STATICSITESBUILDSUSERPROVIDEDFUNCTIONAPPS._serialized_start=1464
-  _STATICSITESBUILDSUSERPROVIDEDFUNCTIONAPPS._serialized_end=1655
-  _STATICSITESBUILDSCONFIG._serialized_start=1657
-  _STATICSITESBUILDSCONFIG._serialized_end=1739
-  _STATICSITES._serialized_start=1742
-  _STATICSITES._serialized_end=2897
-  _STATICSITES_TAGSENTRY._serialized_start=2854
-  _STATICSITES_TAGSENTRY._serialized_end=2897
-  _STATICSITETEMPLATEOPTIONS._serialized_start=2900
-  _STATICSITETEMPLATEOPTIONS._serialized_end=3041
-  _STATICSITEBUILDPROPERTIES._serialized_start=3044
-  _STATICSITEBUILDPROPERTIES._serialized_end=3317
-  _SITESVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_start=3320
-  _SITESVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_end=3489
-  _SITESVIRTUALNETWORKCONNECTIONS._serialized_start=3492
-  _SITESVIRTUALNETWORKCONNECTIONS._serialized_end=3818
-  _SITESSOURCECONTROLS._serialized_start=3821
-  _SITESSOURCECONTROLS._serialized_end=4176
-  _SITESSLOTSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_start=4179
-  _SITESSLOTSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_end=4353
-  _SITESSLOTSVIRTUALNETWORKCONNECTIONS._serialized_start=4356
-  _SITESSLOTSVIRTUALNETWORKCONNECTIONS._serialized_end=4699
-  _SITESSLOTSSOURCECONTROLS._serialized_start=4702
-  _SITESSLOTSSOURCECONTROLS._serialized_end=5062
-  _GITHUBACTIONCONFIGURATION._serialized_start=5065
-  _GITHUBACTIONCONFIGURATION._serialized_end=5336
-  _GITHUBACTIONCONTAINERCONFIGURATION._serialized_start=5338
-  _GITHUBACTIONCONTAINERCONFIGURATION._serialized_end=5450
-  _GITHUBACTIONCODECONFIGURATION._serialized_start=5452
-  _GITHUBACTIONCODECONFIGURATION._serialized_end=5531
-  _SITESSLOTSSITEEXTENSIONS._serialized_start=5533
-  _SITESSLOTSSITEEXTENSIONS._serialized_end=5630
-  _SITESSLOTSPUBLICCERTIFICATES._serialized_start=5633
-  _SITESSLOTSPUBLICCERTIFICATES._serialized_end=5799
-  _SITESSLOTSPRIVATEENDPOINTCONNECTIONS._serialized_start=5802
-  _SITESSLOTSPRIVATEENDPOINTCONNECTIONS._serialized_end=6033
-  _SITESSLOTSPRIVATEACCESS._serialized_start=6036
-  _SITESSLOTSPRIVATEACCESS._serialized_end=6251
-  _SITESSLOTSPREMIERADDONS._serialized_start=6254
-  _SITESSLOTSPREMIERADDONS._serialized_end=6613
-  _SITESSLOTSPREMIERADDONS_TAGSENTRY._serialized_start=2854
-  _SITESSLOTSPREMIERADDONS_TAGSENTRY._serialized_end=2897
-  _SITESSLOTSNETWORKCONFIG._serialized_start=6616
-  _SITESSLOTSNETWORKCONFIG._serialized_end=6779
-  _SITESSLOTSINSTANCESEXTENSIONS._serialized_start=6782
-  _SITESSLOTSINSTANCESEXTENSIONS._serialized_end=7205
-  _SITESSLOTSINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_start=7153
-  _SITESSLOTSINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_end=7205
-  _SITESSLOTSHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_start=7208
-  _SITESSLOTSHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_end=7518
-  _SITESSLOTSHYBRIDCONNECTION._serialized_start=7521
-  _SITESSLOTSHYBRIDCONNECTION._serialized_end=7801
-  _SITESSLOTSHOSTNAMEBINDINGS._serialized_start=7804
-  _SITESSLOTSHOSTNAMEBINDINGS._serialized_end=8118
-  _SITESSLOTSFUNCTIONSKEYS._serialized_start=8120
-  _SITESSLOTSFUNCTIONSKEYS._serialized_end=8231
-  _SITESSLOTSFUNCTIONS._serialized_start=8234
-  _SITESSLOTSFUNCTIONS._serialized_end=8939
-  _SITESSLOTSFUNCTIONS_CONFIGENTRY._serialized_start=8848
-  _SITESSLOTSFUNCTIONS_CONFIGENTRY._serialized_end=8893
-  _SITESSLOTSFUNCTIONS_FILESENTRY._serialized_start=8895
-  _SITESSLOTSFUNCTIONS_FILESENTRY._serialized_end=8939
-  _SITESSLOTSEXTENSIONS._serialized_start=8942
-  _SITESSLOTSEXTENSIONS._serialized_end=9347
-  _SITESSLOTSEXTENSIONS_SETPARAMETERSENTRY._serialized_start=7153
-  _SITESSLOTSEXTENSIONS_SETPARAMETERSENTRY._serialized_end=7205
-  _SITESSLOTSDOMAINOWNERSHIPIDENTIFIERS._serialized_start=9350
-  _SITESSLOTSDOMAINOWNERSHIPIDENTIFIERS._serialized_end=9485
-  _SITESSLOTSDEPLOYMENTS._serialized_start=9488
-  _SITESSLOTSDEPLOYMENTS._serialized_end=9756
-  _SITESSLOTSCONFIG._serialized_start=9758
-  _SITESSLOTSCONFIG._serialized_end=9833
-  _SITESSLOTSBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_start=9835
-  _SITESSLOTSBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_end=9938
-  _SITESSLOTS._serialized_start=9941
-  _SITESSLOTS._serialized_end=12777
-  _SITESSLOTS_TAGSENTRY._serialized_start=2854
-  _SITESSLOTS_TAGSENTRY._serialized_end=2897
-  _SITESSITEEXTENSIONS._serialized_start=12779
-  _SITESSITEEXTENSIONS._serialized_end=12871
-  _SITESPUBLICCERTIFICATES._serialized_start=12874
-  _SITESPUBLICCERTIFICATES._serialized_end=13035
-  _SITESPRIVATEENDPOINTCONNECTIONS._serialized_start=13038
-  _SITESPRIVATEENDPOINTCONNECTIONS._serialized_end=13264
-  _SITESPRIVATEACCESS._serialized_start=13267
-  _SITESPRIVATEACCESS._serialized_end=13477
-  _PRIVATEACCESSVIRTUALNETWORK._serialized_start=13480
-  _PRIVATEACCESSVIRTUALNETWORK._serialized_end=13628
-  _PRIVATEACCESSSUBNET._serialized_start=13630
-  _PRIVATEACCESSSUBNET._serialized_end=13678
-  _SITESPREMIERADDONS._serialized_start=13681
-  _SITESPREMIERADDONS._serialized_end=14030
-  _SITESPREMIERADDONS_TAGSENTRY._serialized_start=2854
-  _SITESPREMIERADDONS_TAGSENTRY._serialized_end=2897
-  _SITESNETWORKCONFIG._serialized_start=14033
-  _SITESNETWORKCONFIG._serialized_end=14191
-  _SITESMIGRATE._serialized_start=14194
-  _SITESMIGRATE._serialized_end=14430
-  _SITESINSTANCESEXTENSIONS._serialized_start=14433
-  _SITESINSTANCESEXTENSIONS._serialized_end=14846
-  _SITESINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_start=7153
-  _SITESINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_end=7205
-  _SITESHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_start=14849
-  _SITESHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_end=15154
-  _SITESHYBRIDCONNECTION._serialized_start=15157
-  _SITESHYBRIDCONNECTION._serialized_end=15432
-  _SITESHOSTNAMEBINDINGS._serialized_start=15435
-  _SITESHOSTNAMEBINDINGS._serialized_end=15744
-  _SITESFUNCTIONSKEYS._serialized_start=15746
-  _SITESFUNCTIONSKEYS._serialized_end=15852
-  _SITESFUNCTIONS._serialized_start=15855
-  _SITESFUNCTIONS._serialized_end=16534
-  _SITESFUNCTIONS_CONFIGENTRY._serialized_start=8848
-  _SITESFUNCTIONS_CONFIGENTRY._serialized_end=8893
-  _SITESFUNCTIONS_FILESENTRY._serialized_start=8895
-  _SITESFUNCTIONS_FILESENTRY._serialized_end=8939
-  _SITESEXTENSIONS._serialized_start=16537
-  _SITESEXTENSIONS._serialized_end=16932
-  _SITESEXTENSIONS_SETPARAMETERSENTRY._serialized_start=7153
-  _SITESEXTENSIONS_SETPARAMETERSENTRY._serialized_end=7205
-  _SITESDOMAINOWNERSHIPIDENTIFIERS._serialized_start=16935
-  _SITESDOMAINOWNERSHIPIDENTIFIERS._serialized_end=17065
-  _SITESDEPLOYMENTS._serialized_start=17068
-  _SITESDEPLOYMENTS._serialized_end=17331
-  _SITESCONFIG._serialized_start=17334
-  _SITESCONFIG._serialized_end=17994
-  _SITESBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_start=17996
-  _SITESBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_end=18094
-  _SITES._serialized_start=18097
-  _SITES._serialized_end=20646
-  _SITES_TAGSENTRY._serialized_start=2854
-  _SITES_TAGSENTRY._serialized_end=2897
-  _SITECONFIG._serialized_start=20649
-  _SITECONFIG._serialized_end=23370
-  _SITECONFIG_AZURESTORAGEACCOUNTSENTRY._serialized_start=23311
-  _SITECONFIG_AZURESTORAGEACCOUNTSENTRY._serialized_end=23370
-  _VIRTUALAPPLICATION._serialized_start=23373
-  _VIRTUALAPPLICATION._serialized_end=23543
-  _VIRTUALDIRECTORY._serialized_start=23545
-  _VIRTUALDIRECTORY._serialized_end=23608
-  _PUSHSETTINGS._serialized_start=23611
-  _PUSHSETTINGS._serialized_end=23748
-  _SITELIMITS._serialized_start=23750
-  _SITELIMITS._serialized_end=23845
-  _IPSECURITYRESTRICTION._serialized_start=23848
-  _IPSECURITYRESTRICTION._serialized_end=24215
-  _IPSECURITYRESTRICTION_HEADERSENTRY._serialized_start=24169
-  _IPSECURITYRESTRICTION_HEADERSENTRY._serialized_end=24215
-  _HANDLERMAPPING._serialized_start=24217
-  _HANDLERMAPPING._serialized_end=24297
-  _EXPERIMENTS._serialized_start=24299
-  _EXPERIMENTS._serialized_end=24380
-  _RAMPUPRULE._serialized_start=24383
-  _RAMPUPRULE._serialized_end=24622
-  _CORSSETTINGS._serialized_start=24624
-  _CORSSETTINGS._serialized_end=24692
-  _CONNSTRINGINFO._serialized_start=24694
-  _CONNSTRINGINFO._serialized_end=24765
-  _AUTOHEALRULES._serialized_start=24768
-  _AUTOHEALRULES._serialized_end=24919
-  _AUTOHEALTRIGGERS._serialized_start=24922
-  _AUTOHEALTRIGGERS._serialized_end=25387
-  _STATUSCODESRANGEBASEDTRIGGER._serialized_start=25389
-  _STATUSCODESRANGEBASEDTRIGGER._serialized_end=25493
-  _STATUSCODESBASEDTRIGGER._serialized_start=25496
-  _STATUSCODESBASEDTRIGGER._serialized_end=25631
-  _SLOWREQUESTSBASEDTRIGGER._serialized_start=25633
-  _SLOWREQUESTSBASEDTRIGGER._serialized_end=25731
-  _REQUESTSBASEDTRIGGER._serialized_start=25733
-  _REQUESTSBASEDTRIGGER._serialized_end=25793
-  _AUTOHEALACTIONS._serialized_start=25796
-  _AUTOHEALACTIONS._serialized_end=25948
-  _AUTOHEALCUSTOMACTION._serialized_start=25950
-  _AUTOHEALCUSTOMACTION._serialized_end=26005
-  _APIMANAGEMENTCONFIG._serialized_start=26007
-  _APIMANAGEMENTCONFIG._serialized_end=26040
-  _APIDEFINITIONINFO._serialized_start=26042
-  _APIDEFINITIONINFO._serialized_end=26074
-  _HOSTNAMESSLSTATE._serialized_start=26077
-  _HOSTNAMESSLSTATE._serialized_end=26206
-  _CLONINGINFO._serialized_start=26209
-  _CLONINGINFO._serialized_end=26690
-  _CLONINGINFO_APPSETTINGSOVERRIDESENTRY._serialized_start=26631
-  _CLONINGINFO_APPSETTINGSOVERRIDESENTRY._serialized_end=26690
-  _MANAGEDSERVICEIDENTITY._serialized_start=26693
-  _MANAGEDSERVICEIDENTITY._serialized_end=26913
-  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_start=26852
-  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_end=26913
-  _SERVERFARMSVIRTUALNETWORKCONNECTIONSROUTES._serialized_start=26916
-  _SERVERFARMSVIRTUALNETWORKCONNECTIONSROUTES._serialized_end=27109
-  _SERVERFARMSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_start=27112
-  _SERVERFARMSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_end=27287
-  _SERVERFARMS._serialized_start=27290
-  _SERVERFARMS._serialized_end=28190
-  _SERVERFARMS_TAGSENTRY._serialized_start=2854
-  _SERVERFARMS_TAGSENTRY._serialized_end=2897
-  _KUBEENVIRONMENTPROFILE._serialized_start=28192
-  _KUBEENVIRONMENTPROFILE._serialized_end=28228
-  _HOSTINGENVIRONMENTPROFILE._serialized_start=28230
-  _HOSTINGENVIRONMENTPROFILE._serialized_end=28269
-  _KUBEENVIRONMENTS._serialized_start=28272
-  _KUBEENVIRONMENTS._serialized_end=28965
-  _KUBEENVIRONMENTS_TAGSENTRY._serialized_start=2854
-  _KUBEENVIRONMENTS_TAGSENTRY._serialized_end=2897
-  _CONTAINERAPPSCONFIGURATION._serialized_start=28968
-  _CONTAINERAPPSCONFIGURATION._serialized_end=29202
-  _ARCCONFIGURATION._serialized_start=29205
-  _ARCCONFIGURATION._serialized_end=29521
-  _FRONTENDCONFIGURATION._serialized_start=29523
-  _FRONTENDCONFIGURATION._serialized_end=29560
-  _APPLOGSCONFIGURATION._serialized_start=29563
-  _APPLOGSCONFIGURATION._serialized_end=29703
-  _LOGANALYTICSCONFIGURATION._serialized_start=29705
-  _LOGANALYTICSCONFIGURATION._serialized_end=29773
-  _EXTENDEDLOCATION._serialized_start=29775
-  _EXTENDEDLOCATION._serialized_end=29807
-  _HOSTINGENVIRONMENTSWORKERPOOLS._serialized_start=29810
-  _HOSTINGENVIRONMENTSWORKERPOOLS._serialized_end=30078
-  _HOSTINGENVIRONMENTSPRIVATEENDPOINTCONNECTIONS._serialized_start=30081
-  _HOSTINGENVIRONMENTSPRIVATEENDPOINTCONNECTIONS._serialized_end=30321
-  _PRIVATELINKCONNECTIONSTATE._serialized_start=30323
-  _PRIVATELINKCONNECTIONSTATE._serialized_end=30414
-  _HOSTINGENVIRONMENTSMULTIROLEPOOLS._serialized_start=30417
-  _HOSTINGENVIRONMENTSMULTIROLEPOOLS._serialized_end=30688
-  _SKUDESCRIPTION._serialized_start=30691
-  _SKUDESCRIPTION._serialized_end=30937
-  _SKUCAPACITY._serialized_start=30939
-  _SKUCAPACITY._serialized_end=31048
-  _CAPABILITY._serialized_start=31050
-  _CAPABILITY._serialized_end=31107
-  _HOSTINGENVIRONMENTSCONFIGURATIONS._serialized_start=31110
-  _HOSTINGENVIRONMENTSCONFIGURATIONS._serialized_end=31278
-  _HOSTINGENVIRONMENTS._serialized_start=31281
-  _HOSTINGENVIRONMENTS._serialized_end=32388
-  _HOSTINGENVIRONMENTS_TAGSENTRY._serialized_start=2854
-  _HOSTINGENVIRONMENTS_TAGSENTRY._serialized_end=2897
-  _VIRTUALNETWORKPROFILE._serialized_start=32390
-  _VIRTUALNETWORKPROFILE._serialized_end=32441
-  _NAMEVALUEPAIR._serialized_start=32443
-  _NAMEVALUEPAIR._serialized_end=32487
-  _CONTAINERAPPS._serialized_start=32490
-  _CONTAINERAPPS._serialized_end=32886
-  _CONTAINERAPPS_TAGSENTRY._serialized_start=2854
-  _CONTAINERAPPS_TAGSENTRY._serialized_end=2897
-  _TEMPLATE._serialized_start=32889
-  _TEMPLATE._serialized_end=33096
-  _SCALE._serialized_start=33098
-  _SCALE._serialized_end=33208
-  _SCALERULE._serialized_start=33211
-  _SCALERULE._serialized_end=33434
-  _HTTPSCALERULE._serialized_start=33437
-  _HTTPSCALERULE._serialized_end=33643
-  _HTTPSCALERULE_METADATAENTRY._serialized_start=33596
-  _HTTPSCALERULE_METADATAENTRY._serialized_end=33643
-  _CUSTOMSCALERULE._serialized_start=33646
-  _CUSTOMSCALERULE._serialized_end=33870
-  _CUSTOMSCALERULE_METADATAENTRY._serialized_start=33596
-  _CUSTOMSCALERULE_METADATAENTRY._serialized_end=33643
-  _QUEUESCALERULE._serialized_start=33872
-  _QUEUESCALERULE._serialized_end=33992
-  _SCALERULEAUTH._serialized_start=33994
-  _SCALERULEAUTH._serialized_end=34056
-  _DAPR._serialized_start=34058
-  _DAPR._serialized_end=34183
-  _DAPRCOMPONENT._serialized_start=34185
-  _DAPRCOMPONENT._serialized_end=34310
-  _DAPRMETADATA._serialized_start=34312
-  _DAPRMETADATA._serialized_end=34375
-  _CONTAINER._serialized_start=34378
-  _CONTAINER._serialized_end=34511
-  _ENVIRONMENTVAR._serialized_start=34513
-  _ENVIRONMENTVAR._serialized_end=34578
-  _CONFIGURATION._serialized_start=34581
-  _CONFIGURATION._serialized_end=34818
-  _SECRET._serialized_start=34820
-  _SECRET._serialized_end=34857
-  _REGISTRYCREDENTIALS._serialized_start=34859
-  _REGISTRYCREDENTIALS._serialized_end=34943
-  _INGRESS._serialized_start=34946
-  _INGRESS._serialized_end=35102
-  _TRAFFICWEIGHT._serialized_start=35104
-  _TRAFFICWEIGHT._serialized_end=35183
-  _CERTIFICATES._serialized_start=35186
-  _CERTIFICATES._serialized_end=35610
-  _CERTIFICATES_TAGSENTRY._serialized_start=2854
-  _CERTIFICATES_TAGSENTRY._serialized_end=2897
+  _MICROSOFT_WEB._serialized_end=818
+  _STATICSITESUSERPROVIDEDFUNCTIONAPPS._serialized_start=821
+  _STATICSITESUSERPROVIDEDFUNCTIONAPPS._serialized_end=1006
+  _STATICSITESPRIVATEENDPOINTCONNECTIONS._serialized_start=1009
+  _STATICSITESPRIVATEENDPOINTCONNECTIONS._serialized_end=1241
+  _STATICSITESLINKEDBACKENDS._serialized_start=1244
+  _STATICSITESLINKEDBACKENDS._serialized_end=1401
+  _STATICSITESCUSTOMDOMAINS._serialized_start=1404
+  _STATICSITESCUSTOMDOMAINS._serialized_end=1542
+  _STATICSITESCONFIG._serialized_start=1544
+  _STATICSITESCONFIG._serialized_end=1620
+  _STATICSITESBUILDSUSERPROVIDEDFUNCTIONAPPS._serialized_start=1623
+  _STATICSITESBUILDSUSERPROVIDEDFUNCTIONAPPS._serialized_end=1814
+  _STATICSITESBUILDSLINKEDBACKENDS._serialized_start=1817
+  _STATICSITESBUILDSLINKEDBACKENDS._serialized_end=1980
+  _STATICSITESBUILDSCONFIG._serialized_start=1982
+  _STATICSITESBUILDSCONFIG._serialized_end=2064
+  _STATICSITES._serialized_start=2067
+  _STATICSITES._serialized_end=3351
+  _STATICSITES_TAGSENTRY._serialized_start=3308
+  _STATICSITES_TAGSENTRY._serialized_end=3351
+  _STATICSITETEMPLATEOPTIONS._serialized_start=3354
+  _STATICSITETEMPLATEOPTIONS._serialized_end=3495
+  _STATICSITEBUILDPROPERTIES._serialized_start=3498
+  _STATICSITEBUILDPROPERTIES._serialized_end=3771
+  _SITESVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_start=3774
+  _SITESVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_end=3943
+  _SITESVIRTUALNETWORKCONNECTIONS._serialized_start=3946
+  _SITESVIRTUALNETWORKCONNECTIONS._serialized_end=4272
+  _SITESSOURCECONTROLS._serialized_start=4275
+  _SITESSOURCECONTROLS._serialized_end=4630
+  _SITESSLOTSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_start=4633
+  _SITESSLOTSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_end=4807
+  _SITESSLOTSVIRTUALNETWORKCONNECTIONS._serialized_start=4810
+  _SITESSLOTSVIRTUALNETWORKCONNECTIONS._serialized_end=5153
+  _SITESSLOTSSOURCECONTROLS._serialized_start=5156
+  _SITESSLOTSSOURCECONTROLS._serialized_end=5516
+  _GITHUBACTIONCONFIGURATION._serialized_start=5519
+  _GITHUBACTIONCONFIGURATION._serialized_end=5790
+  _GITHUBACTIONCONTAINERCONFIGURATION._serialized_start=5792
+  _GITHUBACTIONCONTAINERCONFIGURATION._serialized_end=5904
+  _GITHUBACTIONCODECONFIGURATION._serialized_start=5906
+  _GITHUBACTIONCODECONFIGURATION._serialized_end=5985
+  _SITESSLOTSSITEEXTENSIONS._serialized_start=5987
+  _SITESSLOTSSITEEXTENSIONS._serialized_end=6084
+  _SITESSLOTSPUBLICCERTIFICATES._serialized_start=6087
+  _SITESSLOTSPUBLICCERTIFICATES._serialized_end=6253
+  _SITESSLOTSPRIVATEENDPOINTCONNECTIONS._serialized_start=6256
+  _SITESSLOTSPRIVATEENDPOINTCONNECTIONS._serialized_end=6487
+  _SITESSLOTSPRIVATEACCESS._serialized_start=6490
+  _SITESSLOTSPRIVATEACCESS._serialized_end=6705
+  _SITESSLOTSPREMIERADDONS._serialized_start=6708
+  _SITESSLOTSPREMIERADDONS._serialized_end=7067
+  _SITESSLOTSPREMIERADDONS_TAGSENTRY._serialized_start=3308
+  _SITESSLOTSPREMIERADDONS_TAGSENTRY._serialized_end=3351
+  _SITESSLOTSNETWORKCONFIG._serialized_start=7070
+  _SITESSLOTSNETWORKCONFIG._serialized_end=7233
+  _SITESSLOTSINSTANCESEXTENSIONS._serialized_start=7236
+  _SITESSLOTSINSTANCESEXTENSIONS._serialized_end=7659
+  _SITESSLOTSINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_start=7607
+  _SITESSLOTSINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_end=7659
+  _SITESSLOTSHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_start=7662
+  _SITESSLOTSHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_end=7972
+  _SITESSLOTSHYBRIDCONNECTION._serialized_start=7975
+  _SITESSLOTSHYBRIDCONNECTION._serialized_end=8255
+  _SITESSLOTSHOSTNAMEBINDINGS._serialized_start=8258
+  _SITESSLOTSHOSTNAMEBINDINGS._serialized_end=8572
+  _SITESSLOTSFUNCTIONSKEYS._serialized_start=8574
+  _SITESSLOTSFUNCTIONSKEYS._serialized_end=8685
+  _SITESSLOTSFUNCTIONS._serialized_start=8688
+  _SITESSLOTSFUNCTIONS._serialized_end=9393
+  _SITESSLOTSFUNCTIONS_CONFIGENTRY._serialized_start=9302
+  _SITESSLOTSFUNCTIONS_CONFIGENTRY._serialized_end=9347
+  _SITESSLOTSFUNCTIONS_FILESENTRY._serialized_start=9349
+  _SITESSLOTSFUNCTIONS_FILESENTRY._serialized_end=9393
+  _SITESSLOTSEXTENSIONS._serialized_start=9396
+  _SITESSLOTSEXTENSIONS._serialized_end=9801
+  _SITESSLOTSEXTENSIONS_SETPARAMETERSENTRY._serialized_start=7607
+  _SITESSLOTSEXTENSIONS_SETPARAMETERSENTRY._serialized_end=7659
+  _SITESSLOTSDOMAINOWNERSHIPIDENTIFIERS._serialized_start=9804
+  _SITESSLOTSDOMAINOWNERSHIPIDENTIFIERS._serialized_end=9939
+  _SITESSLOTSDEPLOYMENTS._serialized_start=9942
+  _SITESSLOTSDEPLOYMENTS._serialized_end=10210
+  _SITESSLOTSCONFIG._serialized_start=10212
+  _SITESSLOTSCONFIG._serialized_end=10287
+  _SITESSLOTSBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_start=10289
+  _SITESSLOTSBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_end=10392
+  _SITESSLOTS._serialized_start=10395
+  _SITESSLOTS._serialized_end=13363
+  _SITESSLOTS_TAGSENTRY._serialized_start=3308
+  _SITESSLOTS_TAGSENTRY._serialized_end=3351
+  _SITESSITEEXTENSIONS._serialized_start=13365
+  _SITESSITEEXTENSIONS._serialized_end=13457
+  _SITESPUBLICCERTIFICATES._serialized_start=13460
+  _SITESPUBLICCERTIFICATES._serialized_end=13621
+  _SITESPRIVATEENDPOINTCONNECTIONS._serialized_start=13624
+  _SITESPRIVATEENDPOINTCONNECTIONS._serialized_end=13850
+  _SITESPRIVATEACCESS._serialized_start=13853
+  _SITESPRIVATEACCESS._serialized_end=14063
+  _PRIVATEACCESSVIRTUALNETWORK._serialized_start=14066
+  _PRIVATEACCESSVIRTUALNETWORK._serialized_end=14214
+  _PRIVATEACCESSSUBNET._serialized_start=14216
+  _PRIVATEACCESSSUBNET._serialized_end=14264
+  _SITESPREMIERADDONS._serialized_start=14267
+  _SITESPREMIERADDONS._serialized_end=14616
+  _SITESPREMIERADDONS_TAGSENTRY._serialized_start=3308
+  _SITESPREMIERADDONS_TAGSENTRY._serialized_end=3351
+  _SITESNETWORKCONFIG._serialized_start=14619
+  _SITESNETWORKCONFIG._serialized_end=14777
+  _SITESMIGRATE._serialized_start=14780
+  _SITESMIGRATE._serialized_end=15016
+  _SITESINSTANCESEXTENSIONS._serialized_start=15019
+  _SITESINSTANCESEXTENSIONS._serialized_end=15432
+  _SITESINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_start=7607
+  _SITESINSTANCESEXTENSIONS_SETPARAMETERSENTRY._serialized_end=7659
+  _SITESHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_start=15435
+  _SITESHYBRIDCONNECTIONNAMESPACESRELAYS._serialized_end=15740
+  _SITESHYBRIDCONNECTION._serialized_start=15743
+  _SITESHYBRIDCONNECTION._serialized_end=16018
+  _SITESHOSTNAMEBINDINGS._serialized_start=16021
+  _SITESHOSTNAMEBINDINGS._serialized_end=16330
+  _SITESFUNCTIONSKEYS._serialized_start=16332
+  _SITESFUNCTIONSKEYS._serialized_end=16438
+  _SITESFUNCTIONS._serialized_start=16441
+  _SITESFUNCTIONS._serialized_end=17120
+  _SITESFUNCTIONS_CONFIGENTRY._serialized_start=9302
+  _SITESFUNCTIONS_CONFIGENTRY._serialized_end=9347
+  _SITESFUNCTIONS_FILESENTRY._serialized_start=9349
+  _SITESFUNCTIONS_FILESENTRY._serialized_end=9393
+  _SITESEXTENSIONS._serialized_start=17122
+  _SITESEXTENSIONS._serialized_end=17196
+  _SITESDOMAINOWNERSHIPIDENTIFIERS._serialized_start=17199
+  _SITESDOMAINOWNERSHIPIDENTIFIERS._serialized_end=17329
+  _SITESDEPLOYMENTS._serialized_start=17332
+  _SITESDEPLOYMENTS._serialized_end=17595
+  _SITESCONFIG._serialized_start=17598
+  _SITESCONFIG._serialized_end=18258
+  _SITESBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_start=18260
+  _SITESBASICPUBLISHINGCREDENTIALSPOLICIES._serialized_end=18358
+  _SITES._serialized_start=18361
+  _SITES._serialized_end=21042
+  _SITES_TAGSENTRY._serialized_start=3308
+  _SITES_TAGSENTRY._serialized_end=3351
+  _SITECONFIG._serialized_start=21045
+  _SITECONFIG._serialized_end=23766
+  _SITECONFIG_AZURESTORAGEACCOUNTSENTRY._serialized_start=23707
+  _SITECONFIG_AZURESTORAGEACCOUNTSENTRY._serialized_end=23766
+  _VIRTUALAPPLICATION._serialized_start=23769
+  _VIRTUALAPPLICATION._serialized_end=23939
+  _VIRTUALDIRECTORY._serialized_start=23941
+  _VIRTUALDIRECTORY._serialized_end=24004
+  _PUSHSETTINGS._serialized_start=24007
+  _PUSHSETTINGS._serialized_end=24144
+  _SITELIMITS._serialized_start=24146
+  _SITELIMITS._serialized_end=24241
+  _IPSECURITYRESTRICTION._serialized_start=24244
+  _IPSECURITYRESTRICTION._serialized_end=24611
+  _IPSECURITYRESTRICTION_HEADERSENTRY._serialized_start=24565
+  _IPSECURITYRESTRICTION_HEADERSENTRY._serialized_end=24611
+  _HANDLERMAPPING._serialized_start=24613
+  _HANDLERMAPPING._serialized_end=24693
+  _EXPERIMENTS._serialized_start=24695
+  _EXPERIMENTS._serialized_end=24776
+  _RAMPUPRULE._serialized_start=24779
+  _RAMPUPRULE._serialized_end=25018
+  _CORSSETTINGS._serialized_start=25020
+  _CORSSETTINGS._serialized_end=25088
+  _CONNSTRINGINFO._serialized_start=25090
+  _CONNSTRINGINFO._serialized_end=25161
+  _AUTOHEALRULES._serialized_start=25164
+  _AUTOHEALRULES._serialized_end=25315
+  _AUTOHEALTRIGGERS._serialized_start=25318
+  _AUTOHEALTRIGGERS._serialized_end=25783
+  _STATUSCODESRANGEBASEDTRIGGER._serialized_start=25785
+  _STATUSCODESRANGEBASEDTRIGGER._serialized_end=25889
+  _STATUSCODESBASEDTRIGGER._serialized_start=25892
+  _STATUSCODESBASEDTRIGGER._serialized_end=26027
+  _SLOWREQUESTSBASEDTRIGGER._serialized_start=26029
+  _SLOWREQUESTSBASEDTRIGGER._serialized_end=26127
+  _REQUESTSBASEDTRIGGER._serialized_start=26129
+  _REQUESTSBASEDTRIGGER._serialized_end=26189
+  _AUTOHEALACTIONS._serialized_start=26192
+  _AUTOHEALACTIONS._serialized_end=26344
+  _AUTOHEALCUSTOMACTION._serialized_start=26346
+  _AUTOHEALCUSTOMACTION._serialized_end=26401
+  _APIMANAGEMENTCONFIG._serialized_start=26403
+  _APIMANAGEMENTCONFIG._serialized_end=26436
+  _APIDEFINITIONINFO._serialized_start=26438
+  _APIDEFINITIONINFO._serialized_end=26470
+  _HOSTNAMESSLSTATE._serialized_start=26473
+  _HOSTNAMESSLSTATE._serialized_end=26602
+  _CLONINGINFO._serialized_start=26605
+  _CLONINGINFO._serialized_end=27086
+  _CLONINGINFO_APPSETTINGSOVERRIDESENTRY._serialized_start=27027
+  _CLONINGINFO_APPSETTINGSOVERRIDESENTRY._serialized_end=27086
+  _MANAGEDSERVICEIDENTITY._serialized_start=27089
+  _MANAGEDSERVICEIDENTITY._serialized_end=27309
+  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_start=27248
+  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_end=27309
+  _SERVERFARMSVIRTUALNETWORKCONNECTIONSROUTES._serialized_start=27312
+  _SERVERFARMSVIRTUALNETWORKCONNECTIONSROUTES._serialized_end=27505
+  _SERVERFARMSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_start=27508
+  _SERVERFARMSVIRTUALNETWORKCONNECTIONSGATEWAYS._serialized_end=27683
+  _SERVERFARMS._serialized_start=27686
+  _SERVERFARMS._serialized_end=28586
+  _SERVERFARMS_TAGSENTRY._serialized_start=3308
+  _SERVERFARMS_TAGSENTRY._serialized_end=3351
+  _KUBEENVIRONMENTPROFILE._serialized_start=28588
+  _KUBEENVIRONMENTPROFILE._serialized_end=28624
+  _HOSTINGENVIRONMENTPROFILE._serialized_start=28626
+  _HOSTINGENVIRONMENTPROFILE._serialized_end=28665
+  _KUBEENVIRONMENTS._serialized_start=28668
+  _KUBEENVIRONMENTS._serialized_end=29361
+  _KUBEENVIRONMENTS_TAGSENTRY._serialized_start=3308
+  _KUBEENVIRONMENTS_TAGSENTRY._serialized_end=3351
+  _CONTAINERAPPSCONFIGURATION._serialized_start=29364
+  _CONTAINERAPPSCONFIGURATION._serialized_end=29598
+  _ARCCONFIGURATION._serialized_start=29601
+  _ARCCONFIGURATION._serialized_end=29917
+  _FRONTENDCONFIGURATION._serialized_start=29919
+  _FRONTENDCONFIGURATION._serialized_end=29956
+  _APPLOGSCONFIGURATION._serialized_start=29959
+  _APPLOGSCONFIGURATION._serialized_end=30099
+  _LOGANALYTICSCONFIGURATION._serialized_start=30101
+  _LOGANALYTICSCONFIGURATION._serialized_end=30169
+  _EXTENDEDLOCATION._serialized_start=30171
+  _EXTENDEDLOCATION._serialized_end=30203
+  _HOSTINGENVIRONMENTSWORKERPOOLS._serialized_start=30206
+  _HOSTINGENVIRONMENTSWORKERPOOLS._serialized_end=30474
+  _HOSTINGENVIRONMENTSPRIVATEENDPOINTCONNECTIONS._serialized_start=30477
+  _HOSTINGENVIRONMENTSPRIVATEENDPOINTCONNECTIONS._serialized_end=30717
+  _PRIVATELINKCONNECTIONSTATE._serialized_start=30719
+  _PRIVATELINKCONNECTIONSTATE._serialized_end=30810
+  _HOSTINGENVIRONMENTSMULTIROLEPOOLS._serialized_start=30813
+  _HOSTINGENVIRONMENTSMULTIROLEPOOLS._serialized_end=31084
+  _SKUDESCRIPTION._serialized_start=31087
+  _SKUDESCRIPTION._serialized_end=31333
+  _SKUCAPACITY._serialized_start=31335
+  _SKUCAPACITY._serialized_end=31444
+  _CAPABILITY._serialized_start=31446
+  _CAPABILITY._serialized_end=31503
+  _HOSTINGENVIRONMENTSCONFIGURATIONS._serialized_start=31505
+  _HOSTINGENVIRONMENTSCONFIGURATIONS._serialized_end=31597
+  _HOSTINGENVIRONMENTS._serialized_start=31600
+  _HOSTINGENVIRONMENTS._serialized_end=32936
+  _HOSTINGENVIRONMENTS_TAGSENTRY._serialized_start=3308
+  _HOSTINGENVIRONMENTS_TAGSENTRY._serialized_end=3351
+  _VIRTUALNETWORKPROFILE._serialized_start=32938
+  _VIRTUALNETWORKPROFILE._serialized_end=32989
+  _ASEV3NETWORKINGCONFIGURATION._serialized_start=32992
+  _ASEV3NETWORKINGCONFIGURATION._serialized_end=33172
+  _CUSTOMDNSSUFFIXCONFIGURATION._serialized_start=33174
+  _CUSTOMDNSSUFFIXCONFIGURATION._serialized_end=33301
+  _NAMEVALUEPAIR._serialized_start=33303
+  _NAMEVALUEPAIR._serialized_end=33347
+  _CONTAINERAPPS._serialized_start=33350
+  _CONTAINERAPPS._serialized_end=33746
+  _CONTAINERAPPS_TAGSENTRY._serialized_start=3308
+  _CONTAINERAPPS_TAGSENTRY._serialized_end=3351
+  _TEMPLATE._serialized_start=33749
+  _TEMPLATE._serialized_end=33956
+  _SCALE._serialized_start=33958
+  _SCALE._serialized_end=34068
+  _SCALERULE._serialized_start=34071
+  _SCALERULE._serialized_end=34294
+  _HTTPSCALERULE._serialized_start=34297
+  _HTTPSCALERULE._serialized_end=34503
+  _HTTPSCALERULE_METADATAENTRY._serialized_start=34456
+  _HTTPSCALERULE_METADATAENTRY._serialized_end=34503
+  _CUSTOMSCALERULE._serialized_start=34506
+  _CUSTOMSCALERULE._serialized_end=34730
+  _CUSTOMSCALERULE_METADATAENTRY._serialized_start=34456
+  _CUSTOMSCALERULE_METADATAENTRY._serialized_end=34503
+  _QUEUESCALERULE._serialized_start=34732
+  _QUEUESCALERULE._serialized_end=34852
+  _SCALERULEAUTH._serialized_start=34854
+  _SCALERULEAUTH._serialized_end=34916
+  _DAPR._serialized_start=34918
+  _DAPR._serialized_end=35043
+  _DAPRCOMPONENT._serialized_start=35045
+  _DAPRCOMPONENT._serialized_end=35170
+  _DAPRMETADATA._serialized_start=35172
+  _DAPRMETADATA._serialized_end=35235
+  _CONTAINER._serialized_start=35238
+  _CONTAINER._serialized_end=35371
+  _ENVIRONMENTVAR._serialized_start=35373
+  _ENVIRONMENTVAR._serialized_end=35438
+  _CONFIGURATION._serialized_start=35441
+  _CONFIGURATION._serialized_end=35678
+  _SECRET._serialized_start=35680
+  _SECRET._serialized_end=35717
+  _REGISTRYCREDENTIALS._serialized_start=35719
+  _REGISTRYCREDENTIALS._serialized_end=35803
+  _INGRESS._serialized_start=35806
+  _INGRESS._serialized_end=35962
+  _TRAFFICWEIGHT._serialized_start=35964
+  _TRAFFICWEIGHT._serialized_end=36043
+  _CERTIFICATES._serialized_start=36046
+  _CERTIFICATES._serialized_end=36470
+  _CERTIFICATES_TAGSENTRY._serialized_start=3308
+  _CERTIFICATES_TAGSENTRY._serialized_end=3351
 # @@protoc_insertion_point(module_scope)
```

### Comparing `oak9_tython-1.0.2/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,28 +36,28 @@
     @property
     def serverfarms_virtual_network_connections_gateways(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServerfarmsVirtualNetworkConnectionsGateways]: ...
     @property
     def serverfarms_virtual_network_connections_routes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServerfarmsVirtualNetworkConnectionsRoutes]: ...
     @property
     def sites(self) -> global___Sites: ...
     @property
-    def sites_config(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SitesConfig]: ...
+    def sites_config(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SiteConfig]: ...
     @property
     def sites_deployments(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SitesDeployments]: ...
     @property
     def sites_host_name_bindings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SitesHostNameBindings]: ...
     def __init__(
         self,
         *,
         hosting_environments: global___HostingEnvironments | None = ...,
         serverfarms: global___Serverfarms | None = ...,
         serverfarms_virtual_network_connections_gateways: collections.abc.Iterable[global___ServerfarmsVirtualNetworkConnectionsGateways] | None = ...,
         serverfarms_virtual_network_connections_routes: collections.abc.Iterable[global___ServerfarmsVirtualNetworkConnectionsRoutes] | None = ...,
         sites: global___Sites | None = ...,
-        sites_config: collections.abc.Iterable[global___SitesConfig] | None = ...,
+        sites_config: collections.abc.Iterable[global___SiteConfig] | None = ...,
         sites_deployments: collections.abc.Iterable[global___SitesDeployments] | None = ...,
         sites_host_name_bindings: collections.abc.Iterable[global___SitesHostNameBindings] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["hosting_environments", b"hosting_environments", "serverfarms", b"serverfarms", "sites", b"sites"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["hosting_environments", b"hosting_environments", "serverfarms", b"serverfarms", "serverfarms_virtual_network_connections_gateways", b"serverfarms_virtual_network_connections_gateways", "serverfarms_virtual_network_connections_routes", b"serverfarms_virtual_network_connections_routes", "sites", b"sites", "sites_config", b"sites_config", "sites_deployments", b"sites_deployments", "sites_host_name_bindings", b"sites_host_name_bindings"]) -> None: ...
 
 global___Microsoft_Web = Microsoft_Web
@@ -115,14 +115,43 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["private_link_service_connection_state", b"private_link_service_connection_state", "resource_info", b"resource_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["kind", b"kind", "name", b"name", "private_link_service_connection_state", b"private_link_service_connection_state", "resource_info", b"resource_info"]) -> None: ...
 
 global___StaticSitesPrivateEndpointConnections = StaticSitesPrivateEndpointConnections
 
 @typing_extensions.final
+class StaticSitesLinkedBackends(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    KIND_FIELD_NUMBER: builtins.int
+    NAME_FIELD_NUMBER: builtins.int
+    BACKEND_RESOURCE_ID_FIELD_NUMBER: builtins.int
+    REGION_FIELD_NUMBER: builtins.int
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    kind: builtins.str
+    name: builtins.str
+    backend_resource_id: builtins.str
+    region: builtins.str
+    def __init__(
+        self,
+        *,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+        kind: builtins.str = ...,
+        name: builtins.str = ...,
+        backend_resource_id: builtins.str = ...,
+        region: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["backend_resource_id", b"backend_resource_id", "kind", b"kind", "name", b"name", "region", b"region", "resource_info", b"resource_info"]) -> None: ...
+
+global___StaticSitesLinkedBackends = StaticSitesLinkedBackends
+
+@typing_extensions.final
 class StaticSitesCustomDomains(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
     KIND_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     VALIDATION_METHOD_FIELD_NUMBER: builtins.int
@@ -187,14 +216,43 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["function_app_region", b"function_app_region", "function_app_resource_id", b"function_app_resource_id", "kind", b"kind", "name", b"name", "resource_info", b"resource_info"]) -> None: ...
 
 global___StaticSitesBuildsUserProvidedFunctionApps = StaticSitesBuildsUserProvidedFunctionApps
 
 @typing_extensions.final
+class StaticSitesBuildsLinkedBackends(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    KIND_FIELD_NUMBER: builtins.int
+    NAME_FIELD_NUMBER: builtins.int
+    BACKEND_RESOURCE_ID_FIELD_NUMBER: builtins.int
+    REGION_FIELD_NUMBER: builtins.int
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    kind: builtins.str
+    name: builtins.str
+    backend_resource_id: builtins.str
+    region: builtins.str
+    def __init__(
+        self,
+        *,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+        kind: builtins.str = ...,
+        name: builtins.str = ...,
+        backend_resource_id: builtins.str = ...,
+        region: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["backend_resource_id", b"backend_resource_id", "kind", b"kind", "name", b"name", "region", b"region", "resource_info", b"resource_info"]) -> None: ...
+
+global___StaticSitesBuildsLinkedBackends = StaticSitesBuildsLinkedBackends
+
+@typing_extensions.final
 class StaticSitesBuildsConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
@@ -233,37 +291,40 @@
     LOCATION_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     ALLOW_CONFIG_FILE_UPDATES_FIELD_NUMBER: builtins.int
     BRANCH_FIELD_NUMBER: builtins.int
     BUILD_PROPERTIES_FIELD_NUMBER: builtins.int
     ENTERPRISE_GRADE_CDN_STATUS_FIELD_NUMBER: builtins.int
     PROVIDER_FIELD_NUMBER: builtins.int
+    PUBLIC_NETWORK_ACCESS_FIELD_NUMBER: builtins.int
     REPOSITORY_TOKEN_FIELD_NUMBER: builtins.int
     REPOSITORY_URL_FIELD_NUMBER: builtins.int
     STAGING_ENVIRONMENT_POLICY_FIELD_NUMBER: builtins.int
     TEMPLATE_PROPERTIES_FIELD_NUMBER: builtins.int
     SKU_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     STATIC_SITES_CONFIG_FIELD_NUMBER: builtins.int
     STATIC_SITES_CUSTOM_DOMAINS_FIELD_NUMBER: builtins.int
     STATIC_SITES_PRIVATE_ENDPOINT_CONNECTIONS_FIELD_NUMBER: builtins.int
     STATIC_SITES_USER_PROVIDED_FUNCTION_APPS_FIELD_NUMBER: builtins.int
+    STATIC_SITES_LINKED_BACKENDS_FIELD_NUMBER: builtins.int
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     @property
     def identity(self) -> global___ManagedServiceIdentity: ...
     kind: builtins.str
     location: builtins.str
     name: builtins.str
     allow_config_file_updates: builtins.bool
     branch: builtins.str
     @property
     def build_properties(self) -> global___StaticSiteBuildProperties: ...
     enterprise_grade_cdn_status: builtins.str
     provider: builtins.str
+    public_network_access: builtins.str
     repository_token: builtins.str
     repository_url: builtins.str
     staging_environment_policy: builtins.str
     @property
     def template_properties(self) -> global___StaticSiteTemplateOptions: ...
     @property
     def sku(self) -> global___SkuDescription: ...
@@ -273,40 +334,44 @@
     def static_sites_config(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StaticSitesConfig]: ...
     @property
     def static_sites_custom_domains(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StaticSitesCustomDomains]: ...
     @property
     def static_sites_private_endpoint_connections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StaticSitesPrivateEndpointConnections]: ...
     @property
     def static_sites_user_provided_function_apps(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StaticSitesUserProvidedFunctionApps]: ...
+    @property
+    def static_sites_linked_backends(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StaticSitesLinkedBackends]: ...
     def __init__(
         self,
         *,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
         identity: global___ManagedServiceIdentity | None = ...,
         kind: builtins.str = ...,
         location: builtins.str = ...,
         name: builtins.str = ...,
         allow_config_file_updates: builtins.bool = ...,
         branch: builtins.str = ...,
         build_properties: global___StaticSiteBuildProperties | None = ...,
         enterprise_grade_cdn_status: builtins.str = ...,
         provider: builtins.str = ...,
+        public_network_access: builtins.str = ...,
         repository_token: builtins.str = ...,
         repository_url: builtins.str = ...,
         staging_environment_policy: builtins.str = ...,
         template_properties: global___StaticSiteTemplateOptions | None = ...,
         sku: global___SkuDescription | None = ...,
         tags: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         static_sites_config: collections.abc.Iterable[global___StaticSitesConfig] | None = ...,
         static_sites_custom_domains: collections.abc.Iterable[global___StaticSitesCustomDomains] | None = ...,
         static_sites_private_endpoint_connections: collections.abc.Iterable[global___StaticSitesPrivateEndpointConnections] | None = ...,
         static_sites_user_provided_function_apps: collections.abc.Iterable[global___StaticSitesUserProvidedFunctionApps] | None = ...,
+        static_sites_linked_backends: collections.abc.Iterable[global___StaticSitesLinkedBackends] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["build_properties", b"build_properties", "identity", b"identity", "resource_info", b"resource_info", "sku", b"sku", "template_properties", b"template_properties"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allow_config_file_updates", b"allow_config_file_updates", "branch", b"branch", "build_properties", b"build_properties", "enterprise_grade_cdn_status", b"enterprise_grade_cdn_status", "identity", b"identity", "kind", b"kind", "location", b"location", "name", b"name", "provider", b"provider", "repository_token", b"repository_token", "repository_url", b"repository_url", "resource_info", b"resource_info", "sku", b"sku", "staging_environment_policy", b"staging_environment_policy", "static_sites_config", b"static_sites_config", "static_sites_custom_domains", b"static_sites_custom_domains", "static_sites_private_endpoint_connections", b"static_sites_private_endpoint_connections", "static_sites_user_provided_function_apps", b"static_sites_user_provided_function_apps", "tags", b"tags", "template_properties", b"template_properties"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["allow_config_file_updates", b"allow_config_file_updates", "branch", b"branch", "build_properties", b"build_properties", "enterprise_grade_cdn_status", b"enterprise_grade_cdn_status", "identity", b"identity", "kind", b"kind", "location", b"location", "name", b"name", "provider", b"provider", "public_network_access", b"public_network_access", "repository_token", b"repository_token", "repository_url", b"repository_url", "resource_info", b"resource_info", "sku", b"sku", "staging_environment_policy", b"staging_environment_policy", "static_sites_config", b"static_sites_config", "static_sites_custom_domains", b"static_sites_custom_domains", "static_sites_linked_backends", b"static_sites_linked_backends", "static_sites_private_endpoint_connections", b"static_sites_private_endpoint_connections", "static_sites_user_provided_function_apps", b"static_sites_user_provided_function_apps", "tags", b"tags", "template_properties", b"template_properties"]) -> None: ...
 
 global___StaticSites = StaticSites
 
 @typing_extensions.final
 class StaticSiteTemplateOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1391,21 +1456,25 @@
     HOSTING_ENVIRONMENT_PROFILE_FIELD_NUMBER: builtins.int
     HOST_NAMES_DISABLED_FIELD_NUMBER: builtins.int
     HOST_NAME_SSL_STATES_FIELD_NUMBER: builtins.int
     HTTPS_ONLY_FIELD_NUMBER: builtins.int
     HYPER_V_FIELD_NUMBER: builtins.int
     IS_XENON_FIELD_NUMBER: builtins.int
     KEY_VAULT_REFERENCE_IDENTITY_FIELD_NUMBER: builtins.int
+    PUBLIC_NETWORK_ACCESS_FIELD_NUMBER: builtins.int
     REDUNDANCY_MODE_FIELD_NUMBER: builtins.int
     RESERVED_FIELD_NUMBER: builtins.int
     SCM_SITE_ALSO_STOPPED_FIELD_NUMBER: builtins.int
     SERVER_FARM_ID_FIELD_NUMBER: builtins.int
     SITE_CONFIG_FIELD_NUMBER: builtins.int
     STORAGE_ACCOUNT_REQUIRED_FIELD_NUMBER: builtins.int
     VIRTUAL_NETWORK_SUBNET_ID_FIELD_NUMBER: builtins.int
+    VNET_CONTENT_SHARE_ENABLED_FIELD_NUMBER: builtins.int
+    VNET_IMAGE_PULL_ENABLED_FIELD_NUMBER: builtins.int
+    VNET_ROUTE_ALL_ENABLED_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     SITES_SLOTS_BASIC_PUBLISHING_CREDENTIALS_POLICIES_FIELD_NUMBER: builtins.int
     SITES_SLOTS_CONFIG_FIELD_NUMBER: builtins.int
     SITES_SLOTS_DEPLOYMENTS_FIELD_NUMBER: builtins.int
     SITES_SLOTS_DOMAIN_OWNERSHIP_IDENTIFIERS_FIELD_NUMBER: builtins.int
     SITES_SLOTS_EXTENSIONS_FIELD_NUMBER: builtins.int
     SITES_SLOTS_FUNCTIONS_FIELD_NUMBER: builtins.int
@@ -1443,22 +1512,26 @@
     host_names_disabled: builtins.bool
     @property
     def host_name_ssl_states(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HostNameSslState]: ...
     https_only: builtins.bool
     hyper_v: builtins.bool
     is_xenon: builtins.bool
     key_vault_reference_identity: builtins.str
+    public_network_access: builtins.str
     redundancy_mode: builtins.str
     reserved: builtins.bool
     scm_site_also_stopped: builtins.bool
     server_farm_id: builtins.str
     @property
     def site_config(self) -> global___SiteConfig: ...
     storage_account_required: builtins.bool
     virtual_network_subnet_id: builtins.str
+    vnet_content_share_enabled: builtins.bool
+    vnet_image_pull_enabled: builtins.bool
+    vnet_route_all_enabled: builtins.bool
     @property
     def tags(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     @property
     def sites_slots_basic_publishing_credentials_policies(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SitesSlotsBasicPublishingCredentialsPolicies]: ...
     @property
     def sites_slots_config(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SitesSlotsConfig]: ...
     @property
@@ -1510,21 +1583,25 @@
         hosting_environment_profile: global___HostingEnvironmentProfile | None = ...,
         host_names_disabled: builtins.bool = ...,
         host_name_ssl_states: collections.abc.Iterable[global___HostNameSslState] | None = ...,
         https_only: builtins.bool = ...,
         hyper_v: builtins.bool = ...,
         is_xenon: builtins.bool = ...,
         key_vault_reference_identity: builtins.str = ...,
+        public_network_access: builtins.str = ...,
         redundancy_mode: builtins.str = ...,
         reserved: builtins.bool = ...,
         scm_site_also_stopped: builtins.bool = ...,
         server_farm_id: builtins.str = ...,
         site_config: global___SiteConfig | None = ...,
         storage_account_required: builtins.bool = ...,
         virtual_network_subnet_id: builtins.str = ...,
+        vnet_content_share_enabled: builtins.bool = ...,
+        vnet_image_pull_enabled: builtins.bool = ...,
+        vnet_route_all_enabled: builtins.bool = ...,
         tags: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         sites_slots_basic_publishing_credentials_policies: collections.abc.Iterable[global___SitesSlotsBasicPublishingCredentialsPolicies] | None = ...,
         sites_slots_config: collections.abc.Iterable[global___SitesSlotsConfig] | None = ...,
         sites_slots_deployments: collections.abc.Iterable[global___SitesSlotsDeployments] | None = ...,
         sites_slots_domain_ownership_identifiers: collections.abc.Iterable[global___SitesSlotsDomainOwnershipIdentifiers] | None = ...,
         sites_slots_extensions: collections.abc.Iterable[global___SitesSlotsExtensions] | None = ...,
         sites_slots_functions: collections.abc.Iterable[global___SitesSlotsFunctions] | None = ...,
@@ -1536,15 +1613,15 @@
         sites_slots_private_endpoint_connections: collections.abc.Iterable[global___SitesSlotsPrivateEndpointConnections] | None = ...,
         sites_slots_public_certificates: collections.abc.Iterable[global___SitesSlotsPublicCertificates] | None = ...,
         sites_slots_siteextensions: collections.abc.Iterable[global___SitesSlotsSiteextensions] | None = ...,
         sites_slots_sourcecontrols: collections.abc.Iterable[global___SitesSlotsSourcecontrols] | None = ...,
         sites_slots_virtual_network_connections: collections.abc.Iterable[global___SitesSlotsVirtualNetworkConnections] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["cloning_info", b"cloning_info", "extended_location", b"extended_location", "hosting_environment_profile", b"hosting_environment_profile", "identity", b"identity", "resource_info", b"resource_info", "site_config", b"site_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_affinity_enabled", b"client_affinity_enabled", "client_cert_enabled", b"client_cert_enabled", "client_cert_exclusion_paths", b"client_cert_exclusion_paths", "client_cert_mode", b"client_cert_mode", "cloning_info", b"cloning_info", "container_size", b"container_size", "custom_domain_verification_id", b"custom_domain_verification_id", "daily_memory_time_quota", b"daily_memory_time_quota", "enabled", b"enabled", "extended_location", b"extended_location", "host_name_ssl_states", b"host_name_ssl_states", "host_names_disabled", b"host_names_disabled", "hosting_environment_profile", b"hosting_environment_profile", "https_only", b"https_only", "hyper_v", b"hyper_v", "identity", b"identity", "is_xenon", b"is_xenon", "key_vault_reference_identity", b"key_vault_reference_identity", "kind", b"kind", "location", b"location", "name", b"name", "redundancy_mode", b"redundancy_mode", "reserved", b"reserved", "resource_info", b"resource_info", "scm_site_also_stopped", b"scm_site_also_stopped", "server_farm_id", b"server_farm_id", "site_config", b"site_config", "sites_slots_basic_publishing_credentials_policies", b"sites_slots_basic_publishing_credentials_policies", "sites_slots_config", b"sites_slots_config", "sites_slots_deployments", b"sites_slots_deployments", "sites_slots_domain_ownership_identifiers", b"sites_slots_domain_ownership_identifiers", "sites_slots_extensions", b"sites_slots_extensions", "sites_slots_functions", b"sites_slots_functions", "sites_slots_host_name_bindings", b"sites_slots_host_name_bindings", "sites_slots_hybridconnection", b"sites_slots_hybridconnection", "sites_slots_network_config", b"sites_slots_network_config", "sites_slots_premieraddons", b"sites_slots_premieraddons", "sites_slots_private_access", b"sites_slots_private_access", "sites_slots_private_endpoint_connections", b"sites_slots_private_endpoint_connections", "sites_slots_public_certificates", b"sites_slots_public_certificates", "sites_slots_siteextensions", b"sites_slots_siteextensions", "sites_slots_sourcecontrols", b"sites_slots_sourcecontrols", "sites_slots_virtual_network_connections", b"sites_slots_virtual_network_connections", "storage_account_required", b"storage_account_required", "tags", b"tags", "virtual_network_subnet_id", b"virtual_network_subnet_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_affinity_enabled", b"client_affinity_enabled", "client_cert_enabled", b"client_cert_enabled", "client_cert_exclusion_paths", b"client_cert_exclusion_paths", "client_cert_mode", b"client_cert_mode", "cloning_info", b"cloning_info", "container_size", b"container_size", "custom_domain_verification_id", b"custom_domain_verification_id", "daily_memory_time_quota", b"daily_memory_time_quota", "enabled", b"enabled", "extended_location", b"extended_location", "host_name_ssl_states", b"host_name_ssl_states", "host_names_disabled", b"host_names_disabled", "hosting_environment_profile", b"hosting_environment_profile", "https_only", b"https_only", "hyper_v", b"hyper_v", "identity", b"identity", "is_xenon", b"is_xenon", "key_vault_reference_identity", b"key_vault_reference_identity", "kind", b"kind", "location", b"location", "name", b"name", "public_network_access", b"public_network_access", "redundancy_mode", b"redundancy_mode", "reserved", b"reserved", "resource_info", b"resource_info", "scm_site_also_stopped", b"scm_site_also_stopped", "server_farm_id", b"server_farm_id", "site_config", b"site_config", "sites_slots_basic_publishing_credentials_policies", b"sites_slots_basic_publishing_credentials_policies", "sites_slots_config", b"sites_slots_config", "sites_slots_deployments", b"sites_slots_deployments", "sites_slots_domain_ownership_identifiers", b"sites_slots_domain_ownership_identifiers", "sites_slots_extensions", b"sites_slots_extensions", "sites_slots_functions", b"sites_slots_functions", "sites_slots_host_name_bindings", b"sites_slots_host_name_bindings", "sites_slots_hybridconnection", b"sites_slots_hybridconnection", "sites_slots_network_config", b"sites_slots_network_config", "sites_slots_premieraddons", b"sites_slots_premieraddons", "sites_slots_private_access", b"sites_slots_private_access", "sites_slots_private_endpoint_connections", b"sites_slots_private_endpoint_connections", "sites_slots_public_certificates", b"sites_slots_public_certificates", "sites_slots_siteextensions", b"sites_slots_siteextensions", "sites_slots_sourcecontrols", b"sites_slots_sourcecontrols", "sites_slots_virtual_network_connections", b"sites_slots_virtual_network_connections", "storage_account_required", b"storage_account_required", "tags", b"tags", "virtual_network_subnet_id", b"virtual_network_subnet_id", "vnet_content_share_enabled", b"vnet_content_share_enabled", "vnet_image_pull_enabled", b"vnet_image_pull_enabled", "vnet_route_all_enabled", b"vnet_route_all_enabled"]) -> None: ...
 
 global___SitesSlots = SitesSlots
 
 @typing_extensions.final
 class SitesSiteextensions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -2140,68 +2217,24 @@
 
 global___SitesFunctions = SitesFunctions
 
 @typing_extensions.final
 class SitesExtensions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
-    class SetParametersEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
-
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    KIND_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    APP_OFFLINE_FIELD_NUMBER: builtins.int
-    CONNECTION_STRING_FIELD_NUMBER: builtins.int
-    DB_TYPE_FIELD_NUMBER: builtins.int
-    PACKAGE_URI_FIELD_NUMBER: builtins.int
-    SET_PARAMETERS_FIELD_NUMBER: builtins.int
-    SET_PARAMETERS_XML_FILE_URI_FIELD_NUMBER: builtins.int
-    SKIP_APP_DATA_FIELD_NUMBER: builtins.int
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
-    kind: builtins.str
-    name: builtins.str
-    app_offline: builtins.bool
-    connection_string: builtins.str
-    db_type: builtins.str
-    package_uri: builtins.str
-    @property
-    def set_parameters(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    set_parameters_xml_file_uri: builtins.str
-    skip_app_data: builtins.bool
     def __init__(
         self,
         *,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
-        kind: builtins.str = ...,
-        name: builtins.str = ...,
-        app_offline: builtins.bool = ...,
-        connection_string: builtins.str = ...,
-        db_type: builtins.str = ...,
-        package_uri: builtins.str = ...,
-        set_parameters: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
-        set_parameters_xml_file_uri: builtins.str = ...,
-        skip_app_data: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_offline", b"app_offline", "connection_string", b"connection_string", "db_type", b"db_type", "kind", b"kind", "name", b"name", "package_uri", b"package_uri", "resource_info", b"resource_info", "set_parameters", b"set_parameters", "set_parameters_xml_file_uri", b"set_parameters_xml_file_uri", "skip_app_data", b"skip_app_data"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> None: ...
 
 global___SitesExtensions = SitesExtensions
 
 @typing_extensions.final
 class SitesDomainOwnershipIdentifiers(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -2412,21 +2445,25 @@
     HOSTING_ENVIRONMENT_PROFILE_FIELD_NUMBER: builtins.int
     HOST_NAMES_DISABLED_FIELD_NUMBER: builtins.int
     HOST_NAME_SSL_STATES_FIELD_NUMBER: builtins.int
     HTTPS_ONLY_FIELD_NUMBER: builtins.int
     HYPER_V_FIELD_NUMBER: builtins.int
     IS_XENON_FIELD_NUMBER: builtins.int
     KEY_VAULT_REFERENCE_IDENTITY_FIELD_NUMBER: builtins.int
+    PUBLIC_NETWORK_ACCESS_FIELD_NUMBER: builtins.int
     REDUNDANCY_MODE_FIELD_NUMBER: builtins.int
     RESERVED_FIELD_NUMBER: builtins.int
     SCM_SITE_ALSO_STOPPED_FIELD_NUMBER: builtins.int
     SERVER_FARM_ID_FIELD_NUMBER: builtins.int
     SITE_CONFIG_FIELD_NUMBER: builtins.int
     STORAGE_ACCOUNT_REQUIRED_FIELD_NUMBER: builtins.int
     VIRTUAL_NETWORK_SUBNET_ID_FIELD_NUMBER: builtins.int
+    VNET_CONTENT_SHARE_ENABLED_FIELD_NUMBER: builtins.int
+    VNET_IMAGE_PULL_ENABLED_FIELD_NUMBER: builtins.int
+    VNET_ROUTE_ALL_ENABLED_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     SITES_BASIC_PUBLISHING_CREDENTIALS_POLICIES_FIELD_NUMBER: builtins.int
     SITES_DOMAIN_OWNERSHIP_IDENTIFIERS_FIELD_NUMBER: builtins.int
     SITES_EXTENSIONS_FIELD_NUMBER: builtins.int
     SITES_FUNCTIONS_FIELD_NUMBER: builtins.int
     SITES_HYBRIDCONNECTION_FIELD_NUMBER: builtins.int
     SITES_MIGRATE_FIELD_NUMBER: builtins.int
@@ -2463,22 +2500,26 @@
     host_names_disabled: builtins.bool
     @property
     def host_name_ssl_states(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HostNameSslState]: ...
     https_only: builtins.bool
     hyper_v: builtins.bool
     is_xenon: builtins.bool
     key_vault_reference_identity: builtins.str
+    public_network_access: builtins.str
     redundancy_mode: builtins.str
     reserved: builtins.bool
     scm_site_also_stopped: builtins.bool
     server_farm_id: builtins.str
     @property
     def site_config(self) -> global___SiteConfig: ...
     storage_account_required: builtins.bool
     virtual_network_subnet_id: builtins.str
+    vnet_content_share_enabled: builtins.bool
+    vnet_image_pull_enabled: builtins.bool
+    vnet_route_all_enabled: builtins.bool
     @property
     def tags(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     @property
     def sites_basic_publishing_credentials_policies(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SitesBasicPublishingCredentialsPolicies]: ...
     @property
     def sites_domain_ownership_identifiers(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SitesDomainOwnershipIdentifiers]: ...
     @property
@@ -2528,21 +2569,25 @@
         hosting_environment_profile: global___HostingEnvironmentProfile | None = ...,
         host_names_disabled: builtins.bool = ...,
         host_name_ssl_states: collections.abc.Iterable[global___HostNameSslState] | None = ...,
         https_only: builtins.bool = ...,
         hyper_v: builtins.bool = ...,
         is_xenon: builtins.bool = ...,
         key_vault_reference_identity: builtins.str = ...,
+        public_network_access: builtins.str = ...,
         redundancy_mode: builtins.str = ...,
         reserved: builtins.bool = ...,
         scm_site_also_stopped: builtins.bool = ...,
         server_farm_id: builtins.str = ...,
         site_config: global___SiteConfig | None = ...,
         storage_account_required: builtins.bool = ...,
         virtual_network_subnet_id: builtins.str = ...,
+        vnet_content_share_enabled: builtins.bool = ...,
+        vnet_image_pull_enabled: builtins.bool = ...,
+        vnet_route_all_enabled: builtins.bool = ...,
         tags: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         sites_basic_publishing_credentials_policies: collections.abc.Iterable[global___SitesBasicPublishingCredentialsPolicies] | None = ...,
         sites_domain_ownership_identifiers: collections.abc.Iterable[global___SitesDomainOwnershipIdentifiers] | None = ...,
         sites_extensions: collections.abc.Iterable[global___SitesExtensions] | None = ...,
         sites_functions: collections.abc.Iterable[global___SitesFunctions] | None = ...,
         sites_hybridconnection: collections.abc.Iterable[global___SitesHybridconnection] | None = ...,
         sites_migrate: collections.abc.Iterable[global___SitesMigrate] | None = ...,
@@ -2553,15 +2598,15 @@
         sites_public_certificates: collections.abc.Iterable[global___SitesPublicCertificates] | None = ...,
         sites_siteextensions: collections.abc.Iterable[global___SitesSiteextensions] | None = ...,
         sites_slots: collections.abc.Iterable[global___SitesSlots] | None = ...,
         sites_sourcecontrols: collections.abc.Iterable[global___SitesSourcecontrols] | None = ...,
         sites_virtual_network_connections: collections.abc.Iterable[global___SitesVirtualNetworkConnections] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["cloning_info", b"cloning_info", "extended_location", b"extended_location", "hosting_environment_profile", b"hosting_environment_profile", "identity", b"identity", "resource_info", b"resource_info", "site_config", b"site_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_affinity_enabled", b"client_affinity_enabled", "client_cert_enabled", b"client_cert_enabled", "client_cert_exclusion_paths", b"client_cert_exclusion_paths", "client_cert_mode", b"client_cert_mode", "cloning_info", b"cloning_info", "container_size", b"container_size", "custom_domain_verification_id", b"custom_domain_verification_id", "daily_memory_time_quota", b"daily_memory_time_quota", "enabled", b"enabled", "extended_location", b"extended_location", "host_name_ssl_states", b"host_name_ssl_states", "host_names_disabled", b"host_names_disabled", "hosting_environment_profile", b"hosting_environment_profile", "https_only", b"https_only", "hyper_v", b"hyper_v", "identity", b"identity", "is_xenon", b"is_xenon", "key_vault_reference_identity", b"key_vault_reference_identity", "kind", b"kind", "location", b"location", "name", b"name", "redundancy_mode", b"redundancy_mode", "reserved", b"reserved", "resource_info", b"resource_info", "scm_site_also_stopped", b"scm_site_also_stopped", "server_farm_id", b"server_farm_id", "site_config", b"site_config", "sites_basic_publishing_credentials_policies", b"sites_basic_publishing_credentials_policies", "sites_domain_ownership_identifiers", b"sites_domain_ownership_identifiers", "sites_extensions", b"sites_extensions", "sites_functions", b"sites_functions", "sites_hybridconnection", b"sites_hybridconnection", "sites_migrate", b"sites_migrate", "sites_network_config", b"sites_network_config", "sites_premieraddons", b"sites_premieraddons", "sites_private_access", b"sites_private_access", "sites_private_endpoint_connections", b"sites_private_endpoint_connections", "sites_public_certificates", b"sites_public_certificates", "sites_siteextensions", b"sites_siteextensions", "sites_slots", b"sites_slots", "sites_sourcecontrols", b"sites_sourcecontrols", "sites_virtual_network_connections", b"sites_virtual_network_connections", "storage_account_required", b"storage_account_required", "tags", b"tags", "virtual_network_subnet_id", b"virtual_network_subnet_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_affinity_enabled", b"client_affinity_enabled", "client_cert_enabled", b"client_cert_enabled", "client_cert_exclusion_paths", b"client_cert_exclusion_paths", "client_cert_mode", b"client_cert_mode", "cloning_info", b"cloning_info", "container_size", b"container_size", "custom_domain_verification_id", b"custom_domain_verification_id", "daily_memory_time_quota", b"daily_memory_time_quota", "enabled", b"enabled", "extended_location", b"extended_location", "host_name_ssl_states", b"host_name_ssl_states", "host_names_disabled", b"host_names_disabled", "hosting_environment_profile", b"hosting_environment_profile", "https_only", b"https_only", "hyper_v", b"hyper_v", "identity", b"identity", "is_xenon", b"is_xenon", "key_vault_reference_identity", b"key_vault_reference_identity", "kind", b"kind", "location", b"location", "name", b"name", "public_network_access", b"public_network_access", "redundancy_mode", b"redundancy_mode", "reserved", b"reserved", "resource_info", b"resource_info", "scm_site_also_stopped", b"scm_site_also_stopped", "server_farm_id", b"server_farm_id", "site_config", b"site_config", "sites_basic_publishing_credentials_policies", b"sites_basic_publishing_credentials_policies", "sites_domain_ownership_identifiers", b"sites_domain_ownership_identifiers", "sites_extensions", b"sites_extensions", "sites_functions", b"sites_functions", "sites_hybridconnection", b"sites_hybridconnection", "sites_migrate", b"sites_migrate", "sites_network_config", b"sites_network_config", "sites_premieraddons", b"sites_premieraddons", "sites_private_access", b"sites_private_access", "sites_private_endpoint_connections", b"sites_private_endpoint_connections", "sites_public_certificates", b"sites_public_certificates", "sites_siteextensions", b"sites_siteextensions", "sites_slots", b"sites_slots", "sites_sourcecontrols", b"sites_sourcecontrols", "sites_virtual_network_connections", b"sites_virtual_network_connections", "storage_account_required", b"storage_account_required", "tags", b"tags", "virtual_network_subnet_id", b"virtual_network_subnet_id", "vnet_content_share_enabled", b"vnet_content_share_enabled", "vnet_image_pull_enabled", b"vnet_image_pull_enabled", "vnet_route_all_enabled", b"vnet_route_all_enabled"]) -> None: ...
 
 global___Sites = Sites
 
 @typing_extensions.final
 class SiteConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -4034,32 +4079,23 @@
 global___Capability = Capability
 
 @typing_extensions.final
 class HostingEnvironmentsConfigurations(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    KIND_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    ALLOW_NEW_PRIVATE_ENDPOINT_CONNECTIONS_FIELD_NUMBER: builtins.int
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
-    kind: builtins.str
-    name: builtins.str
-    allow_new_private_endpoint_connections: builtins.bool
     def __init__(
         self,
         *,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
-        kind: builtins.str = ...,
-        name: builtins.str = ...,
-        allow_new_private_endpoint_connections: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allow_new_private_endpoint_connections", b"allow_new_private_endpoint_connections", "kind", b"kind", "name", b"name", "resource_info", b"resource_info"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> None: ...
 
 global___HostingEnvironmentsConfigurations = HostingEnvironmentsConfigurations
 
 @typing_extensions.final
 class HostingEnvironments(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -4080,20 +4116,23 @@
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
     KIND_FIELD_NUMBER: builtins.int
     LOCATION_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     CLUSTER_SETTINGS_FIELD_NUMBER: builtins.int
+    CUSTOM_DNS_SUFFIX_CONFIGURATION_FIELD_NUMBER: builtins.int
     DEDICATED_HOST_COUNT_FIELD_NUMBER: builtins.int
     DNS_SUFFIX_FIELD_NUMBER: builtins.int
     FRONT_END_SCALE_FACTOR_FIELD_NUMBER: builtins.int
     INTERNAL_LOAD_BALANCING_MODE_FIELD_NUMBER: builtins.int
     IPSSL_ADDRESS_COUNT_FIELD_NUMBER: builtins.int
     MULTI_SIZE_FIELD_NUMBER: builtins.int
+    NETWORKING_CONFIGURATION_FIELD_NUMBER: builtins.int
+    UPGRADE_PREFERENCE_FIELD_NUMBER: builtins.int
     USER_WHITELISTED_IP_RANGES_FIELD_NUMBER: builtins.int
     VIRTUAL_NETWORK_FIELD_NUMBER: builtins.int
     ZONE_REDUNDANT_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     HOSTING_ENVIRONMENTS_CONFIGURATIONS_FIELD_NUMBER: builtins.int
     HOSTING_ENVIRONMENTS_MULTI_ROLE_POOLS_FIELD_NUMBER: builtins.int
     HOSTING_ENVIRONMENTS_PRIVATE_ENDPOINT_CONNECTIONS_FIELD_NUMBER: builtins.int
@@ -4101,21 +4140,26 @@
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     kind: builtins.str
     location: builtins.str
     name: builtins.str
     @property
     def cluster_settings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NameValuePair]: ...
+    @property
+    def custom_dns_suffix_configuration(self) -> global___CustomDnsSuffixConfiguration: ...
     dedicated_host_count: builtins.int
     dns_suffix: builtins.str
     front_end_scale_factor: builtins.int
     internal_load_balancing_mode: builtins.str
     ipssl_address_count: builtins.int
     multi_size: builtins.str
     @property
+    def networking_configuration(self) -> global___AseV3NetworkingConfiguration: ...
+    upgrade_preference: builtins.str
+    @property
     def user_whitelisted_ip_ranges(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def virtual_network(self) -> global___VirtualNetworkProfile: ...
     zone_redundant: builtins.bool
     @property
     def tags(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     @property
@@ -4130,31 +4174,34 @@
         self,
         *,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
         kind: builtins.str = ...,
         location: builtins.str = ...,
         name: builtins.str = ...,
         cluster_settings: collections.abc.Iterable[global___NameValuePair] | None = ...,
+        custom_dns_suffix_configuration: global___CustomDnsSuffixConfiguration | None = ...,
         dedicated_host_count: builtins.int = ...,
         dns_suffix: builtins.str = ...,
         front_end_scale_factor: builtins.int = ...,
         internal_load_balancing_mode: builtins.str = ...,
         ipssl_address_count: builtins.int = ...,
         multi_size: builtins.str = ...,
+        networking_configuration: global___AseV3NetworkingConfiguration | None = ...,
+        upgrade_preference: builtins.str = ...,
         user_whitelisted_ip_ranges: collections.abc.Iterable[builtins.str] | None = ...,
         virtual_network: global___VirtualNetworkProfile | None = ...,
         zone_redundant: builtins.bool = ...,
         tags: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         hosting_environments_configurations: collections.abc.Iterable[global___HostingEnvironmentsConfigurations] | None = ...,
         hosting_environments_multi_role_pools: collections.abc.Iterable[global___HostingEnvironmentsMultiRolePools] | None = ...,
         hosting_environments_private_endpoint_connections: collections.abc.Iterable[global___HostingEnvironmentsPrivateEndpointConnections] | None = ...,
         hosting_environments_worker_pools: collections.abc.Iterable[global___HostingEnvironmentsWorkerPools] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "virtual_network", b"virtual_network"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cluster_settings", b"cluster_settings", "dedicated_host_count", b"dedicated_host_count", "dns_suffix", b"dns_suffix", "front_end_scale_factor", b"front_end_scale_factor", "hosting_environments_configurations", b"hosting_environments_configurations", "hosting_environments_multi_role_pools", b"hosting_environments_multi_role_pools", "hosting_environments_private_endpoint_connections", b"hosting_environments_private_endpoint_connections", "hosting_environments_worker_pools", b"hosting_environments_worker_pools", "internal_load_balancing_mode", b"internal_load_balancing_mode", "ipssl_address_count", b"ipssl_address_count", "kind", b"kind", "location", b"location", "multi_size", b"multi_size", "name", b"name", "resource_info", b"resource_info", "tags", b"tags", "user_whitelisted_ip_ranges", b"user_whitelisted_ip_ranges", "virtual_network", b"virtual_network", "zone_redundant", b"zone_redundant"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["custom_dns_suffix_configuration", b"custom_dns_suffix_configuration", "networking_configuration", b"networking_configuration", "resource_info", b"resource_info", "virtual_network", b"virtual_network"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cluster_settings", b"cluster_settings", "custom_dns_suffix_configuration", b"custom_dns_suffix_configuration", "dedicated_host_count", b"dedicated_host_count", "dns_suffix", b"dns_suffix", "front_end_scale_factor", b"front_end_scale_factor", "hosting_environments_configurations", b"hosting_environments_configurations", "hosting_environments_multi_role_pools", b"hosting_environments_multi_role_pools", "hosting_environments_private_endpoint_connections", b"hosting_environments_private_endpoint_connections", "hosting_environments_worker_pools", b"hosting_environments_worker_pools", "internal_load_balancing_mode", b"internal_load_balancing_mode", "ipssl_address_count", b"ipssl_address_count", "kind", b"kind", "location", b"location", "multi_size", b"multi_size", "name", b"name", "networking_configuration", b"networking_configuration", "resource_info", b"resource_info", "tags", b"tags", "upgrade_preference", b"upgrade_preference", "user_whitelisted_ip_ranges", b"user_whitelisted_ip_ranges", "virtual_network", b"virtual_network", "zone_redundant", b"zone_redundant"]) -> None: ...
 
 global___HostingEnvironments = HostingEnvironments
 
 @typing_extensions.final
 class VirtualNetworkProfile(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -4169,14 +4216,65 @@
         subnet: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "subnet", b"subnet"]) -> None: ...
 
 global___VirtualNetworkProfile = VirtualNetworkProfile
 
 @typing_extensions.final
+class AseV3NetworkingConfiguration(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    KIND_FIELD_NUMBER: builtins.int
+    ALLOW_NEW_PRIVATE_ENDPOINT_CONNECTIONS_FIELD_NUMBER: builtins.int
+    FTP_ENABLED_FIELD_NUMBER: builtins.int
+    INBOUND_IP_ADDRESS_OVERRIDE_FIELD_NUMBER: builtins.int
+    REMOTE_DEBUG_ENABLED_FIELD_NUMBER: builtins.int
+    kind: builtins.str
+    allow_new_private_endpoint_connections: builtins.bool
+    ftp_enabled: builtins.bool
+    inbound_ip_address_override: builtins.str
+    remote_debug_enabled: builtins.bool
+    def __init__(
+        self,
+        *,
+        kind: builtins.str = ...,
+        allow_new_private_endpoint_connections: builtins.bool = ...,
+        ftp_enabled: builtins.bool = ...,
+        inbound_ip_address_override: builtins.str = ...,
+        remote_debug_enabled: builtins.bool = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["allow_new_private_endpoint_connections", b"allow_new_private_endpoint_connections", "ftp_enabled", b"ftp_enabled", "inbound_ip_address_override", b"inbound_ip_address_override", "kind", b"kind", "remote_debug_enabled", b"remote_debug_enabled"]) -> None: ...
+
+global___AseV3NetworkingConfiguration = AseV3NetworkingConfiguration
+
+@typing_extensions.final
+class CustomDnsSuffixConfiguration(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    KIND_FIELD_NUMBER: builtins.int
+    CERTIFICATE_URL_FIELD_NUMBER: builtins.int
+    DNS_SUFFIX_FIELD_NUMBER: builtins.int
+    KEY_VAULT_REFERENCE_IDENTITY_FIELD_NUMBER: builtins.int
+    kind: builtins.str
+    certificate_url: builtins.str
+    dns_suffix: builtins.str
+    key_vault_reference_identity: builtins.str
+    def __init__(
+        self,
+        *,
+        kind: builtins.str = ...,
+        certificate_url: builtins.str = ...,
+        dns_suffix: builtins.str = ...,
+        key_vault_reference_identity: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["certificate_url", b"certificate_url", "dns_suffix", b"dns_suffix", "key_vault_reference_identity", b"key_vault_reference_identity", "kind", b"kind"]) -> None: ...
+
+global___CustomDnsSuffixConfiguration = CustomDnsSuffixConfiguration
+
+@typing_extensions.final
 class NameValuePair(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     name: builtins.str
     value: builtins.str
```

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_access_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_access_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_access_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_access_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_active_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_active_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_active_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_active_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apigee_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apigee_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apigee_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apigee_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apikeys_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apikeys_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_app_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_app_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_app_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_artifact_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_artifact_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_assured_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_assured_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_assured_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_assured_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigquery_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigquery_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigtable_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigtable_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_billing_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_billing_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_billing_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_billing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_binary_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_binary_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_binary_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_binary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_certificate_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_certificate_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_certificate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloud_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloud_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloud_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloud_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudiot_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudiot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_composer_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_composer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_composer_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_composer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_address_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_address_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_attached_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_attached_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_backend_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_backend_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_disk_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_disk_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_external_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_external_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_global_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_global_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ha_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ha_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_health_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_health_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_http_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_http_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_https_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_https_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_image_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_image_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_instance_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_managed_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_managed_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_network_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_network_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_node_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_node_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_packet_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_packet_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_per_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_per_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_project_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_project_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_region_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_region_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_resource_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_route_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_route_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_router_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_router_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_security_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_security_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_service_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_shared_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_shared_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_target_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_target_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_url_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_url_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_container_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_container_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_container_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_data_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_data_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_data_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataflow_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataflow_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataplex_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataplex_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataproc_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataproc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_datastore_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_datastore_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_datastore_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_datastore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_deployment_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_deployment_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dialogflow_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dialogflow_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dns_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dns_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_dns_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_dns_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_document_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_document_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_document_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_document_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_endpoints_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_endpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_essential_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_essential_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_essential_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_essential_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_eventarc_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_eventarc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_filestore_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_filestore_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_filestore_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_filestore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firebaserules_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firebaserules_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firestore_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firestore_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_firestore_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_firestore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_folder_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_folder_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_folder_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_folder_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_game_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_game_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_game_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_game_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_gke_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_gke_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_gke_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_gke_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_healthcare_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_healthcare_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iam_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iam_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iam_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iap_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iap_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_iap_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_iap_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_identity_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_identity_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_identity_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_identity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_kms_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_kms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_kms_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_kms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_logging_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_logging_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_logging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_memcache_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_memcache_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_memcache_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_memcache_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_ml_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_ml_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_ml_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_ml_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_monitoring_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_network_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_network_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_network_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_notebooks_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_notebooks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_org_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_org_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_org_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_org_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_organization_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_organization_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_organization_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_organization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_os_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_os_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_os_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_os_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_privateca_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_privateca_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_privateca_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_privateca_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_project_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_project_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_project_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_pubsub_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_pubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_recaptcha_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_recaptcha_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_redis_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_redis_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_redis_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_redis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_resource_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_resource_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_scc_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_scc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_scc_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_scc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_secret_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_secret_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_secret_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_secret_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_service_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_service_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_service_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_spanner_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_spanner_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_spanner_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_spanner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sql_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sql_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_sql_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_sql_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_storage_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_storage_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_storage_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_storage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tags_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tags_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tags_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tags_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tpu_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tpu_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_tpu_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_tpu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vertex_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vertex_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vertex_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vertex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vpc_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vpc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_vpc_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_vpc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_workflows_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_workflows_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/gcp/gcp_workflows_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/gcp/gcp_workflows_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/shared/shared_pb2.py` & `oak9_tython-1.0.3/oak9/tython/models/shared/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/shared/shared_pb2.pyi` & `oak9_tython-1.0.3/oak9/tython/models/shared/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/models/shared/shared_pb2_grpc.py` & `oak9_tython-1.0.3/oak9/tython/models/shared/shared_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/oak9/tython/runner.py` & `oak9_tython-1.0.3/oak9/tython/runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import sys
 from typing import Protocol, runtime_checkable, Set, Optional, List
 from colorama import Fore, Style, init
 from core.services.runner_input_service import RunnerInputService
 
 from core.bp_metadata_utils.customer_blueprint_repo import CustomerBlueprintRepo
@@ -32,21 +33,30 @@
     print(f"    Running oak9's Python Framework                        ")
     print(f"************************************************************************{Style.RESET_ALL}")
 
 
     try:
         init(convert=True) # Ensure that colorama works on Windows
 
-        path = None
-        # TODO: pass arguments here from CLI for specific CLI commands
+        argsPath = None
+        
         if len(argv) > 0:
-            path = argv[0]
-
-        #TODO: get request_id as argument
-        request_id = "ABC123"
+            argsPath = argv[0]
+        
+        argsObj = None
+        try:
+            argsFile = open(argsPath)
+            argsObj = json.load(argsFile)
+            argsFile.close()
+        except:
+            # TODO: CLOUD-9058 save back a JSON instead with understandable errors for CLI to deal with
+            print("Runner arguments not found or could not be understood.")
+            return
+        
+        path = argsObj["blueprint_package_path"]
         
         runner = Runner()
 
         if path:
             blueprint_dir = path
         else:
             # TODO: We could default to /blueprints here
@@ -55,16 +65,20 @@
         findings = set()
 
         blueprint_repo = CustomerBlueprintRepo(path)
 
         # TODO: make this conditional on a CLI command
         blueprint_repo.print_blueprint_summary()
 
+        # Verify config/credentials for runner endpoint
+
         # Fetch runner input data
-        runner_input = RunnerInputService.fetch_runner_input(request_id)
+        runner_inputs = RunnerInputService.fetch_runner_input()
+
+        # Runner input available?
 
         # TODO: initialize blueprint properly
         '''
         Run all blueprints
         '''
         print(f"{Fore.LIGHTBLACK_EX}************************************************************************\n"
               f"    {Fore.BLUE}Running Blueprints{Style.RESET_ALL}\n"
@@ -74,20 +88,24 @@
         # TODO: filter out import of base Blueprint class
         blueprint_classes = []
         for path in blueprint_repo.blueprint_file_paths:
             blueprint_classes.extend(get_blueprint_classes(path))
 
         # Run each blueprint
         for blueprint in blueprint_classes:
-            customer_blueprint = blueprint[1](graph=runner_input.graph)
-            # TODO: check usage guidelines to see if findings should be reported
-            bp_findings = runner.run(customer_blueprint)
-            print(f"[✓] Successfully ran checks in {blueprint[0]}")
-            if bp_findings:
-                findings.update(bp_findings)
+            for runner_input in runner_inputs:
+                customer_blueprint = blueprint[1](graph=runner_input.graph)
+                # TODO: check usage guidelines to see if findings should be reported
+                bp_findings = runner.run(customer_blueprint)
+                print(f"[✓] Successfully ran checks in {blueprint[0]}")
+                if bp_findings:
+                    for finding in bp_findings:
+                        finding.req_id = runner_input.meta_info.resource_id
+                        finding.req_name = runner_input.meta_info.resource_name
+                    findings.update(bp_findings)
 
         # TODO: send gaps to validation broker for the apply command
         print(f"\n{Fore.LIGHTBLACK_EX}************************************************************************\n"
               f"    {Fore.BLUE}Found {Style.BRIGHT}{len(findings)}{Style.NORMAL} Findings{Style.RESET_ALL}\n"
               f"{Fore.LIGHTBLACK_EX}************************************************************************{Style.RESET_ALL}")
         for finding in findings:
             print(finding)
```

### Comparing `oak9_tython-1.0.2/oak9_tython.egg-info/PKG-INFO` & `oak9_tython-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oak9-tython
-Version: 1.0.2
+Name: oak9_tython
+Version: 1.0.3
 Author: ['Claudio Balbin <cbalbin@oak9.io>', 'Brandon Nicoll <bnicoll@oak9.io>']
 Project-URL: Homepage, https://github.com/oak9io/tython
 Project-URL: Bug Tracker, https://github.com/oak9io/tython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `oak9_tython-1.0.2/oak9_tython.egg-info/SOURCES.txt` & `oak9_tython-1.0.3/oak9_tython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.2/setup.py` & `oak9_tython-1.0.3/setup.py`

 * *Files identical despite different names*

