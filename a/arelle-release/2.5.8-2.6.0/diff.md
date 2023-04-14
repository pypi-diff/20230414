# Comparing `tmp/arelle-release-2.5.8.tar.gz` & `tmp/arelle-release-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arelle-release-2.5.8.tar", last modified: Fri Apr  7 03:15:35 2023, max compression
+gzip compressed data, was "arelle-release-2.6.0.tar", last modified: Fri Apr 14 14:25:38 2023, max compression
```

## Comparing `arelle-release-2.5.8.tar` & `arelle-release-2.6.0.tar`

### file list

```diff
@@ -1,743 +1,743 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.768990 arelle-release-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.628981 arelle-release-2.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.628981 arelle-release-2.5.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/ISSUE_TEMPLATE/change.yml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.628981 arelle-release-2.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/build-and-release-linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/build-and-release-mac.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/build-and-release-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/build-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/conformance-suites.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/project.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/test-ui.yml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-07 03:15:07.000000 arelle-release-2.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-07 03:15:07.000000 arelle-release-2.5.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 03:15:07.000000 arelle-release-2.5.8/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 03:15:07.000000 arelle-release-2.5.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-07 03:15:07.000000 arelle-release-2.5.8/EFM-only-test.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-07 03:15:07.000000 arelle-release-2.5.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-07 03:15:35.768990 arelle-release-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-07 03:15:07.000000 arelle-release-2.5.8/QuickBooks.qwc
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-07 03:15:07.000000 arelle-release-2.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.632981 arelle-release-2.5.8/apidocs/
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-07 03:15:07.000000 arelle-release-2.5.8/apidocs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-07 03:15:07.000000 arelle-release-2.5.8/apidocs/arelle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-07 03:15:07.000000 arelle-release-2.5.8/apidocs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-07 03:15:07.000000 arelle-release-2.5.8/apidocs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-07 03:15:07.000000 arelle-release-2.5.8/apidocs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 03:15:07.000000 arelle-release-2.5.8/apidocs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.656983 arelle-release-2.5.8/arelle/
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/Aspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    39740 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/Cntlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    81315 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/CntlrCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/CntlrComServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/CntlrProfiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/CntlrQuickBooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    48719 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/CntlrWebMain.py
--rw-r--r--   0 runner    (1001) docker     (123)    88038 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/CntlrWinMain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/CntlrWinTooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogAbout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogArcroleGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogFind.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogFormulaParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogLanguage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogNewFactItem.py
--rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogOpenArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogOpenTaxonomyPackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogPackageManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogRssWatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogURL.py
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DialogUserPassword.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/DisclosureSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    43688 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/FileSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/FunctionCustom.py
--rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/FunctionFn.py
--rw-r--r--   0 runner    (1001) docker     (123)    80279 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/FunctionIxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/FunctionUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    71334 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/FunctionXfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/FunctionXs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/HashUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/HtmlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/InstanceAspectsEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/LeiUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/LocalViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28242 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/Locale.py
--rw-r--r--   0 runner    (1001) docker     (123)   119586 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelDocument.py
--rw-r--r--   0 runner    (1001) docker     (123)    88883 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelDtsObject.py
--rw-r--r--   0 runner    (1001) docker     (123)   122124 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelFormulaObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    72084 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelInstanceObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelObjectFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    70336 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelRenderingObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelRssItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelRssObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelTestcaseObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    38714 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelValue.py
--rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelVersObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    73327 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ModelXbrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/PackageManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    29001 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/PluginManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/PrototypeDtsObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/PrototypeInstanceObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/PythonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/RenderingEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43733 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/RenderingResolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/SystemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/TableStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/TkTableWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/UITkTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/UiUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/Updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    31897 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/UrlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49309 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/Validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    51553 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateFilingText.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateUtr.py
--rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)    75131 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateXbrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateXbrlCalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100180 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateXbrlDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    38118 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ValidateXbrlDimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileConcepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileFactList.py
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileFactTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileRenderedGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileRoleTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileRssFeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewFileTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewUtilFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinConcepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinDiffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinFactGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinFactList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinFactTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinList.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinPane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    78864 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinRenderedGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinRoleTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinRssFeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinTkTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinTree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinTupleGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/ViewWinXml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/WatchRss.py
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/WebCache.py
--rw-r--r--   0 runner    (1001) docker     (123)    62211 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/XbrlConst.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/XbrlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/XhtmlValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/XmlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    44546 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/XmlValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/XmlValidateParticles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/XmlValidateSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 03:15:35.000000 arelle-release-2.5.8/arelle/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.660983 arelle-release-2.5.8/arelle/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/arelle_test.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/creationSoftwareNames.json
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/disclosuresystems.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/disclosuresystems.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/edbody.dtd
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/empty-instance.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/erxl.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/mappings.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/mappings.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/xbrlschemafiles.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/xhtml-lat1.ent
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/xhtml-special.ent
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/xhtml-symbol.ent
--rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/xhtml1-strict-ix.dtd
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/config/xhtml1_1-strict-ix.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.660983 arelle-release-2.5.8/arelle/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   458032 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/doc/messagesCatalog.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/doc/messagesCatalog.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.664983 arelle-release-2.5.8/arelle/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/.pydevproject
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/CustomLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/LoadEFMvalidate.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/LoadSavePreLbCsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/LoadValidate.cs
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/LoadValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/LoadValidateCmdLine.java
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/LoadValidatePostedZip.java
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/LoadValidateWebService.java
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/SaveTableToExelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/TR3toTR4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.668984 arelle-release-2.5.8/arelle/examples/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/bigInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/cmdWebServerExtension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/crashTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/formulaSuiteConverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/functionsCustom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/hello_dolly.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/hello_i18n.pot
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/hello_i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/importTestChild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/importTestChild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/importTestGrandchild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/importTestGrandchild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/importTestImported1.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/importTestImported11.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/importTestParent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.616980 arelle-release-2.5.8/arelle/examples/plugin/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.616980 arelle-release-2.5.8/arelle/examples/plugin/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.668984 arelle-release-2.5.8/arelle/examples/plugin/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.668984 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestChild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestChild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestImported1.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestImported11.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.668984 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.668984 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/sakaCalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/saveInstanceInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/streamingExtensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/updateTableLB.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/validateSchemaLxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/plugin/validateTableInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/us-gaap-dei-docType-extraction-frm.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/examples/us-gaap-dei-ratio-cash-frm.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.672984 arelle-release-2.5.8/arelle/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/formula/FactAspectsCache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/formula/FormulaConsisAsser.py
--rw-r--r--   0 runner    (1001) docker     (123)    83178 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/formula/FormulaEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    98324 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/formula/ValidateFormula.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/formula/XPathContext.py
--rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/formula/XPathParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/formula/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.680984 arelle-release-2.5.8/arelle/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle-full-word.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle-mac-icon-4.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle-word-only.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle.gif
--rw-r--r--   0 runner    (1001) docker     (123)   212911 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle.icns
--rw-r--r--   0 runner    (1001) docker     (123)   392859 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle.icns.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle.ico
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle.xbm
--rw-r--r--   0 runner    (1001) docker     (123)   269858 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle128.psd
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle16.psd
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle16x16and32x32.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/arelle32.gif
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/columnSortDown.gif
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/columnSortUp.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/octocat.png
--rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/python-clear.png
--rw-r--r--   0 runner    (1001) docker     (123)   696358 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/python-icon-pack-crystalxp.net-842.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarClose.gif
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarCompare.gif
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarDelete.gif
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarFindMenu.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarLogClear - 1-piece-top.gif
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarLogClear-orig.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarLogClear.gif
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarNewFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarOpenDatabase.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarOpenFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarOpenWeb.gif
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarProperties.gif
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarQuit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarReopen.gif
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarSaveFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/toolbarValidate.gif
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/xbrl.gif
--rw-r--r--   0 runner    (1001) docker     (123)   201686 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/xbrl.psd
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/xbrl128-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/xbrl128.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/xbrl16.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/images/xbrl32.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.680984 arelle-release-2.5.8/arelle/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.616980 arelle-release-2.5.8/arelle/locale/ar_EG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.680984 arelle-release-2.5.8/arelle/locale/ar_EG/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   341883 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po
--rw-r--r--   0 runner    (1001) docker     (123)   185904 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.616980 arelle-release-2.5.8/arelle/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.684985 arelle-release-2.5.8/arelle/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149331 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/es/LC_MESSAGES/arelle.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.616980 arelle-release-2.5.8/arelle/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.684985 arelle-release-2.5.8/arelle/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   118897 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/fr/LC_MESSAGES/arelle.mo
--rw-r--r--   0 runner    (1001) docker     (123)   168077 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/fr/LC_MESSAGES/fr.po
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   249762 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/arelle/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.684985 arelle-release-2.5.8/arelle/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   375378 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/ru/LC_MESSAGES/arelle.mo
--rw-r--r--   0 runner    (1001) docker     (123)   449579 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/locale/ru/LC_MESSAGES/ru.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.692985 arelle-release-2.5.8/arelle/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/EdgarRendererAllReports.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/SECCorrespondenceLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/TDnetLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/UKCompaniesHouseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)   101637 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/formulaLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/formulaSaver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/formulaXPathChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/functionsMath.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/functionsXmlCreation.py
--rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/inlineXbrlDocumentSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/instanceInfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/arelle/plugin/internet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.692985 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/U32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/des_c.py
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/des_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html
--rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)   124382 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/loadFromExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    76473 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/loadFromOIM-2018.py
--rw-r--r--   0 runner    (1001) docker     (123)   195836 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/loadFromOIM.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.692985 arelle-release-2.5.8/arelle/plugin/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/logging/dpmSignature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/logging/dqcParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/logging/saveMessages.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/objectmaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/profileCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/profileFormula.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/saveCHComponentFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/saveDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/saveHtmlEBAtables.py
--rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/saveLoadableExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    32261 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/saveLoadableOIM.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/saveSKOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/saveSampleInstance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.692985 arelle-release-2.5.8/arelle/plugin/security/
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/security/cryptAES_CBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/security/cryptAES_EAX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.696985 arelle-release-2.5.8/arelle/plugin/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/FormulaGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/SphinxContext.py
--rw-r--r--   0 runner    (1001) docker     (123)    35742 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/SphinxEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    49810 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/SphinxMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/SphinxParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/SphinxValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/streamingExtensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.696985 arelle-release-2.5.8/arelle/plugin/transforms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.696985 arelle-release-2.5.8/arelle/plugin/transforms/SEC/
--rw-r--r--   0 runner    (1001) docker     (123)    41892 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.704986 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/extractTestcase.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)  4737705 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/saxon9.jar
--rw-r--r--   0 runner    (1001) docker     (123)   225611 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/testcase.xml
--rw-r--r--   0 runner    (1001) docker     (123)    59680 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/text2num.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.704986 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.704986 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    55540 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/transforms/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/unpackSecEisFile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.708986 arelle-release-2.5.8/arelle/plugin/validate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.708986 arelle-release-2.5.8/arelle/plugin/validate/CIPC/
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/CIPC/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/CIPC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/CIPC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.708986 arelle-release-2.5.8/arelle/plugin/validate/EBA/
--rw-r--r--   0 runner    (1001) docker     (123)    45950 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EBA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EBA/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.712987 arelle-release-2.5.8/arelle/plugin/validate/EFM/
--rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/Consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/Document.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   253045 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/Filing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/PreCalAlignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.724987 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/axiswarnings.json
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/cef-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/country-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/currency-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/dei-deprecated-concepts.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   113832 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/dei-validations.json
--rw-r--r--   0 runner    (1001) docker     (123)    76859 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/dqc-us-rules.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/ecd-deprecated-concepts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.732988 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/
--rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    76545 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    76785 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    73012 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150333 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   138364 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml
--rw-r--r--   0 runner    (1001) docker     (123)   135467 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml
--rw-r--r--   0 runner    (1001) docker     (123)   180977 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   125792 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)   134456 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   109498 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    99358 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)    28394 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml
--rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml
--rw-r--r--   0 runner    (1001) docker     (123)    29744 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml
--rw-r--r--   0 runner    (1001) docker     (123)    31676 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml
--rw-r--r--   0 runner    (1001) docker     (123)   109944 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    35860 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    58455 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml
--rw-r--r--   0 runner    (1001) docker     (123)    62455 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    49163 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    48412 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    57294 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    69638 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   367560 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)    93735 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/other-standard-taxonomies.json
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/sic-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/signwarnings.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/srt-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/stpr-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json
--rw-r--r--   0 runner    (1001) docker     (123)   205448 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)  1583747 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json
--rw-r--r--   0 runner    (1001) docker     (123)  1624986 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json
--rw-r--r--   0 runner    (1001) docker     (123)  1593440 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json
--rw-r--r--   0 runner    (1001) docker     (123)  1613560 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/vip-deprecated-concepts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.712987 arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.712987 arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.732988 arelle-release-2.5.8/arelle/plugin/validate/ESEF/
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    75625 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.732988 arelle-release-2.5.8/arelle/plugin/validate/ESEF/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF/resources/authority-validations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    81794 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/FERC/
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/FERC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/FERC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/FERC/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/FERC/resources/ferc-utr.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/GFM/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/GFM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/GFM/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/HMRC/
--rw-r--r--   0 runner    (1001) docker     (123)    29346 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/HMRC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/HMRC/config.xml
--rw-r--r--   0 runner    (1001) docker     (123)    25247 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/HMRC/consistencyChecksByName.json
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/ROS/
--rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ROS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/ROS/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/CustomLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    59358 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/Document.py
--rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/Filing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/config.xml
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml
--rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/USBestPractices.py
--rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/USCorpAction.py
--rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/USSecTagging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/XDC/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/XDC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/XDC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.736988 arelle-release-2.5.8/arelle/plugin/validate/XFsyntax/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/XFsyntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/XFsyntax/xf.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validate/calc2.py
--rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/validateSBRnl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.740988 arelle-release-2.5.8/arelle/plugin/xbrlDB/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/DialogRssWatchExtender.py
--rw-r--r--   0 runner    (1001) docker     (123)    56450 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/SqlDb.py
--rw-r--r--   0 runner    (1001) docker     (123)    78257 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    78348 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    64539 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    55073 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    67782 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/entityInformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.740988 arelle-release-2.5.8/arelle/plugin/xbrlDB/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/ext/china.py
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/ext/edgar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/ext/xdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/primaryDocumentFacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.740988 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.744989 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   714004 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.744989 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open2/
--rw-r--r--   0 runner    (1001) docker     (123)   728541 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.744989 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/public/
--rw-r--r--   0 runner    (1001) docker     (123)   963416 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.748989 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql
--rw-r--r--   0 runner    (1001) docker     (123)    21988 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   728214 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)   729124 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)  1056221 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)   727913 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   726301 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xbrlDB/tableFacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/plugin/xuleSaver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.752989 arelle-release-2.5.8/arelle/scripts-macOS/
--rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-macOS/startWebServer.command
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.752989 arelle-release-2.5.8/arelle/scripts-unix/
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-unix/startWebServer.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.752989 arelle-release-2.5.8/arelle/scripts-windows/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/exportCsvFromXbrlInstance.bat
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/runEFMTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/runFormulaTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/runFunctionTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/runXBRL21Tests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/runXDTTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/startWebServer.bat
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/scripts-windows/validateAndRunFormulas.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.752989 arelle-release-2.5.8/arelle/webserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   116069 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/webserver/bottle-no2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)   171083 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle/webserver/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle.pyw
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelleCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelleGUI.pyw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.752989 arelle-release-2.5.8/arelle_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-07 03:15:35.000000 arelle-release-2.5.8/arelle_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-04-07 03:15:35.000000 arelle-release-2.5.8/arelle_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 03:15:35.000000 arelle-release-2.5.8/arelle_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-07 03:15:35.000000 arelle-release-2.5.8/arelle_release.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-07 03:15:35.000000 arelle-release-2.5.8/arelle_release.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 03:15:35.000000 arelle-release-2.5.8/arelle_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-07 03:15:07.000000 arelle-release-2.5.8/arelle_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.752989 arelle-release-2.5.8/attic/
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-04-07 03:15:07.000000 arelle-release-2.5.8/attic/CntlrGenVersReports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-07 03:15:07.000000 arelle-release-2.5.8/buildVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-07 03:15:07.000000 arelle-release-2.5.8/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-07 03:15:07.000000 arelle-release-2.5.8/debugCmdLineEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-07 03:15:07.000000 arelle-release-2.5.8/distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.752989 arelle-release-2.5.8/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-07 03:15:07.000000 arelle-release-2.5.8/docker/ubuntu.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-07 03:15:07.000000 arelle-release-2.5.8/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 03:15:07.000000 arelle-release-2.5.8/encodeUtf8PySource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-04-07 03:15:07.000000 arelle-release-2.5.8/generateMessagesCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-07 03:15:07.000000 arelle-release-2.5.8/installWin64.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-07 03:15:07.000000 arelle-release-2.5.8/installWin86.nsi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/libs/linux/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.756989 arelle-release-2.5.8/libs/linux/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/linux/Tktable2.11/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.756989 arelle-release-2.5.8/libs/linux/Tktable2.11/html/
--rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/linux/Tktable2.11/html/tkTable.html
--rwxr-xr-x   0 runner    (1001) docker     (123)   161976 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/linux/Tktable2.11/libTktable2.11.so
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/linux/Tktable2.11/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/linux/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/linux/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/linux/Tktable2.11/tktable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/libs/macos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.756989 arelle-release-2.5.8/libs/macos/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/macos/Tktable2.11/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.756989 arelle-release-2.5.8/libs/macos/Tktable2.11/html/
--rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/macos/Tktable2.11/html/tkTable.html
--rw-r--r--   0 runner    (1001) docker     (123)   130952 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/macos/Tktable2.11/libTktable2.11.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/macos/Tktable2.11/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/macos/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/macos/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/macos/Tktable2.11/tktable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.620980 arelle-release-2.5.8/libs/win64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.756989 arelle-release-2.5.8/libs/win64/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/win64/Tktable2.11/Tktable.dll
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/win64/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-07 03:15:07.000000 arelle-release-2.5.8/libs/win64/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-07 03:15:07.000000 arelle-release-2.5.8/messages.pot
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-07 03:15:07.000000 arelle-release-2.5.8/msgfmt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.624981 arelle-release-2.5.8/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.756989 arelle-release-2.5.8/plugins/xbrl-us/
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-07 03:15:07.000000 arelle-release-2.5.8/plugins/xbrl-us/us-gaap-consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-04-07 03:15:07.000000 arelle-release-2.5.8/pygettext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-07 03:15:07.000000 arelle-release-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 03:15:07.000000 arelle-release-2.5.8/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-07 03:15:07.000000 arelle-release-2.5.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-07 03:15:07.000000 arelle-release-2.5.8/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-04-07 03:15:07.000000 arelle-release-2.5.8/runMacGUI.sh
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 03:15:07.000000 arelle-release-2.5.8/runtime.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.760990 arelle-release-2.5.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/buildLinuxDist.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/buildMacDist.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/buildWinDist.bat
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/charlieTest.bat
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/exportCsvFormulae.bat
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/exportCsvFromXbrlInstance.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/generateTestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/reportAllTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runAllTests.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runESMAtests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runGUI.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runGUI.sh
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runGenerateVersioningTestcases.bat
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runGeneratedTestcase.bat
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runLocaleGettext.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runPackageTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runProfilerXDTTest.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runPyTest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runTR2Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runTR3Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runTR4Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runTR5Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runTRSECTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runUS-GFMTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/runVersioningConsumptionTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/startWebServer-27.bat
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-07 03:15:07.000000 arelle-release-2.5.8/scripts/startWebServer.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-07 03:15:35.768990 arelle-release-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-07 03:15:07.000000 arelle-release-2.5.8/testParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 03:15:07.000000 arelle-release-2.5.8/testParser2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.760990 arelle-release-2.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.624981 arelle-release-2.5.8/tests/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.624981 arelle-release-2.5.8/tests/integration_tests/ui_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.760990 arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.760990 arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj
--rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Usings.cs
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.760990 arelle-release-2.5.8/tests/integration_tests/ui_tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   223544 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/ui_tests/resources/workiva.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.764990 arelle-release-2.5.8/tests/integration_tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.768990 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_assertion_severity_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_link_role_registry_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    29081 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_taxonomy_packages_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/download_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/run_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/test_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/integration_tests/validation/validation_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.624981 arelle-release-2.5.8/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.768990 arelle-release-2.5.8/tests/unit_tests/arelle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.768990 arelle-release-2.5.8/tests/unit_tests/arelle/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.768990 arelle-release-2.5.8/tests/unit_tests/arelle/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/plugin/test_loadfromoim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_modelmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_packagemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_qname.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_urlutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tests/unit_tests/arelle/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-07 03:15:07.000000 arelle-release-2.5.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.624981 arelle-release-2.5.8/vms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:15:35.768990 arelle-release-2.5.8/vms/mac/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-07 03:15:07.000000 arelle-release-2.5.8/vms/mac/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-04-07 03:15:07.000000 arelle-release-2.5.8/vms/mac/create-macos-bootable-for-virtualbox.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.394348 arelle-release-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.290345 arelle-release-2.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.290345 arelle-release-2.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/ISSUE_TEMPLATE/change.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.290345 arelle-release-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/build-and-release-linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/build-and-release-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/build-and-release-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/build-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/conformance-suites.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/test-ui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-14 14:25:21.000000 arelle-release-2.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-14 14:25:21.000000 arelle-release-2.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:25:21.000000 arelle-release-2.6.0/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 14:25:21.000000 arelle-release-2.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 14:25:21.000000 arelle-release-2.6.0/EFM-only-test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-14 14:25:21.000000 arelle-release-2.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-14 14:25:38.394348 arelle-release-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 14:25:21.000000 arelle-release-2.6.0/QuickBooks.qwc
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-14 14:25:21.000000 arelle-release-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.294345 arelle-release-2.6.0/apidocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-14 14:25:21.000000 arelle-release-2.6.0/apidocs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-14 14:25:21.000000 arelle-release-2.6.0/apidocs/arelle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-14 14:25:21.000000 arelle-release-2.6.0/apidocs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 14:25:21.000000 arelle-release-2.6.0/apidocs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-14 14:25:21.000000 arelle-release-2.6.0/apidocs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 14:25:21.000000 arelle-release-2.6.0/apidocs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.310345 arelle-release-2.6.0/arelle/
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/Aspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39740 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/Cntlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75674 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/CntlrCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/CntlrComServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/CntlrProfiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/CntlrQuickBooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48719 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/CntlrWebMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88038 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/CntlrWinMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/CntlrWinTooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogAbout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogArcroleGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogFind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogFormulaParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogNewFactItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogOpenArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogOpenTaxonomyPackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogPackageManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogRssWatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogURL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DialogUserPassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/DisclosureSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43688 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/FileSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/FunctionCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/FunctionFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80279 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/FunctionIxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/FunctionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71334 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/FunctionXfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/FunctionXs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/HashUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/HtmlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/InstanceAspectsEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/LeiUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/LocalViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28242 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/Locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119849 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelDocument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88883 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelDtsObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122124 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelFormulaObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72084 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelInstanceObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelObjectFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70336 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelRenderingObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelRssItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelRssObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelTestcaseObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38714 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelVersObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73327 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ModelXbrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/PackageManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29001 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/PluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/PrototypeDtsObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/PrototypeInstanceObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/PythonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/RenderingEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43733 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/RenderingResolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/SystemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/TableStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/TkTableWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/UITkTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/UiUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/Updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31897 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/UrlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49309 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/Validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51553 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateFilingText.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateUtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75131 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateXbrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateXbrlCalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100180 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateXbrlDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38118 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ValidateXbrlDimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileConcepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileFactList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileFactTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileRenderedGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileRoleTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileRssFeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewFileTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewUtilFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinConcepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinDiffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinFactGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinFactList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinFactTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinPane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78864 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinRenderedGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinRoleTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinRssFeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinTkTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinTupleGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/ViewWinXml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/WatchRss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/WebCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62211 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/XbrlConst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/XbrlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/XhtmlValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56504 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/XmlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44546 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/XmlValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/XmlValidateParticles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/XmlValidateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 14:25:37.000000 arelle-release-2.6.0/arelle/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.310345 arelle-release-2.6.0/arelle/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/arelle_test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/creationSoftwareNames.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/disclosuresystems.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/disclosuresystems.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/edbody.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/empty-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/erxl.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/mappings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/mappings.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/xbrlschemafiles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/xhtml-lat1.ent
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/xhtml-special.ent
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/xhtml-symbol.ent
+-rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/xhtml1-strict-ix.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/config/xhtml1_1-strict-ix.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.314345 arelle-release-2.6.0/arelle/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)   458032 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/doc/messagesCatalog.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/doc/messagesCatalog.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.314345 arelle-release-2.6.0/arelle/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/.pydevproject
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/CustomLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/LoadEFMvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/LoadSavePreLbCsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/LoadValidate.cs
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/LoadValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/LoadValidateCmdLine.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/LoadValidatePostedZip.java
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/LoadValidateWebService.java
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/SaveTableToExelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/TR3toTR4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.318345 arelle-release-2.6.0/arelle/examples/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/bigInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/cmdWebServerExtension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/crashTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/formulaSuiteConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/functionsCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/hello_dolly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/hello_i18n.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/hello_i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/importTestChild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/importTestChild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/importTestGrandchild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/importTestGrandchild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/importTestImported1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/importTestImported11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/importTestParent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/examples/plugin/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/examples/plugin/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.318345 arelle-release-2.6.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.318345 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestChild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestChild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestImported1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestImported11.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.318345 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.318345 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/sakaCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/saveInstanceInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/streamingExtensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/updateTableLB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/validateSchemaLxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/plugin/validateTableInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/us-gaap-dei-docType-extraction-frm.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/examples/us-gaap-dei-ratio-cash-frm.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.318345 arelle-release-2.6.0/arelle/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/formula/FactAspectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/formula/FormulaConsisAsser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83178 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/formula/FormulaEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98324 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/formula/ValidateFormula.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/formula/XPathContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/formula/XPathParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/formula/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.326346 arelle-release-2.6.0/arelle/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle-full-word.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle-mac-icon-4.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle-word-only.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   212911 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   392859 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle.icns.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle.xbm
+-rw-r--r--   0 runner    (1001) docker     (123)   269858 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle128.psd
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle16.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle16x16and32x32.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/arelle32.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/columnSortDown.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/columnSortUp.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/octocat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/python-clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)   696358 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/python-icon-pack-crystalxp.net-842.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarClose.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarCompare.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarDelete.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarFindMenu.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarLogClear - 1-piece-top.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarLogClear-orig.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarLogClear.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarNewFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarOpenDatabase.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarOpenFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarOpenWeb.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarProperties.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarQuit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarReopen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarSaveFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/toolbarValidate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/xbrl.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   201686 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/xbrl.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/xbrl128-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/xbrl128.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/xbrl16.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/images/xbrl32.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.326346 arelle-release-2.6.0/arelle/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/locale/ar_EG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.326346 arelle-release-2.6.0/arelle/locale/ar_EG/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   341883 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po
+-rw-r--r--   0 runner    (1001) docker     (123)   185904 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.326346 arelle-release-2.6.0/arelle/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149331 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/es/LC_MESSAGES/arelle.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.326346 arelle-release-2.6.0/arelle/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   118897 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/fr/LC_MESSAGES/arelle.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   168077 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/fr/LC_MESSAGES/fr.po
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   249762 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.326346 arelle-release-2.6.0/arelle/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   375378 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/ru/LC_MESSAGES/arelle.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   449579 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/locale/ru/LC_MESSAGES/ru.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.334346 arelle-release-2.6.0/arelle/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/EdgarRendererAllReports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/SECCorrespondenceLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/TDnetLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/UKCompaniesHouseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101637 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/formulaLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/formulaSaver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/formulaXPathChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/functionsMath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/functionsXmlCreation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41728 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/inlineXbrlDocumentSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/instanceInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/plugin/internet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.334346 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/U32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/des_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/des_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124382 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/loadFromExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76473 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/loadFromOIM-2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)   195836 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/loadFromOIM.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.334346 arelle-release-2.6.0/arelle/plugin/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/logging/dpmSignature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/logging/dqcParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/logging/saveMessages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/objectmaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/profileCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/profileFormula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/saveCHComponentFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/saveDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/saveHtmlEBAtables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/saveLoadableExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32261 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/saveLoadableOIM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/saveSKOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/saveSampleInstance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.334346 arelle-release-2.6.0/arelle/plugin/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/security/cryptAES_CBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/security/cryptAES_EAX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.334346 arelle-release-2.6.0/arelle/plugin/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/FormulaGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/SphinxContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35742 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/SphinxEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49810 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/SphinxMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/SphinxParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/SphinxValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/streamingExtensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.334346 arelle-release-2.6.0/arelle/plugin/transforms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.334346 arelle-release-2.6.0/arelle/plugin/transforms/SEC/
+-rw-r--r--   0 runner    (1001) docker     (123)    41892 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.342346 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/extractTestcase.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  4737705 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/saxon9.jar
+-rw-r--r--   0 runner    (1001) docker     (123)   225611 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/testcase.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    59680 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/text2num.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.342346 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.342346 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    55540 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/transforms/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/unpackSecEisFile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.346346 arelle-release-2.6.0/arelle/plugin/validate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.346346 arelle-release-2.6.0/arelle/plugin/validate/CIPC/
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/CIPC/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/CIPC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/CIPC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.346346 arelle-release-2.6.0/arelle/plugin/validate/EBA/
+-rw-r--r--   0 runner    (1001) docker     (123)    45950 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EBA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EBA/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.346346 arelle-release-2.6.0/arelle/plugin/validate/EFM/
+-rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/Consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/Document.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   253045 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/Filing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/PreCalAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.358347 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/axiswarnings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/cef-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/country-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/currency-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/dei-deprecated-concepts.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113832 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/dei-validations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76859 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/dqc-us-rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/ecd-deprecated-concepts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.362347 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/
+-rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    76545 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    76785 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    73012 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150333 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   138364 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   135467 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   180977 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   125792 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   134456 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   109498 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    99358 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28394 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29744 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31676 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   109944 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    35860 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    58455 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    62455 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    49163 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    48412 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    57294 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    69638 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   367560 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    93735 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/other-standard-taxonomies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/sic-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/signwarnings.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/srt-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/stpr-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205448 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1583747 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1624986 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1593440 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1613560 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/vip-deprecated-concepts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.346346 arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.346346 arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/ESEF/
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75625 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/ESEF/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF/resources/authority-validations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81794 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/FERC/
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/FERC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/FERC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/FERC/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/FERC/resources/ferc-utr.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/GFM/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/GFM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/GFM/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/HMRC/
+-rw-r--r--   0 runner    (1001) docker     (123)    29346 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/HMRC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/HMRC/config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25247 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/HMRC/consistencyChecksByName.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/ROS/
+-rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ROS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/ROS/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.366347 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/CustomLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59358 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/Document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/Filing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/USBestPractices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/USCorpAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/USSecTagging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.370347 arelle-release-2.6.0/arelle/plugin/validate/XDC/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/XDC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/XDC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.370347 arelle-release-2.6.0/arelle/plugin/validate/XFsyntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/XFsyntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/XFsyntax/xf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validate/calc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/validateSBRnl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.370347 arelle-release-2.6.0/arelle/plugin/xbrlDB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/DialogRssWatchExtender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56450 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/SqlDb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78257 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78348 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64539 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55073 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67782 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/entityInformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.370347 arelle-release-2.6.0/arelle/plugin/xbrlDB/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/ext/china.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/ext/edgar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/ext/xdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/primaryDocumentFacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.282344 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.370347 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.374347 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   714004 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.374347 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open2/
+-rw-r--r--   0 runner    (1001) docker     (123)   728541 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.374347 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   963416 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.378347 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    21988 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   728214 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)   729124 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)  1056221 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)   727913 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   726301 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xbrlDB/tableFacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/plugin/xuleSaver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.378347 arelle-release-2.6.0/arelle/scripts-macOS/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-macOS/startWebServer.command
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.378347 arelle-release-2.6.0/arelle/scripts-unix/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-unix/startWebServer.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.378347 arelle-release-2.6.0/arelle/scripts-windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/exportCsvFromXbrlInstance.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/runEFMTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/runFormulaTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/runFunctionTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/runXBRL21Tests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/runXDTTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/startWebServer.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/scripts-windows/validateAndRunFormulas.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/arelle/webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116069 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/webserver/bottle-no2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171083 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle/webserver/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle.pyw
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelleCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelleGUI.pyw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/arelle_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-14 14:25:38.000000 arelle-release-2.6.0/arelle_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-04-14 14:25:38.000000 arelle-release-2.6.0/arelle_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:25:38.000000 arelle-release-2.6.0/arelle_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 14:25:38.000000 arelle-release-2.6.0/arelle_release.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-14 14:25:38.000000 arelle-release-2.6.0/arelle_release.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 14:25:38.000000 arelle-release-2.6.0/arelle_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-14 14:25:21.000000 arelle-release-2.6.0/arelle_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/attic/
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-04-14 14:25:21.000000 arelle-release-2.6.0/attic/CntlrGenVersReports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 14:25:21.000000 arelle-release-2.6.0/buildVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 14:25:21.000000 arelle-release-2.6.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 14:25:21.000000 arelle-release-2.6.0/debugCmdLineEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-14 14:25:21.000000 arelle-release-2.6.0/distro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-14 14:25:21.000000 arelle-release-2.6.0/docker/ubuntu.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 14:25:21.000000 arelle-release-2.6.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-14 14:25:21.000000 arelle-release-2.6.0/encodeUtf8PySource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-04-14 14:25:21.000000 arelle-release-2.6.0/generateMessagesCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-14 14:25:21.000000 arelle-release-2.6.0/installWin64.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-14 14:25:21.000000 arelle-release-2.6.0/installWin86.nsi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/libs/linux/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/libs/linux/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/linux/Tktable2.11/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/libs/linux/Tktable2.11/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/linux/Tktable2.11/html/tkTable.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)   161976 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/linux/Tktable2.11/libTktable2.11.so
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/linux/Tktable2.11/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/linux/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/linux/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/linux/Tktable2.11/tktable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/libs/macos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/libs/macos/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/macos/Tktable2.11/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.382347 arelle-release-2.6.0/libs/macos/Tktable2.11/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/macos/Tktable2.11/html/tkTable.html
+-rw-r--r--   0 runner    (1001) docker     (123)   130952 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/macos/Tktable2.11/libTktable2.11.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/macos/Tktable2.11/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/macos/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/macos/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/macos/Tktable2.11/tktable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/libs/win64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.386347 arelle-release-2.6.0/libs/win64/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/win64/Tktable2.11/Tktable.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/win64/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-14 14:25:21.000000 arelle-release-2.6.0/libs/win64/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 14:25:21.000000 arelle-release-2.6.0/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-14 14:25:21.000000 arelle-release-2.6.0/msgfmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.386347 arelle-release-2.6.0/plugins/xbrl-us/
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-14 14:25:21.000000 arelle-release-2.6.0/plugins/xbrl-us/us-gaap-consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-04-14 14:25:21.000000 arelle-release-2.6.0/pygettext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-14 14:25:21.000000 arelle-release-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-14 14:25:21.000000 arelle-release-2.6.0/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 14:25:21.000000 arelle-release-2.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 14:25:21.000000 arelle-release-2.6.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-04-14 14:25:21.000000 arelle-release-2.6.0/runMacGUI.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-14 14:25:21.000000 arelle-release-2.6.0/runtime.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.386347 arelle-release-2.6.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/buildLinuxDist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/buildMacDist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/buildWinDist.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/charlieTest.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/exportCsvFormulae.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/exportCsvFromXbrlInstance.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/generateTestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/reportAllTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runAllTests.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runESMAtests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runGUI.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runGUI.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runGenerateVersioningTestcases.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runGeneratedTestcase.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runLocaleGettext.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runPackageTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runProfilerXDTTest.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runPyTest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runTR2Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runTR3Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runTR4Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runTR5Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runTRSECTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runUS-GFMTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/runVersioningConsumptionTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/startWebServer-27.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 14:25:21.000000 arelle-release-2.6.0/scripts/startWebServer.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-14 14:25:38.394348 arelle-release-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-14 14:25:21.000000 arelle-release-2.6.0/testParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-14 14:25:21.000000 arelle-release-2.6.0/testParser2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.386347 arelle-release-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/tests/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/tests/integration_tests/ui_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.386347 arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.386347 arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Usings.cs
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.390347 arelle-release-2.6.0/tests/integration_tests/ui_tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   223544 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/ui_tests/resources/workiva.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.390347 arelle-release-2.6.0/tests/integration_tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.390347 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_assertion_severity_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_link_role_registry_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29081 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_taxonomy_packages_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/download_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/run_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/test_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/integration_tests/validation/validation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.394348 arelle-release-2.6.0/tests/unit_tests/arelle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.394348 arelle-release-2.6.0/tests/unit_tests/arelle/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.394348 arelle-release-2.6.0/tests/unit_tests/arelle/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/plugin/test_loadfromoim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_modelmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_packagemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_qname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_urlutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tests/unit_tests/arelle/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 14:25:21.000000 arelle-release-2.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.286344 arelle-release-2.6.0/vms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:25:38.394348 arelle-release-2.6.0/vms/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-14 14:25:21.000000 arelle-release-2.6.0/vms/mac/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-04-14 14:25:21.000000 arelle-release-2.6.0/vms/mac/create-macos-bootable-for-virtualbox.sh
```

### Comparing `arelle-release-2.5.8/.github/ISSUE_TEMPLATE/bug.yml` & `arelle-release-2.6.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/build-and-release-linux.yml` & `arelle-release-2.6.0/.github/workflows/build-and-release-linux.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/build-and-release-mac.yml` & `arelle-release-2.6.0/.github/workflows/build-and-release-mac.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/build-and-release-windows.yml` & `arelle-release-2.6.0/.github/workflows/build-and-release-windows.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/build-windows.yml` & `arelle-release-2.6.0/.github/workflows/build-windows.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/python-package.yml` & `arelle-release-2.6.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/release.yml` & `arelle-release-2.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/test-ui.yml` & `arelle-release-2.6.0/.github/workflows/test-ui.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.github/workflows/tests.yml` & `arelle-release-2.6.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/.gitignore` & `arelle-release-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/CONTRIBUTING.md` & `arelle-release-2.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/EFM-only-test.ini` & `arelle-release-2.6.0/EFM-only-test.ini`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/LICENSE.md` & `arelle-release-2.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/PKG-INFO` & `arelle-release-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arelle-release
-Version: 2.5.8
+Version: 2.6.0
 Summary: An open source XBRL platform.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `arelle-release-2.5.8/QuickBooks.qwc` & `arelle-release-2.6.0/QuickBooks.qwc`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/README.md` & `arelle-release-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/apidocs/Makefile` & `arelle-release-2.6.0/apidocs/Makefile`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/apidocs/arelle.rst` & `arelle-release-2.6.0/apidocs/arelle.rst`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/apidocs/conf.py` & `arelle-release-2.6.0/apidocs/conf.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/apidocs/make.bat` & `arelle-release-2.6.0/apidocs/make.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/Aspect.py` & `arelle-release-2.6.0/arelle/Aspect.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/Cntlr.py` & `arelle-release-2.6.0/arelle/Cntlr.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/CntlrCmdLine.py` & `arelle-release-2.6.0/arelle/CntlrCmdLine.py`

 * *Files 13% similar despite different names*

