# Comparing `tmp/credmark-1.1.0.tar.gz` & `tmp/credmark-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credmark-1.1.0.tar", max compression
+gzip compressed data, was "credmark-1.2.0.tar", max compression
```

## Comparing `credmark-1.1.0.tar` & `credmark-1.2.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0     2942 2023-04-11 03:50:08.006270 credmark-1.1.0/README.md
--rw-r--r--   0        0        0      110 2023-04-11 03:48:43.361532 credmark-1.1.0/credmark/__init__.py
--rw-r--r--   0        0        0       47 2023-04-11 03:48:40.841425 credmark-1.1.0/credmark/api/__init__.py
--rw-r--r--   0        0        0     9809 2023-04-11 03:48:43.507216 credmark-1.1.0/credmark/api/defi_api/__init__.py
--rw-r--r--   0        0        0     7308 2023-04-11 03:48:43.565142 credmark-1.1.0/credmark/api/defi_api/get_cached_model_results.py
--rw-r--r--   0        0        0     4018 2023-04-11 03:48:43.474293 credmark-1.1.0/credmark/api/defi_api/get_model_by_slug.py
--rw-r--r--   0        0        0     4355 2023-04-11 03:48:43.488715 credmark-1.1.0/credmark/api/defi_api/get_model_deployments_by_slug.py
--rw-r--r--   0        0        0     3852 2023-04-11 03:48:43.477515 credmark-1.1.0/credmark/api/defi_api/get_model_runtime_stats.py
--rw-r--r--   0        0        0     4064 2023-04-11 03:48:43.493711 credmark-1.1.0/credmark/api/defi_api/list_models.py
--rw-r--r--   0        0        0     4251 2023-04-11 03:48:43.495256 credmark-1.1.0/credmark/api/defi_api/run_model.py
--rw-r--r--   0        0        0    61221 2023-04-11 03:48:44.554649 credmark-1.1.0/credmark/api/token_api/__init__.py
--rw-r--r--   0        0        0     6476 2023-04-11 03:48:43.593660 credmark-1.1.0/credmark/api/token_api/get_token_abi.py
--rw-r--r--   0        0        0     8314 2023-04-11 03:48:43.766732 credmark-1.1.0/credmark/api/token_api/get_token_balance.py
--rw-r--r--   0        0        0    11501 2023-04-11 03:48:43.853075 credmark-1.1.0/credmark/api/token_api/get_token_balance_historical.py
--rw-r--r--   0        0        0     6734 2023-04-11 03:48:43.769696 credmark-1.1.0/credmark/api/token_api/get_token_creation_block.py
--rw-r--r--   0        0        0     6586 2023-04-11 03:48:43.790323 credmark-1.1.0/credmark/api/token_api/get_token_decimals.py
--rw-r--r--   0        0        0     8882 2023-04-11 03:48:43.872630 credmark-1.1.0/credmark/api/token_api/get_token_holders.py
--rw-r--r--   0        0        0     6840 2023-04-11 03:48:43.817300 credmark-1.1.0/credmark/api/token_api/get_token_holders_count.py
--rw-r--r--   0        0        0    10051 2023-04-11 03:48:43.877457 credmark-1.1.0/credmark/api/token_api/get_token_holders_count_historical.py
--rw-r--r--   0        0        0    11573 2023-04-11 03:48:43.950121 credmark-1.1.0/credmark/api/token_api/get_token_holders_historical.py
--rw-r--r--   0        0        0     6498 2023-04-11 03:48:43.836262 credmark-1.1.0/credmark/api/token_api/get_token_logo.py
--rw-r--r--   0        0        0     6567 2023-04-11 03:48:43.893052 credmark-1.1.0/credmark/api/token_api/get_token_metadata.py
--rw-r--r--   0        0        0     6498 2023-04-11 03:48:43.920809 credmark-1.1.0/credmark/api/token_api/get_token_name.py
--rw-r--r--   0        0        0     9033 2023-04-11 03:48:44.037652 credmark-1.1.0/credmark/api/token_api/get_token_price.py
--rw-r--r--   0        0        0    11607 2023-04-11 03:48:44.086836 credmark-1.1.0/credmark/api/token_api/get_token_price_historical.py
--rw-r--r--   0        0        0     6542 2023-04-11 03:48:43.987606 credmark-1.1.0/credmark/api/token_api/get_token_symbol.py
--rw-r--r--   0        0        0     7258 2023-04-11 03:48:44.025479 credmark-1.1.0/credmark/api/token_api/get_token_total_supply.py
--rw-r--r--   0        0        0    10441 2023-04-11 03:48:44.163673 credmark-1.1.0/credmark/api/token_api/get_token_total_supply_historical.py
--rw-r--r--   0        0        0     8912 2023-04-11 03:48:44.119242 credmark-1.1.0/credmark/api/token_api/get_token_volume.py
--rw-r--r--   0        0        0    10517 2023-04-11 03:48:44.196668 credmark-1.1.0/credmark/api/token_api/get_token_volume_historical.py
--rw-r--r--   0        0        0     5998 2023-04-11 03:48:43.992821 credmark-1.1.0/credmark/api/utilities/__init__.py
--rw-r--r--   0        0        0     4182 2023-04-11 03:48:43.999926 credmark-1.1.0/credmark/api/utilities/check_health.py
--rw-r--r--   0        0        0     5921 2023-04-11 03:48:44.149704 credmark-1.1.0/credmark/api/utilities/get_daily_model_usage.py
--rw-r--r--   0        0        0     3712 2023-04-11 03:48:44.079720 credmark-1.1.0/credmark/api/utilities/get_top_models.py
--rw-r--r--   0        0        0     3690 2023-04-11 03:48:44.145224 credmark-1.1.0/credmark/api/utilities/get_total_model_usage.py
--rw-r--r--   0        0        0     2763 2023-04-11 03:48:44.115214 credmark-1.1.0/credmark/client.py
--rw-r--r--   0        0        0      320 2023-04-11 03:48:40.826829 credmark-1.1.0/credmark/docs/CheckHealthResponse200.md
--rw-r--r--   0        0        0       79 2023-04-11 03:48:40.825602 credmark-1.1.0/credmark/docs/CheckHealthResponse200Details.md
--rw-r--r--   0        0        0      172 2023-04-11 03:48:40.824931 credmark-1.1.0/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
--rw-r--r--   0        0        0       33 2023-04-11 03:48:40.824198 credmark-1.1.0/credmark/docs/CheckHealthResponse200Error.md
--rw-r--r--   0        0        0      170 2023-04-11 03:48:40.823491 credmark-1.1.0/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-04-11 03:48:40.822692 credmark-1.1.0/credmark/docs/CheckHealthResponse200Info.md
--rw-r--r--   0        0        0      169 2023-04-11 03:48:40.821914 credmark-1.1.0/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
--rw-r--r--   0        0        0      320 2023-04-11 03:48:40.832574 credmark-1.1.0/credmark/docs/CheckHealthResponse503.md
--rw-r--r--   0        0        0      140 2023-04-11 03:48:40.831417 credmark-1.1.0/credmark/docs/CheckHealthResponse503Details.md
--rw-r--r--   0        0        0      172 2023-04-11 03:48:40.830764 credmark-1.1.0/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
--rw-r--r--   0        0        0      108 2023-04-11 03:48:40.830089 credmark-1.1.0/credmark/docs/CheckHealthResponse503Error.md
--rw-r--r--   0        0        0      170 2023-04-11 03:48:40.829438 credmark-1.1.0/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-04-11 03:48:40.828400 credmark-1.1.0/credmark/docs/CheckHealthResponse503Info.md
--rw-r--r--   0        0        0      169 2023-04-11 03:48:40.827622 credmark-1.1.0/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
--rw-r--r--   0        0        0     2390 2023-04-11 03:48:40.902832 credmark-1.1.0/credmark/docs/DefiApi.md
--rw-r--r--   0        0        0      390 2023-04-11 03:48:40.773881 credmark-1.1.0/credmark/docs/ModelCallStackEntry.md
--rw-r--r--   0        0        0      259 2023-04-11 03:48:40.716024 credmark-1.1.0/credmark/docs/ModelDeployment.md
--rw-r--r--   0        0        0      519 2023-04-11 03:48:40.715002 credmark-1.1.0/credmark/docs/ModelMetadata.md
--rw-r--r--   0        0        0      753 2023-04-11 03:48:40.778862 credmark-1.1.0/credmark/docs/ModelRunResponse.md
--rw-r--r--   0        0        0      637 2023-04-11 03:48:40.776812 credmark-1.1.0/credmark/docs/ModelRunResponseError.md
--rw-r--r--   0        0        0      418 2023-04-11 03:48:40.718689 credmark-1.1.0/credmark/docs/ModelRuntimeStatistics.md
--rw-r--r--   0        0        0      165 2023-04-11 03:48:40.747025 credmark-1.1.0/credmark/docs/ModelRuntimeStatsResponse.md
--rw-r--r--   0        0        0      485 2023-04-11 03:48:40.772657 credmark-1.1.0/credmark/docs/RunModelDto.md
--rw-r--r--   0        0        0      597 2023-04-11 03:48:40.795189 credmark-1.1.0/credmark/docs/TokenAbiResponse.md
--rw-r--r--   0        0        0    11323 2023-04-11 03:48:40.947456 credmark-1.1.0/credmark/docs/TokenApi.md
--rw-r--r--   0        0        0      318 2023-04-11 03:48:40.803073 credmark-1.1.0/credmark/docs/TokenBalanceHistoricalItem.md
--rw-r--r--   0        0        0      646 2023-04-11 03:48:40.805048 credmark-1.1.0/credmark/docs/TokenBalanceHistoricalResponse.md
--rw-r--r--   0        0        0      530 2023-04-11 03:48:40.801986 credmark-1.1.0/credmark/docs/TokenBalanceResponse.md
--rw-r--r--   0        0        0      371 2023-04-11 03:48:40.792994 credmark-1.1.0/credmark/docs/TokenCreationBlockResponse.md
--rw-r--r--   0        0        0      347 2023-04-11 03:48:40.786060 credmark-1.1.0/credmark/docs/TokenDecimalsResponse.md
--rw-r--r--   0        0        0      491 2023-04-11 03:48:40.781892 credmark-1.1.0/credmark/docs/TokenErrorResponse.md
--rw-r--r--   0        0        0      518 2023-04-11 03:48:40.820845 credmark-1.1.0/credmark/docs/TokenHistoricalHoldersCountResponse.md
--rw-r--r--   0        0        0      214 2023-04-11 03:48:40.811281 credmark-1.1.0/credmark/docs/TokenHolder.md
--rw-r--r--   0        0        0      283 2023-04-11 03:48:40.819193 credmark-1.1.0/credmark/docs/TokenHoldersCountHistoricalItem.md
--rw-r--r--   0        0        0      357 2023-04-11 03:48:40.818232 credmark-1.1.0/credmark/docs/TokenHoldersCountResponse.md
--rw-r--r--   0        0        0      336 2023-04-11 03:48:40.814990 credmark-1.1.0/credmark/docs/TokenHoldersHistoricalItem.md
--rw-r--r--   0        0        0      646 2023-04-11 03:48:40.816948 credmark-1.1.0/credmark/docs/TokenHoldersHistoricalResponse.md
--rw-r--r--   0        0        0      613 2023-04-11 03:48:40.813345 credmark-1.1.0/credmark/docs/TokenHoldersResponse.md
--rw-r--r--   0        0        0      341 2023-04-11 03:48:40.791546 credmark-1.1.0/credmark/docs/TokenLogoResponse.md
--rw-r--r--   0        0        0      399 2023-04-11 03:48:40.780314 credmark-1.1.0/credmark/docs/TokenMetadataResponse.md
--rw-r--r--   0        0        0      333 2023-04-11 03:48:40.783219 credmark-1.1.0/credmark/docs/TokenNameResponse.md
--rw-r--r--   0        0        0      379 2023-04-11 03:48:40.798118 credmark-1.1.0/credmark/docs/TokenPriceHistoricalItem.md
--rw-r--r--   0        0        0      582 2023-04-11 03:48:40.800381 credmark-1.1.0/credmark/docs/TokenPriceHistoricalResponse.md
--rw-r--r--   0        0        0      531 2023-04-11 03:48:40.796897 credmark-1.1.0/credmark/docs/TokenPriceResponse.md
--rw-r--r--   0        0        0      339 2023-04-11 03:48:40.784850 credmark-1.1.0/credmark/docs/TokenSymbolResponse.md
--rw-r--r--   0        0        0      284 2023-04-11 03:48:40.788368 credmark-1.1.0/credmark/docs/TokenTotalSupplyHistoricalItem.md
--rw-r--r--   0        0        0      581 2023-04-11 03:48:40.790178 credmark-1.1.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md
--rw-r--r--   0        0        0      423 2023-04-11 03:48:40.787418 credmark-1.1.0/credmark/docs/TokenTotalSupplyResponse.md
--rw-r--r--   0        0        0      404 2023-04-11 03:48:40.808357 credmark-1.1.0/credmark/docs/TokenVolumeHistoricalItem.md
--rw-r--r--   0        0        0      565 2023-04-11 03:48:40.810302 credmark-1.1.0/credmark/docs/TokenVolumeHistoricalResponse.md
--rw-r--r--   0        0        0      537 2023-04-11 03:48:40.807133 credmark-1.1.0/credmark/docs/TokenVolumeResponse.md
--rw-r--r--   0        0        0     1244 2023-04-11 03:48:40.894326 credmark-1.1.0/credmark/docs/Utilities.md
--rw-r--r--   0        0        0      470 2023-04-11 03:48:44.014187 credmark-1.1.0/credmark/errors.py
--rw-r--r--   0        0        0     5618 2023-04-11 03:48:40.837882 credmark-1.1.0/credmark/models/__init__.py
--rw-r--r--   0        0        0     4203 2023-04-11 03:48:44.226307 credmark-1.1.0/credmark/models/check_health_response_200.py
--rw-r--r--   0        0        0     2144 2023-04-11 03:48:44.168797 credmark-1.1.0/credmark/models/check_health_response_200_details.py
--rw-r--r--   0        0        0     1658 2023-04-11 03:48:44.188389 credmark-1.1.0/credmark/models/check_health_response_200_details_additional_property.py
--rw-r--r--   0        0        0     2061 2023-04-11 03:48:44.192642 credmark-1.1.0/credmark/models/check_health_response_200_error.py
--rw-r--r--   0        0        0     1648 2023-04-11 03:48:44.157247 credmark-1.1.0/credmark/models/check_health_response_200_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-04-11 03:48:44.188178 credmark-1.1.0/credmark/models/check_health_response_200_info.py
--rw-r--r--   0        0        0     1643 2023-04-11 03:48:44.210996 credmark-1.1.0/credmark/models/check_health_response_200_info_additional_property.py
--rw-r--r--   0        0        0     4364 2023-04-11 03:48:44.282037 credmark-1.1.0/credmark/models/check_health_response_503.py
--rw-r--r--   0        0        0     2205 2023-04-11 03:48:44.212103 credmark-1.1.0/credmark/models/check_health_response_503_details.py
--rw-r--r--   0        0        0     1658 2023-04-11 03:48:44.218992 credmark-1.1.0/credmark/models/check_health_response_503_details_additional_property.py
--rw-r--r--   0        0        0     2149 2023-04-11 03:48:44.225452 credmark-1.1.0/credmark/models/check_health_response_503_error.py
--rw-r--r--   0        0        0     1648 2023-04-11 03:48:44.230259 credmark-1.1.0/credmark/models/check_health_response_503_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-04-11 03:48:44.244207 credmark-1.1.0/credmark/models/check_health_response_503_info.py
--rw-r--r--   0        0        0     1643 2023-04-11 03:48:44.243058 credmark-1.1.0/credmark/models/check_health_response_503_info_additional_property.py
--rw-r--r--   0        0        0      165 2023-04-11 03:48:42.483324 credmark-1.1.0/credmark/models/get_cached_model_results_order.py
--rw-r--r--   0        0        0      166 2023-04-11 03:48:42.435579 credmark-1.1.0/credmark/models/get_token_price_align.py
--rw-r--r--   0        0        0      163 2023-04-11 03:48:42.323444 credmark-1.1.0/credmark/models/get_token_price_historical_src.py
--rw-r--r--   0        0        0      153 2023-04-11 03:48:42.490561 credmark-1.1.0/credmark/models/get_token_price_src.py
--rw-r--r--   0        0        0     2470 2023-04-11 03:48:44.273396 credmark-1.1.0/credmark/models/model_call_stack_entry.py
--rw-r--r--   0        0        0     1894 2023-04-11 03:48:44.265761 credmark-1.1.0/credmark/models/model_deployment.py
--rw-r--r--   0        0        0     3325 2023-04-11 03:48:44.318835 credmark-1.1.0/credmark/models/model_metadata.py
--rw-r--r--   0        0        0     4190 2023-04-11 03:48:44.335806 credmark-1.1.0/credmark/models/model_run_response.py
--rw-r--r--   0        0        0     3362 2023-04-11 03:48:44.312579 credmark-1.1.0/credmark/models/model_run_response_error.py
--rw-r--r--   0        0        0     2412 2023-04-11 03:48:44.299140 credmark-1.1.0/credmark/models/model_runtime_statistics.py
--rw-r--r--   0        0        0     2042 2023-04-11 03:48:44.287431 credmark-1.1.0/credmark/models/model_runtime_stats_response.py
--rw-r--r--   0        0        0     3294 2023-04-11 03:48:44.326929 credmark-1.1.0/credmark/models/run_model_dto.py
--rw-r--r--   0        0        0      204 2023-04-11 03:48:42.381661 credmark-1.1.0/credmark/models/run_model_dto_block_number_type_1.py
--rw-r--r--   0        0        0     5771 2023-04-11 03:48:44.340408 credmark-1.1.0/credmark/models/token_abi_response.py
--rw-r--r--   0        0        0     2319 2023-04-11 03:48:44.311771 credmark-1.1.0/credmark/models/token_balance_historical_item.py
--rw-r--r--   0        0        0     4365 2023-04-11 03:48:44.373211 credmark-1.1.0/credmark/models/token_balance_historical_response.py
--rw-r--r--   0        0        0     3378 2023-04-11 03:48:44.364911 credmark-1.1.0/credmark/models/token_balance_response.py
--rw-r--r--   0        0        0     2692 2023-04-11 03:48:44.358929 credmark-1.1.0/credmark/models/token_creation_block_response.py
--rw-r--r--   0        0        0     2587 2023-04-11 03:48:44.363033 credmark-1.1.0/credmark/models/token_decimals_response.py
--rw-r--r--   0        0        0     2779 2023-04-11 03:48:44.382210 credmark-1.1.0/credmark/models/token_error_response.py
--rw-r--r--   0        0        0     3856 2023-04-11 03:48:44.408475 credmark-1.1.0/credmark/models/token_historical_holders_count_response.py
--rw-r--r--   0        0        0     1836 2023-04-11 03:48:44.376935 credmark-1.1.0/credmark/models/token_holder.py
--rw-r--r--   0        0        0     2104 2023-04-11 03:48:44.382363 credmark-1.1.0/credmark/models/token_holders_count_historical_item.py
--rw-r--r--   0        0        0     2589 2023-04-11 03:48:44.394564 credmark-1.1.0/credmark/models/token_holders_count_response.py
--rw-r--r--   0        0        0     2693 2023-04-11 03:48:44.413882 credmark-1.1.0/credmark/models/token_holders_historical_item.py
--rw-r--r--   0        0        0     4365 2023-04-11 03:48:44.449993 credmark-1.1.0/credmark/models/token_holders_historical_response.py
--rw-r--r--   0        0        0     4074 2023-04-11 03:48:44.473184 credmark-1.1.0/credmark/models/token_holders_response.py
--rw-r--r--   0        0        0     2711 2023-04-11 03:48:44.448358 credmark-1.1.0/credmark/models/token_logo_response.py
--rw-r--r--   0        0        0     2951 2023-04-11 03:48:44.447777 credmark-1.1.0/credmark/models/token_metadata_response.py
--rw-r--r--   0        0        0     2527 2023-04-11 03:48:44.439384 credmark-1.1.0/credmark/models/token_name_response.py
--rw-r--r--   0        0        0     2551 2023-04-11 03:48:44.464882 credmark-1.1.0/credmark/models/token_price_historical_item.py
--rw-r--r--   0        0        0     4118 2023-04-11 03:48:44.486483 credmark-1.1.0/credmark/models/token_price_historical_response.py
--rw-r--r--   0        0        0     3387 2023-04-11 03:48:44.472840 credmark-1.1.0/credmark/models/token_price_response.py
--rw-r--r--   0        0        0     2553 2023-04-11 03:48:44.477369 credmark-1.1.0/credmark/models/token_symbol_response.py
--rw-r--r--   0        0        0     2168 2023-04-11 03:48:44.479696 credmark-1.1.0/credmark/models/token_total_supply_historical_item.py
--rw-r--r--   0        0        0     4072 2023-04-11 03:48:44.509065 credmark-1.1.0/credmark/models/token_total_supply_historical_response.py
--rw-r--r--   0        0        0     2881 2023-04-11 03:48:44.507441 credmark-1.1.0/credmark/models/token_total_supply_response.py
--rw-r--r--   0        0        0     2758 2023-04-11 03:48:44.509501 credmark-1.1.0/credmark/models/token_volume_historical_item.py
--rw-r--r--   0        0        0     4001 2023-04-11 03:48:44.527795 credmark-1.1.0/credmark/models/token_volume_historical_response.py
--rw-r--r--   0        0        0     3465 2023-04-11 03:48:44.522644 credmark-1.1.0/credmark/models/token_volume_response.py
--rw-r--r--   0        0        0       25 2023-04-11 03:48:40.680579 credmark-1.1.0/credmark/py.typed
--rw-r--r--   0        0        0      974 2023-04-11 03:48:44.491916 credmark-1.1.0/credmark/types.py
--rw-r--r--   0        0        0      853 2023-04-11 03:49:15.755611 credmark-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 credmark-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4502 2023-04-14 09:02:54.717263 credmark-1.2.0/README.md
+-rw-r--r--   0        0        0      110 2023-04-14 08:56:27.665903 credmark-1.2.0/credmark/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-14 08:56:24.698799 credmark-1.2.0/credmark/api/__init__.py
+-rw-r--r--   0        0        0     9019 2023-04-14 08:56:27.884998 credmark-1.2.0/credmark/api/defi_api/__init__.py
+-rw-r--r--   0        0        0     6959 2023-04-14 08:56:27.970634 credmark-1.2.0/credmark/api/defi_api/get_cached_model_results.py
+-rw-r--r--   0        0        0     3679 2023-04-14 08:56:27.807883 credmark-1.2.0/credmark/api/defi_api/get_model_by_slug.py
+-rw-r--r--   0        0        0     4016 2023-04-14 08:56:27.836973 credmark-1.2.0/credmark/api/defi_api/get_model_deployments_by_slug.py
+-rw-r--r--   0        0        0     3513 2023-04-14 08:56:27.868895 credmark-1.2.0/credmark/api/defi_api/get_model_runtime_stats.py
+-rw-r--r--   0        0        0     3725 2023-04-14 08:56:27.889006 credmark-1.2.0/credmark/api/defi_api/list_models.py
+-rw-r--r--   0        0        0     3912 2023-04-14 08:56:27.900632 credmark-1.2.0/credmark/api/defi_api/run_model.py
+-rw-r--r--   0        0        0    56689 2023-04-14 08:56:29.045156 credmark-1.2.0/credmark/api/token_api/__init__.py
+-rw-r--r--   0        0        0     5906 2023-04-14 08:56:27.981855 credmark-1.2.0/credmark/api/token_api/get_token_abi.py
+-rw-r--r--   0        0        0     7744 2023-04-14 08:56:28.020839 credmark-1.2.0/credmark/api/token_api/get_token_balance.py
+-rw-r--r--   0        0        0    10931 2023-04-14 08:56:28.121722 credmark-1.2.0/credmark/api/token_api/get_token_balance_historical.py
+-rw-r--r--   0        0        0     6164 2023-04-14 08:56:27.997295 credmark-1.2.0/credmark/api/token_api/get_token_creation_block.py
+-rw-r--r--   0        0        0     6016 2023-04-14 08:56:28.034610 credmark-1.2.0/credmark/api/token_api/get_token_decimals.py
+-rw-r--r--   0        0        0     8312 2023-04-14 08:56:28.108309 credmark-1.2.0/credmark/api/token_api/get_token_holders.py
+-rw-r--r--   0        0        0     6270 2023-04-14 08:56:28.073692 credmark-1.2.0/credmark/api/token_api/get_token_holders_count.py
+-rw-r--r--   0        0        0     9481 2023-04-14 08:56:28.174134 credmark-1.2.0/credmark/api/token_api/get_token_holders_count_historical.py
+-rw-r--r--   0        0        0    11003 2023-04-14 08:56:28.204227 credmark-1.2.0/credmark/api/token_api/get_token_holders_historical.py
+-rw-r--r--   0        0        0     5928 2023-04-14 08:56:28.104616 credmark-1.2.0/credmark/api/token_api/get_token_logo.py
+-rw-r--r--   0        0        0     5997 2023-04-14 08:56:28.154689 credmark-1.2.0/credmark/api/token_api/get_token_metadata.py
+-rw-r--r--   0        0        0     5928 2023-04-14 08:56:28.181157 credmark-1.2.0/credmark/api/token_api/get_token_name.py
+-rw-r--r--   0        0        0     8463 2023-04-14 08:56:28.284400 credmark-1.2.0/credmark/api/token_api/get_token_price.py
+-rw-r--r--   0        0        0    11037 2023-04-14 08:56:28.396076 credmark-1.2.0/credmark/api/token_api/get_token_price_historical.py
+-rw-r--r--   0        0        0     5972 2023-04-14 08:56:28.212532 credmark-1.2.0/credmark/api/token_api/get_token_symbol.py
+-rw-r--r--   0        0        0     6688 2023-04-14 08:56:28.288316 credmark-1.2.0/credmark/api/token_api/get_token_total_supply.py
+-rw-r--r--   0        0        0     9871 2023-04-14 08:56:28.502047 credmark-1.2.0/credmark/api/token_api/get_token_total_supply_historical.py
+-rw-r--r--   0        0        0     8342 2023-04-14 08:56:28.445443 credmark-1.2.0/credmark/api/token_api/get_token_volume.py
+-rw-r--r--   0        0        0     9947 2023-04-14 08:56:28.528577 credmark-1.2.0/credmark/api/token_api/get_token_volume_historical.py
+-rw-r--r--   0        0        0     5344 2023-04-14 08:56:28.274887 credmark-1.2.0/credmark/api/utilities/__init__.py
+-rw-r--r--   0        0        0     3575 2023-04-14 08:56:28.336469 credmark-1.2.0/credmark/api/utilities/check_health.py
+-rw-r--r--   0        0        0     5572 2023-04-14 08:56:28.469894 credmark-1.2.0/credmark/api/utilities/get_daily_model_usage.py
+-rw-r--r--   0        0        0     3373 2023-04-14 08:56:28.393005 credmark-1.2.0/credmark/api/utilities/get_top_models.py
+-rw-r--r--   0        0        0     3351 2023-04-14 08:56:28.363551 credmark-1.2.0/credmark/api/utilities/get_total_model_usage.py
+-rw-r--r--   0        0        0     2645 2023-04-14 08:56:28.445048 credmark-1.2.0/credmark/client.py
+-rw-r--r--   0        0        0      320 2023-04-14 08:56:24.676118 credmark-1.2.0/credmark/docs/CheckHealthResponse200.md
+-rw-r--r--   0        0        0       79 2023-04-14 08:56:24.674820 credmark-1.2.0/credmark/docs/CheckHealthResponse200Details.md
+-rw-r--r--   0        0        0      172 2023-04-14 08:56:24.674111 credmark-1.2.0/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0       33 2023-04-14 08:56:24.673351 credmark-1.2.0/credmark/docs/CheckHealthResponse200Error.md
+-rw-r--r--   0        0        0      170 2023-04-14 08:56:24.672714 credmark-1.2.0/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-04-14 08:56:24.671916 credmark-1.2.0/credmark/docs/CheckHealthResponse200Info.md
+-rw-r--r--   0        0        0      169 2023-04-14 08:56:24.671265 credmark-1.2.0/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
+-rw-r--r--   0        0        0      320 2023-04-14 08:56:24.685073 credmark-1.2.0/credmark/docs/CheckHealthResponse503.md
+-rw-r--r--   0        0        0      140 2023-04-14 08:56:24.683093 credmark-1.2.0/credmark/docs/CheckHealthResponse503Details.md
+-rw-r--r--   0        0        0      172 2023-04-14 08:56:24.681879 credmark-1.2.0/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0      108 2023-04-14 08:56:24.680640 credmark-1.2.0/credmark/docs/CheckHealthResponse503Error.md
+-rw-r--r--   0        0        0      170 2023-04-14 08:56:24.679588 credmark-1.2.0/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-04-14 08:56:24.678427 credmark-1.2.0/credmark/docs/CheckHealthResponse503Info.md
+-rw-r--r--   0        0        0      169 2023-04-14 08:56:24.677184 credmark-1.2.0/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
+-rw-r--r--   0        0        0     2390 2023-04-14 08:56:24.852030 credmark-1.2.0/credmark/docs/DefiApi.md
+-rw-r--r--   0        0        0      390 2023-04-14 08:56:24.630981 credmark-1.2.0/credmark/docs/ModelCallStackEntry.md
+-rw-r--r--   0        0        0      259 2023-04-14 08:56:24.583458 credmark-1.2.0/credmark/docs/ModelDeployment.md
+-rw-r--r--   0        0        0      519 2023-04-14 08:56:24.582365 credmark-1.2.0/credmark/docs/ModelMetadata.md
+-rw-r--r--   0        0        0      753 2023-04-14 08:56:24.634974 credmark-1.2.0/credmark/docs/ModelRunResponse.md
+-rw-r--r--   0        0        0      637 2023-04-14 08:56:24.633299 credmark-1.2.0/credmark/docs/ModelRunResponseError.md
+-rw-r--r--   0        0        0      418 2023-04-14 08:56:24.585965 credmark-1.2.0/credmark/docs/ModelRuntimeStatistics.md
+-rw-r--r--   0        0        0      165 2023-04-14 08:56:24.609660 credmark-1.2.0/credmark/docs/ModelRuntimeStatsResponse.md
+-rw-r--r--   0        0        0      485 2023-04-14 08:56:24.629868 credmark-1.2.0/credmark/docs/RunModelDto.md
+-rw-r--r--   0        0        0      597 2023-04-14 08:56:24.648253 credmark-1.2.0/credmark/docs/TokenAbiResponse.md
+-rw-r--r--   0        0        0    10810 2023-04-14 08:56:24.948548 credmark-1.2.0/credmark/docs/TokenApi.md
+-rw-r--r--   0        0        0      318 2023-04-14 08:56:24.655738 credmark-1.2.0/credmark/docs/TokenBalanceHistoricalItem.md
+-rw-r--r--   0        0        0      646 2023-04-14 08:56:24.657361 credmark-1.2.0/credmark/docs/TokenBalanceHistoricalResponse.md
+-rw-r--r--   0        0        0      530 2023-04-14 08:56:24.654720 credmark-1.2.0/credmark/docs/TokenBalanceResponse.md
+-rw-r--r--   0        0        0      371 2023-04-14 08:56:24.646446 credmark-1.2.0/credmark/docs/TokenCreationBlockResponse.md
+-rw-r--r--   0        0        0      347 2023-04-14 08:56:24.640804 credmark-1.2.0/credmark/docs/TokenDecimalsResponse.md
+-rw-r--r--   0        0        0      491 2023-04-14 08:56:24.637582 credmark-1.2.0/credmark/docs/TokenErrorResponse.md
+-rw-r--r--   0        0        0      518 2023-04-14 08:56:24.670518 credmark-1.2.0/credmark/docs/TokenHistoricalHoldersCountResponse.md
+-rw-r--r--   0        0        0      214 2023-04-14 08:56:24.662523 credmark-1.2.0/credmark/docs/TokenHolder.md
+-rw-r--r--   0        0        0      283 2023-04-14 08:56:24.668823 credmark-1.2.0/credmark/docs/TokenHoldersCountHistoricalItem.md
+-rw-r--r--   0        0        0      357 2023-04-14 08:56:24.667985 credmark-1.2.0/credmark/docs/TokenHoldersCountResponse.md
+-rw-r--r--   0        0        0      336 2023-04-14 08:56:24.665253 credmark-1.2.0/credmark/docs/TokenHoldersHistoricalItem.md
+-rw-r--r--   0        0        0      646 2023-04-14 08:56:24.666945 credmark-1.2.0/credmark/docs/TokenHoldersHistoricalResponse.md
+-rw-r--r--   0        0        0      613 2023-04-14 08:56:24.664174 credmark-1.2.0/credmark/docs/TokenHoldersResponse.md
+-rw-r--r--   0        0        0      341 2023-04-14 08:56:24.645373 credmark-1.2.0/credmark/docs/TokenLogoResponse.md
+-rw-r--r--   0        0        0      399 2023-04-14 08:56:24.636255 credmark-1.2.0/credmark/docs/TokenMetadataResponse.md
+-rw-r--r--   0        0        0      333 2023-04-14 08:56:24.638623 credmark-1.2.0/credmark/docs/TokenNameResponse.md
+-rw-r--r--   0        0        0      379 2023-04-14 08:56:24.651782 credmark-1.2.0/credmark/docs/TokenPriceHistoricalItem.md
+-rw-r--r--   0        0        0      582 2023-04-14 08:56:24.653344 credmark-1.2.0/credmark/docs/TokenPriceHistoricalResponse.md
+-rw-r--r--   0        0        0      531 2023-04-14 08:56:24.650158 credmark-1.2.0/credmark/docs/TokenPriceResponse.md
+-rw-r--r--   0        0        0      339 2023-04-14 08:56:24.639730 credmark-1.2.0/credmark/docs/TokenSymbolResponse.md
+-rw-r--r--   0        0        0      284 2023-04-14 08:56:24.642757 credmark-1.2.0/credmark/docs/TokenTotalSupplyHistoricalItem.md
+-rw-r--r--   0        0        0      581 2023-04-14 08:56:24.644260 credmark-1.2.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md
+-rw-r--r--   0        0        0      423 2023-04-14 08:56:24.641941 credmark-1.2.0/credmark/docs/TokenTotalSupplyResponse.md
+-rw-r--r--   0        0        0      404 2023-04-14 08:56:24.659805 credmark-1.2.0/credmark/docs/TokenVolumeHistoricalItem.md
+-rw-r--r--   0        0        0      565 2023-04-14 08:56:24.661611 credmark-1.2.0/credmark/docs/TokenVolumeHistoricalResponse.md
+-rw-r--r--   0        0        0      537 2023-04-14 08:56:24.658717 credmark-1.2.0/credmark/docs/TokenVolumeResponse.md
+-rw-r--r--   0        0        0     1213 2023-04-14 08:56:24.828376 credmark-1.2.0/credmark/docs/Utilities.md
+-rw-r--r--   0        0        0      592 2023-04-14 08:56:28.312151 credmark-1.2.0/credmark/errors.py
+-rw-r--r--   0        0        0     5618 2023-04-14 08:56:24.693188 credmark-1.2.0/credmark/models/__init__.py
+-rw-r--r--   0        0        0     4203 2023-04-14 08:56:28.620678 credmark-1.2.0/credmark/models/check_health_response_200.py
+-rw-r--r--   0        0        0     2144 2023-04-14 08:56:28.501048 credmark-1.2.0/credmark/models/check_health_response_200_details.py
+-rw-r--r--   0        0        0     1658 2023-04-14 08:56:28.446169 credmark-1.2.0/credmark/models/check_health_response_200_details_additional_property.py
+-rw-r--r--   0        0        0     2061 2023-04-14 08:56:28.531334 credmark-1.2.0/credmark/models/check_health_response_200_error.py
+-rw-r--r--   0        0        0     1648 2023-04-14 08:56:28.509615 credmark-1.2.0/credmark/models/check_health_response_200_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-04-14 08:56:28.570637 credmark-1.2.0/credmark/models/check_health_response_200_info.py
+-rw-r--r--   0        0        0     1643 2023-04-14 08:56:28.550145 credmark-1.2.0/credmark/models/check_health_response_200_info_additional_property.py
+-rw-r--r--   0        0        0     4364 2023-04-14 08:56:28.700870 credmark-1.2.0/credmark/models/check_health_response_503.py
+-rw-r--r--   0        0        0     2205 2023-04-14 08:56:28.559117 credmark-1.2.0/credmark/models/check_health_response_503_details.py
+-rw-r--r--   0        0        0     1658 2023-04-14 08:56:28.570637 credmark-1.2.0/credmark/models/check_health_response_503_details_additional_property.py
+-rw-r--r--   0        0        0     2149 2023-04-14 08:56:28.605205 credmark-1.2.0/credmark/models/check_health_response_503_error.py
+-rw-r--r--   0        0        0     1648 2023-04-14 08:56:28.597488 credmark-1.2.0/credmark/models/check_health_response_503_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-04-14 08:56:28.613731 credmark-1.2.0/credmark/models/check_health_response_503_info.py
+-rw-r--r--   0        0        0     1643 2023-04-14 08:56:28.612026 credmark-1.2.0/credmark/models/check_health_response_503_info_additional_property.py
+-rw-r--r--   0        0        0      165 2023-04-14 08:56:26.619117 credmark-1.2.0/credmark/models/get_cached_model_results_order.py
+-rw-r--r--   0        0        0      166 2023-04-14 08:56:26.582381 credmark-1.2.0/credmark/models/get_token_price_align.py
+-rw-r--r--   0        0        0      163 2023-04-14 08:56:26.527688 credmark-1.2.0/credmark/models/get_token_price_historical_src.py
+-rw-r--r--   0        0        0      153 2023-04-14 08:56:26.623362 credmark-1.2.0/credmark/models/get_token_price_src.py
+-rw-r--r--   0        0        0     2470 2023-04-14 08:56:28.691391 credmark-1.2.0/credmark/models/model_call_stack_entry.py
+-rw-r--r--   0        0        0     1894 2023-04-14 08:56:28.644365 credmark-1.2.0/credmark/models/model_deployment.py
+-rw-r--r--   0        0        0     3325 2023-04-14 08:56:28.740310 credmark-1.2.0/credmark/models/model_metadata.py
+-rw-r--r--   0        0        0     4190 2023-04-14 08:56:28.753517 credmark-1.2.0/credmark/models/model_run_response.py
+-rw-r--r--   0        0        0     3362 2023-04-14 08:56:28.726084 credmark-1.2.0/credmark/models/model_run_response_error.py
+-rw-r--r--   0        0        0     2412 2023-04-14 08:56:28.723461 credmark-1.2.0/credmark/models/model_runtime_statistics.py
+-rw-r--r--   0        0        0     2042 2023-04-14 08:56:28.712727 credmark-1.2.0/credmark/models/model_runtime_stats_response.py
+-rw-r--r--   0        0        0     3294 2023-04-14 08:56:28.762660 credmark-1.2.0/credmark/models/run_model_dto.py
+-rw-r--r--   0        0        0      204 2023-04-14 08:56:26.554457 credmark-1.2.0/credmark/models/run_model_dto_block_number_type_1.py
+-rw-r--r--   0        0        0     5771 2023-04-14 08:56:28.762877 credmark-1.2.0/credmark/models/token_abi_response.py
+-rw-r--r--   0        0        0     2319 2023-04-14 08:56:28.726249 credmark-1.2.0/credmark/models/token_balance_historical_item.py
+-rw-r--r--   0        0        0     4365 2023-04-14 08:56:28.798583 credmark-1.2.0/credmark/models/token_balance_historical_response.py
+-rw-r--r--   0        0        0     3378 2023-04-14 08:56:28.796025 credmark-1.2.0/credmark/models/token_balance_response.py
+-rw-r--r--   0        0        0     2692 2023-04-14 08:56:28.782576 credmark-1.2.0/credmark/models/token_creation_block_response.py
+-rw-r--r--   0        0        0     2587 2023-04-14 08:56:28.799948 credmark-1.2.0/credmark/models/token_decimals_response.py
+-rw-r--r--   0        0        0     2779 2023-04-14 08:56:28.818334 credmark-1.2.0/credmark/models/token_error_response.py
+-rw-r--r--   0        0        0     3856 2023-04-14 08:56:28.844892 credmark-1.2.0/credmark/models/token_historical_holders_count_response.py
+-rw-r--r--   0        0        0     1836 2023-04-14 08:56:28.800079 credmark-1.2.0/credmark/models/token_holder.py
+-rw-r--r--   0        0        0     2104 2023-04-14 08:56:28.814430 credmark-1.2.0/credmark/models/token_holders_count_historical_item.py
+-rw-r--r--   0        0        0     2589 2023-04-14 08:56:28.854384 credmark-1.2.0/credmark/models/token_holders_count_response.py
+-rw-r--r--   0        0        0     2693 2023-04-14 08:56:28.866891 credmark-1.2.0/credmark/models/token_holders_historical_item.py
+-rw-r--r--   0        0        0     4365 2023-04-14 08:56:28.937892 credmark-1.2.0/credmark/models/token_holders_historical_response.py
+-rw-r--r--   0        0        0     4074 2023-04-14 08:56:28.971375 credmark-1.2.0/credmark/models/token_holders_response.py
+-rw-r--r--   0        0        0     2711 2023-04-14 08:56:28.938164 credmark-1.2.0/credmark/models/token_logo_response.py
+-rw-r--r--   0        0        0     2951 2023-04-14 08:56:28.948089 credmark-1.2.0/credmark/models/token_metadata_response.py
+-rw-r--r--   0        0        0     2527 2023-04-14 08:56:28.942016 credmark-1.2.0/credmark/models/token_name_response.py
+-rw-r--r--   0        0        0     2551 2023-04-14 08:56:28.937111 credmark-1.2.0/credmark/models/token_price_historical_item.py
+-rw-r--r--   0        0        0     4118 2023-04-14 08:56:28.981032 credmark-1.2.0/credmark/models/token_price_historical_response.py
+-rw-r--r--   0        0        0     3387 2023-04-14 08:56:28.968433 credmark-1.2.0/credmark/models/token_price_response.py
+-rw-r--r--   0        0        0     2553 2023-04-14 08:56:28.976542 credmark-1.2.0/credmark/models/token_symbol_response.py
+-rw-r--r--   0        0        0     2168 2023-04-14 08:56:28.970052 credmark-1.2.0/credmark/models/token_total_supply_historical_item.py
+-rw-r--r--   0        0        0     4072 2023-04-14 08:56:29.013026 credmark-1.2.0/credmark/models/token_total_supply_historical_response.py
+-rw-r--r--   0        0        0     2881 2023-04-14 08:56:29.010022 credmark-1.2.0/credmark/models/token_total_supply_response.py
+-rw-r--r--   0        0        0     2758 2023-04-14 08:56:29.006541 credmark-1.2.0/credmark/models/token_volume_historical_item.py
+-rw-r--r--   0        0        0     4001 2023-04-14 08:56:29.033418 credmark-1.2.0/credmark/models/token_volume_historical_response.py
+-rw-r--r--   0        0        0     3465 2023-04-14 08:56:29.022878 credmark-1.2.0/credmark/models/token_volume_response.py
+-rw-r--r--   0        0        0       25 2023-04-14 08:56:24.547674 credmark-1.2.0/credmark/py.typed
+-rw-r--r--   0        0        0      964 2023-04-14 08:56:28.981297 credmark-1.2.0/credmark/types.py
+-rw-r--r--   0        0        0      853 2023-04-14 09:04:30.076824 credmark-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 credmark-1.2.0/PKG-INFO
```

### Comparing `credmark-1.1.0/credmark/api/defi_api/__init__.py` & `credmark-1.2.0/credmark/api/defi_api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, List, Optional, Union, cast
 
 from ...models.get_cached_model_results_order import GetCachedModelResultsOrder
