# Comparing `tmp/openscap-report-0.2.2.tar.gz` & `tmp/openscap-report-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openscap-report-0.2.2.tar", last modified: Tue Mar 28 12:59:48 2023, max compression
+gzip compressed data, was "openscap-report-0.2.3.tar", last modified: Fri Apr 14 09:26:41 2023, max compression
```

## Comparing `openscap-report-0.2.2.tar` & `openscap-report-0.2.3.tar`

### file list

```diff
@@ -1,229 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.334797 openscap-report-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-28 12:59:37.000000 openscap-report-0.2.2/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-03-28 12:59:37.000000 openscap-report-0.2.2/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-28 12:59:37.000000 openscap-report-0.2.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-03-28 12:59:37.000000 openscap-report-0.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-03-28 12:59:37.000000 openscap-report-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-28 12:59:37.000000 openscap-report-0.2.2/LICENSE.spdx
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-28 12:59:37.000000 openscap-report-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-28 12:59:48.334797 openscap-report-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-28 12:59:37.000000 openscap-report-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.250796 openscap-report-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/README
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.246796 openscap-report-0.2.2/docs/exts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.250796 openscap-report-0.2.2/docs/exts/sphinxarg/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/exts/sphinxarg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/exts/sphinxarg/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/exts/sphinxarg/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/exts/sphinxarg/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.250796 openscap-report-0.2.2/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/manual/instalation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/manual/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.254797 openscap-report-0.2.2/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/modules/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/modules/openscap_report.report_generators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/modules/openscap_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/modules/openscap_report.scap_results_parser.data_structures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/modules/openscap_report.scap_results_parser.parsers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/modules/openscap_report.scap_results_parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/oscap-report.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-28 12:59:37.000000 openscap-report-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.254797 openscap-report-0.2.2/openscap_report/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/debug_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.254797 openscap-report-0.2.2/openscap_report/report_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.258797 openscap-report-0.2.2/openscap_report/report_generators/html_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.246796 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.246796 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.258797 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/fonts/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   102224 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    79100 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.258797 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/pficon/
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/base_report.html
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/cpe_graph.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.258797 openscap-report-0.2.2/openscap_report/report_generators/html_templates/css/
--rw-r--r--   0 runner    (1001) docker     (123)  1413415 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/css/patternfly.css
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/evaluation_characteristics.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.258797 openscap-report-0.2.2/openscap_report/report_generators/html_templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/js/debug_script.js
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/js/interactive_script.js
--rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/oval_definition_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/oval_graph.html
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/profile_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/remedations.html
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/rule_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/rule_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/rules_overview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/score_bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/search_input.html
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/severity_of_failed_rules.html
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/summary_banner.html
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/html_templates/template_report.html
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/old_style_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/report_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.262796 openscap-report-0.2.2/openscap_report/report_generators/xsl/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-branding.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-references.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    55343 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-report-impl.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-report.xsl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.262796 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json
--rw-r--r--   0 runner    (1001) docker     (123)    88498 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/openscap.css
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/openscap.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources-build.sh
--rw-r--r--   0 runner    (1001) docker     (123)   223540 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    21382 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-share.xsl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.262796 openscap-report-0.2.2/openscap_report/scap_results_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.266797 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/cpe_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/json_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/profile_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/remediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/result_of_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.266797 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/cpe_al_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/full_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/group_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_definition_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_object_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_state_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/profile_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/remediation_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/report_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/scan_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/scap_results_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.250796 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.246796 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.266797 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    45405 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    22573 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    72864 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/catalog.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.250796 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.250796 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd
--rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd
--rw-r--r--   0 runner    (1001) docker     (123)   230463 2023-03-28 12:59:37.000000 openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.254797 openscap-report-0.2.2/openscap_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-28 12:59:48.000000 openscap-report-0.2.2/openscap_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-03-28 12:59:48.000000 openscap-report-0.2.2/openscap_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:59:48.000000 openscap-report-0.2.2/openscap_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-28 12:59:48.000000 openscap-report-0.2.2/openscap_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:59:48.000000 openscap-report-0.2.2/openscap_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 12:59:48.000000 openscap-report-0.2.2/openscap_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-28 12:59:48.000000 openscap-report-0.2.2/openscap_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:59:37.000000 openscap-report-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:59:48.334797 openscap-report-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-28 12:59:37.000000 openscap-report-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.270797 openscap-report-0.2.2/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/integration_tests/test_basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/integration_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/integration_tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/json_schema_of_report.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/smoke.fmf
--rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/smoke.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.334797 openscap-report-0.2.2/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123) 12129838 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf-container.xml
--rw-r--r--   0 runner    (1001) docker     (123) 23777754 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf-dangling-reference-to.xml
--rw-r--r--   0 runner    (1001) docker     (123) 19008654 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf-report.xml
--rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf-with-removed-info.xml
--rw-r--r--   0 runner    (1001) docker     (123)    48058 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf_cpe_check_os_platform.xml
--rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf_multi_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf_no_system_data.xml
--rw-r--r--   0 runner    (1001) docker     (123)    36477 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf_rule_and_cpe_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf_simple_rule_fail.xml
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/arf_simple_rule_pass.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/empty.xml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/plant_catalog.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.334797 openscap-report-0.2.2/tests/test_data/remediations_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt
--rw-r--r--   0 runner    (1001) docker     (123)  7631650 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/xccdf-report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/xccdf-with-removed-info.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/xccdf_multi_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/xccdf_no_system_data.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/xccdf_rule_and_cpe_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/xccdf_simple_rule_fail.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_data/xccdf_simple_rule_pass.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:48.334797 openscap-report-0.2.2/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_debug_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_full_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_json_transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_oval_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_oval_tree_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_scap_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tests/unit_tests/test_shared_static_methods_of_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-28 12:59:37.000000 openscap-report-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-04-14 09:26:29.000000 openscap-report-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 09:26:29.000000 openscap-report-0.2.3/LICENSE.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 09:26:29.000000 openscap-report-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 09:26:41.646995 openscap-report-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-14 09:26:29.000000 openscap-report-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.538993 openscap-report-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/README
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/docs/exts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.538993 openscap-report-0.2.3/docs/exts/sphinxarg/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.538993 openscap-report-0.2.3/docs/manual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.550994 openscap-report-0.2.3/docs/manual/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/about_profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44006 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/compliance_and_scoring.png
+-rw-r--r--   0 runner    (1001) docker     (123)   114896 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/cpe_aplicability_language.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79764 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/evaluation_characteristics.png
+-rw-r--r--   0 runner    (1001) docker     (123)  8589473 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/example_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1072728 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/oval.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    41993 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/remediation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   168763 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/rule_detail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50802 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/rule_overview_section.png
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.report_generators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.data_structures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/oscap-report.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/openscap_report/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/debug_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/openscap_report/report_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.558994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.558994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   102224 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    79100 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.558994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/base_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/cpe_graph.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.562994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/
+-rw-r--r--   0 runner    (1001) docker     (123)  1413415 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/patternfly.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/evaluation_characteristics.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.562994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/debug_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/interactive_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27002 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_definition_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_graph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/profile_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/remedations.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/rules_overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/score_bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/search_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/severity_of_failed_rules.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/summary_banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/template_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/old_style_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/report_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.562994 openscap-report-0.2.3/openscap_report/report_generators/xsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-branding.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-references.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    55343 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-impl.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.566994 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    88498 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources-build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)   223540 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    21382 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-share.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.566994 openscap-report-0.2.3/openscap_report/scap_results_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.570994 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/json_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/profile_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/remediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/result_of_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.574994 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/cpe_al_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/full_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/group_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_definition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_object_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_state_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/profile_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/remediation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/scan_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/scap_results_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.574994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    45405 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    22573 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    72864 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/catalog.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)   230463 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/openscap_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:26:29.000000 openscap-report-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:26:41.646995 openscap-report-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-14 09:26:29.000000 openscap-report-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.582994 openscap-report-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration.fmf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.582994 openscap-report-0.2.3/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/test_basic_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/json_schema_of_report.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/smoke.fmf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/smoke.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123) 12129838 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-container.xml
+-rw-r--r--   0 runner    (1001) docker     (123) 23777754 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-dangling-reference-to.xml
+-rw-r--r--   0 runner    (1001) docker     (123) 19008654 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-with-removed-info.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    48058 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_cpe_check_os_platform.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_multi_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_no_system_data.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    36477 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_rule_and_cpe_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_simple_rule_fail.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_simple_rule_pass.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/empty.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/plant_catalog.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/tests/test_data/remediations_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  7631650 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf-report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf-with-removed-info.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_multi_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_no_system_data.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_rule_and_cpe_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_fail.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_pass.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_cpe_al_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_debug_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_full_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_json_transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_oval_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_oval_tree_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_scap_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_shared_static_methods_of_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tox.ini
```

### Comparing `openscap-report-0.2.2/.eslintrc.yml` & `openscap-report-0.2.3/.eslintrc.yml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/.pylintrc` & `openscap-report-0.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/LICENSE` & `openscap-report-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/PKG-INFO` & `openscap-report-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openscap-report
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tool for generating report from results of oscap scan.
 Home-page: https://github.com/OpenSCAP/oscap-report
 Author: Jan Rodak
 Author-email: jrodak@redhat.com
 License: LGPL-2.1 License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 [![Code Coverage](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/badges/coverage.png?b=main)](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/?branch=main)
 [![Code Intelligence Status](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/badges/code-intelligence.svg?b=main)](https://scrutinizer-ci.com/code-intelligence)
 
 Tool for generating report from results of oscap scan.
 
 ## Installation
 
-[Learn how to install tool in the documentation.](https://openscap-report.readthedocs.io/en/latest/manual/instalation.html)
+[Learn how to install tool in the documentation.](https://openscap-report.readthedocs.io/en/latest/manual/installation.html)
 
 ## Example usage
 
 This command consumes the ARF file, which is one of the possible standardized formats for the results of SCAP-compliant scanners. You can read about generating ARF report files using OpenSCAP in the OpenSCAP User Manual. Or you can use test arf files from repository [`/tests/test_data`](https://github.com/OpenSCAP/openscap-report/tree/main/tests/test_data).
 
 ```bash
 oscap-report < ssg-fedora-ds-arf.xml > report.html
```

### Comparing `openscap-report-0.2.2/README.md` & `openscap-report-0.2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Code Coverage](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/badges/coverage.png?b=main)](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/?branch=main)
 [![Code Intelligence Status](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/badges/code-intelligence.svg?b=main)](https://scrutinizer-ci.com/code-intelligence)
 
 Tool for generating report from results of oscap scan.
 
 ## Installation
 
-[Learn how to install tool in the documentation.](https://openscap-report.readthedocs.io/en/latest/manual/instalation.html)
+[Learn how to install tool in the documentation.](https://openscap-report.readthedocs.io/en/latest/manual/installation.html)
 
 ## Example usage
 
 This command consumes the ARF file, which is one of the possible standardized formats for the results of SCAP-compliant scanners. You can read about generating ARF report files using OpenSCAP in the OpenSCAP User Manual. Or you can use test arf files from repository [`/tests/test_data`](https://github.com/OpenSCAP/openscap-report/tree/main/tests/test_data).
 
 ```bash
 oscap-report < ssg-fedora-ds-arf.xml > report.html
```

### Comparing `openscap-report-0.2.2/docs/conf.py` & `openscap-report-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/exts/sphinxarg/ext.py` & `openscap-report-0.2.3/docs/exts/sphinxarg/ext.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/exts/sphinxarg/markdown.py` & `openscap-report-0.2.3/docs/exts/sphinxarg/markdown.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/exts/sphinxarg/parser.py` & `openscap-report-0.2.3/docs/exts/sphinxarg/parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/manual/instalation.rst` & `openscap-report-0.2.3/docs/manual/installation.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/modules/openscap_report.report_generators.rst` & `openscap-report-0.2.3/docs/modules/openscap_report.report_generators.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/modules/openscap_report.rst` & `openscap-report-0.2.3/docs/modules/openscap_report.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/modules/openscap_report.scap_results_parser.data_structures.rst` & `openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.data_structures.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/modules/openscap_report.scap_results_parser.parsers.rst` & `openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.parsers.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/docs/modules/openscap_report.scap_results_parser.rst` & `openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/cli.py` & `openscap-report-0.2.3/openscap_report/cli.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/debug_settings.py` & `openscap-report-0.2.3/openscap_report/debug_settings.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html.py` & `openscap-report-0.2.3/openscap_report/report_generators/html.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 class HTMLReportGenerator(ReportGenerator):
     def __init__(self, parser):  # pylint: disable=W0231
         self.report = parser.parse_report()
         self.file_loader = FileSystemLoader(str(Path(__file__).parent / "html_templates"))
         self.env = Environment(loader=self.file_loader)
         self.env.globals['include_file_in_base64'] = self.include_file_in_base64
         self.env.filters['set_css_for_list'] = self.set_css_for_list
+        self.env.filters['to_jquery_complaint_id'] = self.to_jquery_complaint_id
         self.env.trim_blocks = True
         self.env.lstrip_blocks = True
 
     def generate_report(self, debug_setting):
         template = self.env.get_template("template_report.html")
         html_report = template.render(report=self.report, debug_setting=debug_setting)
         if debug_setting.no_minify:
@@ -52,7 +53,11 @@
         return Markup(base64_data)
 
     @staticmethod
     def set_css_for_list(data):
         out = data.replace("<ul>", "<ul class=\"pf-c-list\">")
         out = out.replace("<ol>", "<ol class=\"pf-c-list\">")
         return out
+
+    @staticmethod
+    def to_jquery_complaint_id(data):
+        return re.sub(r"\.|:", "", data)
```

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/base_report.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/base_report.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/cpe_graph.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/cpe_graph.html`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,18 @@
                 <i class="fas fa-fw fa-exclamation-triangle" aria-hidden="true"></i>
             </span>
             <span class="pf-c-helper-text__item-text"><b>{{ platform_id }} {{ platform.title }}</b></span>
         </div>
     {%- endif %}
 </div>
 {%- if rule.cpe_al -%}
-<div id="cpe_al_tree_of_rule_{{ key }}_{{ rule.rule_id | replace('.', '') }}" is_rendered="false" data='{{ platform.logical_test.as_dict() | tojson }}'></div>
+<div id="cpe_al_tree_of_rule_{{ key }}_{{ rule.rule_id | to_jquery_complaint_id }}" is_rendered="false" data='{{ platform.logical_test.as_dict() | tojson }}'></div>
 {%- endif %}
 {%- if rule.cpe_oval_dict -%}
-<div id="cpe_tree_of_rule_{{ rule.rule_id | replace('.', '') }}" is_rendered="false" data='{{ platform.as_dict() | tojson }}'></div>
+<div id="cpe_tree_of_rule_{{ rule.rule_id | to_jquery_complaint_id }}" is_rendered="false" data='{{ platform.as_dict() | tojson }}'></div>
 {%- endif %}
 </td>
 </tr>
 {% endfor %}
 {%- endif %}
 {% endfor %}
 {%- endif %}
```

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/css/patternfly.css` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/patternfly.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/css/style.css` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/style.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/evaluation_characteristics.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/evaluation_characteristics.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/js/debug_script.js` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/debug_script.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/js/interactive_script.js` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/interactive_script.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 /*
  * Copyright 2022, Red Hat, Inc.
  * SPDX-License-Identifier: LGPL-2.1-or-later
  */
 
 // eslint-disable-next-line no-extend-native
 String.prototype.asJqueryComplaintId = function() {
-    return this.replace(/\./ug, "");
+    return this.replace(/\.|:/ug, "");
 };
 
 // User events methods
 
 function toggle_OVAL_operator() { // eslint-disable-line no-unused-vars
     const operator_parent = this.parentNode.parentNode;
     operator_parent.classList.toggle('pf-m-expanded');
```

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/oval_definition_detail.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_definition_detail.html`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,21 @@
     <td role="cell">
         <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
         <p class="pf-c-table__text">{{ rule.oval_definition_id }}</p>
         </div></div>
     </td>
 </tr>
 <tr role="row">
+    <th class="pf-m-fit-content" role="rowheader" scope="row"><b>Class:</b></th>
+    <td role="cell">
+        <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
+        <p class="pf-c-table__text">{{ rule.oval_definition.definition_class }}</p></div></div>
+    </td>
+</tr>
+<tr role="row">
     <th class="pf-m-fit-content" role="rowheader" scope="row"><b>Title:</b></th>
     <td role="cell">
         <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
         <p class="pf-c-table__text">{{ rule.oval_definition.title }}</p></div></div>
     </td>
 </tr>
 <tr role="row">
@@ -29,14 +36,21 @@
 <tr role="row">
     <th class="pf-m-fit-content" role="rowheader" scope="row"><b>Description:</b></th>
     <td role="cell">
         <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
         <p class="pf-c-table__text">{{ rule.oval_definition.description }}</p></div></div>
     </td>
 </tr>
+<tr role="row">
+    <th class="pf-m-fit-content" role="rowheader" scope="row"><b>Result explained:</b></th>
+    <td role="cell">
+        <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
+        <p class="pf-c-table__text">{{ rule.oval_definition.get_oval_class_description() }}</p></div></div>
+    </td>
+</tr>
 {% else %}
 <tr role="row">
     <td colspan="2" role="cell">
         <div class="pf-c-alert pf-m-warning pf-m-inline">
             <div class="pf-c-alert__icon">
                 <i class="fas fa-fw fa-exclamation-triangle" aria-hidden="true"></i>
             </div>
```

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/oval_graph.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_graph.html`

 * *Files 1% similar despite different names*

```diff
@@ -23,9 +23,9 @@
                 </span>
                 <span class="pf-c-helper-text__item-text"><b>OVAL graph of OVAL definition: {{ rule.oval_definition_id }}</b></span>
             </div>    
         {%- endif %}
     </div>
 {%- endif -%}
 {%- if rule.oval_definition.oval_tree -%}
-    <div id="oval_tree_of_rule_{{ rule.rule_id | replace('.', '') }}" is_rendered="false" data='{{ rule.oval_definition.oval_tree.as_dict() | tojson }}'></div>
+    <div id="oval_tree_of_rule_{{ rule.rule_id | to_jquery_complaint_id }}" is_rendered="false" data='{{ rule.oval_definition.oval_tree.as_dict() | tojson }}'></div>
 {%- endif %}
```

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/remedations.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/remedations.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/rule_detail.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_detail.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/rule_results.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_results.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/rules_overview.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/rules_overview.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/score_bar.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/score_bar.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/search_input.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/search_input.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/severity_of_failed_rules.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/severity_of_failed_rules.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/summary_banner.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/summary_banner.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/html_templates/template_report.html` & `openscap-report-0.2.3/openscap_report/report_generators/html_templates/template_report.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/json.py` & `openscap-report-0.2.3/openscap_report/report_generators/json.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/old_style_html.py` & `openscap-report-0.2.3/openscap_report/report_generators/old_style_html.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-branding.xsl` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-branding.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-references.xsl` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-references.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-report-impl.xsl` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-impl.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-report.xsl` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/openscap.css` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources/openscap.js` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources-build.sh` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources-build.sh`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-resources.xsl` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/report_generators/xsl/xccdf-share.xsl` & `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-share.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/__init__.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/group.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/group.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/json_transformation.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/json_transformation.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_node.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_node.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/oval_result_eval.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/profile_info.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/profile_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,10 +25,22 @@
     def as_dict(self):
         return asdict(self)
 
     def get_applicable_cpe_platforms_for_profile(self):
         return ", ".join(self.cpe_platforms_for_profile.keys())
 
     def get_cpe_platforms_that_satisfy_evaluation_target(self):
-        return ", ".join(
-            [cpe_id for cpe_id, is_satisfy in self.cpe_platforms_for_profile.items() if is_satisfy]
-        )
+        return ", ".join(self.get_list_of_cpe_platforms_that_satisfy_evaluation_target())
+
+    def get_list_of_cpe_platforms_that_satisfy_evaluation_target(self):
+        return [
+            cpe_id for cpe_id, is_satisfy in self.cpe_platforms_for_profile.items() if is_satisfy
+        ]
+
+    def deselect_rules(self, rule_ids):
+        for rule_id in rule_ids:
+            if rule_id in self.selected_rules_ids:
+                self.selected_rules_ids.remove(rule_id)
+
+    def select_rules(self, rule_ids):
+        if len(self.selected_rules_ids) > 0:
+            self.selected_rules_ids.extend(rule_ids)
```

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/remediation.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/remediation.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/report.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/report.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/result_of_scan.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/result_of_scan.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/data_structures/rule.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/rule.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     identifiers: List[Identifier] = field(default_factory=list)
     references: List[Reference] = field(default_factory=list)
     description: str = ""
     rationale: str = ""
     warnings: List[RuleWarning] = field(default_factory=list)
     platforms: List[str] = field(default_factory=list)
     oval_definition_id: str = None
+    oval_reference: str = None
     oval_definition: OvalDefinition = None
     messages: List[str] = field(default_factory=list)
     remediations: List[Remediation] = field(default_factory=list)
     cpe_oval_dict: Dict[str, Dict[str, OvalNode]] = field(default_factory=dict)
     cpe_al: Dict[str, Dict[str, Platform]] = field(default_factory=dict)
 
     def as_dict(self):
```

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/exceptions.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/namespaces.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/namespaces.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,78 +5,112 @@
 
 from .data_structures import LogicalTest, Platform
 from .exceptions import ExceptionNoCPEApplicabilityLanguage, MissingOVALResult
 from .parsers import CPEApplicabilityLanguageParser, OVALDefinitionParser
 
 
 class OVALAndCPETreeBuilder:  # pylint: disable=R0902
-    def __init__(self, root, group_parser, profile_platforms):
+    def __init__(self, root, group_parser, profile_platforms, oval_definitions_and_results_sources):
         self.profile_platforms = profile_platforms
         self.root = root
         self.group_parser = group_parser
+        self.oval_definitions_and_results_sources = oval_definitions_and_results_sources
+        self.cpe_source = ""
         self.missing_oval_results = False
         self.cpe_al = True
-        self.oval_definitions = {}
-        self.oval_cpe_definitions = {}
+        self.reports_with_oval_definitions = None
         self.platform_to_oval_cpe_id = {}
         self.cpe_platforms = {}
+        self.dict_of_oval_cpe_definitions = {}
         self.load_oval_definitions()
 
     def load_oval_definitions(self):
         try:
-            self.cpe_al_parser = CPEApplicabilityLanguageParser(self.root)
-            self.platform_to_oval_cpe_id = self.cpe_al_parser.platform_to_oval_cpe_id
-            self.oval_definition_parser = OVALDefinitionParser(
-                self.root, self.platform_to_oval_cpe_id
+            self.oval_definition_parser = OVALDefinitionParser(self.root)
+            self.reports_with_oval_definitions = self.oval_definition_parser.get_oval_definitions()
+            self._determine_cpe_source()
+            self.dict_of_oval_cpe_definitions = self._get_dict_of_oval_cpe_definitions()
+            self.cpe_al_parser = CPEApplicabilityLanguageParser(
+                self.root, self.dict_of_oval_cpe_definitions
             )
-            self.oval_definitions = self.oval_definition_parser.get_oval_definitions()
-            self.oval_cpe_definitions = self.oval_definition_parser.get_oval_cpe_definitions()
+            self.platform_to_oval_cpe_id = self.cpe_al_parser.platform_to_oval_cpe_id
             self._load_cpe_platforms()
         except MissingOVALResult as error:
             logging.warning((
-                "The given input doesn't contain OVAL results (\"%s\"),"
-                " OVAL details won't be shown in the report."), error)
-            if str(error) != "oval1":
-                self.missing_oval_results = True
+                "The given input doesn't contain OVAL results (\"%s\"), "
+                "OVAL details won't be shown in the report."), error)
+            self.missing_oval_results = True
+
+    def _determine_cpe_source(self):
+        source_id = set(self.reports_with_oval_definitions.keys()).difference(
+            self.oval_definitions_and_results_sources
+        )
+        if len(source_id) == 1:
+            self.cpe_source = source_id.pop()
+
+    def _get_dict_of_oval_cpe_definitions(self):
+        if self.cpe_source in self.reports_with_oval_definitions:
+            return self.reports_with_oval_definitions[self.cpe_source]
+        logging.warning((
+            "The given input does not contain a clear mapping of the OVAL definition used "
+            "for CPE checks. The results of the OVAL definition in the CPE checks could "
+            "be biased."
+        ))
+        all_oval_definition = {}
+        for report in self.reports_with_oval_definitions.values():
+            for id_definition, definition in report.items():
+                if id_definition not in all_oval_definition:
+                    all_oval_definition[id_definition] = definition
+                else:
+                    if definition.oval_tree.evaluate_tree() != "not evaluated":
+                        all_oval_definition[id_definition] = definition
+        return all_oval_definition
+
+    def _get_oval_definition_of_cpe(self, platform):
+        cpe_oval_id = self.platform_to_oval_cpe_id.get(platform)
+        return self.dict_of_oval_cpe_definitions.get(cpe_oval_id)
 
     def _load_cpe_platforms(self):
         try:
-            self.cpe_platforms = self.cpe_al_parser.get_cpe_platforms(self.oval_cpe_definitions)
+            self.cpe_platforms = self.cpe_al_parser.get_cpe_platforms()
             for platform in self.profile_platforms:
-                if platform in self.platform_to_oval_cpe_id:
-                    cpe_oval_id = self.platform_to_oval_cpe_id[platform]
-                    if cpe_oval_id in self.oval_cpe_definitions:
-                        oval_tree = self.oval_cpe_definitions[cpe_oval_id].oval_tree
-                        self.cpe_platforms[platform] = Platform(
-                            platform_id=platform,
-                            logical_test=LogicalTest(
-                                node_type="AND",
-                                children=[LogicalTest(
-                                    node_type="frac-ref",
-                                    value=cpe_oval_id,
-                                    oval_tree=oval_tree
-                                )],
-                            ),
-                            title="Profile platform",
-                        )
+                oval_definition = self._get_oval_definition_of_cpe(platform)
+                if oval_definition is None:
+                    logging.warning(
+                        "Platform (\"%s\") doesn't exist, Platform won't be shown in the report.",
+                        platform
+                    )
+                    continue
+                self.cpe_platforms[platform] = Platform(
+                    platform_id=platform,
+                    logical_test=LogicalTest(
+                        node_type="AND",
+                        children=[LogicalTest(
+                            node_type="frac-ref",
+                            value=oval_definition.definition_id,
+                            oval_tree=oval_definition.oval_tree
+                        )],
+                    ),
+                    title="Profile platform",
+                )
             self._evaluate_all_cpe_platforms()
         except ExceptionNoCPEApplicabilityLanguage:
             self.cpe_al = False
 
     def _evaluate_all_cpe_platforms(self):
         for cpe_platform in self.cpe_platforms.values():
             cpe_platform.result = cpe_platform.logical_test.evaluate_tree()
 
     def _get_oval_tree_from_oval_cpe_definition(self, platform):
         cpe_oval_id = ""
         cpe_platform = platform.lstrip("#")
         if cpe_platform in self.platform_to_oval_cpe_id:
             cpe_oval_id = self.platform_to_oval_cpe_id[cpe_platform]
-        if cpe_oval_id in self.oval_cpe_definitions:
-            return self.oval_cpe_definitions[cpe_oval_id].oval_tree
+        if cpe_oval_id in self.dict_of_oval_cpe_definitions:
+            return self.dict_of_oval_cpe_definitions[cpe_oval_id].oval_tree
         if cpe_platform in self.cpe_platforms:
             return None
         logging.warning("There is no CPE check for the platform \"%s\".", platform)
         return None
 
     def _get_cpe_al_platforms(self, platforms):
         out = {}
@@ -96,21 +130,37 @@
 
     @staticmethod
     def _remove_double_cpe_requirement(rule, group_platforms):
         for platform in rule.platforms:
             if platform in group_platforms:
                 group_platforms.remove(platform)
 
+    def get_oval_definition(self, rule):
+        report = self.reports_with_oval_definitions.get(rule.oval_reference, None)
+        if report is not None:
+            return report.get(rule.oval_definition_id)
+        oval_def = None
+        for report in self.reports_with_oval_definitions.values():
+            if oval_def is not None and rule.oval_definition_id in report:
+                logging.warning(
+                    ("The given input contains the duplicate results of "
+                     "the OVAL definition (\"%s\")."),
+                    rule.oval_definition_id
+                )
+            if rule.oval_definition_id in report:
+                oval_def = report[rule.oval_definition_id]
+        return oval_def
+
     def insert_oval_and_cpe_trees_to_rules(self, rules):
         if self.missing_oval_results:
             return
 
         for rule in rules.values():
-            if rule.oval_definition_id in self.oval_definitions:
-                rule.oval_definition = self.oval_definitions[rule.oval_definition_id]
+            rule.oval_definition = self.get_oval_definition(rule)
+
             rule_group = self.group_parser.rule_to_group_id.get(rule.rule_id, "")
             group_platforms = self.group_parser.group_to_platforms.get(rule_group, [])
             self._remove_double_cpe_requirement(rule, group_platforms)
             if not self.cpe_al:
                 rule.cpe_oval_dict = {
                     "profile_platforms": self._get_cpe_oval_tree(self.profile_platforms),
                     "group_platforms": self._get_cpe_oval_tree(group_platforms),
```

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/__init__.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/cpe_al_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/cpe_al_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 from ..data_structures import LogicalTest, Platform
 from ..exceptions import ExceptionNoCPEApplicabilityLanguage
 from ..namespaces import NAMESPACES
 from .full_text_parser import FullTextParser
 
+TEXT_TO_BOOL = {"true": True, "false": False, "": False}
+
 
 class CPEApplicabilityLanguageParser:
-    def __init__(self, root):
+    def __init__(self, root, oval_cpe_definitions):
         self.root = root
         self.platform_to_oval_cpe_id = self.get_platform_to_oval_cpe_id_dict()
         self.full_text_parser = FullTextParser({})
-        self.oval_cpe_definitions = {}
+        self.oval_cpe_definitions = oval_cpe_definitions
 
     def get_platform_to_oval_cpe_id_dict(self):
         cpe_list = self.root.find(".//ds:component/cpe-dict:cpe-list", NAMESPACES)
         out = {}
         if cpe_list is None:
             return out
         for cpe_item in cpe_list:
@@ -31,42 +33,48 @@
         if platform_specification is None:
             raise ExceptionNoCPEApplicabilityLanguage
         for platform in platform_specification:
             platform_id = platform.get("id")
             cpe_platform_elements[platform_id] = platform
         return cpe_platform_elements
 
-    def _get_oval_cpe_tree(self, platform_name):
+    def _get_oval_cpe_tree(self, platform_name, check_id_ref):
         oval_tree = None
+        oval_cpe_id = None
+
         if platform_name in self.platform_to_oval_cpe_id:
             oval_cpe_id = self.platform_to_oval_cpe_id[platform_name]
-            oval_cpe_definition = self.oval_cpe_definitions.get(oval_cpe_id, None)
-            oval_tree = oval_cpe_definition.oval_tree if oval_cpe_definition is not None else None
+
+        if check_id_ref is not None:
+            oval_cpe_id = check_id_ref
+
+        oval_cpe_definition = self.oval_cpe_definitions.get(oval_cpe_id, None)
+        oval_tree = oval_cpe_definition.oval_tree if oval_cpe_definition is not None else None
         return oval_tree
 
     def get_logical_test(self, logical_test_el):
         operator = logical_test_el.get("operator")
-        negation = logical_test_el.get("negation")
-        logical_test = LogicalTest(operator, negation)
+        negation = logical_test_el.get("negate", "")
+        logical_test = LogicalTest(operator, negation=TEXT_TO_BOOL[negation])
         for child_logical_test_el in logical_test_el:
             if "fact-ref" in child_logical_test_el.tag:
                 platform_name = child_logical_test_el.get("name")
+                check_id_ref = child_logical_test_el.get("id-ref")
                 logical_test.children.append(
                     LogicalTest(
                         node_type="frac-ref",
-                        value=platform_name,
-                        oval_tree=self._get_oval_cpe_tree(platform_name))
+                        value=platform_name if platform_name is not None else check_id_ref,
+                        oval_tree=self._get_oval_cpe_tree(platform_name, check_id_ref))
                 )
             if child_logical_test_el.get('operator') is not None:
                 logical_test.children.append(self.get_logical_test(child_logical_test_el))
         return logical_test
 
-    def get_cpe_platforms(self, oval_cpe_definitions):
+    def get_cpe_platforms(self):
         out = {}
-        self.oval_cpe_definitions = oval_cpe_definitions
         for platform, platform_el in self._get_cpe_platform_elements().items():
             title_el = platform_el.find(".//cpe-lang:title", NAMESPACES)
             title_str = ""
             if title_el is not None:
                 self.full_text_parser.get_full_description(title_el)
             logical_test_el = platform_el.find(".//cpe-lang:logical-test", NAMESPACES)
```

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/full_text_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/full_text_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/group_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/group_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_definition_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_definition_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 from ..data_structures import OvalDefinition, OvalReference
 from ..exceptions import MissingOVALResult
 from ..namespaces import NAMESPACES
 from .oval_result_parser import OVALResultParser
 
 
 class OVALDefinitionParser:
-    def __init__(self, root, platform_to_oval_cpe_id):
+    def __init__(self, root):
         self.root = root
-        self.oval_result_parser = OVALResultParser(self.root, platform_to_oval_cpe_id)
-        self.oval_trees = self.oval_result_parser.get_oval_trees()
-        self.oval_cpe_trees = self.oval_result_parser.get_oval_cpe_trees()
+        self.oval_result_parser = OVALResultParser(self.root)
+        self.oval_trees_by_oval_reports = self.oval_result_parser.get_oval_trees_by_oval_reports()
 
         self.oval_reports = self.oval_result_parser.oval_reports
         self.oval_definitions = self._get_xml_elements_of_oval_definitions()
 
     def _get_xml_elements_of_oval_definitions(self):
         out = {}
         for oval, oval_report in self.oval_reports.items():
-            out[oval] = oval_report.find(
+            out[oval] = oval_report.oval_report_element.find(
                 './/oval-definitions:oval_definitions/oval-definitions:definitions', NAMESPACES)
         return out
 
     def _get_references(self, definition):
         references = []
         for ref in definition.findall('.//oval-definitions:reference', NAMESPACES):
             references.append(OvalReference(ref.get("source"), ref.get("ref_id")))
         return references
 
-    def parse_oval_definition(self, definition_id, definition):
+    def parse_oval_definition(self, definition_id, definition_class, definition):
         oval_definition_dict = {
             "definition_id": definition_id,
+            "definition_class": definition_class,
             "title": definition.find('.//oval-definitions:title', NAMESPACES).text,
             "description": definition.find('.//oval-definitions:description', NAMESPACES).text,
             "version": definition.get("version"),
             "references": self._get_references(definition),
         }
         return OvalDefinition(**oval_definition_dict)
 
@@ -44,28 +44,33 @@
         if oval not in self.oval_definitions:
             raise MissingOVALResult(oval)
 
         definitions = {}
         dict_of_criteria = {}
         for definition in self.oval_definitions[oval]:
             definition_id = definition.get("id")
-            oval_definition = self.parse_oval_definition(definition_id, definition)
+            definition_class = definition.get("class")
+            oval_definition = self.parse_oval_definition(
+                definition_id,
+                definition_class,
+                definition
+            )
             criteria = definition.find('.//oval-definitions:criteria', NAMESPACES)
             dict_of_criteria[definition_id] = self._create_dict_from_criteria(criteria)
             definitions[definition_id] = oval_definition
 
         self._add_comments_to_oval_tree(dict_of_criteria, oval)
         self._add_oval_tree_to_definition(definitions, oval)
         return definitions
 
     def get_oval_definitions(self):
-        return self._get_oval_definitions("oval0")
-
-    def get_oval_cpe_definitions(self):
-        return self._get_oval_definitions("oval1")
+        oval_definitions_by_reports = {}
+        for report_id in self.oval_trees_by_oval_reports:
+            oval_definitions_by_reports[report_id] = self._get_oval_definitions(report_id)
+        return oval_definitions_by_reports
 
     def _get_test_criteria(self, criterion):
         out = {"comment": criterion.get("comment")}
         if criterion.get('definition_ref'):
             out['extend_definition'] = criterion.get('definition_ref')
         else:
             out['value_id'] = criterion.get('test_ref')
@@ -80,19 +85,17 @@
         for criterion in criteria:
             if criterion.get("operator") or "criteria" in criterion.tag:
                 criteria_dict["child_criteria"].append(self._create_dict_from_criteria(criterion))
             else:
                 criteria_dict["child_criteria"].append(self._get_test_criteria(criterion))
         return criteria_dict
 
-    def _add_oval_tree_to_definition(self, definitions, oval):
+    def _add_oval_tree_to_definition(self, definitions, oval_report_id):
+        oval_tree_source = self.oval_trees_by_oval_reports.get(oval_report_id, {})
         for definition_id in definitions:
-            oval_tree_source = self.oval_trees
-            if oval == "oval1":
-                oval_tree_source = self.oval_cpe_trees
             self._set_oval_tree_to_definition(definitions, definition_id, oval_tree_source)
 
     def _set_oval_tree_to_definition(self, definitions, definition_id, oval_tree_source):
         if definition_id in oval_tree_source:
             oval_tree_source[definition_id].comment = definitions[definition_id].description
             definitions[definition_id].oval_tree = oval_tree_source[definition_id]
 
@@ -116,18 +119,16 @@
             if criterion.get('operator'):
                 self._fill_oval_tree_with_comments(
                     oval_node, None, criteria_dict, criterion)
             if criterion.get("extend_definition"):
                 self._fill_oval_tree_with_comments(
                     oval_node, criterion.get("extend_definition"), criteria_dict)
 
-    def _add_comments_to_oval_tree(self, dict_of_criteria, oval):
+    def _add_comments_to_oval_tree(self, dict_of_criteria, oval_report_id):
+        oval_tree_source = self.oval_trees_by_oval_reports.get(oval_report_id, {})
         for id_ in dict_of_criteria:
-            oval_tree_source = self.oval_trees
-            if oval == "oval1":
-                oval_tree_source = self.oval_cpe_trees
 
             if id_ not in oval_tree_source:
                 continue
 
             oval_tree = oval_tree_source[id_]
             self._fill_oval_tree_with_comments(oval_tree, id_, dict_of_criteria)
```

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_object_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_object_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_state_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_state_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/profile_info_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/profile_info_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/remediation_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/remediation_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/report_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/report_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/rule_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/rule_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
+from dataclasses import replace
+
 from ..data_structures import Identifier, Reference, Rule, RuleWarning
 from ..namespaces import NAMESPACES
 from .full_text_parser import FullTextParser
 from .remediation_parser import RemediationParser
 
 
 class RuleParser():
     def __init__(self, root, test_results, ref_values):
         self.root = root
         self.test_results = test_results
         self.full_text_parser = FullTextParser(ref_values)
         self.remediation_parser = RemediationParser(ref_values)
+        self.to_select_rule_ids = set()
+        self.to_deselect_rule_ids = set()
 
     @staticmethod
     def _get_references(rule):
         references = []
         for referenc in rule.findall(".//xccdf:reference", NAMESPACES):
             references.append(Reference(referenc.get("href"), referenc.text))
         return references
@@ -142,30 +146,61 @@
 
     @staticmethod
     def _add_message_about_oval(rule_id, rules):
         if "fix" in rules[rule_id].result:
             msg = "The OVAL graph of the rule as it was displayed before the fix was performed."
             rules[rule_id].messages.append(msg)
 
+    @staticmethod
+    def set_oval_definition_id_if_is_none(rule, check_name):
+        if rule.oval_definition_id is None:
+            rule.oval_definition_id = check_name
+
+    @staticmethod
+    def get_oval_check_href_name(rule_result_el):
+        check_ref = rule_result_el.find('.//xccdf:check/xccdf:check-content-ref', NAMESPACES)
+        if check_ref is None:
+            return None, None
+        return check_ref.get("href").lstrip("#"), check_ref.get("name")
+
     def _insert_rules_results(self, rules):
         rules_results = self.test_results.findall('.//xccdf:rule-result', NAMESPACES)
         for rule_result in rules_results:
             rule_id = rule_result.get('idref')
             rules[rule_id].time = rule_result.get('time')
             rules[rule_id].result = rule_result.find('.//xccdf:result', NAMESPACES).text
             rules[rule_id].weight = float(rule_result.get('weight'))
 
+            rules[rule_id].oval_reference, check_name = self.get_oval_check_href_name(
+                rule_result
+            )
+            self.set_oval_definition_id_if_is_none(rules[rule_id], check_name)
+
             messages = rule_result.findall('.//xccdf:message', NAMESPACES)
             if messages is not None:
                 rules[rule_id].messages = []
                 for message in messages:
                     rules[rule_id].messages.append(message.text)
                 self._improve_result_of_remedied_rule(rule_id, rules)
             self._add_message_about_oval(rule_id, rules)
 
+            if rules[rule_id].multi_check:
+                self._create_new_multi_check_rule(rules, rule_id, check_name)
+
+    def _create_new_multi_check_rule(self, rules, rule_id, check_name):
+        self.to_deselect_rule_ids.add(rule_id)
+        new_rule_id = f"{rule_id}-{check_name}"
+        changes = {
+            "rule_id": new_rule_id,
+            "title": f"{rules[rule_id].title} ({check_name})",
+            "oval_definition_id": check_name,
+        }
+        rules[new_rule_id] = replace(rules[rule_id], **changes)
+        self.to_select_rule_ids.add(new_rule_id)
+
     def get_rules(self):
         rules = {}
         for rule_el in self.root.findall(".//xccdf:Rule", NAMESPACES):
             rule = self.process_rule(rule_el)
             rules[rule.rule_id] = rule
         self._insert_rules_results(rules)
         return rules
```

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/scan_result_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/scan_result_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/scap_results_parser.py` & `openscap-report-0.2.3/openscap_report/scap_results_parser/scap_results_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,44 +58,50 @@
 
     @staticmethod
     def _debug_show_rules(rules):
         for rule_id, rule in rules.items():
             logging.debug(rule_id)
             logging.debug(rule)
 
-    @staticmethod
-    def _get_applicable_cpe_ids_for_machine(cpe_platforms_for_profile):
-        return [
-            cpe_id for cpe_id, applicable_for_machine in cpe_platforms_for_profile.items()
-            if applicable_for_machine
-        ]
-
     def _get_benchmark_element(self):
         benchmark_el = self.root.find(".//xccdf:Benchmark", NAMESPACES)
         if "Benchmark" in self.root.tag:
             benchmark_el = self.root
         return benchmark_el
 
+    @staticmethod
+    def _get_oval_definition_references(rules):
+        references = []
+        for rule in rules.values():
+            if rule.oval_reference is not None:
+                references.append(rule.oval_reference)
+        return set(tuple(references))
+
     def parse_report(self):
         test_results_el = self.root.find('.//xccdf:TestResult', NAMESPACES)
         benchmark_el = self._get_benchmark_element()
 
         report_parser = ReportParser(self.root, test_results_el, benchmark_el)
         report = report_parser.get_report()
         logging.debug(report)
 
         group_parser = GroupParser(self.root, self.ref_values, benchmark_el)
         groups = group_parser.get_groups()
 
         rule_parser = RuleParser(self.root, test_results_el, self.ref_values)
         rules = rule_parser.get_rules()
-
+        oval_definitions_and_results_sources = self._get_oval_definition_references(rules)
         OVAL_and_CPE_tree_builder = OVALAndCPETreeBuilder(  # pylint: disable=C0103
             self.root, group_parser,
-            self._get_applicable_cpe_ids_for_machine(report.profile_info.cpe_platforms_for_profile)
+            report.profile_info.get_list_of_cpe_platforms_that_satisfy_evaluation_target(),
+            oval_definitions_and_results_sources
         )
         OVAL_and_CPE_tree_builder.insert_oval_and_cpe_trees_to_rules(rules)
 
         self._debug_show_rules(rules)
         report.rules = rules
         report.groups = groups
+
+        report.profile_info.select_rules(rule_parser.to_select_rule_ids)
+        report.profile_info.deselect_rules(rule_parser.to_deselect_rule_ids)
+
         return report
```

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/catalog.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/catalog.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/xlink.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xlink.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/xml.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xml.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd` & `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/openscap_report.egg-info/PKG-INFO` & `openscap-report-0.2.3/openscap_report.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openscap-report
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tool for generating report from results of oscap scan.
 Home-page: https://github.com/OpenSCAP/oscap-report
 Author: Jan Rodak
 Author-email: jrodak@redhat.com
 License: LGPL-2.1 License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 [![Code Coverage](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/badges/coverage.png?b=main)](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/?branch=main)
 [![Code Intelligence Status](https://scrutinizer-ci.com/g/OpenSCAP/openscap-report/badges/code-intelligence.svg?b=main)](https://scrutinizer-ci.com/code-intelligence)
 
 Tool for generating report from results of oscap scan.
 
 ## Installation
 
-[Learn how to install tool in the documentation.](https://openscap-report.readthedocs.io/en/latest/manual/instalation.html)
+[Learn how to install tool in the documentation.](https://openscap-report.readthedocs.io/en/latest/manual/installation.html)
 
 ## Example usage
 
 This command consumes the ARF file, which is one of the possible standardized formats for the results of SCAP-compliant scanners. You can read about generating ARF report files using OpenSCAP in the OpenSCAP User Manual. Or you can use test arf files from repository [`/tests/test_data`](https://github.com/OpenSCAP/openscap-report/tree/main/tests/test_data).
 
 ```bash
 oscap-report < ssg-fedora-ds-arf.xml > report.html
```

### Comparing `openscap-report-0.2.2/openscap_report.egg-info/SOURCES.txt` & `openscap-report-0.2.3/openscap_report.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,26 @@
 docs/index.rst
 docs/oscap-report.1.rst
 docs/requirements.txt
 docs/exts/sphinxarg/__init__.py
 docs/exts/sphinxarg/ext.py
 docs/exts/sphinxarg/markdown.py
 docs/exts/sphinxarg/parser.py
-docs/manual/instalation.rst
+docs/manual/installation.rst
+docs/manual/report.rst
 docs/manual/usage.rst
+docs/manual/assets/about_profile.png
+docs/manual/assets/compliance_and_scoring.png
+docs/manual/assets/cpe_aplicability_language.png
+docs/manual/assets/evaluation_characteristics.png
+docs/manual/assets/example_report.html
+docs/manual/assets/oval.gif
+docs/manual/assets/remediation.png
+docs/manual/assets/rule_detail.png
+docs/manual/assets/rule_overview_section.png
 docs/modules/modules.rst
 docs/modules/openscap_report.report_generators.rst
 docs/modules/openscap_report.rst
 docs/modules/openscap_report.scap_results_parser.data_structures.rst
 docs/modules/openscap_report.scap_results_parser.parsers.rst
 docs/modules/openscap_report.scap_results_parser.rst
 openscap_report/__init__.py
@@ -143,14 +153,15 @@
 openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd
 openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd
 openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd
 tests/.gitkeep
 tests/__init__.py
 tests/conftest.py
 tests/constants.py
+tests/integration.fmf
 tests/json_schema_of_report.json
 tests/smoke.fmf
 tests/smoke.sh
 tests/test_utils.py
 tests/integration_tests/__init__.py
 tests/integration_tests/test_basic_usage.py
 tests/integration_tests/test_cli.py
@@ -176,14 +187,16 @@
 tests/test_data/xccdf_simple_rule_fail.xml
 tests/test_data/xccdf_simple_rule_pass.xml
 tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt
 tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt
 tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt
 tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt
 tests/unit_tests/__init__.py
+tests/unit_tests/test_cli.py
+tests/unit_tests/test_cpe_al_parser.py
 tests/unit_tests/test_data_structure.py
 tests/unit_tests/test_debug_settings.py
 tests/unit_tests/test_full_text_parser.py
 tests/unit_tests/test_json_transitions.py
 tests/unit_tests/test_oval_result_eval.py
 tests/unit_tests/test_oval_tree_eval.py
 tests/unit_tests/test_scap_result_parser.py
```

### Comparing `openscap-report-0.2.2/setup.py` & `openscap-report-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def get_long_description():
     with open("README.md", "r", encoding="utf-8") as readme_file:
         return readme_file.read()
 
 
 setup(name='openscap-report',
-      version='0.2.2',
+      version='0.2.3',
       description='Tool for generating report from results of oscap scan.',
       long_description=get_long_description(),
       long_description_content_type="text/markdown",
       url='https://github.com/OpenSCAP/oscap-report',
       author='Jan Rodak',
       author_email='jrodak@redhat.com',
       license='LGPL-2.1 License',
```

### Comparing `openscap-report-0.2.2/tests/constants.py` & `openscap-report-0.2.3/tests/constants.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/integration_tests/test_basic_usage.py` & `openscap-report-0.2.3/tests/integration_tests/test_basic_usage.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/integration_tests/test_cli.py` & `openscap-report-0.2.3/tests/integration_tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,28 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-import argparse
 import subprocess
 import tempfile
-from io import BytesIO
 from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from openscap_report.cli import CommandLineAPI
-from openscap_report.scap_results_parser import (ARF_SCHEMAS_PATH,
-                                                 SCAPResultsParser)
+from openscap_report.scap_results_parser import SCAPResultsParser
 
 from ..constants import PATH_TO_ARF, PATH_TO_EMPTY_FILE
+from ..test_utils import get_fake_args
 
 PATH_TO_RESULT_FILE = Path(tempfile.gettempdir()) / "oscap-report-tests_result.html"
 OSCAP_REPORT_COMMAND = "oscap-report"
 CAT_ARF_FILE = ["cat", str(PATH_TO_ARF)]
 
 
-def get_fake_args():
-    # pylint: disable=bad-option-value,R1732
-    input_file = open(PATH_TO_ARF, "r", encoding="utf-8")
-    output_file = open(PATH_TO_RESULT_FILE, "wb")
-    return argparse.Namespace(
-        FILE=input_file, output=output_file,
-        log_file=None, log_level="WARNING", format="HTML",
-        debug=[""],
-    )
-
-
-@pytest.mark.unit_test
-@mock.patch('argparse.ArgumentParser.parse_args',
-            return_value=get_fake_args())
-def test_load_file(mock_args):  # pylint: disable=W0613
-    api = CommandLineAPI()
-    xml_report = api.load_file()
-    parser = SCAPResultsParser(xml_report)
-    assert parser.validate(ARF_SCHEMAS_PATH)
-    api.close_files()
-
-
-@pytest.mark.unit_test
-@pytest.mark.usefixtures("remove_generated_file")
-@mock.patch('argparse.ArgumentParser.parse_args',
-            return_value=get_fake_args())
-def test_store_file(mock_args):  # pylint: disable=W0613
-    api = CommandLineAPI()
-    data = BytesIO(b'<html><h1>TEST DATA</h1></html>')
-    api.store_file(data)
-    api.close_files()
-    with open(PATH_TO_RESULT_FILE, "r", encoding="utf-8") as result_file:
-        assert result_file.read() == data.getvalue().decode("utf-8")
-
-
 @pytest.mark.integration_test
 @mock.patch('argparse.ArgumentParser.parse_args',
             return_value=get_fake_args())
 def test_generate_report(mock_args):  # pylint: disable=W0613
     data = None
     api = CommandLineAPI()
     with open(PATH_TO_ARF, "r", encoding="utf-8") as arf_report:
```

### Comparing `openscap-report-0.2.2/tests/integration_tests/test_json.py` & `openscap-report-0.2.3/tests/integration_tests/test_json.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/json_schema_of_report.json` & `openscap-report-0.2.3/tests/json_schema_of_report.json`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf-container.xml` & `openscap-report-0.2.3/tests/test_data/arf-container.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf-dangling-reference-to.xml` & `openscap-report-0.2.3/tests/test_data/arf-dangling-reference-to.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf-report.xml` & `openscap-report-0.2.3/tests/test_data/arf-report.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf-with-removed-info.xml` & `openscap-report-0.2.3/tests/test_data/arf-with-removed-info.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf_cpe_check_os_platform.xml` & `openscap-report-0.2.3/tests/test_data/arf_cpe_check_os_platform.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf_multi_check.xml` & `openscap-report-0.2.3/tests/test_data/arf_multi_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf_no_system_data.xml` & `openscap-report-0.2.3/tests/test_data/arf_no_system_data.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf_rule_and_cpe_check.xml` & `openscap-report-0.2.3/tests/test_data/arf_rule_and_cpe_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf_simple_rule_fail.xml` & `openscap-report-0.2.3/tests/test_data/arf_simple_rule_fail.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/arf_simple_rule_pass.xml` & `openscap-report-0.2.3/tests/test_data/arf_simple_rule_pass.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/plant_catalog.xml` & `openscap-report-0.2.3/tests/test_data/plant_catalog.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt` & `openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt` & `openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt` & `openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt` & `openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/xccdf-report.xml` & `openscap-report-0.2.3/tests/test_data/xccdf-report.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/xccdf-with-removed-info.xml` & `openscap-report-0.2.3/tests/test_data/xccdf-with-removed-info.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/xccdf_multi_check.xml` & `openscap-report-0.2.3/tests/test_data/xccdf_multi_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/xccdf_no_system_data.xml` & `openscap-report-0.2.3/tests/test_data/xccdf_no_system_data.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/xccdf_rule_and_cpe_check.xml` & `openscap-report-0.2.3/tests/test_data/xccdf_rule_and_cpe_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/xccdf_simple_rule_fail.xml` & `openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_fail.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/test_data/xccdf_simple_rule_pass.xml` & `openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_pass.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_data_structure.py` & `openscap-report-0.2.3/tests/unit_tests/test_data_structure.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_debug_settings.py` & `openscap-report-0.2.3/tests/unit_tests/test_debug_settings.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_full_text_parser.py` & `openscap-report-0.2.3/tests/unit_tests/test_full_text_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_json_transitions.py` & `openscap-report-0.2.3/tests/unit_tests/test_json_transitions.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_oval_result_eval.py` & `openscap-report-0.2.3/tests/unit_tests/test_oval_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_oval_tree_eval.py` & `openscap-report-0.2.3/tests/unit_tests/test_oval_tree_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_scap_result_parser.py` & `openscap-report-0.2.3/tests/unit_tests/test_scap_result_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tests/unit_tests/test_shared_static_methods_of_parser.py` & `openscap-report-0.2.3/tests/unit_tests/test_shared_static_methods_of_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.2/tox.ini` & `openscap-report-0.2.3/tox.ini`

 * *Files identical despite different names*