```diff
@@ -108,53 +108,45 @@
                              "if either --calcDecimals or --calcPrecision are specified, and "
                              "SEC EDGAR Filing Manual (if --efm selected) or Global Filer Manual "
                              "disclosure system validation (if --gfm=XXX selected). "
                              "If a test suite or testcase, the test case variations "
                              "are individually so validated. "
                              "If formulae are present they will be validated and run unless --formula=none is specified. "
                              ))
-    parser.add_option("--noValidateTestcaseSchema", action="store_false", dest="validateTestcaseSchema", default=True,
+    parser.add_option("--noValidateTestcaseSchema", "--novalidatetestcaseschema", action="store_false", dest="validateTestcaseSchema", default=True,
                       help=_("Validate testcases against their schemas."))
-    parser.add_option("--novalidatetestcaseschema", action="store_false", dest="validateTestcaseSchema", default=True, help=SUPPRESS_HELP)
-    parser.add_option("--calcDecimals", action="store_true", dest="calcDecimals",
+    parser.add_option("--calcDecimals", "--calcdecimals", action="store_true", dest="calcDecimals",
                       help=_("Specify calculation linkbase validation inferring decimals."))
-    parser.add_option("--calcdecimals", action="store_true", dest="calcDecimals", help=SUPPRESS_HELP)
-    parser.add_option("--calcPrecision", action="store_true", dest="calcPrecision",
+    parser.add_option("--calcPrecision", "--calcprecision", action="store_true", dest="calcPrecision",
                       help=_("Specify calculation linkbase validation inferring precision."))
-    parser.add_option("--calcprecision", action="store_true", dest="calcPrecision", help=SUPPRESS_HELP)
-    parser.add_option("--calcDeduplicate", action="store_true", dest="calcDeduplicate",
+    parser.add_option("--calcDeduplicate", "--calcdeduplicate", action="store_true", dest="calcDeduplicate",
                       help=_("Specify de-duplication of consistent facts when performing calculation validation, chooses most accurate fact."))
-    parser.add_option("--calcdeduplicate", action="store_true", dest="calcDeduplicate", help=SUPPRESS_HELP)
     parser.add_option("--efm", action="store_true", dest="validateEFM",
                       help=_("Select Edgar Filer Manual (U.S. SEC) disclosure system validation (strict)."))
     parser.add_option("--efm-skip-calc-tree", action="store_false", default=True, dest="validateEFMCalcTree",
                       help=_("Skip walking of calculation tree during EFM validation."))
     parser.add_option("--gfm", action="store", dest="disclosureSystemName", help=SUPPRESS_HELP)
-    parser.add_option("--disclosureSystem", action="store", dest="disclosureSystemName",
+    parser.add_option("--disclosureSystem", "--disclosuresystem", action="store", dest="disclosureSystemName",
                       help=_("Specify a disclosure system name and"
                              " select disclosure system validation.  "
                              "Enter --disclosureSystem=help for list of names or help-verbose for list of names and descriptions. "))
-    parser.add_option("--disclosuresystem", action="store", dest="disclosureSystemName", help=SUPPRESS_HELP)
     parser.add_option("--hmrc", action="store_true", dest="validateHMRC",
                       help=_("Select U.K. HMRC disclosure system validation."))
     parser.add_option("--utr", action="store_true", dest="utrValidate",
                       help=_("Select validation with respect to Unit Type Registry."))
-    parser.add_option("--utrUrl", action="store", dest="utrUrl",
+    parser.add_option("--utrUrl", "--utrurl", action="store", dest="utrUrl",
                       help=_("Override disclosure systems Unit Type Registry location (URL or file path)."))
-    parser.add_option("--utrurl", action="store", dest="utrUrl", help=SUPPRESS_HELP)
     parser.add_option("--infoset", action="store_true", dest="infosetValidate",
                       help=_("Select validation with respect testcase infosets."))
-    parser.add_option("--labelLang", action="store", dest="labelLang",
+    parser.add_option("--labelLang", "--labellang", action="store", dest="labelLang",
                       help=_("Language for labels in following file options (override system settings)"))
-    parser.add_option("--labellang", action="store", dest="labelLang", help=SUPPRESS_HELP)
     parser.add_option("--disableRtl", action="store_true", dest="disableRtl", default=False,
                        help=_("Flag to disable reversing string read order for right to left languages, useful for some locale settings"))
-    parser.add_option("--labelRole", action="store", dest="labelRole",
+    parser.add_option("--labelRole", "--labelrole", action="store", dest="labelRole",
                       help=_("Label role for labels in following file options (instead of standard label)"))
-    parser.add_option("--labelrole", action="store", dest="labelRole", help=SUPPRESS_HELP)
     parser.add_option("--DTS", "--csvDTS", action="store", dest="DTSFile",
                       help=_("Write DTS tree into FILE (may be .csv or .html)"))
     parser.add_option("--facts", "--csvFacts", action="store", dest="factsFile",
                       help=_("Write fact list into FILE"))
     parser.add_option("--factListCols", action="store", dest="factListCols",
                       help=_("Columns for fact list file"))
     parser.add_option("--factTable", "--csvFactTable", action="store", dest="factTableFile",
@@ -171,200 +163,144 @@
                       help=_("Write calculation linkbase into FILE"))
     parser.add_option("--dim", "--csvDim", action="store", dest="dimFile",
                       help=_("Write dimensions (of definition) linkbase into FILE"))
     parser.add_option("--anch", action="store", dest="anchFile",
                       help=_("Write anchoring relationships (of definition) linkbase into FILE"))
     parser.add_option("--formulae", "--htmlFormulae", action="store", dest="formulaeFile",
                       help=_("Write formulae linkbase into FILE"))
-    parser.add_option("--viewArcrole", action="store", dest="viewArcrole",
+    parser.add_option("--viewArcrole", "--viewarcrole", action="store", dest="viewArcrole",
                       help=_("Write linkbase relationships for viewArcrole into viewFile"))
-    parser.add_option("--viewarcrole", action="store", dest="viewArcrole", help=SUPPRESS_HELP)
-    parser.add_option("--viewFile", action="store", dest="viewFile",
+    parser.add_option("--viewFile", "--viewfile", action="store", dest="viewFile",
                       help=_("Write linkbase relationships for viewArcrole into viewFile"))
-    parser.add_option("--relationshipCols", action="store", dest="relationshipCols",
+    parser.add_option("--relationshipCols", "--relationshipcols", action="store", dest="relationshipCols",
                       help=_("Extra columns for relationship file (comma or space separated: Name, Namespace, LocalName, Documentation and References)"))
-    parser.add_option("--relationshipcols", action="store", dest="relationshipCols", help=SUPPRESS_HELP)
-    parser.add_option("--viewfile", action="store", dest="viewFile", help=SUPPRESS_HELP)
-    parser.add_option("--roleTypes", action="store", dest="roleTypesFile",
+    parser.add_option("--roleTypes", "--roletypes", action="store", dest="roleTypesFile",
                       help=_("Write defined role types into FILE"))
-    parser.add_option("--roletypes", action="store", dest="roleTypesFile", help=SUPPRESS_HELP)
-    parser.add_option("--arcroleTypes", action="store", dest="arcroleTypesFile",
+    parser.add_option("--arcroleTypes", "--arcroletypes", action="store", dest="arcroleTypesFile",
                       help=_("Write defined arcrole types into FILE"))
-    parser.add_option("--arcroletypes", action="store", dest="arcroleTypesFile", help=SUPPRESS_HELP)
-    parser.add_option("--testReport", "--csvTestReport", action="store", dest="testReport",
+    parser.add_option("--testReport", "--csvTestReport", "--testreport", "--csvtestreport", action="store", dest="testReport",
                       help=_("Write test report of validation (of test cases) into FILE"))
-    parser.add_option("--testreport", "--csvtestreport", action="store", dest="testReport", help=SUPPRESS_HELP)
-    parser.add_option("--testReportCols", action="store", dest="testReportCols",
+    parser.add_option("--testReportCols", "--testreportcols", action="store", dest="testReportCols",
                       help=_("Columns for test report file"))
-    parser.add_option("--testreportcols", action="store", dest="testReportCols", help=SUPPRESS_HELP)
-    parser.add_option("--rssReport", action="store", dest="rssReport",
+    parser.add_option("--rssReport", "--rssreport", action="store", dest="rssReport",
                       help=_("Write RSS report into FILE"))
-    parser.add_option("--rssreport", action="store", dest="rssReport", help=SUPPRESS_HELP)
-    parser.add_option("--rssReportCols", action="store", dest="rssReportCols",
+    parser.add_option("--rssReportCols", "--rssreportcols", action="store", dest="rssReportCols",
                       help=_("Columns for RSS report file"))
-    parser.add_option("--rssreportcols", action="store", dest="rssReportCols", help=SUPPRESS_HELP)
-    parser.add_option("--skipDTS", action="store_true", dest="skipDTS",
+    parser.add_option("--skipDTS", "--skipdts", action="store_true", dest="skipDTS",
                       help=_("Skip DTS activities (loading, discovery, validation), useful when an instance needs only to be parsed."))
-    parser.add_option("--skipdts", action="store_true", dest="skipDTS", help=SUPPRESS_HELP)
-    parser.add_option("--skipLoading", action="store", dest="skipLoading",
+    parser.add_option("--skipLoading", "--skiploading", action="store", dest="skipLoading",
                       help=_("Skip loading discovered or schemaLocated files matching pattern (unix-style file name patterns separated by '|'), useful when not all linkbases are needed."))
-    parser.add_option("--skiploading", action="store", dest="skipLoading", help=SUPPRESS_HELP)
-    parser.add_option("--logFile", action="store", dest="logFile",
+    parser.add_option("--logFile", "--logfile", action="store", dest="logFile",
                       help=_("Write log messages into file, otherwise they go to standard output.  "
                              "If file ends in .xml it is xml-formatted, otherwise it is text. "))
-    parser.add_option("--logfile", action="store", dest="logFile", help=SUPPRESS_HELP)
-    parser.add_option("--logFormat", action="store", dest="logFormat",
+    parser.add_option("--logFormat", "--logformat", action="store", dest="logFormat",
                       help=_("Logging format for messages capture, otherwise default is \"[%(messageCode)s] %(message)s - %(file)s\"."))
-    parser.add_option("--logformat", action="store", dest="logFormat", help=SUPPRESS_HELP)
-    parser.add_option("--logLevel", action="store", dest="logLevel",
+    parser.add_option("--logLevel", "--loglevel", action="store", dest="logLevel",
                       help=_("Minimum level for messages capture, otherwise the message is ignored.  "
                              "Current order of levels are debug, info, info-semantic, warning, warning-semantic, warning, assertion-satisfied, inconsistency, error-semantic, assertion-not-satisfied, and error. "))
-    parser.add_option("--loglevel", action="store", dest="logLevel", help=SUPPRESS_HELP)
-    parser.add_option("--logLevelFilter", action="store", dest="logLevelFilter",
+    parser.add_option("--logLevelFilter", "--loglevelfilter", action="store", dest="logLevelFilter",
                       help=_("Regular expression filter for logLevel.  "
                              "(E.g., to not match *-semantic levels, logLevelFilter=(?!^.*-semantic$)(.+). "))
-    parser.add_option("--loglevelfilter", action="store", dest="logLevelFilter", help=SUPPRESS_HELP)
-    parser.add_option("--logCodeFilter", action="store", dest="logCodeFilter",
+    parser.add_option("--logCodeFilter", "--logcodefilter", action="store", dest="logCodeFilter",
                       help=_("Regular expression filter for log message code."))
-    parser.add_option("--logcodefilter", action="store", dest="logCodeFilter", help=SUPPRESS_HELP)
-    parser.add_option("--logTextMaxLength", action="store", dest="logTextMaxLength", type="int",
+    parser.add_option("--logTextMaxLength", "--logtextmaxlength", action="store", dest="logTextMaxLength", type="int",
                       help=_("Log file text field max length override."))
-    parser.add_option("--logtextmaxlength", action="store", dest="logTextMaxLength", type="int", help=SUPPRESS_HELP)
-    parser.add_option("--logRefObjectProperties", action="store_true", dest="logRefObjectProperties",
+    parser.add_option("--logRefObjectProperties", "--logrefobjectproperties", action="store_true", dest="logRefObjectProperties",
                       help=_("Log reference object properties (default)."), default=True)
-    parser.add_option("--logrefobjectproperties", action="store_true", dest="logRefObjectProperties", help=SUPPRESS_HELP)
-    parser.add_option("--logNoRefObjectProperties", action="store_false", dest="logRefObjectProperties",
+    parser.add_option("--logNoRefObjectProperties", "--lognorefobjectproperties", action="store_false", dest="logRefObjectProperties",
                       help=_("Do not log reference object properties."))
-    parser.add_option("--lognorefobjectproperties", action="store_false", dest="logRefObjectProperties", help=SUPPRESS_HELP)
     parser.add_option("--statusPipe", action="store", dest="statusPipe", help=SUPPRESS_HELP)
     parser.add_option("--monitorParentProcess", action="store", dest="monitorParentProcess", help=SUPPRESS_HELP)
-    parser.add_option("--outputAttribution", action="store", dest="outputAttribution", help=SUPPRESS_HELP)
-    parser.add_option("--outputattribution", action="store", dest="outputAttribution", help=SUPPRESS_HELP)
+    parser.add_option("--outputAttribution", "--outputattribution", action="store", dest="outputAttribution", help=SUPPRESS_HELP)
     parser.add_option("--showOptions", action="store_true", dest="showOptions", help=SUPPRESS_HELP)
     parser.add_option("--parameters", action="store", dest="parameters", help=_("Specify parameters for formula and validation (name=value[,name=value])."))
-    parser.add_option("--parameterSeparator", action="store", dest="parameterSeparator", help=_("Specify parameters separator string (if other than comma)."))
-    parser.add_option("--parameterseparator", action="store", dest="parameterSeparator", help=SUPPRESS_HELP)
+    parser.add_option("--parameterSeparator", "--parameterseparator", action="store", dest="parameterSeparator", help=_("Specify parameters separator string (if other than comma)."))
     parser.add_option("--formula", choices=("validate", "run", "none"), dest="formulaAction",
                       help=_("Specify formula action: "
                              "validate - validate only, without running, "
                              "run - validate and run, or "
                              "none - prevent formula validation or running when also specifying -v or --validate.  "
                              "if this option is not specified, -v or --validate will validate and run formulas if present"))
-    parser.add_option("--formulaParamExprResult", action="store_true", dest="formulaParamExprResult", help=_("Specify formula tracing."))
-    parser.add_option("--formulaparamexprresult", action="store_true", dest="formulaParamExprResult", help=SUPPRESS_HELP)
-    parser.add_option("--formulaParamInputValue", action="store_true", dest="formulaParamInputValue", help=_("Specify formula tracing."))
-    parser.add_option("--formulaparaminputvalue", action="store_true", dest="formulaParamInputValue", help=SUPPRESS_HELP)
-    parser.add_option("--formulaCallExprSource", action="store_true", dest="formulaCallExprSource", help=_("Specify formula tracing."))
-    parser.add_option("--formulacallexprsource", action="store_true", dest="formulaCallExprSource", help=SUPPRESS_HELP)
-    parser.add_option("--formulaCallExprCode", action="store_true", dest="formulaCallExprCode", help=_("Specify formula tracing."))
-    parser.add_option("--formulacallexprcode", action="store_true", dest="formulaCallExprCode", help=SUPPRESS_HELP)
-    parser.add_option("--formulaCallExprEval", action="store_true", dest="formulaCallExprEval", help=_("Specify formula tracing."))
-    parser.add_option("--formulacallexpreval", action="store_true", dest="formulaCallExprEval", help=SUPPRESS_HELP)
-    parser.add_option("--formulaCallExprResult", action="store_true", dest="formulaCallExprResult", help=_("Specify formula tracing."))
-    parser.add_option("--formulacallexprtesult", action="store_true", dest="formulaCallExprResult", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarSetExprEval", action="store_true", dest="formulaVarSetExprEval", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarsetexpreval", action="store_true", dest="formulaVarSetExprEval", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarSetExprResult", action="store_true", dest="formulaVarSetExprResult", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarsetexprresult", action="store_true", dest="formulaVarSetExprResult", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarSetTiming", action="store_true", dest="timeVariableSetEvaluation", help=_("Specify showing times of variable set evaluation."))
-    parser.add_option("--formulavarsettiming", action="store_true", dest="timeVariableSetEvaluation", help=SUPPRESS_HELP)
-    parser.add_option("--formulaAsserResultCounts", action="store_true", dest="formulaAsserResultCounts", help=_("Specify formula tracing."))
-    parser.add_option("--formulaasserresultcounts", action="store_true", dest="formulaAsserResultCounts", help=SUPPRESS_HELP)
-    parser.add_option("--formulaSatisfiedAsser", action="store_true", dest="formulaSatisfiedAsser", help=_("Specify formula tracing."))
-    parser.add_option("--formulasatisfiedasser", action="store_true", dest="formulaSatisfiedAsser", help=SUPPRESS_HELP)
-    parser.add_option("--formulaUnsatisfiedAsser", action="store_true", dest="formulaUnsatisfiedAsser", help=_("Specify formula tracing."))
-    parser.add_option("--formulaunsatisfiedasser", action="store_true", dest="formulaUnsatisfiedAsser", help=SUPPRESS_HELP)
-    parser.add_option("--formulaUnsatisfiedAsserError", action="store_true", dest="formulaUnsatisfiedAsserError", help=_("Specify formula tracing."))
-    parser.add_option("--formulaunsatisfiedassererror", action="store_true", dest="formulaUnsatisfiedAsserError", help=SUPPRESS_HELP)
-    parser.add_option("--formulaUnmessagedUnsatisfiedAsser", action="store_true", dest="formulaUnmessagedUnsatisfiedAsser", help=_("Specify trace messages for unsatisfied assertions with no formula messages."))
-    parser.add_option("--formulaunmessagedunsatisfiedasser", action="store_true", dest="formulaUnmessagedUnsatisfiedAsser", help=SUPPRESS_HELP)
-    parser.add_option("--formulaFormulaRules", action="store_true", dest="formulaFormulaRules", help=_("Specify formula tracing."))
-    parser.add_option("--formulaformularules", action="store_true", dest="formulaFormulaRules", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarsOrder", action="store_true", dest="formulaVarsOrder", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarsorder", action="store_true", dest="formulaVarsOrder", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarExpressionSource", action="store_true", dest="formulaVarExpressionSource", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarexpressionsource", action="store_true", dest="formulaVarExpressionSource", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarExpressionCode", action="store_true", dest="formulaVarExpressionCode", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarexpressioncode", action="store_true", dest="formulaVarExpressionCode", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarExpressionEvaluation", action="store_true", dest="formulaVarExpressionEvaluation", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarexpressionevaluation", action="store_true", dest="formulaVarExpressionEvaluation", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarExpressionResult", action="store_true", dest="formulaVarExpressionResult", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarexpressionresult", action="store_true", dest="formulaVarExpressionResult", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarFilterWinnowing", action="store_true", dest="formulaVarFilterWinnowing", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarfilterwinnowing", action="store_true", dest="formulaVarFilterWinnowing", help=SUPPRESS_HELP)
-    parser.add_option("--formulaVarFiltersResult", action="store_true", dest="formulaVarFiltersResult", help=_("Specify formula tracing."))
-    parser.add_option("--formulavarfiltersresult", action="store_true", dest="formulaVarFiltersResult", help=SUPPRESS_HELP)
-    parser.add_option("--testcaseResultsCaptureWarnings", action="store_true", dest="testcaseResultsCaptureWarnings",
+    parser.add_option("--formulaParamExprResult", "--formulaparamexprresult", action="store_true", dest="formulaParamExprResult", help=_("Specify formula tracing."))
+    parser.add_option("--formulaParamInputValue", "--formulaparaminputvalue", action="store_true", dest="formulaParamInputValue", help=_("Specify formula tracing."))
+    parser.add_option("--formulaCallExprSource", "--formulacallexprsource", action="store_true", dest="formulaCallExprSource", help=_("Specify formula tracing."))
+    parser.add_option("--formulaCallExprCode", "--formulacallexprcode", action="store_true", dest="formulaCallExprCode", help=_("Specify formula tracing."))
+    parser.add_option("--formulaCallExprEval", "--formulacallexpreval", action="store_true", dest="formulaCallExprEval", help=_("Specify formula tracing."))
+    parser.add_option("--formulaCallExprResult", "--formulacallexprtesult", action="store_true", dest="formulaCallExprResult", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarSetExprEval", "--formulavarsetexpreval", action="store_true", dest="formulaVarSetExprEval", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarSetExprResult", "--formulavarsetexprresult", action="store_true", dest="formulaVarSetExprResult", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarSetTiming", "--formulavarsettiming", action="store_true", dest="timeVariableSetEvaluation", help=_("Specify showing times of variable set evaluation."))
+    parser.add_option("--formulaAsserResultCounts", "--formulaasserresultcounts", action="store_true", dest="formulaAsserResultCounts", help=_("Specify formula tracing."))
+    parser.add_option("--formulaSatisfiedAsser", "--formulasatisfiedasser", action="store_true", dest="formulaSatisfiedAsser", help=_("Specify formula tracing."))
+    parser.add_option("--formulaUnsatisfiedAsser", "--formulaunsatisfiedasser", action="store_true", dest="formulaUnsatisfiedAsser", help=_("Specify formula tracing."))
+    parser.add_option("--formulaUnsatisfiedAsserError", "--formulaunsatisfiedassererror", action="store_true", dest="formulaUnsatisfiedAsserError", help=_("Specify formula tracing."))
+    parser.add_option("--formulaUnmessagedUnsatisfiedAsser", "--formulaunmessagedunsatisfiedasser", action="store_true", dest="formulaUnmessagedUnsatisfiedAsser", help=_("Specify trace messages for unsatisfied assertions with no formula messages."))
+    parser.add_option("--formulaFormulaRules", "--formulaformularules", action="store_true", dest="formulaFormulaRules", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarsOrder", "--formulavarsorder", action="store_true", dest="formulaVarsOrder", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarExpressionSource", "--formulavarexpressionsource", action="store_true", dest="formulaVarExpressionSource", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarExpressionCode", "--formulavarexpressioncode", action="store_true", dest="formulaVarExpressionCode", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarExpressionEvaluation", "--formulavarexpressionevaluation", action="store_true", dest="formulaVarExpressionEvaluation", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarExpressionResult", "--formulavarexpressionresult", action="store_true", dest="formulaVarExpressionResult", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarFilterWinnowing", "--formulavarfilterwinnowing", action="store_true", dest="formulaVarFilterWinnowing", help=_("Specify formula tracing."))
+    parser.add_option("--formulaVarFiltersResult", "--formulavarfiltersresult", action="store_true", dest="formulaVarFiltersResult", help=_("Specify formula tracing."))
+    parser.add_option("--testcaseResultsCaptureWarnings", "--testcaseresultscapturewarnings", action="store_true", dest="testcaseResultsCaptureWarnings",
                       help=_("For testcase variations capture warning results, default is inconsistency or warning if there is any warning expected result.  "))
-    parser.add_option("--testcaseresultscapturewarnings", action="store_true", dest="testcaseResultsCaptureWarnings", help=SUPPRESS_HELP)
     parser.add_option("--testcaseResultOptions", choices=("match-any", "match-all"), action="store", dest="testcaseResultOptions",
                       help=_("For testcase results, default is match any expected result, options to match any or match all expected result(s).  "))
-    parser.add_option("--formulaRunIDs", action="store", dest="formulaRunIDs", help=_("Specify formula/assertion IDs to run, separated by a '|' character, or a regex expression."))
-    parser.add_option("--formularunids", action="store", dest="formulaRunIDs", help=SUPPRESS_HELP)
-    parser.add_option("--formulaCompileOnly", action="store_true", dest="formulaCompileOnly", help=_("Specify formula are to be compiled but not executed."))
-    parser.add_option("--formulacompileonly", action="store_true", dest="formulaCompileOnly", help=SUPPRESS_HELP)
+    parser.add_option("--formulaRunIDs", "--formularunids", action="store", dest="formulaRunIDs", help=_("Specify formula/assertion IDs to run, separated by a '|' character, or a regex expression."))
+    parser.add_option("--formulaCompileOnly", "--formulacompileonly", action="store_true", dest="formulaCompileOnly", help=_("Specify formula are to be compiled but not executed."))
     parser.add_option("--formulaCacheSize", "--formulacachesize", action="store", dest="formulaCacheSize", help=_("Specify the number of fact aspect combinations to cache during formula evaluations. Negative numbers have no limit. (10_000_000 is default)"))
-    parser.add_option(UILANG_OPTION, action="store", dest="uiLang",
+    parser.add_option(UILANG_OPTION, UILANG_OPTION.lower(), action="store", dest="uiLang",
                       help=_("Language for user interface (override system settings, such as program messages).  Does not save setting.  Requires locale country code, e.g. en-GB or en-US."))
-    parser.add_option(UILANG_OPTION.lower(), action="store", dest="uiLang", help=SUPPRESS_HELP)
     parser.add_option("--proxy", action="store", dest="proxy",
                       help=_("Modify and re-save proxy settings configuration.  "
                              "Enter 'system' to use system proxy setting, 'none' to use no proxy, "
                              "'http://[user[:password]@]host[:port]' "
                              " (e.g., http://192.168.1.253, http://example.com:8080, http://joe:secret@example.com:8080), "
                              " or 'show' to show current setting, ." ))
-    parser.add_option("--internetConnectivity", choices=("online", "offline"), dest="internetConnectivity",
+    parser.add_option("--internetConnectivity", "--internetconnectivity", choices=("online", "offline"), dest="internetConnectivity",
                       help=_("Specify internet connectivity: online or offline"))
-    parser.add_option("--internetconnectivity", action="store", dest="internetConnectivity", help=SUPPRESS_HELP)
-    parser.add_option("--internetTimeout", type="int", dest="internetTimeout",
+    parser.add_option("--internetTimeout", "--internettimeout", type="int", dest="internetTimeout",
                       help=_("Specify internet connection timeout in seconds (0 means unlimited)."))
-    parser.add_option("--internettimeout", type="int", action="store", dest="internetTimeout", help=SUPPRESS_HELP)
-    parser.add_option("--internetRecheck", choices=("weekly", "daily", "never", "hourly", "quarter-hourly"), action="store", dest="internetRecheck",
+    parser.add_option("--internetRecheck", "--internetrecheck", choices=("weekly", "daily", "never", "hourly", "quarter-hourly"), action="store", dest="internetRecheck",
                       help=_("Specify rechecking for newer cache files 'daily', 'weekly', 'monthly' or 'never' ('weekly' is default)"))
-    parser.add_option("--internetrecheck", choices=("weekly", "daily", "never"), action="store", dest="internetRecheck", help=SUPPRESS_HELP)
-    parser.add_option("--internetLogDownloads", action="store_true", dest="internetLogDownloads",
+    parser.add_option("--internetLogDownloads", "--internetlogdownloads", action="store_true", dest="internetLogDownloads",
                       help=_("Log info message for downloads to web cache."))
-    parser.add_option("--internetlogdownloads", action="store_true", dest="internetLogDownloads", help=SUPPRESS_HELP)
-    parser.add_option("--noCertificateCheck", action="store_true", dest="noCertificateCheck",
+    parser.add_option("--noCertificateCheck", "--nocertificatecheck", action="store_true", dest="noCertificateCheck",
                       help=_("Specify no checking of internet secure connection certificate"))
-    parser.add_option("--nocertificatecheck", action="store_true", dest="noCertificateCheck", help=SUPPRESS_HELP)
-    parser.add_option("--httpsRedirectCache", action="store_true", dest="httpsRedirectCache",
+    parser.add_option("--httpsRedirectCache", "--httpsredirectcache", action="store_true", dest="httpsRedirectCache",
                       help=_("Treat http and https schemes interchangeably when looking up files from the webcache"))
-    parser.add_option("--httpsredirectcache", action="store_true", dest="httpsRedirectCache", help=SUPPRESS_HELP)
-    parser.add_option("--httpUserAgent", action="store", dest="httpUserAgent",
+    parser.add_option("--httpUserAgent", "--httpuseragent", action="store", dest="httpUserAgent",
                       help=_("Specify non-standard http header User-Agent value"))
-    parser.add_option("--httpuseragent", action="store", dest="httpUserAgent", help=SUPPRESS_HELP)
     parser.add_option("--xdgConfigHome", action="store", dest="xdgConfigHome",
                       help=_("Specify non-standard location for configuration and cache files (overrides environment parameter XDG_CONFIG_HOME)."))
     parser.add_option("--plugins", action="store", dest="plugins",
                       help=_("Specify plug-in configuration for this invocation.  "
                              "Enter 'show' to confirm plug-in configuration.  "
                              "Commands show, and module urls are '|' separated: "
                              "url specifies a plug-in by its url or filename, "
                              "relative URLs are relative to installation plug-in directory, "
                              R" (e.g., 'http://arelle.org/files/hello_web.py', 'C:\Program Files\Arelle\examples\plugin\hello_dolly.py' to load, "
                              "or ../examples/plugin/hello_dolly.py for relative use of examples directory) "
                              "Local python files do not require .py suffix, e.g., hello_dolly without .py is sufficient, "
                              "Packaged plug-in urls are their directory's url (e.g., --plugins EdgarRenderer or --plugins xbrlDB).  " ))
-    parser.add_option("--packages", action="store", dest="packages",
+    parser.add_option("--packages", "--package", action="store", dest="packages",
                       help=_("Specify taxonomy packages configuration.  "
                              "Enter 'show' to show current packages configuration.  "
                              "Commands show, and module urls are '|' separated: "
                              "url specifies a package by its url or filename, please use full paths. "
                              "(Package settings from GUI are no longer shared with cmd line operation. "
                              "Cmd line package settings are not persistent.)  " ))
-    parser.add_option("--package", action="store", dest="packages", help=SUPPRESS_HELP)
     parser.add_option("--packageManifestName", action="store", dest="packageManifestName",
                       help=_("Provide non-standard archive manifest file name pattern (e.g., *taxonomyPackage.xml).  "
                              "Uses unix file name pattern matching.  "
                              "Multiple manifest files are supported in archive (such as oasis catalogs).  "
                              "(Replaces search for either .taxonomyPackage.xml or catalog.xml).  " ))
     parser.add_option("--abortOnMajorError", action="store_true", dest="abortOnMajorError", help=_("Abort process on major error, such as when load is unable to find an entry or discovered file."))
-    parser.add_option("--showEnvironment", action="store_true", dest="showEnvironment", help=_("Show Arelle's config and cache directory and host OS environment parameters."))
-    parser.add_option("--showenvironment", action="store_true", dest="showEnvironment", help=SUPPRESS_HELP)
+    parser.add_option("--showEnvironment", "--showenvironment", action="store_true", dest="showEnvironment", help=_("Show Arelle's config and cache directory and host OS environment parameters."))
     parser.add_option("--collectProfileStats", action="store_true", dest="collectProfileStats", help=_("Collect profile statistics, such as timing of validation activities and formulae."))
     if hasWebServer:
         parser.add_option("--webserver", action="store", dest="webserver",
                           help=_("start web server on host:port[:server] for REST and web access, e.g., --webserver locahost:8080, "
                                  "or specify nondefault a server name, such as cherrypy, --webserver locahost:8080:cherrypy. "
                                  "(It is possible to specify options to be defaults for the web server, such as disclosureSystem and validations, but not including file names.) "))
     pluginOptionsIndex = len(parser.option_list)
```