@@ -24,174 +24,174 @@
 
 class DefiApi:
     def __init__(self, client: "Credmark"):
         self.__client = client
 
     def list_models(
         self,
-    ) -> Optional[List["ModelMetadata"]]:
+    ) -> List["ModelMetadata"]:
         """List metadata for available models
 
          Returns a list of metadata for available models.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List['ModelMetadata']]
         """
 
         return list_models.sync(
             client=self.__client,
         )
 
     async def list_models_async(
         self,
-    ) -> Optional[List["ModelMetadata"]]:
+    ) -> List["ModelMetadata"]:
         """List metadata for available models
 
          Returns a list of metadata for available models.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List['ModelMetadata']]
         """
 
         return await list_models.asyncio(
             client=self.__client,
         )
 
     def get_model_by_slug(
         self,
         slug: str,
-    ) -> Optional[ModelMetadata]:
+    ) -> ModelMetadata:
         """Get model metadata by slug
 
          Returns the metadata for the specified model.
 
         Args:
             slug (str):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelMetadata]
         """
 
         return get_model_by_slug.sync(
             client=self.__client,
             slug=slug,
         )
 
     async def get_model_by_slug_async(
         self,
         slug: str,
-    ) -> Optional[ModelMetadata]:
+    ) -> ModelMetadata:
         """Get model metadata by slug
 
          Returns the metadata for the specified model.
 
         Args:
             slug (str):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelMetadata]
         """
 
         return await get_model_by_slug.asyncio(
             client=self.__client,
             slug=slug,
         )
 
     def get_model_deployments_by_slug(
         self,
         slug: str,
-    ) -> Optional[List["ModelDeployment"]]:
+    ) -> List["ModelDeployment"]:
         """Get model deployments of a model by slug
 
          Returns the deployments for a model.
 
         Args:
             slug (str):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List['ModelDeployment']]
         """
 
         return get_model_deployments_by_slug.sync(
             client=self.__client,
             slug=slug,
         )
 
     async def get_model_deployments_by_slug_async(
         self,
         slug: str,
-    ) -> Optional[List["ModelDeployment"]]:
+    ) -> List["ModelDeployment"]:
         """Get model deployments of a model by slug
 
          Returns the deployments for a model.
 
         Args:
             slug (str):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List['ModelDeployment']]
         """
 
         return await get_model_deployments_by_slug.asyncio(
             client=self.__client,
             slug=slug,
         )
 
     def get_model_runtime_stats(
         self,
-    ) -> Optional[ModelRuntimeStatsResponse]:
+    ) -> ModelRuntimeStatsResponse:
         """Model runtime stats
 
          Returns runtime stats for all models.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRuntimeStatsResponse]
         """
 
         return get_model_runtime_stats.sync(
             client=self.__client,
         )
 
     async def get_model_runtime_stats_async(
         self,
-    ) -> Optional[ModelRuntimeStatsResponse]:
+    ) -> ModelRuntimeStatsResponse:
         """Model runtime stats
 
          Returns runtime stats for all models.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRuntimeStatsResponse]
         """
 
         return await get_model_runtime_stats.asyncio(
@@ -202,29 +202,29 @@
         self,
         *,
         slug: str,
         sort: Union[Unset, None, str] = UNSET,
         order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
         limit: Union[Unset, None, float] = UNSET,
         offset: Union[Unset, None, float] = UNSET,
-    ) -> Optional[ModelRuntimeStatsResponse]:
+    ) -> ModelRuntimeStatsResponse:
         """Cached model results
 
          Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
         and get results, use `POST /v1/model/run`.
 
         Args:
             slug (str):
             sort (Union[Unset, None, str]):
             order (Union[Unset, None, GetCachedModelResultsOrder]):
             limit (Union[Unset, None, float]):
             offset (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRuntimeStatsResponse]
         """
 
         return get_cached_model_results.sync(
@@ -240,29 +240,29 @@
         self,
         *,
         slug: str,
         sort: Union[Unset, None, str] = UNSET,
         order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
         limit: Union[Unset, None, float] = UNSET,
         offset: Union[Unset, None, float] = UNSET,
-    ) -> Optional[ModelRuntimeStatsResponse]:
+    ) -> ModelRuntimeStatsResponse:
         """Cached model results
 
          Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
         and get results, use `POST /v1/model/run`.
 
         Args:
             slug (str):
             sort (Union[Unset, None, str]):
             order (Union[Unset, None, GetCachedModelResultsOrder]):
             limit (Union[Unset, None, float]):
             offset (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRuntimeStatsResponse]
         """
 
         return await get_cached_model_results.asyncio(
@@ -274,24 +274,24 @@
             offset=offset,
         )
 
     def run_model(
         self,
         *,
         json_body: RunModelDto,
-    ) -> Optional[ModelRunResponse]:
+    ) -> ModelRunResponse:
         """Run model
 
          Runs a model and returns result object.
 
         Args:
             json_body (RunModelDto):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRunResponse]
         """
 
         return run_model.sync(
@@ -299,24 +299,24 @@
             json_body=json_body,
         )
 
     async def run_model_async(
         self,
         *,
         json_body: RunModelDto,
-    ) -> Optional[ModelRunResponse]:
+    ) -> ModelRunResponse:
         """Run model
 
          Runs a model and returns result object.
 
         Args:
             json_body (RunModelDto):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[ModelRunResponse]
         """
 
         return await run_model.asyncio(
```

### Comparing `credmark-1.1.0/credmark/api/defi_api/get_cached_model_results.py` & `credmark-1.2.0/credmark/api/defi_api/get_cached_model_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.get_cached_model_results_order import GetCachedModelResultsOrder
 from ...models.model_runtime_stats_response import ModelRuntimeStatsResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -52,23 +52,20 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelRuntimeStatsResponse]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> ModelRuntimeStatsResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = ModelRuntimeStatsResponse.from_dict(response.json())
 
         return response_200
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
 def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelRuntimeStatsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
@@ -94,15 +91,15 @@
         slug (str):
         sort (Union[Unset, None, str]):
         order (Union[Unset, None, GetCachedModelResultsOrder]):
         limit (Union[Unset, None, float]):
         offset (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     kwargs = _get_kwargs(
@@ -126,29 +123,29 @@
     *,
     slug: str,
     sort: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
     limit: Union[Unset, None, float] = UNSET,
     offset: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[ModelRuntimeStatsResponse]:
+) -> ModelRuntimeStatsResponse:
     """Cached model results
 
      Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
     and get results, use `POST /v1/model/run`.
 
     Args:
         slug (str):
         sort (Union[Unset, None, str]):
         order (Union[Unset, None, GetCachedModelResultsOrder]):
         limit (Union[Unset, None, float]):
         offset (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     return sync_detailed(
@@ -179,15 +176,15 @@
         slug (str):
         sort (Union[Unset, None, str]):
         order (Union[Unset, None, GetCachedModelResultsOrder]):
         limit (Union[Unset, None, float]):
         offset (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     kwargs = _get_kwargs(
@@ -209,29 +206,29 @@
     *,
     slug: str,
     sort: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, GetCachedModelResultsOrder] = UNSET,
     limit: Union[Unset, None, float] = UNSET,
     offset: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[ModelRuntimeStatsResponse]:
+) -> ModelRuntimeStatsResponse:
     """Cached model results
 
      Returns cached run results for a slug.<p>This endpoint is for analyzing model runs. To run a model
     and get results, use `POST /v1/model/run`.
 
     Args:
         slug (str):
         sort (Union[Unset, None, str]):
         order (Union[Unset, None, GetCachedModelResultsOrder]):
         limit (Union[Unset, None, float]):
         offset (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     return (
```

### Comparing `credmark-1.1.0/credmark/api/defi_api/get_model_by_slug.py` & `credmark-1.2.0/credmark/api/utilities/check_health.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,129 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict
 
 from ... import errors
-from ...models.model_metadata import ModelMetadata
+from ...models.check_health_response_200 import CheckHealthResponse200
+from ...models.check_health_response_503 import CheckHealthResponse503
 from ...types import Response
 
 
-def _get_kwargs(slug: str, client: "Credmark") -> Dict[str, Any]:
-    url = "{}/v1/models/{slug}".format(client.base_url, slug=slug)
+def _get_kwargs(client: "Credmark") -> Dict[str, Any]:
+    url = "{}/health".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelMetadata]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> CheckHealthResponse200:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ModelMetadata.from_dict(response.json())
+        response_200 = CheckHealthResponse200.from_dict(response.json())
 
         return response_200
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    if response.status_code == HTTPStatus.SERVICE_UNAVAILABLE:
+        response_503 = CheckHealthResponse503.from_dict(response.json())
 
+        raise errors.CredmarkError(response.status_code, response.content, response_503)
+    raise errors.CredmarkError(response.status_code, response.content)
 
-def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelMetadata]:
+
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[CheckHealthResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def sync_detailed(slug: str, client: "Credmark") -> Response[ModelMetadata]:
-    """Get model metadata by slug
-
-     Returns the metadata for the specified model.
-
-    Args:
-        slug (str):
+def sync_detailed(client: "Credmark") -> Response[CheckHealthResponse200]:
+    """Healthcheck status
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ModelMetadata]
+        Response[CheckHealthResponse200]
     """
 
     kwargs = _get_kwargs(
-        slug=slug,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(slug: str, client: "Credmark") -> Optional[ModelMetadata]:
-    """Get model metadata by slug
-
-     Returns the metadata for the specified model.
-
-    Args:
-        slug (str):
+def sync(client: "Credmark") -> CheckHealthResponse200:
+    """Healthcheck status
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ModelMetadata]
+        Response[CheckHealthResponse200]
     """
 
     return sync_detailed(
-        slug=slug,
         client=client,
     ).parsed
 
 
-async def asyncio_detailed(slug: str, client: "Credmark") -> Response[ModelMetadata]:
-    """Get model metadata by slug
-
-     Returns the metadata for the specified model.
-
-    Args:
-        slug (str):
+async def asyncio_detailed(client: "Credmark") -> Response[CheckHealthResponse200]:
+    """Healthcheck status
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ModelMetadata]
+        Response[CheckHealthResponse200]
     """
 
     kwargs = _get_kwargs(
-        slug=slug,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(slug: str, client: "Credmark") -> Optional[ModelMetadata]:
-    """Get model metadata by slug
-
-     Returns the metadata for the specified model.
-
-    Args:
-        slug (str):
+async def asyncio(client: "Credmark") -> CheckHealthResponse200:
+    """Healthcheck status
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ModelMetadata]
+        Response[CheckHealthResponse200]
     """
 
     return (
         await asyncio_detailed(
-            slug=slug,
             client=client,
         )
     ).parsed