### Comparing `arelle-release-2.5.8/arelle/CntlrComServer.py` & `arelle-release-2.6.0/arelle/CntlrComServer.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/CntlrProfiler.py` & `arelle-release-2.6.0/arelle/CntlrProfiler.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/CntlrQuickBooks.py` & `arelle-release-2.6.0/arelle/CntlrQuickBooks.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/CntlrWebMain.py` & `arelle-release-2.6.0/arelle/CntlrWebMain.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/CntlrWinMain.py` & `arelle-release-2.6.0/arelle/CntlrWinMain.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/CntlrWinTooltip.py` & `arelle-release-2.6.0/arelle/CntlrWinTooltip.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogAbout.py` & `arelle-release-2.6.0/arelle/DialogAbout.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogArcroleGroup.py` & `arelle-release-2.6.0/arelle/DialogArcroleGroup.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogFind.py` & `arelle-release-2.6.0/arelle/DialogFind.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogFormulaParameters.py` & `arelle-release-2.6.0/arelle/DialogFormulaParameters.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogLanguage.py` & `arelle-release-2.6.0/arelle/DialogLanguage.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogNewFactItem.py` & `arelle-release-2.6.0/arelle/DialogNewFactItem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogOpenArchive.py` & `arelle-release-2.6.0/arelle/DialogOpenArchive.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogPackageManager.py` & `arelle-release-2.6.0/arelle/DialogPackageManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogPluginManager.py` & `arelle-release-2.6.0/arelle/DialogPluginManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogRssWatch.py` & `arelle-release-2.6.0/arelle/DialogRssWatch.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogURL.py` & `arelle-release-2.6.0/arelle/DialogURL.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DialogUserPassword.py` & `arelle-release-2.6.0/arelle/DialogUserPassword.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/DisclosureSystem.py` & `arelle-release-2.6.0/arelle/DisclosureSystem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/FileSource.py` & `arelle-release-2.6.0/arelle/FileSource.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/FunctionCustom.py` & `arelle-release-2.6.0/arelle/FunctionCustom.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/FunctionFn.py` & `arelle-release-2.6.0/arelle/FunctionFn.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/FunctionIxt.py` & `arelle-release-2.6.0/arelle/FunctionIxt.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/FunctionUtil.py` & `arelle-release-2.6.0/arelle/FunctionUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/FunctionXfi.py` & `arelle-release-2.6.0/arelle/FunctionXfi.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/FunctionXs.py` & `arelle-release-2.6.0/arelle/FunctionXs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/HashUtil.py` & `arelle-release-2.6.0/arelle/HashUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/HtmlUtil.py` & `arelle-release-2.6.0/arelle/HtmlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/InstanceAspectsEvaluator.py` & `arelle-release-2.6.0/arelle/InstanceAspectsEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/LeiUtil.py` & `arelle-release-2.6.0/arelle/LeiUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/LocalViewer.py` & `arelle-release-2.6.0/arelle/LocalViewer.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/Locale.py` & `arelle-release-2.6.0/arelle/Locale.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelDocument.py` & `arelle-release-2.6.0/arelle/ModelDocument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1317,19 +1317,21 @@
             self.modelXbrl.error("ix:multipleIxNamespaces",
                     _("Multiple ix namespaces were found"),
                     modelObject=conflictingNSelts)
         self.ixNS = ixNS
         self.ixNStag = ixNStag = "{" + ixNS + "}" if ixNS else ""
         self.htmlBase = htmlBase
         ixdsTarget = getattr(self.modelXbrl, "ixdsTarget", None)
-        # load referenced schemas and linkbases (before validating inline HTML
-        for inlineElement in htmlElement.iterdescendants(tag=ixNStag + "references"):
-            if inlineElement.get("target") == ixdsTarget:
-                self.schemaLinkbaseRefsDiscover(inlineElement)
-                xmlValidate(self.modelXbrl, inlineElement) # validate instance elements
+        if all(pluginMethod(self.modelXbrl)
+               for pluginMethod in pluginClassMethods("ModelDocument.DiscoverIxdsDts")):
+            # load referenced schemas and linkbases (before validating inline HTML
+            for inlineElement in htmlElement.iterdescendants(tag=ixNStag + "references"):
+                if inlineElement.get("target") == ixdsTarget:
+                    self.schemaLinkbaseRefsDiscover(inlineElement)
+                    xmlValidate(self.modelXbrl, inlineElement) # validate instance elements
         # with DTS loaded, now validate inline HTML (so schema definition of facts is available)
         if htmlElement.namespaceURI == XbrlConst.xhtml:  # must validate xhtml
             XhtmlValidate.xhtmlValidate(self.modelXbrl, htmlElement)  # fails on prefixed content
         for inlineElement in htmlElement.iterdescendants(tag=ixNStag + "resources"):
             xmlValidate(self.modelXbrl, inlineElement) # validate instance elements
 
         # subsequent inline elements have to be processed after all of the document set is loaded