```

### Comparing `credmark-1.1.0/credmark/api/defi_api/get_model_deployments_by_slug.py` & `credmark-1.2.0/credmark/api/defi_api/get_model_deployments_by_slug.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, List
@@ -25,28 +25,25 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List["ModelDeployment"]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> List["ModelDeployment"]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
             response_200_item = ModelDeployment.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
 def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List["ModelDeployment"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
@@ -59,15 +56,15 @@
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelDeployment']]
     """
 
     kwargs = _get_kwargs(
@@ -79,24 +76,24 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(slug: str, client: "Credmark") -> Optional[List["ModelDeployment"]]:
+def sync(slug: str, client: "Credmark") -> List["ModelDeployment"]:
     """Get model deployments of a model by slug
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelDeployment']]
     """
 
     return sync_detailed(
@@ -110,15 +107,15 @@
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelDeployment']]
     """
 
     kwargs = _get_kwargs(
@@ -128,24 +125,24 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(slug: str, client: "Credmark") -> Optional[List["ModelDeployment"]]:
+async def asyncio(slug: str, client: "Credmark") -> List["ModelDeployment"]:
     """Get model deployments of a model by slug
 
      Returns the deployments for a model.
 
     Args:
         slug (str):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelDeployment']]
     """
 
     return (
```

### Comparing `credmark-1.1.0/credmark/api/defi_api/get_model_runtime_stats.py` & `credmark-1.2.0/credmark/api/defi_api/get_model_runtime_stats.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict
@@ -25,23 +25,20 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelRuntimeStatsResponse]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> ModelRuntimeStatsResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = ModelRuntimeStatsResponse.from_dict(response.json())
 
         return response_200
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
 def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelRuntimeStatsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
@@ -51,15 +48,15 @@
 
 def sync_detailed(client: "Credmark") -> Response[ModelRuntimeStatsResponse]:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     kwargs = _get_kwargs(
@@ -70,21 +67,21 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(client: "Credmark") -> Optional[ModelRuntimeStatsResponse]:
+def sync(client: "Credmark") -> ModelRuntimeStatsResponse:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     return sync_detailed(
@@ -94,15 +91,15 @@
 
 async def asyncio_detailed(client: "Credmark") -> Response[ModelRuntimeStatsResponse]:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     kwargs = _get_kwargs(
@@ -111,21 +108,21 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(client: "Credmark") -> Optional[ModelRuntimeStatsResponse]:
+async def asyncio(client: "Credmark") -> ModelRuntimeStatsResponse:
     """Model runtime stats
 
      Returns runtime stats for all models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRuntimeStatsResponse]
     """
 
     return (
```

### Comparing `credmark-1.1.0/credmark/api/defi_api/list_models.py` & `credmark-1.2.0/credmark/api/defi_api/list_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, List
@@ -25,28 +25,25 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List["ModelMetadata"]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> List["ModelMetadata"]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
             response_200_item = ModelMetadata.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
 def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List["ModelMetadata"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
@@ -56,15 +53,15 @@
 
 def sync_detailed(client: "Credmark") -> Response[List["ModelMetadata"]]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelMetadata']]
     """
 
     kwargs = _get_kwargs(
@@ -75,21 +72,21 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(client: "Credmark") -> Optional[List["ModelMetadata"]]:
+def sync(client: "Credmark") -> List["ModelMetadata"]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelMetadata']]
     """
 
     return sync_detailed(
@@ -99,15 +96,15 @@
 
 async def asyncio_detailed(client: "Credmark") -> Response[List["ModelMetadata"]]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelMetadata']]
     """
 
     kwargs = _get_kwargs(
@@ -116,21 +113,21 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(client: "Credmark") -> Optional[List["ModelMetadata"]]:
+async def asyncio(client: "Credmark") -> List["ModelMetadata"]:
     """List metadata for available models
 
      Returns a list of metadata for available models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List['ModelMetadata']]
     """
 
     return (
```

### Comparing `credmark-1.1.0/credmark/api/defi_api/run_model.py` & `credmark-1.2.0/credmark/api/defi_api/run_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict
@@ -29,23 +29,20 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[ModelRunResponse]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> ModelRunResponse:
     if response.status_code == HTTPStatus.CREATED:
         response_201 = ModelRunResponse.from_dict(response.json())
 
         return response_201
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
 def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[ModelRunResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
@@ -58,15 +55,15 @@
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRunResponse]
     """
 
     kwargs = _get_kwargs(
@@ -78,24 +75,24 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(*, json_body: RunModelDto, client: "Credmark") -> Optional[ModelRunResponse]:
+def sync(*, json_body: RunModelDto, client: "Credmark") -> ModelRunResponse:
     """Run model
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRunResponse]
     """
 
     return sync_detailed(
@@ -109,15 +106,15 @@
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRunResponse]
     """
 
     kwargs = _get_kwargs(
@@ -127,24 +124,24 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(*, json_body: RunModelDto, client: "Credmark") -> Optional[ModelRunResponse]:
+async def asyncio(*, json_body: RunModelDto, client: "Credmark") -> ModelRunResponse:
     """Run model
 
      Runs a model and returns result object.
 
     Args:
         json_body (RunModelDto):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ModelRunResponse]
     """
 
     return (
```

### Comparing `credmark-1.1.0/credmark/api/token_api/__init__.py` & `credmark-1.2.0/credmark/api/token_api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, Optional, Union, cast
 
 from ...models.get_token_price_align import GetTokenPriceAlign
@@ -59,31 +59,31 @@
     def get_token_metadata(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
+    ) -> TokenMetadataResponse:
         """Get token metadata
 
          Returns metadata for a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenMetadataResponse]]
+            Response[TokenMetadataResponse]
         """
 
         return get_token_metadata.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -93,31 +93,31 @@
     async def get_token_metadata_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
+    ) -> TokenMetadataResponse:
         """Get token metadata
 
          Returns metadata for a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenMetadataResponse]]
+            Response[TokenMetadataResponse]
         """
 
         return await get_token_metadata.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -127,31 +127,31 @@
     def get_token_name(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
+    ) -> TokenNameResponse:
         """Get token name
 
          Returns name of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenNameResponse]]
+            Response[TokenNameResponse]
         """
 
         return get_token_name.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -161,31 +161,31 @@
     async def get_token_name_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
+    ) -> TokenNameResponse:
         """Get token name
 
          Returns name of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenNameResponse]]
+            Response[TokenNameResponse]
         """
 
         return await get_token_name.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -195,31 +195,31 @@
     def get_token_symbol(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    ) -> TokenSymbolResponse:
         """Get token symbol
 
          Returns symbol of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+            Response[TokenSymbolResponse]
         """
 
         return get_token_symbol.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -229,31 +229,31 @@
     async def get_token_symbol_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
+    ) -> TokenSymbolResponse:
         """Get token symbol
 
          Returns symbol of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+            Response[TokenSymbolResponse]
         """
 
         return await get_token_symbol.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -263,31 +263,31 @@
     def get_token_decimals(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    ) -> TokenDecimalsResponse:
         """Get token decimals
 
          Returns decimals of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+            Response[TokenDecimalsResponse]
         """
 
         return get_token_decimals.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -297,31 +297,31 @@
     async def get_token_decimals_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+    ) -> TokenDecimalsResponse:
         """Get token decimals
 
          Returns decimals of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+            Response[TokenDecimalsResponse]
         """
 
         return await get_token_decimals.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -332,32 +332,32 @@
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    ) -> TokenTotalSupplyResponse:
         """Get token's total supply
 
          Returns total supply of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
+            Response[TokenTotalSupplyResponse]
         """
 
         return get_token_total_supply.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -369,32 +369,32 @@
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyResponse]]:
+    ) -> TokenTotalSupplyResponse:
         """Get token's total supply
 
          Returns total supply of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenTotalSupplyResponse]]