@@ -1432,14 +1434,16 @@
                 if r.referringModelObject is None and referringModelObject is not None:
                     r.referringModelObject = referringModelObject
 
 
 # inline document set level compilation
 # modelIxdsDocument is an inlineDocumentSet or entry inline document (if not a document set)
 def inlineIxdsDiscover(modelXbrl, modelIxdsDocument):
+    for pluginMethod in pluginClassMethods("ModelDocument.SelectIxdsTarget"):
+        pluginMethod(modelXbrl)
     # extract for a single target document
     ixdsTarget = getattr(modelXbrl, "ixdsTarget", None)
     # compile inline result set
     ixdsEltById = defaultdict(list)
     for htmlElement in modelXbrl.ixdsHtmlElements:
         for elt in htmlElement.iterfind(".//*[@id]"):
             if isinstance(elt,ModelObject) and elt.id:
```

### Comparing `arelle-release-2.5.8/arelle/ModelDtsObject.py` & `arelle-release-2.6.0/arelle/ModelDtsObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelFormulaObject.py` & `arelle-release-2.6.0/arelle/ModelFormulaObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelInstanceObject.py` & `arelle-release-2.6.0/arelle/ModelInstanceObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelManager.py` & `arelle-release-2.6.0/arelle/ModelManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelObject.py` & `arelle-release-2.6.0/arelle/ModelObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelObjectFactory.py` & `arelle-release-2.6.0/arelle/ModelObjectFactory.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelRelationshipSet.py` & `arelle-release-2.6.0/arelle/ModelRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelRenderingObject.py` & `arelle-release-2.6.0/arelle/ModelRenderingObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelRssItem.py` & `arelle-release-2.6.0/arelle/ModelRssItem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelRssObject.py` & `arelle-release-2.6.0/arelle/ModelRssObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelTestcaseObject.py` & `arelle-release-2.6.0/arelle/ModelTestcaseObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelValue.py` & `arelle-release-2.6.0/arelle/ModelValue.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelVersObject.py` & `arelle-release-2.6.0/arelle/ModelVersObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelVersReport.py` & `arelle-release-2.6.0/arelle/ModelVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ModelXbrl.py` & `arelle-release-2.6.0/arelle/ModelXbrl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/PackageManager.py` & `arelle-release-2.6.0/arelle/PackageManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/PluginManager.py` & `arelle-release-2.6.0/arelle/PluginManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/PrototypeDtsObject.py` & `arelle-release-2.6.0/arelle/PrototypeDtsObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/PrototypeInstanceObject.py` & `arelle-release-2.6.0/arelle/PrototypeInstanceObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/PythonUtil.py` & `arelle-release-2.6.0/arelle/PythonUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/RenderingEvaluator.py` & `arelle-release-2.6.0/arelle/RenderingEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/RenderingResolver.py` & `arelle-release-2.6.0/arelle/RenderingResolver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/SystemInfo.py` & `arelle-release-2.6.0/arelle/SystemInfo.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/TableStructure.py` & `arelle-release-2.6.0/arelle/TableStructure.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/TkTableWrapper.py` & `arelle-release-2.6.0/arelle/TkTableWrapper.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/UITkTable.py` & `arelle-release-2.6.0/arelle/UITkTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/UiUtil.py` & `arelle-release-2.6.0/arelle/UiUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/Updater.py` & `arelle-release-2.6.0/arelle/Updater.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/UrlUtil.py` & `arelle-release-2.6.0/arelle/UrlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/Validate.py` & `arelle-release-2.6.0/arelle/Validate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateFilingText.py` & `arelle-release-2.6.0/arelle/ValidateFilingText.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateInfoset.py` & `arelle-release-2.6.0/arelle/ValidateInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateUtr.py` & `arelle-release-2.6.0/arelle/ValidateUtr.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateVersReport.py` & `arelle-release-2.6.0/arelle/ValidateVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateXbrl.py` & `arelle-release-2.6.0/arelle/ValidateXbrl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateXbrlCalcs.py` & `arelle-release-2.6.0/arelle/ValidateXbrlCalcs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateXbrlDTS.py` & `arelle-release-2.6.0/arelle/ValidateXbrlDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ValidateXbrlDimensions.py` & `arelle-release-2.6.0/arelle/ValidateXbrlDimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/Version.py` & `arelle-release-2.6.0/arelle/Version.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFile.py` & `arelle-release-2.6.0/arelle/ViewFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileConcepts.py` & `arelle-release-2.6.0/arelle/ViewFileConcepts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileDTS.py` & `arelle-release-2.6.0/arelle/ViewFileDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileFactList.py` & `arelle-release-2.6.0/arelle/ViewFileFactList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileFactTable.py` & `arelle-release-2.6.0/arelle/ViewFileFactTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileFormulae.py` & `arelle-release-2.6.0/arelle/ViewFileFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileRelationshipSet.py` & `arelle-release-2.6.0/arelle/ViewFileRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileRenderedGrid.py` & `arelle-release-2.6.0/arelle/ViewFileRenderedGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileRoleTypes.py` & `arelle-release-2.6.0/arelle/ViewFileRoleTypes.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileRssFeed.py` & `arelle-release-2.6.0/arelle/ViewFileRssFeed.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewFileTests.py` & `arelle-release-2.6.0/arelle/ViewFileTests.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewUtil.py` & `arelle-release-2.6.0/arelle/ViewUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewUtilFormulae.py` & `arelle-release-2.6.0/arelle/ViewUtilFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinConcepts.py` & `arelle-release-2.6.0/arelle/ViewWinConcepts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinDTS.py` & `arelle-release-2.6.0/arelle/ViewWinDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinDiffs.py` & `arelle-release-2.6.0/arelle/ViewWinDiffs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinFactGrid.py` & `arelle-release-2.6.0/arelle/ViewWinFactGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinFactList.py` & `arelle-release-2.6.0/arelle/ViewWinFactList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinFactTable.py` & `arelle-release-2.6.0/arelle/ViewWinFactTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinFormulae.py` & `arelle-release-2.6.0/arelle/ViewWinFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinGrid.py` & `arelle-release-2.6.0/arelle/ViewWinGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinList.py` & `arelle-release-2.6.0/arelle/ViewWinList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinPane.py` & `arelle-release-2.6.0/arelle/ViewWinPane.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinProperties.py` & `arelle-release-2.6.0/arelle/ViewWinProperties.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinRelationshipSet.py` & `arelle-release-2.6.0/arelle/ViewWinRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinRenderedGrid.py` & `arelle-release-2.6.0/arelle/ViewWinRenderedGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinRoleTypes.py` & `arelle-release-2.6.0/arelle/ViewWinRoleTypes.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinRssFeed.py` & `arelle-release-2.6.0/arelle/ViewWinRssFeed.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinTests.py` & `arelle-release-2.6.0/arelle/ViewWinTests.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinTkTable.py` & `arelle-release-2.6.0/arelle/ViewWinTkTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinTree.py` & `arelle-release-2.6.0/arelle/ViewWinTree.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinTupleGrid.py` & `arelle-release-2.6.0/arelle/ViewWinTupleGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinVersReport.py` & `arelle-release-2.6.0/arelle/ViewWinVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/ViewWinXml.py` & `arelle-release-2.6.0/arelle/ViewWinXml.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/WatchRss.py` & `arelle-release-2.6.0/arelle/WatchRss.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/WebCache.py` & `arelle-release-2.6.0/arelle/WebCache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/XbrlConst.py` & `arelle-release-2.6.0/arelle/XbrlConst.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/XbrlUtil.py` & `arelle-release-2.6.0/arelle/XbrlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/XhtmlValidate.py` & `arelle-release-2.6.0/arelle/XhtmlValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/XmlUtil.py` & `arelle-release-2.6.0/arelle/XmlUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1170,15 +1170,16 @@
                 break   # stop depth first iteration after comment and root node
             if child.tag == 'nsmap':
                 for nsmapChild in child:
                     writexml(writer, nsmapChild, indent=indent, xmlcharrefreplace=xmlcharrefreplace, parentNsmap={}) # force all xmlns in next element
             else:
                 writexml(writer, child, indent=indent, xmlcharrefreplace=xmlcharrefreplace, parentNsmap={})
     elif isinstance(node,etree._Comment): # ok to use minidom implementation
-        writer.write(indent+"<!--" + node.text if isinstance(node.text, str) else '' + "-->\n")
+        commentText = node.text if isinstance(node.text, str) else ''
+        writer.write(indent + "<!--" + commentText + "-->\n")
     elif isinstance(node,etree._ProcessingInstruction): # ok to use minidom implementation
         writer.write(indent + str(node) + "\n")
     elif isinstance(node,etree._Element):
         if parentNsmap is None:
             parent = node.getparent()
             if parent is not None:
                 parentNsmap = parent.nsmap
```

### Comparing `arelle-release-2.5.8/arelle/XmlValidate.py` & `arelle-release-2.6.0/arelle/XmlValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/XmlValidateParticles.py` & `arelle-release-2.6.0/arelle/XmlValidateParticles.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/XmlValidateSchema.py` & `arelle-release-2.6.0/arelle/XmlValidateSchema.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/arelle_test.ini` & `arelle-release-2.6.0/arelle/config/arelle_test.ini`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/creationSoftwareNames.json` & `arelle-release-2.6.0/arelle/config/creationSoftwareNames.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/disclosuresystems.xml` & `arelle-release-2.6.0/arelle/config/disclosuresystems.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/disclosuresystems.xsd` & `arelle-release-2.6.0/arelle/config/disclosuresystems.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/edbody.dtd` & `arelle-release-2.6.0/arelle/config/edbody.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/erxl.xsd` & `arelle-release-2.6.0/arelle/config/erxl.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/mappings.xml` & `arelle-release-2.6.0/arelle/config/mappings.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/mappings.xsd` & `arelle-release-2.6.0/arelle/config/mappings.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/xbrlschemafiles.xml` & `arelle-release-2.6.0/arelle/config/xbrlschemafiles.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/xhtml-lat1.ent` & `arelle-release-2.6.0/arelle/config/xhtml-lat1.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/xhtml-special.ent` & `arelle-release-2.6.0/arelle/config/xhtml-special.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/xhtml-symbol.ent` & `arelle-release-2.6.0/arelle/config/xhtml-symbol.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/xhtml1-strict-ix.dtd` & `arelle-release-2.6.0/arelle/config/xhtml1-strict-ix.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/config/xhtml1_1-strict-ix.dtd` & `arelle-release-2.6.0/arelle/config/xhtml1_1-strict-ix.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/doc/messagesCatalog.xml` & `arelle-release-2.6.0/arelle/doc/messagesCatalog.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/doc/messagesCatalog.xsd` & `arelle-release-2.6.0/arelle/doc/messagesCatalog.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/CustomLogger.py` & `arelle-release-2.6.0/arelle/examples/CustomLogger.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/LoadEFMvalidate.py` & `arelle-release-2.6.0/arelle/examples/LoadEFMvalidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/LoadSavePreLbCsv.py` & `arelle-release-2.6.0/arelle/examples/LoadSavePreLbCsv.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/LoadValidate.cs` & `arelle-release-2.6.0/arelle/examples/LoadValidate.cs`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/LoadValidate.py` & `arelle-release-2.6.0/arelle/examples/LoadValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/LoadValidateCmdLine.java` & `arelle-release-2.6.0/arelle/examples/LoadValidateCmdLine.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/LoadValidatePostedZip.java` & `arelle-release-2.6.0/arelle/examples/LoadValidatePostedZip.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/LoadValidateWebService.java` & `arelle-release-2.6.0/arelle/examples/LoadValidateWebService.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/SaveTableToExelle.py` & `arelle-release-2.6.0/arelle/examples/SaveTableToExelle.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/TR3toTR4.py` & `arelle-release-2.6.0/arelle/examples/TR3toTR4.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/bigInstance.py` & `arelle-release-2.6.0/arelle/examples/plugin/bigInstance.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/cmdWebServerExtension.py` & `arelle-release-2.6.0/arelle/examples/plugin/cmdWebServerExtension.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/crashTest.py` & `arelle-release-2.6.0/arelle/examples/plugin/crashTest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/formulaSuiteConverter.py` & `arelle-release-2.6.0/arelle/examples/plugin/formulaSuiteConverter.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/functionsCustom.py` & `arelle-release-2.6.0/arelle/examples/plugin/functionsCustom.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/hello_dolly.py` & `arelle-release-2.6.0/arelle/examples/plugin/hello_dolly.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/hello_i18n.pot` & `arelle-release-2.6.0/arelle/examples/plugin/hello_i18n.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/hello_i18n.py` & `arelle-release-2.6.0/arelle/examples/plugin/hello_i18n.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/importTestChild1.py` & `arelle-release-2.6.0/arelle/examples/plugin/importTestChild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/importTestChild2.py` & `arelle-release-2.6.0/arelle/examples/plugin/importTestChild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/importTestGrandchild1.py` & `arelle-release-2.6.0/arelle/examples/plugin/importTestGrandchild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/importTestGrandchild2.py` & `arelle-release-2.6.0/arelle/examples/plugin/importTestGrandchild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/importTestImported1.py` & `arelle-release-2.6.0/arelle/examples/plugin/importTestImported1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/importTestImported11.py` & `arelle-release-2.6.0/arelle/examples/plugin/importTestImported11.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/importTestParent.py` & `arelle-release-2.6.0/arelle/examples/plugin/importTestParent.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po` & `arelle-release-2.6.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/__init__.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestChild1.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestChild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestChild2.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestChild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestImported1.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestImported1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/importTestImported11.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/importTestImported11.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py` & `arelle-release-2.6.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/sakaCalendar.py` & `arelle-release-2.6.0/arelle/examples/plugin/sakaCalendar.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/saveInstanceInfoset.py` & `arelle-release-2.6.0/arelle/examples/plugin/saveInstanceInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/streamingExtensions.py` & `arelle-release-2.6.0/arelle/examples/plugin/streamingExtensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py` & `arelle-release-2.6.0/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/updateTableLB.py` & `arelle-release-2.6.0/arelle/examples/plugin/updateTableLB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/validateSchemaLxml.py` & `arelle-release-2.6.0/arelle/examples/plugin/validateSchemaLxml.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/plugin/validateTableInfoset.py` & `arelle-release-2.6.0/arelle/examples/plugin/validateTableInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/us-gaap-dei-docType-extraction-frm.xml` & `arelle-release-2.6.0/arelle/examples/us-gaap-dei-docType-extraction-frm.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/examples/us-gaap-dei-ratio-cash-frm.xml` & `arelle-release-2.6.0/arelle/examples/us-gaap-dei-ratio-cash-frm.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/formula/FactAspectsCache.py` & `arelle-release-2.6.0/arelle/formula/FactAspectsCache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/formula/FormulaConsisAsser.py` & `arelle-release-2.6.0/arelle/formula/FormulaConsisAsser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/formula/FormulaEvaluator.py` & `arelle-release-2.6.0/arelle/formula/FormulaEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/formula/ValidateFormula.py` & `arelle-release-2.6.0/arelle/formula/ValidateFormula.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/formula/XPathContext.py` & `arelle-release-2.6.0/arelle/formula/XPathContext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/formula/XPathParser.py` & `arelle-release-2.6.0/arelle/formula/XPathParser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle-full-word.ico` & `arelle-release-2.6.0/arelle/images/arelle-full-word.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle-mac-icon-4.gif` & `arelle-release-2.6.0/arelle/images/arelle-mac-icon-4.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle-word-only.ico` & `arelle-release-2.6.0/arelle/images/arelle-word-only.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle.gif` & `arelle-release-2.6.0/arelle/images/arelle.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle.icns` & `arelle-release-2.6.0/arelle/images/arelle.icns`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle.icns.zip` & `arelle-release-2.6.0/arelle/images/arelle.icns.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle.ico` & `arelle-release-2.6.0/arelle/images/arelle.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle128.psd` & `arelle-release-2.6.0/arelle/images/arelle128.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle16.psd` & `arelle-release-2.6.0/arelle/images/arelle16.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle16x16and32x32.ico` & `arelle-release-2.6.0/arelle/images/arelle16x16and32x32.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/arelle32.gif` & `arelle-release-2.6.0/arelle/images/arelle32.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/dmg_background.png` & `arelle-release-2.6.0/arelle/images/dmg_background.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/octocat.png` & `arelle-release-2.6.0/arelle/images/octocat.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/python-clear.png` & `arelle-release-2.6.0/arelle/images/python-clear.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/python-icon-pack-crystalxp.net-842.zip` & `arelle-release-2.6.0/arelle/images/python-icon-pack-crystalxp.net-842.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarClose.gif` & `arelle-release-2.6.0/arelle/images/toolbarClose.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarCompare.gif` & `arelle-release-2.6.0/arelle/images/toolbarCompare.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarFindMenu.gif` & `arelle-release-2.6.0/arelle/images/toolbarFindMenu.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarLogClear - 1-piece-top.gif` & `arelle-release-2.6.0/arelle/images/toolbarLogClear - 1-piece-top.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarLogClear-orig.gif` & `arelle-release-2.6.0/arelle/images/toolbarLogClear-orig.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarLogClear.gif` & `arelle-release-2.6.0/arelle/images/toolbarLogClear.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarNewFile.gif` & `arelle-release-2.6.0/arelle/images/toolbarNewFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarOpenFile.gif` & `arelle-release-2.6.0/arelle/images/toolbarOpenFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarOpenWeb.gif` & `arelle-release-2.6.0/arelle/images/toolbarOpenWeb.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarReopen.gif` & `arelle-release-2.6.0/arelle/images/toolbarReopen.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarSaveFile.gif` & `arelle-release-2.6.0/arelle/images/toolbarSaveFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/toolbarValidate.gif` & `arelle-release-2.6.0/arelle/images/toolbarValidate.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/xbrl.gif` & `arelle-release-2.6.0/arelle/images/xbrl.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/xbrl.psd` & `arelle-release-2.6.0/arelle/images/xbrl.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/xbrl128-2.gif` & `arelle-release-2.6.0/arelle/images/xbrl128-2.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/xbrl128.gif` & `arelle-release-2.6.0/arelle/images/xbrl128.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/xbrl16.ico` & `arelle-release-2.6.0/arelle/images/xbrl16.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/images/xbrl32.ico` & `arelle-release-2.6.0/arelle/images/xbrl32.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po` & `arelle-release-2.6.0/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo` & `arelle-release-2.6.0/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/es/LC_MESSAGES/arelle.mo` & `arelle-release-2.6.0/arelle/locale/es/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/fr/LC_MESSAGES/arelle.mo` & `arelle-release-2.6.0/arelle/locale/fr/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/fr/LC_MESSAGES/fr.po` & `arelle-release-2.6.0/arelle/locale/fr/LC_MESSAGES/fr.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/messages.pot` & `arelle-release-2.6.0/arelle/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/ru/LC_MESSAGES/arelle.mo` & `arelle-release-2.6.0/arelle/locale/ru/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/locale/ru/LC_MESSAGES/ru.po` & `arelle-release-2.6.0/arelle/locale/ru/LC_MESSAGES/ru.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/EdgarRendererAllReports.py` & `arelle-release-2.6.0/arelle/plugin/EdgarRendererAllReports.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/SECCorrespondenceLoader.py` & `arelle-release-2.6.0/arelle/plugin/SECCorrespondenceLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/TDnetLoader.py` & `arelle-release-2.6.0/arelle/plugin/TDnetLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/UKCompaniesHouseLoader.py` & `arelle-release-2.6.0/arelle/plugin/UKCompaniesHouseLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/formulaLoader.py` & `arelle-release-2.6.0/arelle/plugin/formulaLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/formulaSaver.py` & `arelle-release-2.6.0/arelle/plugin/formulaSaver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/formulaXPathChecker.py` & `arelle-release-2.6.0/arelle/plugin/formulaXPathChecker.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/functionsMath.py` & `arelle-release-2.6.0/arelle/plugin/functionsMath.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/functionsXmlCreation.py` & `arelle-release-2.6.0/arelle/plugin/functionsXmlCreation.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/inlineXbrlDocumentSet.py` & `arelle-release-2.6.0/arelle/plugin/inlineXbrlDocumentSet.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,42 @@
 
 If the file source is a zip, CmdLine will discover the inline files in the zip as thus:
     --file '[{"ixds":[{"file":file1.zip}]}]'
 
 If the file source is a local directory, CmdLine will discover the inline files in the directory as thus:
     --file '[{"ixds":[{"file":dir1}]}]'
 
-For GUI operation specify a formula parameter named ixdsTarget of type xs:string (in formula tools->formula parameters).
+If there is a JSON structure in --file without ixdsTarget the default target is assumed.
 
-If a ixdsTarget parameter is absent or has a value of an empty string it is the default target document and matches
-ix facts and resources with no @target attribute.
+If no JSON structure then formula parameter ixdsTarget may be used to specify a non-default target or the
+special value "(default)" for the default target (e.g., resources with no @target attribute).
+
+For GUI instance loading a pop up selection dialog is provided when there is no formula parameter and there are multiple targets.
+
+Example to load multi-document IXDS and save extracted xBRL-XML target document:
+
+  For GUI using ix11 conformance suite directory multi-io test case "PASS-multiple-input-multiple-output"
+     File->Open File Inline Doc Set->multi-select PASS-multiple-input-multiple-output-ID1.html and PASS-multiple-input-multiple-output-ID2.html
+     Select Target -> (default)
+     Tools->Save Target Document
+     new file PASS-multiple-input-multiple-output-ID1_extracted.xbrl has (default) target xBRL-XML instance
+     close instance
+     Reopen as above and Select Target -> TARGET
+     Tools->Save Target Document
+     replaced file PASS-multiple-input-multiple-output-ID1_extracted.xbrl now has TARGET target xBRL-XML instance
+  For Command Line:
+     arelleCmdLine --plugin inlineXbrlDocumentSet
+                   --file '[{"ixds":[{"file":".../PASS-multiple-input-multiple-output-ID1.html"},
+                                     {"file":".../PASS-multiple-input-multiple-output-ID2.html"}],
+                             "ixdsTarget":"(default)"}]'
+                   --saveInstance
+     For second target specify "ixdsTarget":"TARGET"
+     For default target either omit ixdsTarget or specify (default).
+     File will be saved as PASS-multiple-input-multiple-output-ID1_extracted.xbrl regardless of ixdsTarget parameter
+     For EDGAR style encoding of non-ASCII characters add --encodeSavedXmlChars
 
 See COPYRIGHT.md for copyright information.
 '''
 from arelle import FileSource, ModelXbrl, ValidateXbrlDimensions, XbrlConst
 DialogURL = None # dynamically imported when first used
 from arelle.PrototypeDtsObject import LocPrototype, ArcPrototype
 from arelle.FileSource import archiveFilenameParts, archiveFilenameSuffixes
@@ -39,14 +63,15 @@
 from arelle.ModelValue import qname
 from arelle.PluginManager import pluginClassMethods
 from arelle.PythonUtil import attrdict
 from arelle.UrlUtil import isHttpUrl
 from arelle.ValidateFilingText import CDATApattern
 from arelle.Version import authorLabel, copyrightLabel
 from arelle.XmlUtil import addChild, copyIxFootnoteHtml, elementFragmentIdentifier, elementChildSequence, xmlnsprefix, setXmlns
+from arelle.XmlValidate import validate as xmlValidate
 import os, zipfile
 import regex as re
 from optparse import SUPPRESS_HELP
 from lxml.etree import XML, XMLSyntaxError
 from collections import defaultdict
 
 IXDS_SURROGATE = "_IXDS#?#" # surrogate (fake) file name for inline XBRL doc set (IXDS)
@@ -82,22 +107,22 @@
         return True
 
 # this loader is used for test cases of multi-ix doc sets
 def inlineXbrlDocumentSetLoader(modelXbrl, normalizedUri, filepath, isEntry=False, namespace=None, **kwargs):
     if isEntry:
         try:
             if "entrypoint" in kwargs:
-                _target = kwargs["entrypoint"]["ixdsTarget"]
+                _target = kwargs["entrypoint"].get("ixdsTarget") # assume None if not specified in entrypoint
             elif "ixdsTarget" in kwargs: # passed from validate (multio test cases)
                 _target = kwargs["ixdsTarget"]
             else:
-                _target = modelXbrl.modelManager.formulaOptions.parameterValues.get("ixdsTarget")[1]
+                _target = modelXbrl.modelManager.formulaOptions.parameterValues["ixdsTarget"][1]
+            modelXbrl.ixdsTarget = None if _target == "(default)" else _target or None
         except (KeyError, AttributeError, IndexError, TypeError):
-            _target = None
-        modelXbrl.ixdsTarget = _target or None # None if an empty string specified
+            pass # set later in selectTargetDocument plugin method
     if IXDS_SURROGATE in normalizedUri:
         # create surrogate entry object for inline document set which references ix documents
         xml = ["<instances>\n"]
         modelXbrl.ixdsDocUrls = []
         schemeFixup = isHttpUrl(normalizedUri) # schemes after separator have // normalized to single /
         msUNCfixup = modelXbrl.modelManager.cntlr.isMSW and normalizedUri.startswith("\\\\") # path starts with double backslash \\
         if schemeFixup:
@@ -612,14 +637,67 @@
         _entrypointFiles = entrypointFiles.copy()
         del entrypointFiles[:]
         entrypointFiles.append( {"ixds": _entrypointFiles} )
 
 def inlineDocsetUrlSeparator():
     return IXDS_DOC_SEPARATOR
 
+def discoverIxdsDts(modelXbrl):
+    return hasattr(modelXbrl, "ixdsTarget") # if no target specified, block ixds discovery until all IX docs are loaded
+
+class TargetChoiceDialog:
+    def __init__(self,parent, choices):
+        from tkinter import Toplevel, Label, Listbox, StringVar
+        parentGeometry = re.match("(\d+)x(\d+)[+]?([-]?\d+)[+]?([-]?\d+)", parent.geometry())
+        dialogX = int(parentGeometry.group(3))
+        dialogY = int(parentGeometry.group(4))
+        self.parent = parent
+        self.t = Toplevel()
+        self.t.transient(self.parent)
+        self.t.geometry("+{0}+{1}".format(dialogX+200,dialogY+200))
+        self.t.title(_("Select Target"))
+        self.selection = choices[0] # default choice in case dialog is closed without selecting an entry
+        self.lb = Listbox(self.t, height=10, width=30, listvariable=StringVar(value=choices))
+        self.lb.grid(row=0, column=0)
+        self.lb.focus_set()
+        self.lb.bind("<<ListboxSelect>>", self.select)
+        self.t.grab_set()
+        self.t.wait_window(self.t)
+
+    def select(self,event):
+        self.parent.focus_set()
+        self.selection = self.lb.selection_get()
+        self.t.destroy()
+
+def selectTargetDocument(modelXbrl):
+    if not hasattr(modelXbrl, "ixdsTarget"): # DTS discoverey deferred until all ix docs loaded
+        # find target attributes
+        _targets = sorted(set(elt.get("target", "(default)")
+                              for htmlElt in modelXbrl.ixdsHtmlElements
+                              for elt in htmlElt.iterfind(f".//{{{htmlElt.modelDocument.ixNS}}}references")))
+        if len(_targets) == 1:
+            _target = _targets[0]
+        elif modelXbrl.modelManager.cntlr.hasGui:
+            dlg = TargetChoiceDialog(modelXbrl.modelManager.cntlr.parent, _targets)
+            _target = dlg.selection
+        else:
+            _target = _targets[0]
+            modelXbrl.warning("arelle:unspecifiedTargetDocument",
+                              _("Target document not specified, loading %(target)s, found targets %(targets)s"),
+                              modelObject=modelXbrl, target=_target, targets=_targets)
+        modelXbrl.ixdsTarget = None if _target == "(default)" else _target or None
+        # load referenced schemas and linkbases (before validating inline HTML
+        for htmlElt in modelXbrl.ixdsHtmlElements:
+            modelDoc = htmlElt.modelDocument
+            for ixRefElt in htmlElt.iterdescendants(tag=modelDoc.ixNStag + "references"):
+                if ixRefElt.get("target") == modelXbrl.ixdsTarget:
+                    modelDoc.schemaLinkbaseRefsDiscover(ixRefElt)
+                    xmlValidate(modelXbrl, ixRefElt) # validate instance elements
+
+
 __pluginInfo__ = {
     'name': 'Inline XBRL Document Set',
     'version': '1.1',
     'description': "This plug-in adds a feature to read manifest files of inline XBRL document sets "
                     " and to save the embedded XBRL instance document.  "
                     "Support single target instance documents in a single document set.  ",
     'license': 'Apache-2',
@@ -633,12 +711,14 @@
     'CntlrWinMain.Menu.Tools': saveTargetDocumentMenuEntender,
     'CntlrCmdLine.Options': commandLineOptionExtender,
     'CntlrCmdLine.Filing.Start': commandLineFilingStart,
     'CntlrCmdLine.Xbrl.Run': commandLineXbrlRun,
     'ModelDocument.PullLoader': inlineXbrlDocumentSetLoader,
     'ModelDocument.IdentifyType': identifyInlineXbrlDocumentSet,
     'ModelDocument.Discover': discoverInlineXbrlDocumentSet,
+    'ModelDocument.DiscoverIxdsDts': discoverIxdsDts,
+    'ModelDocument.SelectIxdsTarget': selectTargetDocument,
     'ModelTestcaseVariation.ReadMeFirstUris': testcaseVariationReadMeFirstUris,
     'ModelTestcaseVariation.ArchiveIxds': testcaseVariationArchiveIxds,
     'ModelTestcaseVariation.ReportPackageIxds': testcaseVariationReportPackageIxds,
     'ModelTestcaseVariation.ResultXbrlInstanceUri': testcaseVariationResultInstanceUri,
 }
```