+            Response[TokenTotalSupplyResponse]
         """
 
         return await get_token_total_supply.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -410,15 +410,15 @@
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    ) -> TokenTotalSupplyHistoricalResponse:
         """Get historical total supply
 
          Returns historical total supply for a token.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -427,19 +427,19 @@
             block_interval (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+            Response[TokenTotalSupplyHistoricalResponse]
         """
 
         return get_token_total_supply_historical.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -459,15 +459,15 @@
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+    ) -> TokenTotalSupplyHistoricalResponse:
         """Get historical total supply
 
          Returns historical total supply for a token.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -476,19 +476,19 @@
             block_interval (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+            Response[TokenTotalSupplyHistoricalResponse]
         """
 
         return await get_token_total_supply_historical.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -503,31 +503,31 @@
     def get_token_logo(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
+    ) -> TokenLogoResponse:
         """Get token logo
 
          Returns logo of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenLogoResponse]]
+            Response[TokenLogoResponse]
         """
 
         return get_token_logo.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -537,31 +537,31 @@
     async def get_token_logo_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
+    ) -> TokenLogoResponse:
         """Get token logo
 
          Returns logo of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenLogoResponse]]
+            Response[TokenLogoResponse]
         """
 
         return await get_token_logo.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -571,31 +571,31 @@
     def get_token_creation_block(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
+    ) -> TokenCreationBlockResponse:
         """Get token creation block
 
          Returns creation block number of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]
+            Response[TokenCreationBlockResponse]
         """
 
         return get_token_creation_block.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -605,31 +605,31 @@
     async def get_token_creation_block_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
+    ) -> TokenCreationBlockResponse:
         """Get token creation block
 
          Returns creation block number of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]
+            Response[TokenCreationBlockResponse]
         """
 
         return await get_token_creation_block.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -639,31 +639,31 @@
     def get_token_abi(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
+    ) -> TokenAbiResponse:
         """Get token ABI
 
          Returns ABI of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenAbiResponse, TokenErrorResponse]]
+            Response[TokenAbiResponse]
         """
 
         return get_token_abi.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -673,31 +673,31 @@
     async def get_token_abi_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
+    ) -> TokenAbiResponse:
         """Get token ABI
 
          Returns ABI of a token.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenAbiResponse, TokenErrorResponse]]
+            Response[TokenAbiResponse]
         """
 
         return await get_token_abi.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -710,34 +710,34 @@
         token_address: str,
         *,
         quote_address: Union[Unset, None, str] = UNSET,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
         align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
+    ) -> TokenPriceResponse:
         """Get token price data
 
          Returns price data for a token.
 
         Args:
             chain_id (float):
             token_address (str):
             quote_address (Union[Unset, None, str]):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
             src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
             align (Union[Unset, None, GetTokenPriceAlign]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenPriceResponse]]
+            Response[TokenPriceResponse]
         """
 
         return get_token_price.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             quote_address=quote_address,
@@ -753,34 +753,34 @@
         token_address: str,
         *,
         quote_address: Union[Unset, None, str] = UNSET,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
         src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
         align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
+    ) -> TokenPriceResponse:
         """Get token price data
 
          Returns price data for a token.
 
         Args:
             chain_id (float):
             token_address (str):
             quote_address (Union[Unset, None, str]):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
             src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
             align (Union[Unset, None, GetTokenPriceAlign]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenPriceResponse]]
+            Response[TokenPriceResponse]
         """
 
         return await get_token_price.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             quote_address=quote_address,
@@ -799,15 +799,15 @@
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         quote_address: Union[Unset, None, str] = UNSET,
         src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
-    ) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+    ) -> TokenPriceHistoricalResponse:
         """Get historical price
 
          Returns historical price data for a token.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -818,19 +818,19 @@
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             quote_address (Union[Unset, None, str]):
             src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
                 GetTokenPriceHistoricalSrc.DEX.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
+            Response[TokenPriceHistoricalResponse]
         """
 
         return get_token_price_historical.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -852,15 +852,15 @@
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         quote_address: Union[Unset, None, str] = UNSET,
         src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
-    ) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+    ) -> TokenPriceHistoricalResponse:
         """Get historical price
 
          Returns historical price data for a token.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -871,19 +871,19 @@
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             quote_address (Union[Unset, None, str]):
             src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
                 GetTokenPriceHistoricalSrc.DEX.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
+            Response[TokenPriceHistoricalResponse]
         """
 
         return await get_token_price_historical.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -902,34 +902,34 @@
         token_address: str,
         *,
         account_address: str,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
+    ) -> TokenBalanceResponse:
         """Get token balance
 
          Returns token balance for an account.
 
         Args:
             chain_id (float):
             token_address (str):
             account_address (str):
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenBalanceResponse, TokenErrorResponse]]
+            Response[TokenBalanceResponse]
         """
 
         return get_token_balance.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             account_address=account_address,
@@ -945,34 +945,34 @@
         token_address: str,
         *,
         account_address: str,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
+    ) -> TokenBalanceResponse:
         """Get token balance
 
          Returns token balance for an account.
 
         Args:
             chain_id (float):
             token_address (str):
             account_address (str):
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenBalanceResponse, TokenErrorResponse]]
+            Response[TokenBalanceResponse]
         """
 
         return await get_token_balance.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             account_address=account_address,
@@ -992,15 +992,15 @@
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         account_address: str,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+    ) -> TokenBalanceHistoricalResponse:
         """Get historical balance
 
          Returns historical token balance for an account.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1011,19 +1011,19 @@
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             account_address (str):
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
+            Response[TokenBalanceHistoricalResponse]
         """
 
         return get_token_balance_historical.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -1047,15 +1047,15 @@
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         account_address: str,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+    ) -> TokenBalanceHistoricalResponse:
         """Get historical balance
 
          Returns historical token balance for an account.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1066,19 +1066,19 @@
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             account_address (str):
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
+            Response[TokenBalanceHistoricalResponse]
         """
 
         return await get_token_balance_historical.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -1098,34 +1098,34 @@
         token_address: str,
         *,
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    ) -> TokenVolumeResponse:
         """Get token volume
 
          Returns traded volume for a token over a period of blocks or time.
 
         Args:
             chain_id (float):
             token_address (str):
             scaled (Union[Unset, None, bool]):  Default: True.
             start_block_number (Union[Unset, None, float]):
             end_block_number (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+            Response[TokenVolumeResponse]
         """
 
         return get_token_volume.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             scaled=scaled,
@@ -1141,34 +1141,34 @@
         token_address: str,
         *,
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
+    ) -> TokenVolumeResponse:
         """Get token volume
 
          Returns traded volume for a token over a period of blocks or time.
 
         Args:
             chain_id (float):
             token_address (str):
             scaled (Union[Unset, None, bool]):  Default: True.
             start_block_number (Union[Unset, None, float]):
             end_block_number (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+            Response[TokenVolumeResponse]
         """
 
         return await get_token_volume.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             scaled=scaled,
@@ -1186,15 +1186,15 @@
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
+    ) -> TokenVolumeHistoricalResponse:
         """Get historical volume
 
          Returns traded volume for a token over a period of blocks or time divided by intervals.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1203,19 +1203,19 @@
             end_block_number (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
             block_interval (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+            Response[TokenVolumeHistoricalResponse]
         """
 
         return get_token_volume_historical.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             scaled=scaled,
@@ -1235,15 +1235,15 @@
         scaled: Union[Unset, None, bool] = True,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
+    ) -> TokenVolumeHistoricalResponse:
         """Get historical volume
 
          Returns traded volume for a token over a period of blocks or time divided by intervals.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1252,19 +1252,19 @@
             end_block_number (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
             block_interval (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+            Response[TokenVolumeHistoricalResponse]
         """
 
         return await get_token_volume_historical.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             scaled=scaled,
@@ -1283,15 +1283,15 @@
         *,
         page_size: float = 100.0,
         cursor: Union[Unset, None, str] = UNSET,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
+    ) -> TokenHoldersResponse:
         """Get token holders
 
          Returns holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1299,19 +1299,19 @@
             cursor (Union[Unset, None, str]):
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHoldersResponse]]
+            Response[TokenHoldersResponse]
         """
 
         return get_token_holders.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             page_size=page_size,
@@ -1329,15 +1329,15 @@
         *,
         page_size: float = 100.0,
         cursor: Union[Unset, None, str] = UNSET,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
+    ) -> TokenHoldersResponse:
         """Get token holders
 
          Returns holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1345,19 +1345,19 @@
             cursor (Union[Unset, None, str]):
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHoldersResponse]]
+            Response[TokenHoldersResponse]
         """
 
         return await get_token_holders.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             page_size=page_size,
@@ -1378,15 +1378,15 @@
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         page_size: float = 100.0,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+    ) -> TokenHoldersHistoricalResponse:
         """Get token historical holders
 
          Returns historical holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1397,19 +1397,19 @@
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             page_size (float):  Default: 100.0.
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
+            Response[TokenHoldersHistoricalResponse]
         """
 
         return get_token_holders_historical.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -1433,15 +1433,15 @@
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
         page_size: float = 100.0,
         quote_address: Union[Unset, None, str] = UNSET,
         scaled: Union[Unset, None, bool] = True,
-    ) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+    ) -> TokenHoldersHistoricalResponse:
         """Get token historical holders
 
          Returns historical holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1452,19 +1452,19 @@
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
             page_size (float):  Default: 100.0.
             quote_address (Union[Unset, None, str]):
             scaled (Union[Unset, None, bool]):  Default: True.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
+            Response[TokenHoldersHistoricalResponse]
         """
 
         return await get_token_holders_historical.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -1481,31 +1481,31 @@
     def get_token_holders_count(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    ) -> TokenHoldersCountResponse:
         """Get total number of token holders
 
          Returns total number of holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+            Response[TokenHoldersCountResponse]
         """
 
         return get_token_holders_count.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -1515,31 +1515,31 @@
     async def get_token_holders_count_async(
         self,
         chain_id: float,
         token_address: str,
         *,
         block_number: Union[Unset, None, float] = UNSET,
         timestamp: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+    ) -> TokenHoldersCountResponse:
         """Get total number of token holders
 
          Returns total number of holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
             block_number (Union[Unset, None, float]):
             timestamp (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+            Response[TokenHoldersCountResponse]
         """
 
         return await get_token_holders_count.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             block_number=block_number,
@@ -1553,15 +1553,15 @@
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+    ) -> TokenHistoricalHoldersCountResponse:
         """Get historical total number of token holders
 
          Returns historical total number of holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1569,19 +1569,19 @@
             end_block_number (Union[Unset, None, float]):
             block_interval (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
+            Response[TokenHistoricalHoldersCountResponse]
         """
 
         return get_token_holders_count_historical.sync(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
@@ -1599,15 +1599,15 @@
         *,
         start_block_number: Union[Unset, None, float] = UNSET,
         end_block_number: Union[Unset, None, float] = UNSET,
         block_interval: Union[Unset, None, float] = UNSET,
         start_timestamp: Union[Unset, None, float] = UNSET,
         end_timestamp: Union[Unset, None, float] = UNSET,
         time_interval: Union[Unset, None, float] = UNSET,
-    ) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+    ) -> TokenHistoricalHoldersCountResponse:
         """Get historical total number of token holders
 
          Returns historical total number of holders of a token at a block or time.
 
         Args:
             chain_id (float):
             token_address (str):
@@ -1615,19 +1615,19 @@
             end_block_number (Union[Unset, None, float]):
             block_interval (Union[Unset, None, float]):
             start_timestamp (Union[Unset, None, float]):
             end_timestamp (Union[Unset, None, float]):
             time_interval (Union[Unset, None, float]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
+            Response[TokenHistoricalHoldersCountResponse]
         """
 
         return await get_token_holders_count_historical.asyncio(
             client=self.__client,
             chain_id=chain_id,
             token_address=token_address,
             start_block_number=start_block_number,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_abi.py` & `credmark-1.2.0/credmark/api/token_api/get_token_abi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_abi_response import TokenAbiResponse
 from ...models.token_error_response import TokenErrorResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -43,34 +43,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenAbiResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenAbiResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenAbiResponse, TokenErrorResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenAbiResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -78,31 +71,31 @@
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenAbiResponse, TokenErrorResponse]]:
+) -> Response[TokenAbiResponse]:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenAbiResponse, TokenErrorResponse]]
+        Response[TokenAbiResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -120,31 +113,31 @@
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
+) -> TokenAbiResponse:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenAbiResponse, TokenErrorResponse]]
+        Response[TokenAbiResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -155,31 +148,31 @@
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenAbiResponse, TokenErrorResponse]]:
+) -> Response[TokenAbiResponse]:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenAbiResponse, TokenErrorResponse]]
+        Response[TokenAbiResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -195,31 +188,31 @@
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenAbiResponse, TokenErrorResponse]]:
+) -> TokenAbiResponse:
     """Get token ABI
 
      Returns ABI of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenAbiResponse, TokenErrorResponse]]
+        Response[TokenAbiResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_balance.py` & `credmark-1.2.0/credmark/api/token_api/get_token_balance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_balance_response import TokenBalanceResponse
 from ...models.token_error_response import TokenErrorResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -52,34 +52,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenBalanceResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenBalanceResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenBalanceResponse, TokenErrorResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenBalanceResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -90,34 +83,34 @@
     *,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenBalanceResponse, TokenErrorResponse]]:
+) -> Response[TokenBalanceResponse]:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceResponse, TokenErrorResponse]]
+        Response[TokenBalanceResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         account_address=account_address,
@@ -141,34 +134,34 @@
     *,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
+) -> TokenBalanceResponse:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceResponse, TokenErrorResponse]]
+        Response[TokenBalanceResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         account_address=account_address,
@@ -185,34 +178,34 @@
     *,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenBalanceResponse, TokenErrorResponse]]:
+) -> Response[TokenBalanceResponse]:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceResponse, TokenErrorResponse]]
+        Response[TokenBalanceResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         account_address=account_address,
@@ -234,34 +227,34 @@
     *,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenBalanceResponse, TokenErrorResponse]]:
+) -> TokenBalanceResponse:
     """Get token balance
 
      Returns token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceResponse, TokenErrorResponse]]
+        Response[TokenBalanceResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_balance_historical.py` & `credmark-1.2.0/credmark/api/token_api/get_token_balance_historical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_balance_historical_response import TokenBalanceHistoricalResponse
 from ...models.token_error_response import TokenErrorResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -64,34 +64,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenBalanceHistoricalResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenBalanceHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenBalanceHistoricalResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -106,15 +99,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+) -> Response[TokenBalanceHistoricalResponse]:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -125,19 +118,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
+        Response[TokenBalanceHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -169,15 +162,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+) -> TokenBalanceHistoricalResponse:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -188,19 +181,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
+        Response[TokenBalanceHistoricalResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -225,15 +218,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+) -> Response[TokenBalanceHistoricalResponse]:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -244,19 +237,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
+        Response[TokenBalanceHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -286,15 +279,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     account_address: str,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]:
+) -> TokenBalanceHistoricalResponse:
     """Get historical balance
 
      Returns historical token balance for an account.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -305,19 +298,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         account_address (str):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenBalanceHistoricalResponse, TokenErrorResponse]]
+        Response[TokenBalanceHistoricalResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_creation_block.py` & `credmark-1.2.0/credmark/api/token_api/get_token_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
-from ...models.token_creation_block_response import TokenCreationBlockResponse
 from ...models.token_error_response import TokenErrorResponse
+from ...models.token_metadata_response import TokenMetadataResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/creation-block".format(
-        client.base_url, chainId=chain_id, tokenAddress=token_address
-    )
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}".format(client.base_url, chainId=chain_id, tokenAddress=token_address)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["blockNumber"] = block_number
 