### Comparing `arelle-release-2.5.8/arelle/plugin/instanceInfo.py` & `arelle-release-2.6.0/arelle/plugin/instanceInfo.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/U32.py` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/U32.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/__init__.py` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/des.py` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/des.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/des_c.py` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/des_c.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/des_data.py` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/des_data.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/internet/proxyNTLM/ntlm.py` & `arelle-release-2.6.0/arelle/plugin/internet/proxyNTLM/ntlm.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/loadFromExcel.py` & `arelle-release-2.6.0/arelle/plugin/loadFromExcel.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/loadFromOIM-2018.py` & `arelle-release-2.6.0/arelle/plugin/loadFromOIM-2018.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/loadFromOIM.py` & `arelle-release-2.6.0/arelle/plugin/loadFromOIM.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/logging/dpmSignature.py` & `arelle-release-2.6.0/arelle/plugin/logging/dpmSignature.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/logging/dqcParameters.py` & `arelle-release-2.6.0/arelle/plugin/logging/dqcParameters.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/logging/saveMessages.py` & `arelle-release-2.6.0/arelle/plugin/logging/saveMessages.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/objectmaker.py` & `arelle-release-2.6.0/arelle/plugin/objectmaker.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/profileCmdLine.py` & `arelle-release-2.6.0/arelle/plugin/profileCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/profileFormula.py` & `arelle-release-2.6.0/arelle/plugin/profileFormula.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/saveCHComponentFile.py` & `arelle-release-2.6.0/arelle/plugin/saveCHComponentFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/saveDTS.py` & `arelle-release-2.6.0/arelle/plugin/saveDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/saveHtmlEBAtables.py` & `arelle-release-2.6.0/arelle/plugin/saveHtmlEBAtables.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/saveLoadableExcel.py` & `arelle-release-2.6.0/arelle/plugin/saveLoadableExcel.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/saveLoadableOIM.py` & `arelle-release-2.6.0/arelle/plugin/saveLoadableOIM.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/saveSKOS.py` & `arelle-release-2.6.0/arelle/plugin/saveSKOS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/saveSampleInstance.py` & `arelle-release-2.6.0/arelle/plugin/saveSampleInstance.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/security/cryptAES_CBC.py` & `arelle-release-2.6.0/arelle/plugin/security/cryptAES_CBC.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/security/cryptAES_EAX.py` & `arelle-release-2.6.0/arelle/plugin/security/cryptAES_EAX.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/FormulaGenerator.py` & `arelle-release-2.6.0/arelle/plugin/sphinx/FormulaGenerator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/SphinxContext.py` & `arelle-release-2.6.0/arelle/plugin/sphinx/SphinxContext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/SphinxEvaluator.py` & `arelle-release-2.6.0/arelle/plugin/sphinx/SphinxEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/SphinxMethods.py` & `arelle-release-2.6.0/arelle/plugin/sphinx/SphinxMethods.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/SphinxParser.py` & `arelle-release-2.6.0/arelle/plugin/sphinx/SphinxParser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/SphinxValidator.py` & `arelle-release-2.6.0/arelle/plugin/sphinx/SphinxValidator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr` & `arelle-release-2.6.0/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/sphinx/__init__.py` & `arelle-release-2.6.0/arelle/plugin/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/streamingExtensions.py` & `arelle-release-2.6.0/arelle/plugin/streamingExtensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/__init__.py` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/README.md` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/saxon9.jar` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/saxon9.jar`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/testcase.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/testcase.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/conf/tests.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/conf/tests.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/text2num.py` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/text2num.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd` & `arelle-release-2.6.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/transforms/tester.py` & `arelle-release-2.6.0/arelle/plugin/transforms/tester.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/unpackSecEisFile.py` & `arelle-release-2.6.0/arelle/plugin/unpackSecEisFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/CIPC/Const.py` & `arelle-release-2.6.0/arelle/plugin/validate/CIPC/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/CIPC/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/CIPC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/CIPC/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/CIPC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EBA/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/EBA/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EBA/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EBA/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/Consts.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/Consts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/DTS.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/Dimensions.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/Document.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/Document.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/Filing.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/Filing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/PreCalAlignment.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/PreCalAlignment.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/Util.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/Util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/README.md` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/axiswarnings.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/axiswarnings.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/dei-validations.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/dei-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/dqc-us-rules.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/dqc-us-rules.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/signwarnings.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/signwarnings.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json` & `arelle-release-2.6.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/Const.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd` & `arelle-release-2.6.0/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF/Const.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF/DTS.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF/Dimensions.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF/Util.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF/Util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF/resources/authority-validations.json` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF/resources/authority-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/Const.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/DTS.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/Dimensions.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/Util.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/Util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json` & `arelle-release-2.6.0/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/FERC/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/FERC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/FERC/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/FERC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/FERC/resources/ferc-utr.xml` & `arelle-release-2.6.0/arelle/plugin/validate/FERC/resources/ferc-utr.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/GFM/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/GFM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/GFM/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/GFM/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/HMRC/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/HMRC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/HMRC/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/HMRC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/HMRC/consistencyChecksByName.json` & `arelle-release-2.6.0/arelle/plugin/validate/HMRC/consistencyChecksByName.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml` & `arelle-release-2.6.0/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ROS/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/ROS/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/ROS/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/ROS/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/CustomLoader.py` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/CustomLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/DTS.py` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/Dimensions.py` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/Document.py` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/Document.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/Filing.py` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/Filing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml` & `arelle-release-2.6.0/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/USBestPractices.py` & `arelle-release-2.6.0/arelle/plugin/validate/USBestPractices.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/USCorpAction.py` & `arelle-release-2.6.0/arelle/plugin/validate/USCorpAction.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/USSecTagging.py` & `arelle-release-2.6.0/arelle/plugin/validate/USSecTagging.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/XDC/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/XDC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/XDC/config.xml` & `arelle-release-2.6.0/arelle/plugin/validate/XDC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/XFsyntax/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/XFsyntax/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/XFsyntax/xf.py` & `arelle-release-2.6.0/arelle/plugin/validate/XFsyntax/xf.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/__init__.py` & `arelle-release-2.6.0/arelle/plugin/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validate/calc2.py` & `arelle-release-2.6.0/arelle/plugin/validate/calc2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/validateSBRnl.py` & `arelle-release-2.6.0/arelle/plugin/validateSBRnl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/DialogRssWatchExtender.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/DialogRssWatchExtender.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/SqlDb.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/SqlDb.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/__init__.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/entityInformation.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/entityInformation.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/ext/china.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/ext/china.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/ext/edgar.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/ext/edgar.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/ext/xdc.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/ext/xdc.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/primaryDocumentFacts.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/primaryDocumentFacts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xbrlDB/tableFacts.py` & `arelle-release-2.6.0/arelle/plugin/xbrlDB/tableFacts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/plugin/xuleSaver.py` & `arelle-release-2.6.0/arelle/plugin/xuleSaver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/scripts-windows/exportCsvFromXbrlInstance.bat` & `arelle-release-2.6.0/arelle/scripts-windows/exportCsvFromXbrlInstance.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/scripts-windows/runFormulaTests.bat` & `arelle-release-2.6.0/arelle/scripts-windows/runFormulaTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/scripts-windows/validateAndRunFormulas.bat` & `arelle-release-2.6.0/arelle/scripts-windows/validateAndRunFormulas.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/typing.py` & `arelle-release-2.6.0/arelle/typing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/webserver/bottle-no2to3.py` & `arelle-release-2.6.0/arelle/webserver/bottle-no2to3.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle/webserver/bottle.py` & `arelle-release-2.6.0/arelle/webserver/bottle.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelleCmdLine.py` & `arelle-release-2.6.0/arelleCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle_release.egg-info/PKG-INFO` & `arelle-release-2.6.0/arelle_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arelle-release
-Version: 2.5.8
+Version: 2.6.0
 Summary: An open source XBRL platform.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `arelle-release-2.5.8/arelle_release.egg-info/SOURCES.txt` & `arelle-release-2.6.0/arelle_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/arelle_test.py` & `arelle-release-2.6.0/arelle_test.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/attic/CntlrGenVersReports.py` & `arelle-release-2.6.0/attic/CntlrGenVersReports.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/buildVersion.py` & `arelle-release-2.6.0/buildVersion.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/conftest.py` & `arelle-release-2.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/distro.py` & `arelle-release-2.6.0/distro.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/docker/ubuntu.Dockerfile` & `arelle-release-2.6.0/docker/ubuntu.Dockerfile`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/encodeUtf8PySource.py` & `arelle-release-2.6.0/encodeUtf8PySource.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/generateMessagesCatalog.py` & `arelle-release-2.6.0/generateMessagesCatalog.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/installWin64.nsi` & `arelle-release-2.6.0/installWin64.nsi`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/installWin86.nsi` & `arelle-release-2.6.0/installWin86.nsi`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/linux/Tktable2.11/README.txt` & `arelle-release-2.6.0/libs/linux/Tktable2.11/README.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/linux/Tktable2.11/html/tkTable.html` & `arelle-release-2.6.0/libs/linux/Tktable2.11/html/tkTable.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/linux/Tktable2.11/libTktable2.11.so` & `arelle-release-2.6.0/libs/linux/Tktable2.11/libTktable2.11.so`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/linux/Tktable2.11/license.txt` & `arelle-release-2.6.0/libs/linux/Tktable2.11/license.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/linux/Tktable2.11/tkTable.tcl` & `arelle-release-2.6.0/libs/linux/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/linux/Tktable2.11/tktable.py` & `arelle-release-2.6.0/libs/linux/Tktable2.11/tktable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/macos/Tktable2.11/README.txt` & `arelle-release-2.6.0/libs/macos/Tktable2.11/README.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/macos/Tktable2.11/html/tkTable.html` & `arelle-release-2.6.0/libs/macos/Tktable2.11/html/tkTable.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/macos/Tktable2.11/libTktable2.11.dylib` & `arelle-release-2.6.0/libs/macos/Tktable2.11/libTktable2.11.dylib`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/macos/Tktable2.11/license.txt` & `arelle-release-2.6.0/libs/macos/Tktable2.11/license.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/macos/Tktable2.11/tkTable.tcl` & `arelle-release-2.6.0/libs/macos/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/macos/Tktable2.11/tktable.py` & `arelle-release-2.6.0/libs/macos/Tktable2.11/tktable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/win64/Tktable2.11/Tktable.dll` & `arelle-release-2.6.0/libs/win64/Tktable2.11/Tktable.dll`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/libs/win64/Tktable2.11/tkTable.tcl` & `arelle-release-2.6.0/libs/win64/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/messages.pot` & `arelle-release-2.6.0/messages.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/msgfmt.py` & `arelle-release-2.6.0/msgfmt.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/plugins/xbrl-us/us-gaap-consistency.py` & `arelle-release-2.6.0/plugins/xbrl-us/us-gaap-consistency.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/pygettext.py` & `arelle-release-2.6.0/pygettext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/pyproject.toml` & `arelle-release-2.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/requirements.txt` & `arelle-release-2.6.0/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 pycountry==22.3.5
 # plugins
 # EdgarRenderer plugin
 NumPy==1.21.6 ; python_version < "3.8"
 NumPy==1.23.4 ; python_version >= "3.8"
 Matplotlib==3.5.3 ; python_version < "3.8"
 Matplotlib==3.6.1 ; python_version >= "3.8"
-holidays==0.21.13
+holidays==0.22
 Tornado==6.2
 # security plugin
 PyCryptodome==3.17
 # xbrlDB plugin
 cx_Oracle==8.3.0
 pg8000==1.29.4
 PyMySQL==1.0.3
```

### Comparing `arelle-release-2.5.8/scripts/buildLinuxDist.sh` & `arelle-release-2.6.0/scripts/buildLinuxDist.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/buildMacDist.sh` & `arelle-release-2.6.0/scripts/buildMacDist.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/buildWinDist.bat` & `arelle-release-2.6.0/scripts/buildWinDist.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/charlieTest.bat` & `arelle-release-2.6.0/scripts/charlieTest.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/exportCsvFormulae.bat` & `arelle-release-2.6.0/scripts/exportCsvFormulae.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/exportCsvFromXbrlInstance.bat` & `arelle-release-2.6.0/scripts/exportCsvFromXbrlInstance.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/generateTestcase.py` & `arelle-release-2.6.0/scripts/generateTestcase.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/reportAllTests.bat` & `arelle-release-2.6.0/scripts/reportAllTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runESMAtests.sh` & `arelle-release-2.6.0/scripts/runESMAtests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runGenerateVersioningTestcases.bat` & `arelle-release-2.6.0/scripts/runGenerateVersioningTestcases.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runPackageTests.sh` & `arelle-release-2.6.0/scripts/runPackageTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runPyTest.sh` & `arelle-release-2.6.0/scripts/runPyTest.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runTR2Tests.sh` & `arelle-release-2.6.0/scripts/runTR2Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runTR3Tests.sh` & `arelle-release-2.6.0/scripts/runTR3Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runTR4Tests.sh` & `arelle-release-2.6.0/scripts/runTR4Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runTR5Tests.sh` & `arelle-release-2.6.0/scripts/runTR5Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runTRSECTests.sh` & `arelle-release-2.6.0/scripts/runTRSECTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/scripts/runVersioningConsumptionTests.bat` & `arelle-release-2.6.0/scripts/runVersioningConsumptionTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/setup.cfg` & `arelle-release-2.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj` & `arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs` & `arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln` & `arelle-release-2.6.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/ui_tests/resources/workiva.zip` & `arelle-release-2.6.0/tests/integration_tests/ui_tests/resources/workiva.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/README.md` & `arelle-release-2.6.0/tests/integration_tests/validation/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_config.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_config.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configs.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/conftest.py` & `arelle-release-2.6.0/tests/integration_tests/validation/conftest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/download_conformance_suites.py` & `arelle-release-2.6.0/tests/integration_tests/validation/download_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/run_conformance_suites.py` & `arelle-release-2.6.0/tests/integration_tests/validation/run_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/test_conformance_suites.py` & `arelle-release-2.6.0/tests/integration_tests/validation/test_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/integration_tests/validation/validation_util.py` & `arelle-release-2.6.0/tests/integration_tests/validation/validation_util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/plugin/test_loadfromoim.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/plugin/test_loadfromoim.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_import.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_import.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_locale.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_locale.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_packagemanager.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_packagemanager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_pluginmanager.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_pluginmanager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_qname.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_qname.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_system_info.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_system_info.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_updater.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_updater.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_urlutil.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_urlutil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/tests/unit_tests/arelle/test_version.py` & `arelle-release-2.6.0/tests/unit_tests/arelle/test_version.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/vms/mac/README.md` & `arelle-release-2.6.0/vms/mac/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.5.8/vms/mac/create-macos-bootable-for-virtualbox.sh` & `arelle-release-2.6.0/vms/mac/create-macos-bootable-for-virtualbox.sh`

 * *Files identical despite different names*