@@ -43,34 +41,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenMetadataResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenCreationBlockResponse.from_dict(response.json())
+        response_200 = TokenMetadataResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenMetadataResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -78,31 +69,31 @@
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
-    """Get token creation block
+) -> Response[TokenMetadataResponse]:
+    """Get token metadata
 
-     Returns creation block number of a token.
+     Returns metadata for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]
+        Response[TokenMetadataResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -120,31 +111,31 @@
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
-    """Get token creation block
+) -> TokenMetadataResponse:
+    """Get token metadata
 
-     Returns creation block number of a token.
+     Returns metadata for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]
+        Response[TokenMetadataResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -155,31 +146,31 @@
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
-    """Get token creation block
+) -> Response[TokenMetadataResponse]:
+    """Get token metadata
 
-     Returns creation block number of a token.
+     Returns metadata for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]
+        Response[TokenMetadataResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -195,31 +186,31 @@
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenCreationBlockResponse, TokenErrorResponse]]:
-    """Get token creation block
+) -> TokenMetadataResponse:
+    """Get token metadata
 
-     Returns creation block number of a token.
+     Returns metadata for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenCreationBlockResponse, TokenErrorResponse]]
+        Response[TokenMetadataResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_decimals.py` & `credmark-1.2.0/credmark/api/token_api/get_token_decimals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_decimals_response import TokenDecimalsResponse
 from ...models.token_error_response import TokenErrorResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -43,34 +43,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenDecimalsResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenDecimalsResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenDecimalsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -78,31 +71,31 @@
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+) -> Response[TokenDecimalsResponse]:
     """Get token decimals
 
      Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[TokenDecimalsResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -120,31 +113,31 @@
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+) -> TokenDecimalsResponse:
     """Get token decimals
 
      Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[TokenDecimalsResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -155,31 +148,31 @@
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+) -> Response[TokenDecimalsResponse]:
     """Get token decimals
 
      Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[TokenDecimalsResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -195,31 +188,31 @@
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenDecimalsResponse, TokenErrorResponse]]:
+) -> TokenDecimalsResponse:
     """Get token decimals
 
      Returns decimals of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenDecimalsResponse, TokenErrorResponse]]
+        Response[TokenDecimalsResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_holders.py` & `credmark-1.2.0/credmark/api/token_api/get_token_holders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
 from ...models.token_holders_response import TokenHoldersResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -55,34 +55,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenHoldersResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenHoldersResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenHoldersResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenHoldersResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -94,15 +87,15 @@
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHoldersResponse]]:
+) -> Response[TokenHoldersResponse]:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -110,19 +103,19 @@
         cursor (Union[Unset, None, str]):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersResponse]]
+        Response[TokenHoldersResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         page_size=page_size,
@@ -148,15 +141,15 @@
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
+) -> TokenHoldersResponse:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -164,19 +157,19 @@
         cursor (Union[Unset, None, str]):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersResponse]]
+        Response[TokenHoldersResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         page_size=page_size,
@@ -195,15 +188,15 @@
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHoldersResponse]]:
+) -> Response[TokenHoldersResponse]:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -211,19 +204,19 @@
         cursor (Union[Unset, None, str]):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersResponse]]
+        Response[TokenHoldersResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         page_size=page_size,
@@ -247,15 +240,15 @@
     page_size: float = 100.0,
     cursor: Union[Unset, None, str] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHoldersResponse]]:
+) -> TokenHoldersResponse:
     """Get token holders
 
      Returns holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -263,19 +256,19 @@
         cursor (Union[Unset, None, str]):
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersResponse]]
+        Response[TokenHoldersResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_holders_count.py` & `credmark-1.2.0/credmark/api/token_api/get_token_holders_count.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
 from ...models.token_holders_count_response import TokenHoldersCountResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -43,34 +43,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenHoldersCountResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenHoldersCountResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenHoldersCountResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -78,31 +71,31 @@
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+) -> Response[TokenHoldersCountResponse]:
     """Get total number of token holders
 
      Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[TokenHoldersCountResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -120,31 +113,31 @@
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+) -> TokenHoldersCountResponse:
     """Get total number of token holders
 
      Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[TokenHoldersCountResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -155,31 +148,31 @@
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+) -> Response[TokenHoldersCountResponse]:
     """Get total number of token holders
 
      Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[TokenHoldersCountResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -195,31 +188,31 @@
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHoldersCountResponse]]:
+) -> TokenHoldersCountResponse:
     """Get total number of token holders
 
      Returns total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersCountResponse]]
+        Response[TokenHoldersCountResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_holders_count_historical.py` & `credmark-1.2.0/credmark/api/token_api/get_token_volume_historical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_historical_holders_count_response import TokenHistoricalHoldersCountResponse
+from ...models.token_volume_historical_response import TokenVolumeHistoricalResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
+    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/count/historical".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
+    params["scaled"] = scaled
+
     params["startBlockNumber"] = start_block_number
 
     params["endBlockNumber"] = end_block_number
 
-    params["blockInterval"] = block_interval
-
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
+    params["blockInterval"] = block_interval
+
     params["timeInterval"] = time_interval
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
@@ -55,85 +58,81 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenVolumeHistoricalResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenHistoricalHoldersCountResponse.from_dict(response.json())
+        response_200 = TokenVolumeHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenVolumeHistoricalResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
+    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
-    """Get historical total number of token holders
+) -> Response[TokenVolumeHistoricalResponse]:
+    """Get historical volume
 
-     Returns historical total number of holders of a token at a block or time.
+     Returns traded volume for a token over a period of blocks or time divided by intervals.
 
     Args:
         chain_id (float):
         token_address (str):
+        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
+        Response[TokenVolumeHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
+        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
-        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        block_interval=block_interval,
         time_interval=time_interval,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
@@ -141,149 +140,158 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
+    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
-    """Get historical total number of token holders
+) -> TokenVolumeHistoricalResponse:
+    """Get historical volume
 
-     Returns historical total number of holders of a token at a block or time.
+     Returns traded volume for a token over a period of blocks or time divided by intervals.
 
     Args:
         chain_id (float):
         token_address (str):
+        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
+        Response[TokenVolumeHistoricalResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
+        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
-        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        block_interval=block_interval,
         time_interval=time_interval,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
+    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
-    """Get historical total number of token holders
+) -> Response[TokenVolumeHistoricalResponse]:
+    """Get historical volume
 
-     Returns historical total number of holders of a token at a block or time.
+     Returns traded volume for a token over a period of blocks or time divided by intervals.
 
     Args:
         chain_id (float):
         token_address (str):
+        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
+        Response[TokenVolumeHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
+        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
-        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        block_interval=block_interval,
         time_interval=time_interval,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
+    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]:
-    """Get historical total number of token holders
+) -> TokenVolumeHistoricalResponse:
+    """Get historical volume
 
-     Returns historical total number of holders of a token at a block or time.
+     Returns traded volume for a token over a period of blocks or time divided by intervals.
 
     Args:
         chain_id (float):
         token_address (str):
+        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]]
+        Response[TokenVolumeHistoricalResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
+            scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
-            block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
+            block_interval=block_interval,
             time_interval=time_interval,
         )
     ).parsed
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_holders_historical.py` & `credmark-1.2.0/credmark/api/token_api/get_token_holders_historical.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
 from ...models.token_holders_historical_response import TokenHoldersHistoricalResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -64,34 +64,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenHoldersHistoricalResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenHoldersHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenHoldersHistoricalResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -106,15 +99,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     page_size: float = 100.0,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+) -> Response[TokenHoldersHistoricalResponse]:
     """Get token historical holders
 
      Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -125,19 +118,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         page_size (float):  Default: 100.0.
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
+        Response[TokenHoldersHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -169,15 +162,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     page_size: float = 100.0,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+) -> TokenHoldersHistoricalResponse:
     """Get token historical holders
 
      Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -188,19 +181,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         page_size (float):  Default: 100.0.
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
+        Response[TokenHoldersHistoricalResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -225,15 +218,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     page_size: float = 100.0,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+) -> Response[TokenHoldersHistoricalResponse]:
     """Get token historical holders
 
      Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -244,19 +237,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         page_size (float):  Default: 100.0.
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
+        Response[TokenHoldersHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -286,15 +279,15 @@
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     page_size: float = 100.0,
     quote_address: Union[Unset, None, str] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]:
+) -> TokenHoldersHistoricalResponse:
     """Get token historical holders
 
      Returns historical holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -305,19 +298,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         page_size (float):  Default: 100.0.
         quote_address (Union[Unset, None, str]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenHoldersHistoricalResponse]]
+        Response[TokenHoldersHistoricalResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_logo.py` & `credmark-1.2.0/credmark/api/token_api/get_token_total_supply.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_logo_response import TokenLogoResponse
+from ...models.token_total_supply_response import TokenTotalSupplyResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/logo".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/total-supply".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["blockNumber"] = block_number
 
     params["timestamp"] = timestamp
 
+    params["scaled"] = scaled
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenTotalSupplyResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenLogoResponse.from_dict(response.json())
+        response_200 = TokenTotalSupplyResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenLogoResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenTotalSupplyResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+) -> Response[TokenTotalSupplyResponse]:
+    """Get token's total supply
 
-     Returns logo of a token.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[TokenTotalSupplyResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
+        scaled=scaled,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
@@ -119,111 +118,120 @@
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+) -> TokenTotalSupplyResponse:
+    """Get token's total supply
 
-     Returns logo of a token.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[TokenTotalSupplyResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
+        scaled=scaled,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+) -> Response[TokenTotalSupplyResponse]:
+    """Get token's total supply
 
-     Returns logo of a token.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[TokenTotalSupplyResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
         timestamp=timestamp,
+        scaled=scaled,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
+    scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenLogoResponse]]:
-    """Get token logo
+) -> TokenTotalSupplyResponse:
+    """Get token's total supply
 
-     Returns logo of a token.
+     Returns total supply of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
+        scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenLogoResponse]]
+        Response[TokenTotalSupplyResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
             block_number=block_number,
             timestamp=timestamp,
+            scaled=scaled,
         )
     ).parsed
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_metadata.py` & `credmark-1.2.0/credmark/api/token_api/get_token_name.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_metadata_response import TokenMetadataResponse
+from ...models.token_name_response import TokenNameResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}".format(client.base_url, chainId=chain_id, tokenAddress=token_address)
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/name".format(
+        client.base_url, chainId=chain_id, tokenAddress=token_address
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["blockNumber"] = block_number
 
@@ -41,34 +43,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenNameResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenMetadataResponse.from_dict(response.json())
+        response_200 = TokenNameResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenMetadataResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenNameResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -76,31 +71,31 @@
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenMetadataResponse]]:
-    """Get token metadata
+) -> Response[TokenNameResponse]:
+    """Get token name
 
-     Returns metadata for a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenMetadataResponse]]
+        Response[TokenNameResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -118,31 +113,31 @@
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
-    """Get token metadata
+) -> TokenNameResponse:
+    """Get token name
 
-     Returns metadata for a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenMetadataResponse]]
+        Response[TokenNameResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -153,31 +148,31 @@
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenMetadataResponse]]:
-    """Get token metadata
+) -> Response[TokenNameResponse]:
+    """Get token name
 
-     Returns metadata for a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenMetadataResponse]]
+        Response[TokenNameResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -193,31 +188,31 @@
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenMetadataResponse]]:
-    """Get token metadata
+) -> TokenNameResponse:
+    """Get token name
 
-     Returns metadata for a token.
+     Returns name of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenMetadataResponse]]
+        Response[TokenNameResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_name.py` & `credmark-1.2.0/credmark/api/token_api/get_token_symbol.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_name_response import TokenNameResponse
+from ...models.token_symbol_response import TokenSymbolResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/name".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/symbol".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -43,34 +43,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenSymbolResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenNameResponse.from_dict(response.json())
+        response_200 = TokenSymbolResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenSymbolResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -78,31 +71,31 @@
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+) -> Response[TokenSymbolResponse]:
+    """Get token symbol
 
-     Returns name of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[TokenSymbolResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -120,31 +113,31 @@
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+) -> TokenSymbolResponse:
+    """Get token symbol
 
-     Returns name of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[TokenSymbolResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -155,31 +148,31 @@
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+) -> Response[TokenSymbolResponse]:
+    """Get token symbol
 
-     Returns name of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[TokenSymbolResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -195,31 +188,31 @@
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenNameResponse]]:
-    """Get token name
+) -> TokenSymbolResponse:
+    """Get token symbol
 
-     Returns name of a token.
+     Returns symbol of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenNameResponse]]
+        Response[TokenSymbolResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_price.py` & `credmark-1.2.0/credmark/api/token_api/get_token_price.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.get_token_price_align import GetTokenPriceAlign
 from ...models.get_token_price_src import GetTokenPriceSrc
 from ...models.token_error_response import TokenErrorResponse
 from ...models.token_price_response import TokenPriceResponse
 from ...types import UNSET, Response, Unset
@@ -62,34 +62,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenPriceResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenPriceResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenPriceResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenPriceResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -100,34 +93,34 @@
     *,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenPriceResponse]]:
+) -> Response[TokenPriceResponse]:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         quote_address (Union[Unset, None, str]):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
         src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
         align (Union[Unset, None, GetTokenPriceAlign]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceResponse]]
+        Response[TokenPriceResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         quote_address=quote_address,
@@ -151,34 +144,34 @@
     *,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
+) -> TokenPriceResponse:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         quote_address (Union[Unset, None, str]):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
         src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
         align (Union[Unset, None, GetTokenPriceAlign]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceResponse]]
+        Response[TokenPriceResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         quote_address=quote_address,
@@ -195,34 +188,34 @@
     *,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenPriceResponse]]:
+) -> Response[TokenPriceResponse]:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         quote_address (Union[Unset, None, str]):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
         src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
         align (Union[Unset, None, GetTokenPriceAlign]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceResponse]]
+        Response[TokenPriceResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         quote_address=quote_address,
@@ -244,34 +237,34 @@
     *,
     quote_address: Union[Unset, None, str] = UNSET,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     src: Union[Unset, None, GetTokenPriceSrc] = GetTokenPriceSrc.DEX,
     align: Union[Unset, None, GetTokenPriceAlign] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenPriceResponse]]:
+) -> TokenPriceResponse:
     """Get token price data
 
      Returns price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
         quote_address (Union[Unset, None, str]):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
         src (Union[Unset, None, GetTokenPriceSrc]):  Default: GetTokenPriceSrc.DEX.
         align (Union[Unset, None, GetTokenPriceAlign]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceResponse]]
+        Response[TokenPriceResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_price_historical.py` & `credmark-1.2.0/credmark/api/token_api/get_token_price_historical.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.get_token_price_historical_src import GetTokenPriceHistoricalSrc
 from ...models.token_error_response import TokenErrorResponse
 from ...models.token_price_historical_response import TokenPriceHistoricalResponse
 from ...types import UNSET, Response, Unset
 
@@ -66,34 +66,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenPriceHistoricalResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenPriceHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenPriceHistoricalResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -107,15 +100,15 @@
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+) -> Response[TokenPriceHistoricalResponse]:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -126,19 +119,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         quote_address (Union[Unset, None, str]):
         src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
             GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
+        Response[TokenPriceHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -168,15 +161,15 @@
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+) -> TokenPriceHistoricalResponse:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -187,19 +180,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         quote_address (Union[Unset, None, str]):
         src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
             GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
+        Response[TokenPriceHistoricalResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -222,15 +215,15 @@
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+) -> Response[TokenPriceHistoricalResponse]:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -241,19 +234,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         quote_address (Union[Unset, None, str]):
         src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
             GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
+        Response[TokenPriceHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -281,15 +274,15 @@
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     quote_address: Union[Unset, None, str] = UNSET,
     src: Union[Unset, None, GetTokenPriceHistoricalSrc] = GetTokenPriceHistoricalSrc.DEX,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]:
+) -> TokenPriceHistoricalResponse:
     """Get historical price
 
      Returns historical price data for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -300,19 +293,19 @@
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         quote_address (Union[Unset, None, str]):
         src (Union[Unset, None, GetTokenPriceHistoricalSrc]):  Default:
             GetTokenPriceHistoricalSrc.DEX.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenPriceHistoricalResponse]]
+        Response[TokenPriceHistoricalResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_symbol.py` & `credmark-1.2.0/credmark/api/token_api/get_token_logo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_symbol_response import TokenSymbolResponse
+from ...models.token_logo_response import TokenLogoResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/symbol".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/logo".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -43,34 +43,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenLogoResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenSymbolResponse.from_dict(response.json())
+        response_200 = TokenLogoResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenLogoResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -78,31 +71,31 @@
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+) -> Response[TokenLogoResponse]:
+    """Get token logo
 
-     Returns symbol of a token.
+     Returns logo of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[TokenLogoResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -120,31 +113,31 @@
 def sync(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+) -> TokenLogoResponse:
+    """Get token logo
 
-     Returns symbol of a token.
+     Returns logo of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[TokenLogoResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -155,31 +148,31 @@
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+) -> Response[TokenLogoResponse]:
+    """Get token logo
 
-     Returns symbol of a token.
+     Returns logo of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[TokenLogoResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         block_number=block_number,
@@ -195,31 +188,31 @@
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
     block_number: Union[Unset, None, float] = UNSET,
     timestamp: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenSymbolResponse]]:
-    """Get token symbol
+) -> TokenLogoResponse:
+    """Get token logo
 
-     Returns symbol of a token.
+     Returns logo of a token.
 
     Args:
         chain_id (float):
         token_address (str):
         block_number (Union[Unset, None, float]):
         timestamp (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenSymbolResponse]]
+        Response[TokenLogoResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_total_supply_historical.py` & `credmark-1.2.0/credmark/api/token_api/get_token_total_supply_historical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
 from ...models.token_total_supply_historical_response import TokenTotalSupplyHistoricalResponse
 from ...types import UNSET, Response, Unset
 
 
@@ -58,34 +58,27 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenTotalSupplyHistoricalResponse:
     if response.status_code == HTTPStatus.OK:
         response_200 = TokenTotalSupplyHistoricalResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenTotalSupplyHistoricalResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -98,15 +91,15 @@
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+) -> Response[TokenTotalSupplyHistoricalResponse]:
     """Get historical total supply
 
      Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -115,19 +108,19 @@
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[TokenTotalSupplyHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -155,15 +148,15 @@
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+) -> TokenTotalSupplyHistoricalResponse:
     """Get historical total supply
 
      Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -172,19 +165,19 @@
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[TokenTotalSupplyHistoricalResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -205,15 +198,15 @@
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+) -> Response[TokenTotalSupplyHistoricalResponse]:
     """Get historical total supply
 
      Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -222,19 +215,19 @@
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[TokenTotalSupplyHistoricalResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         start_block_number=start_block_number,
@@ -260,15 +253,15 @@
     end_block_number: Union[Unset, None, float] = UNSET,
     block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
     time_interval: Union[Unset, None, float] = UNSET,
     scaled: Union[Unset, None, bool] = True,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]:
+) -> TokenTotalSupplyHistoricalResponse:
     """Get historical total supply
 
      Returns historical total supply for a token.
 
     Args:
         chain_id (float):
         token_address (str):
@@ -277,19 +270,19 @@
         block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
         time_interval (Union[Unset, None, float]):
         scaled (Union[Unset, None, bool]):  Default: True.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]]
+        Response[TokenTotalSupplyHistoricalResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_volume.py` & `credmark-1.2.0/credmark/api/token_api/get_token_holders_count_historical.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,274 +1,282 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_volume_response import TokenVolumeResponse
+from ...models.token_historical_holders_count_response import TokenHistoricalHoldersCountResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/holders/count/historical".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["scaled"] = scaled
-
     params["startBlockNumber"] = start_block_number
 
     params["endBlockNumber"] = end_block_number
 
+    params["blockInterval"] = block_interval
+
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
+    params["timeInterval"] = time_interval
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenHistoricalHoldersCountResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenVolumeResponse.from_dict(response.json())
+        response_200 = TokenHistoricalHoldersCountResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenHistoricalHoldersCountResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     chain_id: float,
     token_address: str,
     *,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+) -> Response[TokenHistoricalHoldersCountResponse]:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        time_interval=time_interval,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     chain_id: float,
     token_address: str,
     *,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+) -> TokenHistoricalHoldersCountResponse:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        time_interval=time_interval,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+) -> Response[TokenHistoricalHoldersCountResponse]:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
-        scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
+        block_interval=block_interval,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
+        time_interval=time_interval,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     chain_id: float,
     token_address: str,
     *,
-    scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
+    block_interval: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
+    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenVolumeResponse]]:
-    """Get token volume
+) -> TokenHistoricalHoldersCountResponse:
+    """Get historical total number of token holders
 
-     Returns traded volume for a token over a period of blocks or time.
+     Returns historical total number of holders of a token at a block or time.
 
     Args:
         chain_id (float):
         token_address (str):
-        scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
+        block_interval (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
+        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeResponse]]
+        Response[TokenHistoricalHoldersCountResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
-            scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
+            block_interval=block_interval,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
+            time_interval=time_interval,
         )
     ).parsed
```

### Comparing `credmark-1.1.0/credmark/api/token_api/get_token_volume_historical.py` & `credmark-1.2.0/credmark/api/token_api/get_token_volume.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import Dict, Optional, Union
+from typing import Dict, Union
 
 from ... import errors
 from ...models.token_error_response import TokenErrorResponse
-from ...models.token_volume_historical_response import TokenVolumeHistoricalResponse
+from ...models.token_volume_response import TokenVolumeResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     chain_id: float,
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
 ) -> Dict[str, Any]:
-    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume/historical".format(
+    url = "{}/v1/tokens/{chainId}/{tokenAddress}/volume".format(
         client.base_url, chainId=chain_id, tokenAddress=token_address
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -41,51 +39,40 @@
 
     params["endBlockNumber"] = end_block_number
 
     params["startTimestamp"] = start_timestamp
 
     params["endTimestamp"] = end_timestamp
 
-    params["blockInterval"] = block_interval
-
-    params["timeInterval"] = time_interval
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> TokenVolumeResponse:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TokenVolumeHistoricalResponse.from_dict(response.json())
+        response_200 = TokenVolumeResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = TokenErrorResponse.from_dict(response.json())
 
-        return response_400
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+        raise errors.CredmarkError(response.status_code, response.content, response_400)
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
-def _build_response(
-    *, client: "Credmark", response: httpx.Response
-) -> Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
+def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[TokenVolumeResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -95,52 +82,46 @@
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+) -> Response[TokenVolumeResponse]:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
         scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[TokenVolumeResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
-        time_interval=time_interval,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
@@ -152,102 +133,90 @@
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+) -> TokenVolumeResponse:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
         scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[TokenVolumeResponse]
     """
 
     return sync_detailed(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
-        time_interval=time_interval,
     ).parsed
 
 
 async def asyncio_detailed(
     chain_id: float,
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+) -> Response[TokenVolumeResponse]:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
         scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[TokenVolumeResponse]
     """
 
     kwargs = _get_kwargs(
         chain_id=chain_id,
         token_address=token_address,
         client=client,
         scaled=scaled,
         start_block_number=start_block_number,
         end_block_number=end_block_number,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
-        block_interval=block_interval,
-        time_interval=time_interval,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
@@ -257,48 +226,42 @@
     token_address: str,
     *,
     scaled: Union[Unset, None, bool] = True,
     start_block_number: Union[Unset, None, float] = UNSET,
     end_block_number: Union[Unset, None, float] = UNSET,
     start_timestamp: Union[Unset, None, float] = UNSET,
     end_timestamp: Union[Unset, None, float] = UNSET,
-    block_interval: Union[Unset, None, float] = UNSET,
-    time_interval: Union[Unset, None, float] = UNSET,
     client: "Credmark",
-) -> Optional[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]:
-    """Get historical volume
+) -> TokenVolumeResponse:
+    """Get token volume
 
-     Returns traded volume for a token over a period of blocks or time divided by intervals.
+     Returns traded volume for a token over a period of blocks or time.
 
     Args:
         chain_id (float):
         token_address (str):
         scaled (Union[Unset, None, bool]):  Default: True.
         start_block_number (Union[Unset, None, float]):
         end_block_number (Union[Unset, None, float]):
         start_timestamp (Union[Unset, None, float]):
         end_timestamp (Union[Unset, None, float]):
-        block_interval (Union[Unset, None, float]):
-        time_interval (Union[Unset, None, float]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[TokenErrorResponse, TokenVolumeHistoricalResponse]]
+        Response[TokenVolumeResponse]
     """
 
     return (
         await asyncio_detailed(
             chain_id=chain_id,
             token_address=token_address,
             client=client,
             scaled=scaled,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
-            block_interval=block_interval,
-            time_interval=time_interval,
         )
     ).parsed
```

### Comparing `credmark-1.1.0/credmark/api/utilities/__init__.py` & `credmark-1.2.0/credmark/api/utilities/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import Dict, List, Optional, Union, cast
 
 from ...models.check_health_response_200 import CheckHealthResponse200
@@ -13,64 +13,64 @@
 
 class Utilities:
     def __init__(self, client: "Credmark"):
         self.__client = client
 
     def check_health(
         self,
-    ) -> Optional[Union[CheckHealthResponse200, CheckHealthResponse503]]:
+    ) -> CheckHealthResponse200:
         """Healthcheck status
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[CheckHealthResponse200, CheckHealthResponse503]]
+            Response[CheckHealthResponse200]
         """
 
         return check_health.sync(
             client=self.__client,
         )
 
     async def check_health_async(
         self,
-    ) -> Optional[Union[CheckHealthResponse200, CheckHealthResponse503]]:
+    ) -> CheckHealthResponse200:
         """Healthcheck status
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[Union[CheckHealthResponse200, CheckHealthResponse503]]
+            Response[CheckHealthResponse200]
         """
 
         return await check_health.asyncio(
             client=self.__client,
         )
 
     def get_daily_model_usage(
         self,
         *,
         days: Union[Unset, None, float] = UNSET,
         group_by: Union[Unset, None, str] = UNSET,
         requester: Union[Unset, None, str] = UNSET,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> List[Dict[str, Any]]:
         """Model Request statistics
 
          Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
         Args:
             days (Union[Unset, None, float]):
             group_by (Union[Unset, None, str]):
             requester (Union[Unset, None, str]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
         """
 
         return get_daily_model_usage.sync(
@@ -82,26 +82,26 @@
 
     async def get_daily_model_usage_async(
         self,
         *,
         days: Union[Unset, None, float] = UNSET,
         group_by: Union[Unset, None, str] = UNSET,
         requester: Union[Unset, None, str] = UNSET,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> List[Dict[str, Any]]:
         """Model Request statistics
 
          Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
         Args:
             days (Union[Unset, None, float]):
             group_by (Union[Unset, None, str]):
             requester (Union[Unset, None, str]):
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
         """
 
         return await get_daily_model_usage.asyncio(
@@ -109,78 +109,78 @@
             days=days,
             group_by=group_by,
             requester=requester,
         )
 
     def get_top_models(
         self,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> List[Dict[str, Any]]:
         """Top Used Models
 
          Returns a list of the top used models.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
         """
 
         return get_top_models.sync(
             client=self.__client,
         )
 
     async def get_top_models_async(
         self,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> List[Dict[str, Any]]:
         """Top Used Models
 
          Returns a list of the top used models.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
         """
 
         return await get_top_models.asyncio(
             client=self.__client,
         )
 
     def get_total_model_usage(
         self,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> List[Dict[str, Any]]:
         """Total Model Usage
 
          Returns a count of model runs.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
         """
 
         return get_total_model_usage.sync(
             client=self.__client,
         )
 
     async def get_total_model_usage_async(
         self,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> List[Dict[str, Any]]:
         """Total Model Usage
 
          Returns a count of model runs.
 
         Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            errors.CredmarkError: If the server returns a non 2xx status code.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
             Response[List[Dict[str, Any]]]
         """
 
         return await get_total_model_usage.asyncio(
```

### Comparing `credmark-1.1.0/credmark/api/utilities/get_daily_model_usage.py` & `credmark-1.2.0/credmark/api/utilities/get_daily_model_usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Union, cast
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
-from typing import List, Optional, Union, cast
+from typing import List, Union, cast
 
 from ... import errors
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -40,23 +40,20 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List[Dict[str, Any]]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> List[Dict[str, Any]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = cast(List[Dict[str, Any]], response.json())
 
         return response_200
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
 def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List[Dict[str, Any]]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
@@ -77,15 +74,15 @@
 
     Args:
         days (Union[Unset, None, float]):
         group_by (Union[Unset, None, str]):
         requester (Union[Unset, None, str]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     kwargs = _get_kwargs(
@@ -105,26 +102,26 @@
 
 def sync(
     *,
     days: Union[Unset, None, float] = UNSET,
     group_by: Union[Unset, None, str] = UNSET,
     requester: Union[Unset, None, str] = UNSET,
     client: "Credmark",
-) -> Optional[List[Dict[str, Any]]]:
+) -> List[Dict[str, Any]]:
     """Model Request statistics
 
      Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
         days (Union[Unset, None, float]):
         group_by (Union[Unset, None, str]):
         requester (Union[Unset, None, str]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     return sync_detailed(
@@ -148,15 +145,15 @@
 
     Args:
         days (Union[Unset, None, float]):
         group_by (Union[Unset, None, str]):
         requester (Union[Unset, None, str]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     kwargs = _get_kwargs(
@@ -174,26 +171,26 @@
 
 async def asyncio(
     *,
     days: Union[Unset, None, float] = UNSET,
     group_by: Union[Unset, None, str] = UNSET,
     requester: Union[Unset, None, str] = UNSET,
     client: "Credmark",
-) -> Optional[List[Dict[str, Any]]]:
+) -> List[Dict[str, Any]]:
     """Model Request statistics
 
      Returns a list of daily model request statistics, either for a specific requester or for everyone.
 
     Args:
         days (Union[Unset, None, float]):
         group_by (Union[Unset, None, str]):
         requester (Union[Unset, None, str]):
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     return (
```

### Comparing `credmark-1.1.0/credmark/api/utilities/get_total_model_usage.py` & `credmark-1.2.0/credmark/api/utilities/get_top_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, cast
+from typing import TYPE_CHECKING, Any, Dict, List, cast
 
 import httpx
 
 if TYPE_CHECKING:
     from ...client import Credmark
 
 from typing import List, cast
 
 from ... import errors
 from ...types import Response
 
 
 def _get_kwargs(client: "Credmark") -> Dict[str, Any]:
-    url = "{}/v1/usage/total".format(client.base_url)
+    url = "{}/v1/usage/top".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: "Credmark", response: httpx.Response) -> Optional[List[Dict[str, Any]]]:
+def _parse_response(*, client: "Credmark", response: httpx.Response) -> List[Dict[str, Any]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = cast(List[Dict[str, Any]], response.json())
 
         return response_200
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
+    raise errors.CredmarkError(response.status_code, response.content)
 
 
 def _build_response(*, client: "Credmark", response: httpx.Response) -> Response[List[Dict[str, Any]]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(client: "Credmark") -> Response[List[Dict[str, Any]]]:
-    """Total Model Usage
+    """Top Used Models
 
-     Returns a count of model runs.
+     Returns a list of the top used models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     kwargs = _get_kwargs(
@@ -69,39 +66,39 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(client: "Credmark") -> Optional[List[Dict[str, Any]]]:
-    """Total Model Usage
+def sync(client: "Credmark") -> List[Dict[str, Any]]:
+    """Top Used Models
 
-     Returns a count of model runs.
+     Returns a list of the top used models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(client: "Credmark") -> Response[List[Dict[str, Any]]]:
-    """Total Model Usage
+    """Top Used Models
 
-     Returns a count of model runs.
+     Returns a list of the top used models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     kwargs = _get_kwargs(
@@ -110,21 +107,21 @@
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio(client: "Credmark") -> Optional[List[Dict[str, Any]]]:
-    """Total Model Usage
+async def asyncio(client: "Credmark") -> List[Dict[str, Any]]:
+    """Top Used Models
 
-     Returns a count of model runs.
+     Returns a list of the top used models.
 
     Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        errors.CredmarkError: If the server returns a non 2xx status code.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[List[Dict[str, Any]]]
     """
 
     return (
```

### Comparing `credmark-1.1.0/credmark/client.py` & `credmark-1.2.0/credmark/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,39 +16,37 @@
         headers: A dictionary of headers to be sent with every request
         timeout: The maximum amount of a time in seconds a request can take. API functions will raise
             httpx.TimeoutException if this is exceeded.
         verify_ssl: Whether or not to verify the SSL certificate of the API server. This should be True in production,
             but can be set to False for testing purposes.
         raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
             status code that was not documented in the source OpenAPI document.
-        follow_redirects: Whether or not to follow redirects. Default value is False.
+        follow_redirects: Whether or not to follow redirects. Default value is True.
     """
 
     def __init__(
         self,
         base_url: str = "https://gateway.credmark.com",
         cookies: Union[Dict[str, str], None] = None,
         headers: Union[Dict[str, str], None] = None,
-        timeout: float = 5.0,
+        timeout: float = 1800.0,
         verify_ssl: Union[str, bool, ssl.SSLContext] = True,
-        raise_on_unexpected_status: bool = False,
-        follow_redirects: bool = False,
+        follow_redirects: bool = True,
         api_key: Union[str, None] = os.getenv("CREDMARK_API_KEY"),
         prefix: str = "Bearer",
         auth_header_name: str = "Authorization",
     ):
         cookies = cookies if cookies is not None else {}
         headers = headers if headers is not None else {}
 
         self.base_url = base_url
         self.cookies = cookies
         self.headers = headers
         self.timeout = timeout
         self.verify_ssl = verify_ssl
-        self.raise_on_unexpected_status = raise_on_unexpected_status
         self.follow_redirects = follow_redirects
         self.api_key = api_key
         self.prefix = prefix
         self.auth_header_name = auth_header_name
 
         self.utilities = Utilities(client=self)
         self.defi_api = DefiApi(client=self)
```

### Comparing `credmark-1.1.0/credmark/docs/DefiApi.md` & `credmark-1.2.0/credmark/docs/DefiApi.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/ModelMetadata.md` & `credmark-1.2.0/credmark/docs/ModelMetadata.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/ModelRunResponse.md` & `credmark-1.2.0/credmark/docs/ModelRunResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/ModelRunResponseError.md` & `credmark-1.2.0/credmark/docs/ModelRunResponseError.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenAbiResponse.md` & `credmark-1.2.0/credmark/docs/TokenAbiResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenApi.md` & `credmark-1.2.0/credmark/docs/TokenApi.md`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenMetadataResponse]
+TokenMetadataResponse
 
 # **get_token_name**
 
 Get token name
 
  Returns name of a token.
 
@@ -56,15 +56,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenNameResponse]
+TokenNameResponse
 
 # **get_token_symbol**
 
 Get token symbol
 
  Returns symbol of a token.
 
@@ -75,15 +75,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenSymbolResponse]
+TokenSymbolResponse
 
 # **get_token_decimals**
 
 Get token decimals
 
  Returns decimals of a token.
 
@@ -94,15 +94,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenDecimalsResponse, TokenErrorResponse]
+TokenDecimalsResponse
 
 # **get_token_total_supply**
 
 Get token's total supply
 
  Returns total supply of a token.
 
@@ -114,15 +114,15 @@
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 scaled | bool | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenTotalSupplyResponse]
+TokenTotalSupplyResponse
 
 # **get_token_total_supply_historical**
 
 Get historical total supply
 
  Returns historical total supply for a token.
 
@@ -138,15 +138,15 @@
 start_timestamp | float | None
 end_timestamp | float | None
 time_interval | float | None
 scaled | bool | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenTotalSupplyHistoricalResponse]
+TokenTotalSupplyHistoricalResponse
 
 # **get_token_logo**
 
 Get token logo
 
  Returns logo of a token.
 
@@ -157,15 +157,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenLogoResponse]
+TokenLogoResponse
 
 # **get_token_creation_block**
 
 Get token creation block
 
  Returns creation block number of a token.
 
@@ -176,15 +176,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenCreationBlockResponse, TokenErrorResponse]
+TokenCreationBlockResponse
 
 # **get_token_abi**
 
 Get token ABI
 
  Returns ABI of a token.
 
@@ -195,15 +195,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenAbiResponse, TokenErrorResponse]
+TokenAbiResponse
 
 # **get_token_price**
 
 Get token price data
 
  Returns price data for a token.
 
@@ -217,15 +217,15 @@
 block_number | float | None
 timestamp | float | None
 src | GetTokenPriceSrc | None
 align | GetTokenPriceAlign | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenPriceResponse]
+TokenPriceResponse
 
 # **get_token_price_historical**
 
 Get historical price
 
  Returns historical price data for a token.
 
@@ -242,15 +242,15 @@
 end_timestamp | float | None
 time_interval | float | None
 quote_address | str | None
 src | GetTokenPriceHistoricalSrc | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenPriceHistoricalResponse]
+TokenPriceHistoricalResponse
 
 # **get_token_balance**
 
 Get token balance
 
  Returns token balance for an account.
 
@@ -264,15 +264,15 @@
 quote_address | str | None
 scaled | bool | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenBalanceResponse, TokenErrorResponse]
+TokenBalanceResponse
 
 # **get_token_balance_historical**
 
 Get historical balance
 
  Returns historical token balance for an account.
 
@@ -290,15 +290,15 @@
 time_interval | float | None
 account_address | str | None
 quote_address | str | None
 scaled | bool | None
 
 
 ### Response Type
-Union[TokenBalanceHistoricalResponse, TokenErrorResponse]
+TokenBalanceHistoricalResponse
 
 # **get_token_volume**
 
 Get token volume
 
  Returns traded volume for a token over a period of blocks or time.
 
@@ -312,15 +312,15 @@
 start_block_number | float | None
 end_block_number | float | None
 start_timestamp | float | None
 end_timestamp | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenVolumeResponse]
+TokenVolumeResponse
 
 # **get_token_volume_historical**
 
 Get historical volume
 
  Returns traded volume for a token over a period of blocks or time divided by intervals.
 
@@ -336,15 +336,15 @@
 start_timestamp | float | None
 end_timestamp | float | None
 block_interval | float | None
 time_interval | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenVolumeHistoricalResponse]
+TokenVolumeHistoricalResponse
 
 # **get_token_holders**
 
 Get token holders
 
  Returns holders of a token at a block or time.
 
@@ -359,15 +359,15 @@
 quote_address | str | None
 scaled | bool | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenHoldersResponse]
+TokenHoldersResponse
 
 # **get_token_holders_historical**
 
 Get token historical holders
 
  Returns historical holders of a token at a block or time.
 
@@ -385,15 +385,15 @@
 time_interval | float | None
 page_size | float | None
 quote_address | str | None
 scaled | bool | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenHoldersHistoricalResponse]
+TokenHoldersHistoricalResponse
 
 # **get_token_holders_count**
 
 Get total number of token holders
 
  Returns total number of holders of a token at a block or time.
 
@@ -404,15 +404,15 @@
 chain_id | float | None
 token_address | str | None
 block_number | float | None
 timestamp | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenHoldersCountResponse]
+TokenHoldersCountResponse
 
 # **get_token_holders_count_historical**
 
 Get historical total number of token holders
 
  Returns historical total number of holders of a token at a block or time.
 
@@ -427,9 +427,9 @@
 block_interval | float | None
 start_timestamp | float | None
 end_timestamp | float | None
 time_interval | float | None
 
 
 ### Response Type
-Union[TokenErrorResponse, TokenHistoricalHoldersCountResponse]
+TokenHistoricalHoldersCountResponse
```

### Comparing `credmark-1.1.0/credmark/docs/TokenBalanceHistoricalResponse.md` & `credmark-1.2.0/credmark/docs/TokenBalanceHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenBalanceResponse.md` & `credmark-1.2.0/credmark/docs/TokenBalanceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenHistoricalHoldersCountResponse.md` & `credmark-1.2.0/credmark/docs/TokenHistoricalHoldersCountResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenHoldersHistoricalResponse.md` & `credmark-1.2.0/credmark/docs/TokenHoldersHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenHoldersResponse.md` & `credmark-1.2.0/credmark/docs/TokenHoldersResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenPriceHistoricalResponse.md` & `credmark-1.2.0/credmark/docs/TokenPriceHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenPriceResponse.md` & `credmark-1.2.0/credmark/docs/TokenPriceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md` & `credmark-1.2.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenVolumeHistoricalResponse.md` & `credmark-1.2.0/credmark/docs/TokenVolumeHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/TokenVolumeResponse.md` & `credmark-1.2.0/credmark/docs/TokenVolumeResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/docs/Utilities.md` & `credmark-1.2.0/credmark/docs/Utilities.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # **check_health**
 
 Healthcheck status
 
 
 
 ### Response Type
-Union[CheckHealthResponse200, CheckHealthResponse503]
+CheckHealthResponse200
 
 # **get_daily_model_usage**
 
 Model Request statistics
 
  Returns a list of daily model request statistics, either for a specific requester or for everyone.
```

### Comparing `credmark-1.1.0/credmark/models/__init__.py` & `credmark-1.2.0/credmark/models/__init__.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_200.py` & `credmark-1.2.0/credmark/models/check_health_response_200.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_200_details.py` & `credmark-1.2.0/credmark/models/check_health_response_200_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_200_details_additional_property.py` & `credmark-1.2.0/credmark/models/check_health_response_200_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_200_error.py` & `credmark-1.2.0/credmark/models/check_health_response_200_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_200_error_additional_property.py` & `credmark-1.2.0/credmark/models/check_health_response_200_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_200_info.py` & `credmark-1.2.0/credmark/models/check_health_response_200_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_200_info_additional_property.py` & `credmark-1.2.0/credmark/models/check_health_response_200_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_503.py` & `credmark-1.2.0/credmark/models/check_health_response_503.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_503_details.py` & `credmark-1.2.0/credmark/models/check_health_response_503_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_503_details_additional_property.py` & `credmark-1.2.0/credmark/models/check_health_response_503_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_503_error.py` & `credmark-1.2.0/credmark/models/check_health_response_503_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_503_error_additional_property.py` & `credmark-1.2.0/credmark/models/check_health_response_503_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_503_info.py` & `credmark-1.2.0/credmark/models/check_health_response_503_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/check_health_response_503_info_additional_property.py` & `credmark-1.2.0/credmark/models/check_health_response_503_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/model_call_stack_entry.py` & `credmark-1.2.0/credmark/models/model_call_stack_entry.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/model_deployment.py` & `credmark-1.2.0/credmark/models/model_deployment.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/model_metadata.py` & `credmark-1.2.0/credmark/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/model_run_response.py` & `credmark-1.2.0/credmark/models/model_run_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/model_run_response_error.py` & `credmark-1.2.0/credmark/models/model_run_response_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/model_runtime_statistics.py` & `credmark-1.2.0/credmark/models/model_runtime_statistics.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/model_runtime_stats_response.py` & `credmark-1.2.0/credmark/models/model_runtime_stats_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/run_model_dto.py` & `credmark-1.2.0/credmark/models/run_model_dto.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_abi_response.py` & `credmark-1.2.0/credmark/models/token_abi_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_balance_historical_item.py` & `credmark-1.2.0/credmark/models/token_balance_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_balance_historical_response.py` & `credmark-1.2.0/credmark/models/token_balance_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_balance_response.py` & `credmark-1.2.0/credmark/models/token_balance_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_creation_block_response.py` & `credmark-1.2.0/credmark/models/token_creation_block_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_decimals_response.py` & `credmark-1.2.0/credmark/models/token_decimals_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_error_response.py` & `credmark-1.2.0/credmark/models/token_error_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_historical_holders_count_response.py` & `credmark-1.2.0/credmark/models/token_historical_holders_count_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_holder.py` & `credmark-1.2.0/credmark/models/token_holder.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_holders_count_historical_item.py` & `credmark-1.2.0/credmark/models/token_holders_count_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_holders_count_response.py` & `credmark-1.2.0/credmark/models/token_holders_count_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_holders_historical_item.py` & `credmark-1.2.0/credmark/models/token_holders_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_holders_historical_response.py` & `credmark-1.2.0/credmark/models/token_holders_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_holders_response.py` & `credmark-1.2.0/credmark/models/token_holders_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_logo_response.py` & `credmark-1.2.0/credmark/models/token_logo_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_metadata_response.py` & `credmark-1.2.0/credmark/models/token_metadata_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_name_response.py` & `credmark-1.2.0/credmark/models/token_name_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_price_historical_item.py` & `credmark-1.2.0/credmark/models/token_price_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_price_historical_response.py` & `credmark-1.2.0/credmark/models/token_price_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_price_response.py` & `credmark-1.2.0/credmark/models/token_price_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_symbol_response.py` & `credmark-1.2.0/credmark/models/token_symbol_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_total_supply_historical_item.py` & `credmark-1.2.0/credmark/models/token_total_supply_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_total_supply_historical_response.py` & `credmark-1.2.0/credmark/models/token_total_supply_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_total_supply_response.py` & `credmark-1.2.0/credmark/models/token_total_supply_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_volume_historical_item.py` & `credmark-1.2.0/credmark/models/token_volume_historical_item.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_volume_historical_response.py` & `credmark-1.2.0/credmark/models/token_volume_historical_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/models/token_volume_response.py` & `credmark-1.2.0/credmark/models/token_volume_response.py`

 * *Files identical despite different names*

### Comparing `credmark-1.1.0/credmark/types.py` & `credmark-1.2.0/credmark/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 @attr.s(auto_attribs=True)
 class Response(Generic[T]):
     """A response from an endpoint"""
 
     status_code: HTTPStatus
     content: bytes
     headers: MutableMapping[str, str]
-    parsed: Optional[T]
+    parsed: T
 
 
 __all__ = ["File", "Response", "FileJsonType"]
```

### Comparing `credmark-1.1.0/pyproject.toml` & `credmark-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "credmark"
-version = "1.1.0"
+version = "1.2.0"
 description = "A client library for accessing Credmark Gateway"
 license = "MIT"
 
 authors = [
   "Credmark <info@credmark.com>",
 ]
```

