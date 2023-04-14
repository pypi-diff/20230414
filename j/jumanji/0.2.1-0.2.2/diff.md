# Comparing `tmp/jumanji-0.2.1.tar.gz` & `tmp/jumanji-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jumanji-0.2.1.tar", last modified: Tue Mar 21 17:11:55 2023, max compression
+gzip compressed data, was "jumanji-0.2.2.tar", last modified: Fri Apr 14 16:56:59 2023, max compression
```

## Comparing `jumanji-0.2.1.tar` & `jumanji-0.2.2.tar`

### file list

```diff
@@ -1,206 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.305560 jumanji-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-03-21 17:11:42.000000 jumanji-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-21 17:11:42.000000 jumanji-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-03-21 17:11:55.305560 jumanji-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14597 2023-03-21 17:11:42.000000 jumanji-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.273560 jumanji-0.2.1/jumanji/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.277560 jumanji-0.2.1/jumanji/environments/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.277560 jumanji-0.2.1/jumanji/environments/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.277560 jumanji-0.2.1/jumanji/environments/commons/maze_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/commons/maze_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/commons/maze_utils/maze_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/commons/maze_utils/maze_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/commons/maze_utils/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.277560 jumanji-0.2.1/jumanji/environments/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.277560 jumanji-0.2.1/jumanji/environments/logic/game_2048/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/game_2048/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/game_2048/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/game_2048/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/game_2048/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/game_2048/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.281560 jumanji-0.2.1/jumanji/environments/logic/minesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/minesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/minesweeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/minesweeper/done.py
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/minesweeper/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/minesweeper/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/minesweeper/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/minesweeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.281560 jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.281560 jumanji-0.2.1/jumanji/environments/packing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.281560 jumanji-0.2.1/jumanji/environments/packing/bin_pack/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/bin_pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30800 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/bin_pack/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/bin_pack/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31516 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/bin_pack/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/bin_pack/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/bin_pack/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/bin_pack/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.285560 jumanji-0.2.1/jumanji/environments/packing/job_shop/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/job_shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/job_shop/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/job_shop/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/job_shop/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/job_shop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.285560 jumanji-0.2.1/jumanji/environments/packing/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/knapsack/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/knapsack/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/knapsack/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/packing/knapsack/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.285560 jumanji-0.2.1/jumanji/environments/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.285560 jumanji-0.2.1/jumanji/environments/routing/cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cleaner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cleaner/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cleaner/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cleaner/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cleaner/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.289560 jumanji-0.2.1/jumanji/environments/routing/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/connector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.289560 jumanji-0.2.1/jumanji/environments/routing/cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cvrp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cvrp/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cvrp/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cvrp/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/cvrp/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.289560 jumanji-0.2.1/jumanji/environments/routing/maze/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/maze/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/maze/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/maze/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/maze/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/maze/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.289560 jumanji-0.2.1/jumanji/environments/routing/snake/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/snake/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/snake/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.293560 jumanji-0.2.1/jumanji/environments/routing/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/tsp/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/tsp/env_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/tsp/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/environments/routing/tsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.293560 jumanji-0.2.1/jumanji/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/testing/env_not_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/testing/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/testing/pytrees.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.293560 jumanji-0.2.1/jumanji/training/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.293560 jumanji-0.2.1/jumanji/training/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.297560 jumanji-0.2.1/jumanji/training/agents/a2c/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/agents/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/agents/a2c/a2c_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/agents/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.297560 jumanji-0.2.1/jumanji/training/agents/random/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/agents/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/agents/random/random_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.297560 jumanji-0.2.1/jumanji/training/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.297560 jumanji-0.2.1/jumanji/training/networks/bin_pack/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/bin_pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/bin_pack/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/bin_pack/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.297560 jumanji-0.2.1/jumanji/training/networks/cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/cleaner/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/cleaner/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.301560 jumanji-0.2.1/jumanji/training/networks/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/connector/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/connector/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.301560 jumanji-0.2.1/jumanji/training/networks/cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/cvrp/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/cvrp/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.301560 jumanji-0.2.1/jumanji/training/networks/game_2048/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/game_2048/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/game_2048/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/game_2048/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.301560 jumanji-0.2.1/jumanji/training/networks/job_shop/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/job_shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/job_shop/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/job_shop/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.301560 jumanji-0.2.1/jumanji/training/networks/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/knapsack/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/knapsack/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/masked_categorical_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.301560 jumanji-0.2.1/jumanji/training/networks/maze/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/maze/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/maze/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.301560 jumanji-0.2.1/jumanji/training/networks/minesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/minesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/minesweeper/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/minesweeper/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/parametric_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.305560 jumanji-0.2.1/jumanji/training/networks/rubiks_cube/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/rubiks_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/rubiks_cube/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/rubiks_cube/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.305560 jumanji-0.2.1/jumanji/training/networks/snake/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/snake/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/snake/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/transformer_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.305560 jumanji-0.2.1/jumanji/training/networks/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/tsp/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/networks/tsp/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/setup_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/training/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-03-21 17:11:42.000000 jumanji-0.2.1/jumanji/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.277560 jumanji-0.2.1/jumanji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-03-21 17:11:55.000000 jumanji-0.2.1/jumanji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-03-21 17:11:55.000000 jumanji-0.2.1/jumanji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:11:55.000000 jumanji-0.2.1/jumanji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:11:55.000000 jumanji-0.2.1/jumanji.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-21 17:11:55.000000 jumanji-0.2.1/jumanji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-21 17:11:55.000000 jumanji-0.2.1/jumanji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-21 17:11:42.000000 jumanji-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:11:55.305560 jumanji-0.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-21 17:11:42.000000 jumanji-0.2.1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-21 17:11:42.000000 jumanji-0.2.1/requirements/requirements-train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-21 17:11:42.000000 jumanji-0.2.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-21 17:11:55.305560 jumanji-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-21 17:11:42.000000 jumanji-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-14 16:56:47.000000 jumanji-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 16:56:47.000000 jumanji-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-04-14 16:56:59.213251 jumanji-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-04-14 16:56:47.000000 jumanji-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/commons/maze_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/logic/game_2048/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.193250 jumanji-0.2.2/jumanji/environments/logic/minesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/done.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.193250 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.193250 jumanji-0.2.2/jumanji/environments/packing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/packing/bin_pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31516 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/packing/job_shop/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/packing/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/routing/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/maze/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/snake/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/snake/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/environments/routing/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/env_not_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/pytrees.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/agents/a2c/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/a2c/a2c_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/agents/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/random/random_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/bin_pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/bin_pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/bin_pack/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/bin_pack/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cleaner/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cleaner/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/connector/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/connector/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cvrp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cvrp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/game_2048/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/game_2048/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/game_2048/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/game_2048/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/job_shop/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/job_shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/job_shop/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/job_shop/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/knapsack/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/knapsack/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/masked_categorical_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/maze/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/maze/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/maze/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/minesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/minesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/minesweeper/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/minesweeper/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/parametric_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/snake/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/snake/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/transformer_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/tsp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/tsp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/setup_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 16:56:47.000000 jumanji-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 16:56:47.000000 jumanji-0.2.2/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 16:56:47.000000 jumanji-0.2.2/requirements/requirements-train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-14 16:56:47.000000 jumanji-0.2.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 16:56:59.217251 jumanji-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-14 16:56:47.000000 jumanji-0.2.2/setup.py
```

### Comparing `jumanji-0.2.1/LICENSE` & `jumanji-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/PKG-INFO` & `jumanji-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumanji
-Version: 0.2.1
+Version: 0.2.2
 Summary: A suite of diverse and challenging RL environments in JAX
 Home-page: https://github.com/instadeepai/jumanji/
 Author: InstaDeep
 Author-email: hello@instadeep.com
 License: Apache 2.0
 Keywords: reinforcement-learning python jax
 Classifier: Development Status :: 4 - Beta
@@ -232,32 +232,33 @@
 @software{jumanji2023github,
   author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
         and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
         Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
         and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
   title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
   url = {https://github.com/instadeepai/jumanji},
-  version = {0.2.1},
+  version = {0.2.2},
   year = {2023},
 }
 ```
 
 
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
 
 - 🤖 [Qdax](https://github.com/adaptive-intelligent-robotics/QDax) is a library to accelerate
 Quality-Diversity and neuro-evolution algorithms through hardware accelerators and parallelization.
+- 🌳 [Evojax](https://github.com/google/evojax) provides tools to enable neuroevolution algorithms
+to work with neural networks running across multiple TPU/GPUs.
 - 🦾 [Brax](https://github.com/google/brax) is a differentiable physics engine that simulates
 environments made up of rigid bodies, joints, and actuators.
 - 🏋️‍ [Gymnax](https://github.com/RobertTLange/gymnax) implements classic environments including
 classic control, bsuite, MinAtar and a collection of meta RL tasks.
-- 🌳 [Evojax](https://github.com/google/evojax) provides tools to enable neuroevolution algorithms
-to work with neural networks running across multiple TPU/GPUs.
-
+- 🎲 [Pgx](https://github.com/sotetsuk/pgx) provides classic board game environments like
+Backgammon, Shogi, and Go.
 
 ## Acknowledgements 🙏
 
 The development of this library was supported with Cloud TPUs
 from Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC) 🌤.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jumanji Version: 0.2.1 Summary: A suite of diverse
+Metadata-Version: 2.1 Name: jumanji Version: 0.2.2 Summary: A suite of diverse
 and challenging RL environments in JAX Home-page: https://github.com/
 instadeepai/jumanji/ Author: InstaDeep Author-email: hello@instadeep.com
 License: Apache 2.0 Keywords: reinforcement-learning python jax Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -164,22 +164,24 @@
 guidelines. ## Citing Jumanji âï¸ If you use Jumanji in your work, please
 cite the library using: ``` @software{jumanji2023github, author = {ClÃ©ment
 Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz and Vincent Coyette
 and Paul Duckworth and Daniel Furelos-Blanco and Nathan Grinsztajn and Tristan
 Kalloniatis and Victor Le and Omayma Mahjoub and Laurence Midgley and Shikha
 Surana and Cemlyn Waters and Alexandre Laterre}, title = {Jumanji: a Suite of
 Diverse and Challenging Reinforcement Learning Environments in JAX}, url =
-{https://github.com/instadeepai/jumanji}, version = {0.2.1}, year = {2023}, }
+{https://github.com/instadeepai/jumanji}, version = {0.2.2}, year = {2023}, }
 ``` ## See Also ð Other works have embraced the approach of writing RL
 environments in JAX. In particular, we suggest users check out the following
 sister repositories: - ð¤ [Qdax](https://github.com/adaptive-intelligent-
 robotics/QDax) is a library to accelerate Quality-Diversity and neuro-evolution
-algorithms through hardware accelerators and parallelization. - ð¦¾ [Brax]
-(https://github.com/google/brax) is a differentiable physics engine that
-simulates environments made up of rigid bodies, joints, and actuators. -
+algorithms through hardware accelerators and parallelization. - ð³ [Evojax]
+(https://github.com/google/evojax) provides tools to enable neuroevolution
+algorithms to work with neural networks running across multiple TPU/GPUs. -
+ð¦¾ [Brax](https://github.com/google/brax) is a differentiable physics engine
+that simulates environments made up of rigid bodies, joints, and actuators. -
 ðï¸â [Gymnax](https://github.com/RobertTLange/gymnax) implements classic
 environments including classic control, bsuite, MinAtar and a collection of
-meta RL tasks. - ð³ [Evojax](https://github.com/google/evojax) provides tools
-to enable neuroevolution algorithms to work with neural networks running across
-multiple TPU/GPUs. ## Acknowledgements ð The development of this library was
-supported with Cloud TPUs from Google's [TPU Research Cloud](https://
-sites.research.google/trc/about/) (TRC) ð¤.
+meta RL tasks. - ð² [Pgx](https://github.com/sotetsuk/pgx) provides classic
+board game environments like Backgammon, Shogi, and Go. ## Acknowledgements
+ð The development of this library was supported with Cloud TPUs from
+Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC)
+ð¤.
```

### Comparing `jumanji-0.2.1/README.md` & `jumanji-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -207,32 +207,33 @@
 @software{jumanji2023github,
   author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
         and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
         Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
         and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
   title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
   url = {https://github.com/instadeepai/jumanji},
-  version = {0.2.1},
+  version = {0.2.2},
   year = {2023},
 }
 ```
 
 
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
 
 - 🤖 [Qdax](https://github.com/adaptive-intelligent-robotics/QDax) is a library to accelerate
 Quality-Diversity and neuro-evolution algorithms through hardware accelerators and parallelization.
+- 🌳 [Evojax](https://github.com/google/evojax) provides tools to enable neuroevolution algorithms
+to work with neural networks running across multiple TPU/GPUs.
 - 🦾 [Brax](https://github.com/google/brax) is a differentiable physics engine that simulates
 environments made up of rigid bodies, joints, and actuators.
 - 🏋️‍ [Gymnax](https://github.com/RobertTLange/gymnax) implements classic environments including
 classic control, bsuite, MinAtar and a collection of meta RL tasks.
-- 🌳 [Evojax](https://github.com/google/evojax) provides tools to enable neuroevolution algorithms
-to work with neural networks running across multiple TPU/GPUs.
-
+- 🎲 [Pgx](https://github.com/sotetsuk/pgx) provides classic board game environments like
+Backgammon, Shogi, and Go.
 
 ## Acknowledgements 🙏
 
 The development of this library was supported with Cloud TPUs
 from Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC) 🌤.
```

#### html2text {}

```diff
@@ -151,22 +151,24 @@
 guidelines. ## Citing Jumanji âï¸ If you use Jumanji in your work, please
 cite the library using: ``` @software{jumanji2023github, author = {ClÃ©ment
 Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz and Vincent Coyette
 and Paul Duckworth and Daniel Furelos-Blanco and Nathan Grinsztajn and Tristan
 Kalloniatis and Victor Le and Omayma Mahjoub and Laurence Midgley and Shikha
 Surana and Cemlyn Waters and Alexandre Laterre}, title = {Jumanji: a Suite of
 Diverse and Challenging Reinforcement Learning Environments in JAX}, url =
-{https://github.com/instadeepai/jumanji}, version = {0.2.1}, year = {2023}, }
+{https://github.com/instadeepai/jumanji}, version = {0.2.2}, year = {2023}, }
 ``` ## See Also ð Other works have embraced the approach of writing RL
 environments in JAX. In particular, we suggest users check out the following
 sister repositories: - ð¤ [Qdax](https://github.com/adaptive-intelligent-
 robotics/QDax) is a library to accelerate Quality-Diversity and neuro-evolution
-algorithms through hardware accelerators and parallelization. - ð¦¾ [Brax]
-(https://github.com/google/brax) is a differentiable physics engine that
-simulates environments made up of rigid bodies, joints, and actuators. -
+algorithms through hardware accelerators and parallelization. - ð³ [Evojax]
+(https://github.com/google/evojax) provides tools to enable neuroevolution
+algorithms to work with neural networks running across multiple TPU/GPUs. -
+ð¦¾ [Brax](https://github.com/google/brax) is a differentiable physics engine
+that simulates environments made up of rigid bodies, joints, and actuators. -
 ðï¸â [Gymnax](https://github.com/RobertTLange/gymnax) implements classic
 environments including classic control, bsuite, MinAtar and a collection of
-meta RL tasks. - ð³ [Evojax](https://github.com/google/evojax) provides tools
-to enable neuroevolution algorithms to work with neural networks running across
-multiple TPU/GPUs. ## Acknowledgements ð The development of this library was
-supported with Cloud TPUs from Google's [TPU Research Cloud](https://
-sites.research.google/trc/about/) (TRC) ð¤.
+meta RL tasks. - ð² [Pgx](https://github.com/sotetsuk/pgx) provides classic
+board game environments like Backgammon, Shogi, and Go. ## Acknowledgements
+ð The development of this library was supported with Cloud TPUs from
+Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC)
+ð¤.
```

### Comparing `jumanji-0.2.1/jumanji/__init__.py` & `jumanji-0.2.2/jumanji/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from jumanji.env import Environment
+from jumanji.environments.logic.rubiks_cube import generator as rubik_generator
 from jumanji.registration import make, register, registered_environments
 from jumanji.version import __version__
 
 """Environment Registration"""
 
 ###
 # Logic Environments
@@ -28,18 +29,21 @@
 # Minesweeper on a board of size 10x10 with 10 mines.
 register(id="Minesweeper-v0", entry_point="jumanji.environments:Minesweeper")
 
 # RubiksCube - the standard Rubik's Cube puzzle with faces of size 3x3.
 register(id="RubiksCube-v0", entry_point="jumanji.environments:RubiksCube")
 # RubiksCube - an easier version of the standard Rubik's Cube puzzle with faces of size 3x3 yet only
 # 7 scrambles at reset time, making it technically maximum 7 actions away from the solution.
+partly_scrambled_rubiks_cube_generator = rubik_generator.ScramblingGenerator(
+    cube_size=3, num_scrambles_on_reset=7
+)
 register(
     id="RubiksCube-partly-scrambled-v0",
     entry_point="jumanji.environments:RubiksCube",
-    kwargs={"cube_size": 3, "time_limit": 20, "num_scrambles_on_reset": 7},
+    kwargs={"time_limit": 20, "generator": partly_scrambled_rubiks_cube_generator},
 )
 
 
 ###
 # Packing Environments
 ###
```

### Comparing `jumanji-0.2.1/jumanji/env.py` & `jumanji-0.2.2/jumanji/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/__init__.py` & `jumanji-0.2.2/jumanji/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/commons/__init__.py` & `jumanji-0.2.2/jumanji/environments/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/commons/maze_utils/__init__.py` & `jumanji-0.2.2/jumanji/environments/commons/maze_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/commons/maze_utils/maze_generation.py` & `jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_generation.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,80 +37,77 @@
 wall must be at an even x coordinate.
 """
 from typing import NamedTuple, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
-from typing_extensions import TypeAlias
 
 from jumanji.environments.commons.maze_utils.stack import (
     Stack,
     create_stack,
     empty_stack,
     stack_pop,
     stack_push,
 )
 
-Maze: TypeAlias = chex.Array
-
 EMPTY = 0
 WALL = 1
 
 
 class MazeGenerationState(NamedTuple):
     """The state of the maze generation.
 
     - maze: the maze containing the walls created so far.
     - chambers: the stack of remaining chambers to split.
     - key: the Jax random generation key.
     """
 
-    maze: Maze
+    maze: chex.Array
     chambers: Stack
     key: chex.PRNGKey
 
 
 def create_chambers_stack(maze_width: int, maze_height: int) -> Stack:
     """Initialize the stack of chambers."""
     max_num_chamber = maze_width * maze_height
     # A chamber is defined by 4 digits: x0, y0, width, height
     chambers = create_stack(max_num_chamber, 4)
     # Initially only one chamber: the whole maze
     return stack_push(chambers, jnp.array([0, 0, maze_width, maze_height]))
 
 
-def create_empty_maze(width: int, height: int) -> Maze:
+def create_empty_maze(width: int, height: int) -> chex.Array:
     """Create an empty maze."""
     return jnp.full((height, width), EMPTY, dtype=jnp.int8)
 
 
 def random_even(key: chex.PRNGKey, max_val: int) -> chex.Array:
     """Randomly draw an even integer between 0 (inclusive) and max_val (exclusive)."""
     return jax.random.randint(key, (), 0, (max_val + 1) // 2) * 2
 
 
 def random_odd(key: chex.PRNGKey, max_val: int) -> chex.Array:
     """Randomly draw an odd integer between 0 (inclusive) and max_val (exclusive)."""
     return jax.random.randint(key, (), 0, max_val // 2) * 2 + 1
 
 
-def draw_horizontal_wall(maze: Maze, x: int, y: int, width: int) -> Maze:
+def draw_horizontal_wall(maze: chex.Array, x: int, y: int, width: int) -> chex.Array:
     """Draw a horizontal wall on the maze starting from (x,y) with the specified width."""
 
-    def body_fun(i: int, maze: Maze) -> Maze:
+    def body_fun(i: int, maze: chex.Array) -> chex.Array:
         return maze.at[y, i].set(WALL)
 
     return jax.lax.fori_loop(x, x + width, body_fun, maze)
 
 
-def draw_vertical_wall(maze: Maze, x: int, y: int, height: int) -> Maze:
+def draw_vertical_wall(maze: chex.Array, x: int, y: int, height: int) -> chex.Array:
     """Draw a vertical wall on the maze starting from (x,y) with the specified height."""
 
-    def body_fun(i: int, maze: Maze) -> Maze:
+    def body_fun(i: int, maze: chex.Array) -> chex.Array:
         return maze.at[i, x].set(WALL)
 
     return jax.lax.fori_loop(y, y + height, body_fun, maze)
 
 
 def create_chamber(chambers: Stack, x: int, y: int, width: int, height: int) -> Stack:
     """Create a new chamber from (x,y) and a given width and height.
@@ -152,15 +149,15 @@
     maze = maze.at[wall_y, x + passage_x].set(EMPTY)
 
     return MazeGenerationState(maze, chambers, key)
 
 
 def split_horizontally(
     state: MazeGenerationState, chamber: chex.Array
-) -> Tuple[Maze, Stack, chex.PRNGKey]:
+) -> Tuple[chex.Array, Stack, chex.PRNGKey]:
     """Split the chamber horizontally.
 
     Randomly draw a vertical wall to split the chamber horizontally. Randomly open a passage
     within this wall, and push the two newly created sub-chambers to the stack if they are not
     of minimum size.
     """
     x, y, width, height = chamber
@@ -198,15 +195,15 @@
 
 
 def chambers_remaining(state: MazeGenerationState) -> int:
     """Check if there is any chamber remaining to split."""
     return ~empty_stack(state.chambers)
 
 
-def generate_maze(width: int, height: int, key: chex.PRNGKey) -> Maze:
+def generate_maze(width: int, height: int, key: chex.PRNGKey) -> chex.Array:
     """Randomly generate a maze.
 
     Args:
         width: the number of rows of the maze to create.
         height: the number of columns of the maze to create.
         key: the Jax random number generation key.
```

### Comparing `jumanji-0.2.1/jumanji/environments/commons/maze_utils/maze_rendering.py` & `jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_rendering.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Callable, Optional, Sequence, Tuple
 
+import chex
 import matplotlib.animation
 import matplotlib.cm
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import image
 from matplotlib.axes import Axes
 from numpy.typing import NDArray
 
 import jumanji.environments
-from jumanji.environments.commons.maze_utils.maze_generation import EMPTY, WALL, Maze
+from jumanji.environments.commons.maze_utils.maze_generation import EMPTY, WALL
+from jumanji.viewer import Viewer
 
 
-class MazeViewer:
+class MazeViewer(Viewer):
     FONT_STYLE = "monospace"
     FIGURE_SIZE = (10.0, 10.0)
     # EMPTY is white, WALL is black
     COLORS = {EMPTY: [1, 1, 1], WALL: [0, 0, 0]}
 
     def __init__(self, name: str, render_mode: str = "human") -> None:
-        """
-        Viewer for a maze environment.
+        """Viewer for a maze environment.
 
         Args:
             name: the window name to be used when initialising the window.
             render_mode: the mode used to render the environment. Must be one of:
                 - "human": render the environment on screen.
                 - "rgb_array": return a numpy array frame representing the environment.
         """
@@ -51,15 +52,15 @@
         if render_mode == "rgb_array":
             self._display = self._display_rgb_array
         elif render_mode == "human":
             self._display = self._display_human
         else:
             raise ValueError(f"Invalid render mode: {render_mode}")
 
-    def render(self, maze: Maze) -> Optional[NDArray]:
+    def render(self, maze: chex.Array) -> Optional[NDArray]:
         """
         Render maze.
 
         Args:
             maze: the maze to render.
 
         Returns:
@@ -69,15 +70,15 @@
         fig, ax = self._get_fig_ax()
         ax.clear()
         self._add_grid_image(maze, ax)
         return self._display(fig)
 
     def animate(
         self,
-        mazes: Sequence[Maze],
+        mazes: Sequence[chex.Array],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
         """Create an animation from a sequence of mazes.
 
         Args:
             mazes: sequence of `Maze` corresponding to consecutive timesteps.
@@ -120,20 +121,20 @@
             if not plt.isinteractive():
                 fig.show()
             ax = fig.add_subplot()
         else:
             ax = fig.get_axes()[0]
         return fig, ax
 
-    def _add_grid_image(self, maze: Maze, ax: Axes) -> image.AxesImage:
+    def _add_grid_image(self, maze: chex.Array, ax: Axes) -> image.AxesImage:
         img = self._create_grid_image(maze)
         ax.set_axis_off()
         return ax.imshow(img)
 
-    def _create_grid_image(self, maze: Maze) -> NDArray:
+    def _create_grid_image(self, maze: chex.Array) -> NDArray:
         img = np.zeros((*maze.shape, 3))
         for tile_value, color in self.COLORS.items():
             img[np.where(maze == tile_value)] = color
         # Draw black frame around maze by padding axis 0 and 1
         img = np.pad(img, ((1, 1), (1, 1), (0, 0)))  # type: ignore
         return img
```

### Comparing `jumanji-0.2.1/jumanji/environments/commons/maze_utils/stack.py` & `jumanji-0.2.2/jumanji/environments/commons/maze_utils/stack.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/__init__.py` & `jumanji-0.2.2/jumanji/environments/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/game_2048/__init__.py` & `jumanji-0.2.2/jumanji/environments/logic/game_2048/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/game_2048/env.py` & `jumanji-0.2.2/jumanji/environments/logic/game_2048/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 
 from typing import Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import matplotlib.animation as animation
+from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.logic.game_2048.env_viewer import Game2048Viewer
 from jumanji.environments.logic.game_2048.types import Board, Observation, State
 from jumanji.environments.logic.game_2048.utils import (
     move_down,
     move_left,
     move_right,
     move_up,
 )
+from jumanji.environments.logic.game_2048.viewer import Game2048Viewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
 class Game2048(Environment[State]):
     """Environment for the game 2048. The game consists of a board of size board_size x board_size
     (4x4 by default) in which the player can take actions to move the tiles on the board up, down,
     left, or right. The goal of the game is to combine tiles with the same number to create a tile
     with twice the value, until the player at least creates a tile with the value 2048 to consider
@@ -74,24 +76,27 @@
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
-    def __init__(self, board_size: int = 4) -> None:
+    def __init__(
+        self, board_size: int = 4, viewer: Optional[Viewer[State]] = None
+    ) -> None:
         """Initialize the 2048 game.
 
         Args:
             board_size: size of the board. Defaults to 4.
+            viewer: `Viewer` used for rendering. Defaults to `Game2048Viewer`.
         """
         self.board_size = board_size
 
         # Create viewer used for rendering
-        self._env_viewer = Game2048Viewer("2048", board_size)
+        self._viewer = viewer or Game2048Viewer("2048", board_size)
 
     def __repr__(self) -> str:
         """String representation of the environment.
 
         Returns:
             str: the string representation of the environment.
         """
@@ -304,23 +309,21 @@
                 jnp.any(move_right(board, final_shift=False)[0] != board),
                 jnp.any(move_down(board, final_shift=False)[0] != board),
                 jnp.any(move_left(board, final_shift=False)[0] != board),
             ],
         )
         return action_mask
 
-    def render(self, state: State, save_path: Optional[str] = None) -> None:
+    def render(self, state: State) -> Optional[NDArray]:
         """Renders the current state of the game board.
 
         Args:
             state: is the current game state to be rendered.
-            save_path: the path where the image should be saved. If it is None, the plot
-            will not be stored.
         """
-        return self._env_viewer.render(state=state, save_path=save_path)
+        return self._viewer.render(state=state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> animation.FuncAnimation:
@@ -331,18 +334,18 @@
             interval: the delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
             will not be stored.
 
         Returns:
             animation.FuncAnimation: the animation object that was created.
         """
-        return self._env_viewer.animate(
+        return self._viewer.animate(
             states=states, interval=interval, save_path=save_path
         )
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self._env_viewer.close()
+        self._viewer.close()
```

### Comparing `jumanji-0.2.1/jumanji/environments/logic/game_2048/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/logic/game_2048/viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 
 import jax.numpy as jnp
 import matplotlib.animation
 import matplotlib.pyplot as plt
 
 import jumanji.environments
 from jumanji.environments.logic.game_2048.types import State
+from jumanji.viewer import Viewer
 
 
-class Game2048Viewer:
+class Game2048Viewer(Viewer):
     COLORS = {
         1: "#ccc0b3",
         2: "#eee4da",
         4: "#ede0c8",
         8: "#f59563",
         16: "#f59563",
         32: "#f67c5f",
@@ -60,33 +61,27 @@
         self._name = name
         self._board_size = board_size
 
         # The animation must be stored in a variable that lives as long as the
         # animation should run. Otherwise, the animation will get garbage-collected.
         self._animation: Optional[matplotlib.animation.Animation] = None
 
-    def render(self, state: State, save_path: Optional[str] = None) -> None:
+    def render(self, state: State) -> None:
         """Renders the current state of the game board.
 
         Args:
             state: is the current game state to be rendered.
-            save_path: the path where the image should be saved. If it is None, the plot
-            will not be stored.
         """
         self._clear_display()
         # Get the figure and axes for the game board.
         fig, ax = self.get_fig_ax()
         # Set the figure title to display the current score.
         fig.suptitle(f"2048    Score: {int(state.score)}", size=20)
         # Draw the game board
         self.draw_board(ax, state)
-        # Save the figure as an image file.
-        if save_path:
-            fig.savefig(save_path, bbox_inches="tight", pad_inches=0.5)
-
         self._display_human(fig)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
```

### Comparing `jumanji-0.2.1/jumanji/environments/logic/game_2048/types.py` & `jumanji-0.2.2/jumanji/environments/logic/game_2048/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/game_2048/utils.py` & `jumanji-0.2.2/jumanji/environments/logic/game_2048/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/minesweeper/__init__.py` & `jumanji-0.2.2/jumanji/environments/logic/minesweeper/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/minesweeper/constants.py` & `jumanji-0.2.2/jumanji/environments/logic/minesweeper/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 UNEXPLORED_ID: int = -1
 IS_MINE: int = 1
 PATCH_SIZE: int = 3
-REVEALED_EMPTY_SQUARE_REWARD: float = 1.0
-REVEALED_MINE_OR_INVALID_ACTION_REWARD: float = 0.0
-COLOUR_MAPPING: list = [
+DEFAULT_COLOR_MAPPING: list = [
     "orange",
     "blue",
     "green",
     "red",
     "purple",
     "maroon",
     "teal",
```

### Comparing `jumanji-0.2.1/jumanji/environments/logic/minesweeper/done.py` & `jumanji-0.2.2/jumanji/environments/logic/minesweeper/done.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/minesweeper/env.py` & `jumanji-0.2.2/jumanji/environments/routing/maze/env.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,398 +8,349 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import List, Optional, Sequence, Tuple
+from typing import Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import matplotlib.animation
-import matplotlib.pyplot as plt
+from numpy.typing import NDArray
 
-import jumanji.environments
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.logic.minesweeper.constants import (
-    COLOUR_MAPPING,
-    PATCH_SIZE,
-    UNEXPLORED_ID,
-)
-from jumanji.environments.logic.minesweeper.done import DefaultDoneFn, DoneFn
-from jumanji.environments.logic.minesweeper.reward import DefaultRewardFn, RewardFn
-from jumanji.environments.logic.minesweeper.types import Observation, State
-from jumanji.environments.logic.minesweeper.utils import (
-    count_adjacent_mines,
-    create_flat_mine_locations,
-    explored_mine,
-)
+from jumanji.environments.routing.maze.constants import MOVES
+from jumanji.environments.routing.maze.generator import Generator, RandomGenerator
+from jumanji.environments.routing.maze.types import Observation, Position, State
+from jumanji.environments.routing.maze.viewer import MazeEnvViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
-class Minesweeper(Environment[State]):
-    """A JAX implementation of the minesweeper game.
-
-    - observation: `Observation`
-        - board: jax array (int32) of shape (num_rows, num_cols):
-            each cell contains -1 if not yet explored, or otherwise the number of mines in
-            the 8 adjacent squares.
-        - action_mask: jax array (bool) of shape (num_rows, num_cols):
-            indicates which actions are valid (not yet explored squares).
-        - num_mines: jax array (int32) of shape `()`, indicates the number of mines to locate.
-        - step_count: jax array (int32) of shape ():
-            specifies how many timesteps have elapsed since environment reset.
-
-    - action:
-        multi discrete array containing the square to explore (height and width).
-
-    - reward: jax array (float32):
-        Configurable function of state and action. By default:
-            1 for every timestep where a valid action is chosen that doesn't reveal a mine,
-            0 for revealing a mine or selecting an already revealed square
-                (and terminate the episode).
-
-    - episode termination:
-        Configurable function of state, next_state, and action. By default:
-            Stop the episode if a mine is explored, an invalid action is selected
-            (exploring an already explored square), or the board is solved.
-
-    - state: `State`
-        - board: jax array (int32) of shape (num_rows, num_cols):
-            each cell contains -1 if not yet explored, or otherwise the number of mines in
-            the 8 adjacent squares.
-        - step_count: jax array (int32) of shape ():
-            specifies how many timesteps have elapsed since environment reset.
-        - flat_mine_locations: jax array (int32) of shape (num_rows * num_cols,):
-            indicates the (flat) locations of all the mines on the board.
-            Will be of length num_mines.
-        - key: jax array (int32) of shape (2,) used for seeding the sampling of mine placement
-            on reset.
+class Maze(Environment[State]):
+    """A JAX implementation of a 2D Maze. The goal is to navigate the maze to find the target
+    position.
+
+    - observation:
+        - agent_position: current 2D Position of agent.
+        - target_position: 2D Position of target cell.
+        - walls: jax array (bool) of shape (num_rows, num_cols)
+            whose values are `True` where walls are and `False` for empty cells.
+        - action_mask: array (bool) of shape (4,)
+            defining the available actions in the current position.
+        - step_count: jax array (int32) of shape ()
+            step number of the episode.
+
+    - action: jax array (int32) of shape () specifying which action to take: [0,1,2,3] correspond to
+        [Up, Right, Down, Left]. If an invalid action is taken, i.e. there is a wall blocking the
+        action, then no action (no-op) is taken.
+
+    - reward: jax array (float32) of shape (): 1 if the target is reached, 0 otherwise.
+
+    - episode termination (if any):
+        - agent reaches the target position.
+        - the time_limit is reached.
+
+    - state: State:
+        - agent_position: current 2D Position of agent.
+        - target_position: 2D Position of target cell.
+        - walls: jax array (bool) of shape (num_rows, num_cols)
+            whose values are `True` where walls are and `False` for empty cells.
+        - action_mask: array (bool) of shape (4,)
+            defining the available actions in the current position.
+        - step_count: jax array (int32) of shape ()
+            step number of the episode.
+        - key: random key (uint) of shape (2,).
 
     ```python
-    from jumanji.environments import Minesweeper
-    env = Minesweeper()
+    from jumanji.environments import Maze
+    env = Maze()
     key = jax.random.key(0)
     state, timestep = jax.jit(env.reset)(key)
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
+    FIGURE_NAME = "Maze"
+    FIGURE_SIZE = (6.0, 6.0)
+
     def __init__(
         self,
-        num_rows: int = 10,
-        num_cols: int = 10,
-        num_mines: int = 10,
-        reward_function: Optional[RewardFn] = None,
-        done_function: Optional[DoneFn] = None,
-        color_mapping: Optional[List[str]] = None,
-    ):
-        """Instantiate a `Minesweeper` environment.
+        generator: Optional[Generator] = None,
+        time_limit: Optional[int] = None,
+        viewer: Optional[Viewer[State]] = None,
+    ) -> None:
+        """Instantiates a `Maze` environment.
 
         Args:
-            num_rows: number of rows, i.e. height of the board. Defaults to 10.
-            num_cols: number of columns, i.e. width of the board. Defaults to 10.
-            num_mines: number of mines on the board. Defaults to 10.
-            reward_function: `RewardFn` whose `__call__` method computes the reward of an
-                environment transition based on the given current state and selected action.
-                Implemented options are [`DefaultRewardFn`]. Defaults to `DefaultRewardFn`.
-            done_function: `DoneFn` whose `__call__` method computes the done signal given the
-                current state, action taken, and next state.
-                Implemented options are [`DefaultDoneFn`]. Defaults to `DefaultDoneFn`.
-            color_mapping: colour map used for rendering.
+            generator: `Generator` whose `__call__` instantiates an environment instance.
+                Implemented options are [`ToyGenerator`, `RandomGenerator`].
+                Defaults to `RandomGenerator` with `num_rows=10` and `num_cols=10`.
+            time_limit: the time_limit of an episode, i.e. the maximum number of environment steps
+                before the episode terminates. By default, `time_limit = num_rows * num_cols`.
+            viewer: `Viewer` used for rendering. Defaults to `MazeEnvViewer` with "human" render
+                mode.
         """
-        if num_rows <= 1 or num_cols <= 1:
-            raise ValueError(
-                f"Should make a board of height and width greater than 1, "
-                f"got num_rows={num_rows}, num_cols={num_cols}"
-            )
-        if num_mines < 0 or num_mines >= num_rows * num_cols:
-            raise ValueError(
-                f"Number of mines should be constrained between 0 and the size of the board, "
-                f"got {num_mines}"
-            )
-        self.num_rows = num_rows
-        self.num_cols = num_cols
-        self.num_mines = num_mines
-        self.reward_function = reward_function or DefaultRewardFn()
-        self.done_function = done_function or DefaultDoneFn()
-
-        self.cmap = color_mapping if color_mapping else COLOUR_MAPPING
-        self.figure_name = f"{num_rows}x{num_cols} Minesweeper"
-        self.figure_size = (6.0, 6.0)
+        self.generator = generator or RandomGenerator(num_rows=10, num_cols=10)
+        self.num_rows = self.generator.num_rows
+        self.num_cols = self.generator.num_cols
+        self.shape = (self.num_rows, self.num_cols)
+        self.time_limit = time_limit or self.num_rows * self.num_cols
+
+        # Create viewer used for rendering
+        self._viewer = viewer or MazeEnvViewer("Maze", render_mode="human")
+
+    def __repr__(self) -> str:
+        return "\n".join(
+            [
+                "Maze environment:",
+                f" - num_rows: {self.num_rows}",
+                f" - num_cols: {self.num_cols}",
+                f" - time_limit: {self.time_limit}",
+                f" - generator: {self.generator}",
+            ]
+        )
+
+    def observation_spec(self) -> specs.Spec[Observation]:
+        """Specifications of the observation of the `Maze` environment.
+
+        Returns:
+            Spec for the `Observation` whose fields are:
+            - agent_position: tree of BoundedArray (int32) of shape ().
+            - target_position: tree of BoundedArray (int32) of shape ().
+            - walls: BoundedArray (bool) of shape (num_rows, num_cols).
+            - step_count: Array (int32) of shape ().
+            - action_mask: BoundedArray (bool) of shape (4,).
+        """
+        agent_position = specs.Spec(
+            Position,
+            "PositionSpec",
+            row=specs.BoundedArray(
+                (), jnp.int32, 0, self.num_rows - 1, "row_coordinate"
+            ),
+            col=specs.BoundedArray(
+                (), jnp.int32, 0, self.num_cols - 1, "col_coordinate"
+            ),
+        )
+        walls = specs.BoundedArray(
+            shape=(self.num_rows, self.num_cols),
+            dtype=bool,
+            minimum=False,
+            maximum=True,
+            name="walls",
+        )
+        step_count = specs.Array((), jnp.int32, "step_count")
+        action_mask = specs.BoundedArray(
+            shape=(4,), dtype=bool, minimum=False, maximum=True, name="action_mask"
+        )
+        return specs.Spec(
+            Observation,
+            "ObservationSpec",
+            agent_position=agent_position,
+            target_position=agent_position,
+            walls=walls,
+            step_count=step_count,
+            action_mask=action_mask,
+        )
+
+    def action_spec(self) -> specs.DiscreteArray:
+        """Returns the action spec. 4 actions: [0,1,2,3] -> [Up, Right, Down, Left].
+
+        Returns:
+            action_spec: discrete action space with 4 values.
+        """
+        return specs.DiscreteArray(4, name="action")
 
     def reset(self, key: chex.PRNGKey) -> Tuple[State, TimeStep[Observation]]:
-        """Resets the environment.
+        """Resets the environment by calling the instance generator for a new instance.
 
         Args:
-            key: needed for placing mines.
+            key: random key used to reset the environment since it is stochastic.
 
         Returns:
-            state: `State` corresponding to the new state of the environment,
-            timestep: `TimeStep` corresponding to the first timestep returned by the
-                environment.
+            state: `State` object corresponding to the new state of the environment after a reset.
+            timestep: `TimeStep` object corresponding the first timestep returned by the environment
+                after a reset.
         """
-        key, sample_key = jax.random.split(key)
-        board = jnp.full(
-            shape=(self.num_rows, self.num_cols),
-            fill_value=UNEXPLORED_ID,
-            dtype=jnp.int32,
+
+        key, maze_key, agent_key = jax.random.split(key, 3)
+
+        walls = self.generator(maze_key)
+
+        # Randomise agent start and target positions.
+        start_and_target_indices = jax.random.choice(
+            agent_key,
+            jnp.arange(self.num_rows * self.num_cols),
+            (2,),
+            replace=False,
+            p=~walls.flatten(),
         )
-        step_count = jnp.array(0, jnp.int32)
-        flat_mine_locations = create_flat_mine_locations(
-            key=sample_key,
-            num_rows=self.num_rows,
-            num_cols=self.num_cols,
-            num_mines=self.num_mines,
+        (agent_row, target_row), (agent_col, target_col) = jnp.divmod(
+            start_and_target_indices, self.num_cols
         )
+
+        agent_position = Position(row=agent_row, col=agent_col)
+        target_position = Position(row=target_row, col=target_col)
+
+        # Build the state.
         state = State(
-            board=board,
-            step_count=step_count,
+            agent_position=agent_position,
+            target_position=target_position,
+            walls=walls,
+            action_mask=self._compute_action_mask(walls, agent_position),
             key=key,
-            flat_mine_locations=flat_mine_locations,
+            step_count=jnp.array(0, jnp.int32),
         )
-        observation = self._state_to_observation(state=state)
-        timestep = restart(observation=observation)
+
+        # Generate the observation from the environment state.
+        observation = self._observation_from_state(state)
+
+        # Return a restart timestep whose step type is FIRST.
+        timestep = restart(observation)
+
         return state, timestep
 
     def step(
         self, state: State, action: chex.Array
     ) -> Tuple[State, TimeStep[Observation]]:
-        """Run one timestep of the environment's dynamics.
+        """
+        Run one timestep of the environment's dynamics.
+
+        If an action is invalid, the agent does not move, i.e. the episode does not
+        automatically terminate.
 
         Args:
-            state: `State` object containing the dynamics of the environment.
-            action: `Array` containing the row and column of the square to be explored.
+            state: State object containing the dynamics of the environment.
+            action: (int32) specifying which action to take: [0,1,2,3] correspond to
+                [Up, Right, Down, Left]. If an invalid action is taken, i.e. there is a wall
+                blocking the action, then no action (no-op) is taken.
 
         Returns:
-            next_state: `State` corresponding to the next state of the environment,
-            next_timestep: `TimeStep` corresponding to the timestep returned by the environment.
+            state: the next state of the environment.
+            timestep: the next timestep to be observed.
         """
-        board = state.board
-        action_height, action_width = action
-        board = board.at[action_height, action_width].set(
-            count_adjacent_mines(state=state, action=action)
-        )
-        step_count = state.step_count + 1
-        next_state = State(
-            board=board,
-            step_count=step_count,
+        # If the chosen action is invalid, i.e. blocked by a wall, overwrite it to no-op.
+        action = jax.lax.select(state.action_mask[action], action, 4)
+
+        # Take the action in the environment:  up, right, down, or left
+        # Remember the walls coordinates: (0,0) is top left.
+        agent_position = jax.lax.switch(
+            action,
+            [
+                lambda position: Position(position.row - 1, position.col),  # Up
+                lambda position: Position(position.row, position.col + 1),  # Right
+                lambda position: Position(position.row + 1, position.col),  # Down
+                lambda position: Position(position.row, position.col - 1),  # Left
+                lambda position: position,  # No-op
+            ],
+            state.agent_position,
+        )
+
+        # Generate action mask to keep in the state for the next step and
+        # to provide to the agent in the observation.
+        action_mask = self._compute_action_mask(state.walls, agent_position)
+
+        # Build the state.
+        state = State(
+            agent_position=agent_position,
+            target_position=state.target_position,
+            walls=state.walls,
+            action_mask=action_mask,
             key=state.key,
-            flat_mine_locations=state.flat_mine_locations,
+            step_count=state.step_count + 1,
         )
-        reward = self.reward_function(state, action)
-        done = self.done_function(state, next_state, action)
-        next_observation = self._state_to_observation(state=next_state)
-        next_timestep = jax.lax.cond(
+        # Generate the observation from the environment state.
+        observation = self._observation_from_state(state)
+
+        # Check if the episode terminates (i.e. done is True).
+        no_actions_available = ~jnp.any(action_mask)
+        target_reached = state.agent_position == state.target_position
+        time_limit_exceeded = state.step_count >= self.time_limit
+
+        done = no_actions_available | target_reached | time_limit_exceeded
+
+        # Compute the reward.
+        reward = jnp.array(state.agent_position == state.target_position, float)
+
+        # Return either a MID or a LAST timestep depending on done.
+        timestep = jax.lax.cond(
             done,
             termination,
             transition,
             reward,
-            next_observation,
+            observation,
         )
-        return next_state, next_timestep
-
-    def observation_spec(self) -> specs.Spec[Observation]:
-        """Specifications of the observation of the `Minesweeper` environment.
+        return state, timestep
 
-        Returns:
-            Spec for the `Observation` whose fields are:
-             - board: BoundedArray (int32) of shape (num_rows, num_cols).
-             - action_mask: BoundedArray (bool) of shape (num_rows, num_cols).
-             - num_mines: BoundedArray (int32) of shape ().
-             - step_count: BoundedArray (int32) of shape ().
+    def _compute_action_mask(
+        self, walls: chex.Array, agent_position: Position
+    ) -> chex.Array:
+        """Compute the action mask.
+        An action is considered invalid if it leads to a WALL or goes outside of the maze.
         """
-        board = specs.BoundedArray(
-            shape=(self.num_rows, self.num_cols),
-            dtype=jnp.int32,
-            minimum=-1,
-            maximum=PATCH_SIZE * PATCH_SIZE - 1,
-            name="board",
-        )
-        action_mask = specs.BoundedArray(
-            shape=(self.num_rows, self.num_cols),
-            dtype=bool,
-            minimum=False,
-            maximum=True,
-            name="action_mask",
-        )
-        num_mines = specs.BoundedArray(
-            shape=(),
-            dtype=jnp.int32,
-            minimum=0,
-            maximum=self.num_rows * self.num_cols - 1,
-            name="num_mines",
-        )
-        step_count = specs.BoundedArray(
-            shape=(),
-            dtype=jnp.int32,
-            minimum=0,
-            maximum=self.num_rows * self.num_cols - self.num_mines,
-            name="step_count",
-        )
-        return specs.Spec(
-            Observation,
-            "ObservationSpec",
-            board=board,
-            action_mask=action_mask,
-            num_mines=num_mines,
-            step_count=step_count,
-        )
 
-    def action_spec(self) -> specs.MultiDiscreteArray:
-        """Returns the action spec.
-        An action consists of the height and width of the square to be explored.
+        def is_move_valid(agent_position: Position, move: chex.Array) -> chex.Array:
+            x, y = jnp.array([agent_position.row, agent_position.col]) + move
+            return (
+                (x >= 0)
+                & (x < self.num_cols)
+                & (y >= 0)
+                & (y < self.num_rows)
+                & ~(walls[x, y])
+            )
+
+        # vmap over the moves.
+        action_mask = jax.vmap(is_move_valid, in_axes=(None, 0))(agent_position, MOVES)
 
-        Returns:
-            action_spec: `specs.MultiDiscreteArray` object.
-        """
-        return specs.MultiDiscreteArray(
-            num_values=jnp.array([self.num_rows, self.num_cols], jnp.int32),
-            name="action",
-            dtype=jnp.int32,
-        )
+        return action_mask
 
-    def _state_to_observation(self, state: State) -> Observation:
+    def _observation_from_state(self, state: State) -> Observation:
+        """Create an observation from the state of the environment."""
         return Observation(
-            board=state.board,
-            action_mask=jnp.equal(state.board, UNEXPLORED_ID),
-            num_mines=jnp.array(self.num_mines, jnp.int32),
+            agent_position=state.agent_position,
+            target_position=state.target_position,
+            walls=state.walls,
             step_count=state.step_count,
+            action_mask=state.action_mask,
         )
 
-    def render(self, state: State) -> None:
-        """Render the given environment state using matplotlib.
+    def render(self, state: State) -> Optional[NDArray]:
+        """Render the given state of the environment.
 
         Args:
-            state: environment state to be rendered.
-
+            state: `State` object containing the current environment state.
         """
-        self._clear_display()
-        fig, ax = self._get_fig_ax()
-        self._draw(ax, state)
-        self._update_display(fig)
+        return self._viewer.render(state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
-        """Create an animation from a sequence of environment states.
+        """Creates an animated gif of the `Maze` environment based on the sequence of states.
 
         Args:
             states: sequence of environment states corresponding to consecutive timesteps.
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
-            Animation object that can be saved as a GIF, MP4, or rendered with HTML.
+            animation.FuncAnimation: the animation object that was created.
         """
-        fig, ax = self._get_fig_ax()
-        plt.tight_layout()
-        plt.close(fig)
-
-        def make_frame(state_index: int) -> None:
-            state = states[state_index]
-            self._draw(ax, state)
-
-        # Create the animation object.
-        self._animation = matplotlib.animation.FuncAnimation(
-            fig,
-            make_frame,
-            frames=len(states),
-            interval=interval,
-        )
-
-        # Save the animation as a GIF.
-        if save_path:
-            self._animation.save(save_path)
-
-        return self._animation
+        return self._viewer.animate(states, interval, save_path)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        plt.close(self.figure_name)
-
-    def _get_fig_ax(self) -> Tuple[plt.Figure, plt.Axes]:
-        exists = plt.fignum_exists(self.figure_name)
-        if exists:
-            fig = plt.figure(self.figure_name)
-            ax = fig.get_axes()[0]
-        else:
-            fig = plt.figure(self.figure_name, figsize=self.figure_size)
-            plt.suptitle(self.figure_name)
-            plt.tight_layout()
-            if not plt.isinteractive():
-                fig.show()
-            ax = fig.add_subplot()
-        return fig, ax
-
-    def _draw(self, ax: plt.Axes, state: State) -> None:
-        ax.clear()
-        ax.set_xticks(jnp.arange(-0.5, self.num_cols - 1, 1))
-        ax.set_yticks(jnp.arange(-0.5, self.num_rows - 1, 1))
-        ax.tick_params(
-            top=False,
-            bottom=False,
-            left=False,
-            right=False,
-            labelleft=False,
-            labelbottom=False,
-            labeltop=False,
-            labelright=False,
-        )
-        background = jnp.ones_like(state.board)
-        for i in range(self.num_rows):
-            for j in range(self.num_cols):
-                background = self._render_grid_square(
-                    state=state, ax=ax, i=i, j=j, background=background
-                )
-        ax.imshow(background, cmap="gray", vmin=0, vmax=1)
-        ax.grid(color="black", linestyle="-", linewidth=2)
-
-    def _render_grid_square(
-        self, state: State, ax: plt.Axes, i: int, j: int, background: chex.Array
-    ) -> chex.Array:
-        board_value = state.board[i, j]
-        if board_value != UNEXPLORED_ID:
-            if explored_mine(state=state, action=jnp.array([i, j], dtype=jnp.int32)):
-                background = background.at[i, j].set(0)
-            else:
-                ax.text(
-                    j,
-                    i,
-                    str(board_value),
-                    color=self.cmap[board_value],
-                    ha="center",
-                    va="center",
-                    fontsize="xx-large",
-                )
-        return background
-
-    def _update_display(self, fig: plt.Figure) -> None:
-        if plt.isinteractive():
-            # Required to update render when using Jupyter Notebook.
-            fig.canvas.draw()
-            if jumanji.environments.is_colab():
-                plt.show(self.figure_name)
-        else:
-            # Required to update render when not using Jupyter Notebook.
-            fig.canvas.draw_idle()
-            fig.canvas.flush_events()
-
-    def _clear_display(self) -> None:
-        if jumanji.environments.is_colab():
-            import IPython.display
-
-            IPython.display.clear_output(True)
+        self._viewer.close()
```

### Comparing `jumanji-0.2.1/jumanji/environments/logic/minesweeper/reward.py` & `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/reward.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,36 +13,23 @@
 # limitations under the License.
 
 import abc
 
 import chex
 import jax.numpy as jnp
 
-from jumanji.environments.logic.minesweeper.constants import (
-    REVEALED_EMPTY_SQUARE_REWARD,
-    REVEALED_MINE_OR_INVALID_ACTION_REWARD,
-)
-from jumanji.environments.logic.minesweeper.types import State
-from jumanji.environments.logic.minesweeper.utils import explored_mine, is_valid_action
+from jumanji.environments.logic.rubiks_cube.types import State
+from jumanji.environments.logic.rubiks_cube.utils import is_solved
 
 
 class RewardFn(abc.ABC):
     @abc.abstractmethod
-    def __call__(self, state: State, action: chex.Array) -> chex.Array:
-        """Call method for computing the reward given current state and selected action."""
+    def __call__(self, state: State) -> chex.Array:
+        """Call method for computing the reward given new state."""
 
 
-class DefaultRewardFn(RewardFn):
-    """A dense reward function: 1 for every timestep on which a mine is not explored
-    (or a small penalty if action is invalid), otherwise 0.
-    """
-
-    def __call__(self, state: State, action: chex.Array) -> chex.Array:
-        return jnp.where(
-            is_valid_action(state=state, action=action),
-            jnp.where(
-                explored_mine(state=state, action=action),
-                jnp.array(REVEALED_MINE_OR_INVALID_ACTION_REWARD, float),
-                jnp.array(REVEALED_EMPTY_SQUARE_REWARD, float),
-            ),
-            jnp.array(REVEALED_MINE_OR_INVALID_ACTION_REWARD, float),
-        )
+class SparseRewardFn(RewardFn):
+    """A sparse reward function, returning +1 if cube is solved and otherwise 0."""
+
+    def __call__(self, state: State) -> chex.Array:
+        solved = is_solved(state.cube)
+        return jnp.array(solved, float)
```

### Comparing `jumanji-0.2.1/jumanji/environments/logic/minesweeper/types.py` & `jumanji-0.2.2/jumanji/environments/logic/minesweeper/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/minesweeper/utils.py` & `jumanji-0.2.2/jumanji/environments/logic/minesweeper/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import chex
+import jax
 import jax.numpy as jnp
-from jax import random
-from jax.lax import dynamic_slice_in_dim
 
 from jumanji.environments.logic.minesweeper.constants import (
     IS_MINE,
     PATCH_SIZE,
     UNEXPLORED_ID,
 )
-from jumanji.environments.logic.minesweeper.types import Board, State
+from jumanji.environments.logic.minesweeper.types import State
 
 
 def create_flat_mine_locations(
     key: chex.PRNGKey,
     num_rows: int,
     num_cols: int,
     num_mines: int,
-) -> Board:
+) -> chex.Array:
     """Create locations of mines on a board with a specified height, width, and number
     of mines. The locations are in flattened coordinates.
+
+    Args:
+        key: used for sampling mine positions.
+        num_rows: the height of the board.
+        num_cols: the width of the board.
+        num_mines: how many mines to place.
     """
-    return random.choice(
+    return jax.random.choice(
         key,
         num_rows * num_cols,
         shape=(num_mines,),
         replace=False,
     )
 
 
@@ -49,47 +54,44 @@
     num_rows, num_cols = board.shape
     num_explored = (board >= 0).sum()
     return num_explored == num_rows * num_cols - num_mines
 
 
 def is_valid_action(state: State, action: chex.Array) -> chex.Array:
     """Check if an action is exploring a square that has not already been explored."""
-    action_height, action_width = action
-    return state.board[action_height, action_width] == UNEXPLORED_ID
+    return state.board[tuple(action)] == UNEXPLORED_ID
 
 
 def get_mined_board(state: State) -> chex.Array:
     """Compute the board with 1 in mine locations, otherwise 0."""
     return (
         jnp.zeros((state.board.shape[-1] * state.board.shape[-2],), dtype=jnp.int32)
         .at[state.flat_mine_locations]
         .set(IS_MINE)
     )
 
 
 def explored_mine(state: State, action: chex.Array) -> chex.Array:
     """Check if an action is exploring a square containing a mine."""
-    height, width = action
-    index = width + height * state.board.shape[-1]
+    row, col = action
+    index = col + row * state.board.shape[-1]
     mined_board = get_mined_board(state=state)
     return mined_board[index] == IS_MINE
 
 
 def count_adjacent_mines(state: State, action: chex.Array) -> chex.Array:
     """Count the number of mines in a 3x3 patch surrounding the selected action."""
-    action_height, action_width = action
-    mined_board = get_mined_board(state=state).reshape(
-        state.board.shape[-2], state.board.shape[-1]
-    )
+    action_row, action_col = action
+    mined_board = get_mined_board(state=state).reshape(*state.board.shape)
     pad_board = jnp.pad(mined_board, pad_width=PATCH_SIZE - 1)
-    selected_rows = dynamic_slice_in_dim(
-        pad_board, start_index=action_height + 1, slice_size=PATCH_SIZE, axis=-2
+    selected_rows = jax.lax.dynamic_slice_in_dim(
+        pad_board, start_index=action_row + 1, slice_size=PATCH_SIZE, axis=-2
     )
     return (
-        dynamic_slice_in_dim(
+        jax.lax.dynamic_slice_in_dim(
             selected_rows,
-            start_index=action_width + 1,
+            start_index=action_col + 1,
             slice_size=PATCH_SIZE,
             axis=-1,
         ).sum()
-        - mined_board[action_height, action_width]
+        - mined_board[tuple(action)]
     )
```

### Comparing `jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/__init__.py` & `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/constants.py` & `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/env.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/env.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,432 +8,406 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import List, Optional, Sequence, Tuple
+from typing import Dict, Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import matplotlib
-import matplotlib.animation
-import matplotlib.pyplot as plt
+from numpy.typing import NDArray
 
-import jumanji.environments
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.logic.rubiks_cube.constants import (
-    DEFAULT_STICKER_COLORS,
-    CubeMovementAmount,
-    Face,
+from jumanji.environments.routing.connector.constants import (
+    AGENT_INITIAL_VALUE,
+    NOOP,
+    PATH,
 )
-from jumanji.environments.logic.rubiks_cube.reward import RewardFn, SparseRewardFn
-from jumanji.environments.logic.rubiks_cube.types import Cube, Observation, State
-from jumanji.environments.logic.rubiks_cube.utils import (
-    generate_all_moves,
-    is_solved,
-    make_solved_cube,
+from jumanji.environments.routing.connector.generator import (
+    Generator,
+    UniformRandomGenerator,
 )
+from jumanji.environments.routing.connector.reward import DenseRewardFn, RewardFn
+from jumanji.environments.routing.connector.types import Agent, Observation, State
+from jumanji.environments.routing.connector.utils import (
+    connected_or_blocked,
+    get_agent_grid,
+    get_correction_mask,
+    is_valid_position,
+    move_agent,
+    move_position,
+    switch_perspective,
+)
+from jumanji.environments.routing.connector.viewer import ConnectorViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
-class RubiksCube(Environment[State]):
-    """A JAX implementation of the Rubik's Cube with a configurable cube size (by default, 3) and
-    number of scrambles at reset.
-
-    - observation: `Observation`
-        - cube: jax array (int8) of shape (6, cube_size, cube_size):
-            each cell contains the index of the corresponding colour of the sticker in the scramble.
-        - step_count: jax array (int32) of shape ():
-            specifies how many timesteps have elapsed since environment reset.
-
-    - action:
-        multi discrete array containing the move to perform (face, depth, and direction).
+class Connector(Environment[State]):
+    """The `Connector` environment is a multi-agent gridworld problem where each agent must connect a
+    start to a target. However, when moving through this gridworld the agent leaves an impassable
+    trail behind it. Therefore, agents must connect to their targets without overlapping the routes
+    taken by any other agent.
+
+    - observation - `Observation`
+        - action mask: jax array (bool) of shape (num_agents, 5).
+        - step_count: jax array (int32) of shape ()
+            the current episode step.
+        - grid: jax array (int32) of shape (num_agents, size, size)
+            - each 2d array (size, size) along axis 0 is the agent's local observation.
+            - agents have ids from 0 to (num_agents - 1)
+            - with 2 agents you might have a grid like this:
+              4 0 1
+              5 0 1
+              6 3 2
+              which means agent 1 has moved from the top right of the grid down and is currently in
+              the bottom right corner and is aiming to get to the middle bottom cell. Agent 2
+              started in the top left and moved down once towards its target in the bottom left.
+
+              This would just be agent 0's view, the numbers would be flipped for agent 1's view.
+              So the full observation would be of shape (2, 3, 3).
+
+    - action: jax array (int32) of shape (num_agents,):
+        - can take the values [0,1,2,3,4] which correspond to [No Op, Up, Right, Down, Left].
+        - each value in the array corresponds to an agent's action.
 
     - reward: jax array (float) of shape ():
-        by default, 1.0 if cube is solved, otherwise 0.0.
-
-    - episode termination:
-        if either the cube is solved or a time limit is reached.
+        - dense: each agent is given 1.0 if it connects on that step, otherwise 0.0. Additionally,
+            each agent that has not connected receives a penalty reward of -0.03.
 
-    - state: `State`
-        - cube: jax array (int8) of shape (6, cube_size, cube_size):
-            each cell contains the index of the corresponding colour of the sticker in the scramble.
-        - step_count: jax array (int32) of shape ():
-            specifies how many timesteps have elapsed since environment reset.
-        - key: jax array (uint) of shape (2,) used for seeding the sampling for scrambling on
-            reset.
-        - action_history: jax array (int32) of shape (num_scrambles_on_reset + time_limit, 3):
-            indicates the entire history of applied moves (including those taken on scrambling the
-            cube in the environment reset). This is useful for debugging purposes, providing a
-            method to solve the cube from any position without relying on the agent, by just
-            inverting the action history. The first axis indexes over the length of the sequence
-            The second axis indexes over the component of the action (face, depth, amount). The
-            number of scrambles applied for each state is given by
-            `env.num_scrambles_on_reset + state.step_count`.
+    - episode termination: if an agent can't move, or the time limit is reached, or the agent
+        connects to its target, it is considered done. Once all agents are done, the episode
+        terminates. The timestep discounts are of shape (num_agents,).
+
+    - state: State:
+        - key: jax PRNG key used to randomly spawn agents and targets.
+        - grid: jax array (int32) of shape (size, size) which corresponds to agent 0's observation.
+        - step_count: jax array (int32) of shape () number of steps elapsed in the current episode.
 
     ```python
-    from jumanji.environments import RubiksCube
-    env = RubiksCube()
+    from jumanji.environments import Connector
+    env = Connector()
     key = jax.random.key(0)
     state, timestep = jax.jit(env.reset)(key)
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        cube_size: int = 3,
-        time_limit: int = 200,
-        num_scrambles_on_reset: int = 100,
+        generator: Optional[Generator] = None,
         reward_fn: Optional[RewardFn] = None,
-        sticker_colors: Optional[list] = None,
-    ):
-        """Instantiate a `RubiksCube` environment.
+        time_limit: int = 50,
+        viewer: Optional[Viewer[State]] = None,
+    ) -> None:
+        """Create the `Connector` environment.
 
         Args:
-            cube_size: the size of the cube, i.e. length of an edge. Defaults to 3.
-            time_limit: the number of steps allowed before an episode terminates. Defaults to 200.
-            num_scrambles_on_reset: the number of scrambles done from a solved Rubik's Cube in the
-                generation of a random instance. The lower, the closer to a solved cube the reset
-                state is. Defaults to 100.
-            reward_fn: `RewardFn` whose `__call__` method computes the reward given the new state.
-                Implemented options are [`SparseRewardFn`]. Defaults to `SparseRewardFn`.
-            sticker_colors: colors used in rendering the faces of the rubiks cube.
-                Defaults to `DEFAULT_STICKER_COLORS`.
-        """
-        if cube_size < 2:
-            raise ValueError(
-                f"Cannot meaningfully construct a cube smaller than 2x2x2, "
-                f"but received cube_size={cube_size}"
-            )
-        if time_limit <= 0:
-            raise ValueError(
-                f"The time_limit must be positive, but received time_limit={time_limit}"
-            )
-        if num_scrambles_on_reset < 0:
-            raise ValueError(
-                f"The num_scrambles_on_reset must be non-negative, "
-                f"but received num_scrambles_on_reset={num_scrambles_on_reset}"
-            )
-        self.cube_size = cube_size
+            generator: `Generator` whose `__call__` instantiates an environment instance.
+                Implemented options are [`UniformRandomGenerator`].
+                Defaults to `UniformRandomGenerator` with `grid_size=10` and `num_agents=5`.
+            reward_fn: class of type `RewardFn`, whose `__call__` is used as a reward function.
+                Implemented options are [`DenseRewardFn`]. Defaults to `DenseRewardFn`.
+            time_limit: the number of steps allowed before an episode terminates. Defaults to 50.
+            viewer: `Viewer` used for rendering. Defaults to `ConnectorViewer` with "human" render
+                mode.
+        """
+        self._generator = generator or UniformRandomGenerator(
+            grid_size=10, num_agents=5
+        )
+        self._reward_fn = reward_fn or DenseRewardFn()
         self.time_limit = time_limit
-        self.num_scrambles_on_reset = num_scrambles_on_reset
-        self.reward_function = reward_fn or SparseRewardFn()
-        sticker_colors = sticker_colors or DEFAULT_STICKER_COLORS
-        self.sticker_colors_cmap = matplotlib.colors.ListedColormap(sticker_colors)
-        self.num_actions = len(Face) * (cube_size // 2) * len(CubeMovementAmount)
-        self.all_moves = generate_all_moves(cube_size=cube_size)
-
-        self.figure_name = f"{cube_size}x{cube_size}x{cube_size} Rubik's Cube"
-        self.figure_size = (6.0, 6.0)
+        self.num_agents = self._generator.num_agents
+        self.grid_size = self._generator.grid_size
+        self._agent_ids = jnp.arange(self.num_agents)
+        self._viewer = viewer or ConnectorViewer(
+            "Connector", self.num_agents, render_mode="human"
+        )
 
     def reset(self, key: chex.PRNGKey) -> Tuple[State, TimeStep[Observation]]:
         """Resets the environment.
 
         Args:
-            key: needed for scramble.
+            key: used to randomly generate the connector grid.
 
         Returns:
-            state: `State` corresponding to the new state of the environment.
-            timestep: `TimeStep` corresponding to the first timestep returned by the
-                environment.
-        """
-        key, scramble_key = jax.random.split(key)
-        flat_actions_in_scramble = jax.random.randint(
-            scramble_key,
-            minval=0,
-            maxval=self.num_actions,
-            shape=(self.num_scrambles_on_reset,),
-            dtype=jnp.int32,
-        )
-        cube = self._scramble_solved_cube(
-            flat_actions_in_scramble=flat_actions_in_scramble
-        )
-        action_history = jnp.zeros(
-            shape=(self.num_scrambles_on_reset + self.time_limit, 3), dtype=jnp.int32
+            state: `State` object corresponding to the new state of the environment.
+            timestep: `TimeStep` object corresponding to the initial environment timestep.
+        """
+        state = self._generator(key)
+
+        action_mask = jax.vmap(self._get_action_mask, (0, None))(
+            state.agents, state.grid
         )
-        action_history = action_history.at[: self.num_scrambles_on_reset].set(
-            self._unflatten_action(flat_actions_in_scramble).transpose()
+        observation = Observation(
+            grid=self._obs_from_grid(state.grid),
+            action_mask=action_mask,
+            step_count=state.step_count,
+        )
+        extras = self._get_extras(state)
+        timestep = restart(
+            observation=observation, extras=extras, shape=(self.num_agents,)
         )
-        step_count = jnp.array(0, jnp.int32)
-        state = State(
-            cube=cube,
-            step_count=step_count,
-            key=key,
-            action_history=action_history,
-        )
-        observation = self._state_to_observation(state=state)
-        timestep = restart(observation=observation)
         return state, timestep
 
     def step(
         self, state: State, action: chex.Array
     ) -> Tuple[State, TimeStep[Observation]]:
-        """Run one timestep of the environment's dynamics.
+        """Perform an environment step.
 
         Args:
-            state: `State` object containing the dynamics of the environment.
-            action: `Array` of shape (3,) indicating the face to move, depth of the move, and the
-                amount to move by.
+            state: State object containing the dynamics of the environment.
+            action: Array containing the actions to take for each agent.
+                - 0 no op
+                - 1 move up
+                - 2 move right
+                - 3 move down
+                - 4 move left
 
         Returns:
-            next_state: `State` corresponding to the next state of the environment.
-            next_timestep: `TimeStep` corresponding to the timestep returned by the environment.
+            state: `State` object corresponding to the next state of the environment.
+            timestep: `TimeStep` object corresponding the timestep returned by the environment.
         """
-        flat_action = self._flatten_action(action)
-        cube = self._rotate_cube(cube=state.cube, flat_action=flat_action)
-        action_history = state.action_history.at[
-            self.num_scrambles_on_reset + state.step_count
-        ].set(action)
-        step_count = state.step_count + 1
-        next_state = State(
-            cube=cube,
-            step_count=step_count,
-            key=state.key,
-            action_history=action_history,
+        agents, grid = self._step_agents(state, action)
+        new_state = State(
+            grid=grid, step_count=state.step_count + 1, agents=agents, key=state.key
+        )
+
+        # Construct timestep: get observations, rewards, discounts
+        grids = self._obs_from_grid(grid)
+        reward = self._reward_fn(state, action, new_state)
+        action_mask = jax.vmap(self._get_action_mask, (0, None))(agents, grid)
+        observation = Observation(
+            grid=grids, action_mask=action_mask, step_count=new_state.step_count
+        )
+
+        dones = jax.vmap(connected_or_blocked)(agents, action_mask)
+        discount = jnp.asarray(jnp.logical_not(dones), dtype=float)
+        extras = self._get_extras(new_state)
+        timestep = jax.lax.cond(
+            dones.all() | (new_state.step_count >= self.time_limit),
+            lambda: termination(
+                reward=reward,
+                observation=observation,
+                extras=extras,
+                shape=self.num_agents,
+            ),
+            lambda: transition(
+                reward=reward,
+                observation=observation,
+                discount=discount,
+                extras=extras,
+                shape=self.num_agents,
+            ),
         )
-        reward = self.reward_function(state=next_state)
-        solved = is_solved(cube)
-        done = (step_count >= self.time_limit) | solved
-        next_observation = self._state_to_observation(state=next_state)
-        next_timestep = jax.lax.cond(
-            done,
-            termination,
-            transition,
-            reward,
-            next_observation,
-        )
-        return next_state, next_timestep
-
-    def get_action_history(self, state: State) -> chex.Array:
-        """Slice and return the action history from the state."""
-        action_history_index = self.num_scrambles_on_reset + state.step_count
-        return state.action_history[:action_history_index]
 
-    def observation_spec(self) -> specs.Spec[Observation]:
-        """Specifications of the observation of the `RubiksCube` environment.
+        return new_state, timestep
 
-        Returns:
-            Spec containing all the specifications for all the `Observation` fields:
-             - cube: BoundedArray (jnp.int8) of shape (num_faces, cube_size, cube_size).
-             - step_count: BoundedArray (jnp.int32) of shape ().
-        """
-        cube = specs.BoundedArray(
-            shape=(len(Face), self.cube_size, self.cube_size),
-            dtype=jnp.int8,
-            minimum=0,
-            maximum=len(Face) - 1,
-            name="cube",
-        )
-        step_count = specs.BoundedArray(
-            shape=(),
-            dtype=jnp.int32,
-            minimum=0,
-            maximum=self.time_limit,
-            name="step_count",
-        )
-        return specs.Spec(
-            Observation,
-            "ObservationSpec",
-            cube=cube,
-            step_count=step_count,
-        )
+    def _step_agents(
+        self, state: State, action: chex.Array
+    ) -> Tuple[Agent, chex.Array]:
+        """Steps all agents at the same time correcting for possible collisions.
 
-    def action_spec(self) -> specs.MultiDiscreteArray:
-        """Returns the action spec. An action is composed of 3 elements that range in: 6 faces, each
-        with cube_size//2 possible depths, and 3 possible directions.
+        If a collision occurs we place the agent with the lower `agent_id` in its previous position.
 
         Returns:
-            action_spec: `MultiDiscreteArray` object.
+            Tuple: (agents, grid) after having applied each agents' action
         """
-        return specs.MultiDiscreteArray(
-            num_values=jnp.array([len(Face), self.cube_size // 2, 3], jnp.int32),
-            name="action",
-            dtype=jnp.int32,
-        )
+        agent_ids = jnp.arange(self.num_agents)
+        # Step all agents at the same time (separately) and return all of the grids
+        agents, grids = jax.vmap(self._step_agent, in_axes=(0, None, 0))(
+            state.agents, state.grid, action
+        )
+
+        # Get grids with only values related to a single agent.
+        # For example: remove all other agents from agent 1's grid. Do this for all agents.
+        agent_grids = jax.vmap(get_agent_grid)(agent_ids, grids)
+        joined_grid = jnp.max(agent_grids, 0)  # join the grids
+
+        # Create a correction mask for possible collisions (see the docs of `get_correction_mask`)
+        correction_fn = jax.vmap(get_correction_mask, in_axes=(None, None, 0))
+        correction_masks, collided_agents = correction_fn(
+            state.grid, joined_grid, agent_ids
+        )
+        correction_mask = jnp.sum(correction_masks, 0)
+
+        # Correct state.agents
+        # Get the correct agents, either old agents (if collision) or new agents if no collision
+        agents = jax.vmap(
+            lambda collided, old_agent, new_agent: jax.lax.cond(
+                collided,
+                lambda: old_agent,
+                lambda: new_agent,
+            )
+        )(collided_agents, state.agents, agents)
+        # Create the new grid by fixing old one with correction mask and adding the obstacles
+        return agents, joined_grid + correction_mask
+
+    def _step_agent(
+        self, agent: Agent, grid: chex.Array, action: chex.Numeric
+    ) -> Tuple[Agent, chex.Array]:
+        """Moves the agent according to the given action if it is possible.
 
-    def _unflatten_action(self, action: chex.Array) -> chex.Array:
-        """Turn a flat action (index into the sequence of all moves) into a tuple:
-            - face (0-5). This indicates the face on which the layer will turn.
-            - depth (0-cube_size//2). This indicates how many layers down from the face
-                the turn will take place.
-            - amount (0-2). This indicates the amount of turning (see below).
-
-        Convention:
-        - 0 = up face
-        - 1 = front face
-        - 2 = right face
-        - 3 = back face
-        - 4 = left face
-        - 5 = down face
-        All read in reading order when looking directly at a face.
-
-        To look directly at the faces:
-        - UP: LEFT face on the left and BACK face pointing up
-        - FRONT: LEFT face on the left and UP face pointing up
-        - RIGHT: FRONT face on the left and UP face pointing up
-        - BACK: RIGHT face on the left and UP face pointing up
-        - LEFT: BACK face on the left and UP face pointing up
-        - DOWN: LEFT face on the left and FRONT face pointing up
-
-        Turning amounts are when looking directly at a face:
-        - 0 = clockwise turn
-        - 1 = anticlockwise turn
-        - 2 = half turn
-        """
-        face_and_depth, amount = jnp.divmod(action, len(CubeMovementAmount))
-        face, depth = jnp.divmod(face_and_depth, self.cube_size // 2)
-        return jnp.stack([face, depth, amount], axis=0)
-
-    def _flatten_action(self, action: chex.Array) -> chex.Array:
-        """Inverse of the `_flatten_action` method."""
-        face, depth, amount = action
-        return (
-            face * len(CubeMovementAmount) * (self.cube_size // 2)
-            + depth * len(CubeMovementAmount)
-            + amount
-        )
-
-    def _rotate_cube(self, cube: Cube, flat_action: chex.Array) -> Cube:
-        """Apply a flattened action (index into the sequence of all moves) to a cube."""
-        moved_cube = jax.lax.switch(flat_action, self.all_moves, cube)
-        return moved_cube
-
-    def _scramble_solved_cube(self, flat_actions_in_scramble: chex.Array) -> Cube:
-        """Return a scrambled cube according to a given sequence of flat actions."""
-        cube = make_solved_cube(cube_size=self.cube_size)
-        cube, _ = jax.lax.scan(
-            lambda *args: (self._rotate_cube(*args), None),
-            cube,
-            flat_actions_in_scramble,
-        )
-        return cube
+        Returns:
+            Tuple: (agent, grid) after having applied the given action.
+        """
+        new_pos = move_position(agent.position, action)
 
-    def _state_to_observation(self, state: State) -> Observation:
-        return Observation(cube=state.cube, step_count=state.step_count)
+        new_agent, new_grid = jax.lax.cond(
+            is_valid_position(grid, agent, new_pos) & (action != NOOP),
+            move_agent,
+            lambda *_: (agent, grid),
+            agent,
+            grid,
+            new_pos,
+        )
+
+        return new_agent, new_grid
+
+    def _obs_from_grid(self, grid: chex.Array) -> chex.Array:
+        """Gets the observation vector for all agents."""
+        return jax.vmap(switch_perspective, (None, 0, None))(
+            grid, self._agent_ids, self.num_agents
+        )
+
+    def _get_action_mask(self, agent: Agent, grid: chex.Array) -> chex.Array:
+        """Gets an agent's action mask."""
+        # Don't check action 0 because no-op is always valid
+        actions = jnp.arange(1, 5)
+
+        def is_valid_action(action: int) -> chex.Array:
+            agent_pos = move_position(agent.position, action)
+            return is_valid_position(grid, agent, agent_pos)
+
+        mask = jnp.ones(5, dtype=bool)
+        mask = mask.at[actions].set(jax.vmap(is_valid_action)(actions))
+        return mask
+
+    def _get_extras(self, state: State) -> Dict:
+        """Computes extras metrics to be return within the timestep."""
+        offset = AGENT_INITIAL_VALUE
+        total_path_length = jnp.sum((offset + (state.grid - offset) % 3) == PATH)
+        # Add agents' head
+        total_path_length += self.num_agents
+        extras = {
+            "num_connections": jnp.sum(state.agents.connected),
+            "ratio_connections": jnp.mean(state.agents.connected),
+            "total_path_length": total_path_length,
+        }
+        return extras
 
-    def render(self, state: State) -> None:
-        """Render frames of the environment for a given state using matplotlib.
+    def render(self, state: State) -> Optional[NDArray]:
+        """Render the given state of the environment.
 
         Args:
-            state: `State` object corresponding to the new state of the environment.
+            state: `State` object containing the current environment state.
         """
-        self._clear_display()
-        fig, ax = self._get_fig_ax()
-        self._draw(ax, state)
-        self._update_display(fig)
+        return self._viewer.render(state.grid)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
-        """Create an animation from a sequence of environment states.
+        """Create an animation from a sequence of states.
 
         Args:
-            states: sequence of environment states corresponding to consecutive timesteps.
+            states: sequence of `State` corresponding to subsequent timesteps.
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
-            Animation that can be saved as a GIF, MP4, or rendered with HTML.
+            animation that can export to gif, mp4, or render with HTML.
         """
-        fig, ax = plt.subplots(nrows=3, ncols=2, figsize=self.figure_size)
-        fig.suptitle(self.figure_name)
-        plt.tight_layout()
-        ax = ax.flatten()
-        plt.close(fig)
-
-        def make_frame(state_index: int) -> None:
-            state = states[state_index]
-            self._draw(ax, state)
-
-        # Create the animation object.
-        self._animation = matplotlib.animation.FuncAnimation(
-            fig,
-            make_frame,
-            frames=len(states),
-            interval=interval,
-        )
-
-        # Save the animation as a gif.
-        if save_path:
-            self._animation.save(save_path)
-
-        return self._animation
+        grids = [state.grid for state in states]
+        return self._viewer.animate(grids, interval, save_path)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        plt.close(self.figure_name)
+        self._viewer.close()
 
-    def _get_fig_ax(self) -> Tuple[plt.Figure, List[plt.Axes]]:
-        exists = plt.fignum_exists(self.figure_name)
-        if exists:
-            fig = plt.figure(self.figure_name)
-            ax = fig.get_axes()
-        else:
-            fig, ax = plt.subplots(
-                nrows=3, ncols=2, figsize=self.figure_size, num=self.figure_name
-            )
-            fig.suptitle(self.figure_name)
-            ax = ax.flatten()
-            plt.tight_layout()
-            plt.axis("off")
-            if not plt.isinteractive():
-                fig.show()
-        return fig, ax
-
-    def _draw(self, ax: List[plt.Axes], state: State) -> None:
-        i = 0
-        for face in Face:
-            ax[i].clear()
-            ax[i].set_title(label=f"{face}")
-            ax[i].set_xticks(jnp.arange(-0.5, self.cube_size - 1, 1))
-            ax[i].set_yticks(jnp.arange(-0.5, self.cube_size - 1, 1))
-            ax[i].tick_params(
-                top=False,
-                bottom=False,
-                left=False,
-                right=False,
-                labelleft=False,
-                labelbottom=False,
-                labeltop=False,
-                labelright=False,
-            )
-            ax[i].imshow(
-                state.cube[i],
-                cmap=self.sticker_colors_cmap,
-                vmin=0,
-                vmax=len(Face) - 1,
-            )
-            ax[i].grid(color="black", linestyle="-", linewidth=2)
-            i += 1
+    def observation_spec(self) -> specs.Spec[Observation]:
+        """Specifications of the observation of the `Connector` environment.
 
-    def _update_display(self, fig: plt.Figure) -> None:
-        if plt.isinteractive():
-            # Required to update render when using Jupyter Notebook.
-            fig.canvas.draw()
-            if jumanji.environments.is_colab():
-                plt.show(self.figure_name)
-        else:
-            # Required to update render when not using Jupyter Notebook.
-            fig.canvas.draw_idle()
-            fig.canvas.flush_events()
-
-    def _clear_display(self) -> None:
-        if jumanji.environments.is_colab():
-            import IPython.display
+        Returns:
+            Spec for the `Observation` whose fields are:
+            - grid: BoundedArray (int32) of shape (num_agents, grid_size, grid_size).
+            - action_mask: BoundedArray (bool) of shape (num_agents, 5).
+            - step_count: BoundedArray (int32) of shape ().
+        """
+        grid = specs.BoundedArray(
+            shape=(self.num_agents, self.grid_size, self.grid_size),
+            dtype=jnp.int32,
+            name="grid",
+            minimum=0,
+            maximum=self.num_agents * 3 + AGENT_INITIAL_VALUE,
+        )
+        action_mask = specs.BoundedArray(
+            shape=(self.num_agents, 5),
+            dtype=bool,
+            minimum=False,
+            maximum=True,
+            name="action_mask",
+        )
+        step_count = specs.BoundedArray(
+            shape=(),
+            dtype=jnp.int32,
+            minimum=0,
+            maximum=self.time_limit,
+            name="step_count",
+        )
+        return specs.Spec(
+            Observation,
+            "ObservationSpec",
+            grid=grid,
+            action_mask=action_mask,
+            step_count=step_count,
+        )
+
+    def action_spec(self) -> specs.MultiDiscreteArray:
+        """Returns the action spec for the Connector environment.
+
+        5 actions: [0,1,2,3,4] -> [No Op, Up, Right, Down, Left]. Since this is a multi-agent
+        environment, the environment expects an array of actions of shape (num_agents,).
 
-            IPython.display.clear_output(True)
+        Returns:
+            observation_spec: `MultiDiscreteArray` of shape (num_agents,).
+        """
+        return specs.MultiDiscreteArray(
+            num_values=jnp.array([5] * self.num_agents),
+            dtype=jnp.int32,
+            name="action",
+        )
+
+    def reward_spec(self) -> specs.Array:
+        """
+        Returns:
+            reward_spec: a `specs.Array` spec of shape (num_agents,). One for each agent.
+        """
+        return specs.Array(shape=(self.num_agents,), dtype=float, name="reward")
+
+    def discount_spec(self) -> specs.BoundedArray:
+        """
+        Returns:
+            discount_spec: a `specs.Array` spec of shape (num_agents,). One for each agent
+        """
+        return specs.BoundedArray(
+            shape=(self.num_agents,),
+            dtype=float,
+            minimum=0.0,
+            maximum=1.0,
+            name="discount",
+        )
```

### Comparing `jumanji-0.2.1/jumanji/environments/logic/rubiks_cube/types.py` & `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING, NamedTuple
 
 import chex
-from chex import Array
 from typing_extensions import TypeAlias
 
 if TYPE_CHECKING:
     from dataclasses import dataclass
 else:
     from chex import dataclass
 
@@ -28,22 +27,19 @@
 
 @dataclass
 class State:
     """
     cube: 3D array whose cells contain the index of the corresponding colour of the sticker in the
         scramble.
     step_count: specifies how many timesteps have elapsed since environment reset.
-    action_history: array that indicates the entire history of applied moves (including those taken
-        on scrambling the cube in the environment reset).
     key: random key used for auto-reset.
     """
 
     cube: Cube  # (6, cube_size, cube_size)
     step_count: chex.Numeric  # ()
-    action_history: Array  # (num_scrambles_on_reset + time_limit, 3)
     key: chex.PRNGKey  # (2,)
 
 
 class Observation(NamedTuple):
     """
     cube: 3D array whose cells contain the index of the corresponding colour of the sticker in the
         scramble.
```

### Comparing `jumanji-0.2.1/jumanji/environments/packing/__init__.py` & `jumanji-0.2.2/jumanji/environments/packing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/bin_pack/__init__.py` & `jumanji-0.2.2/jumanji/environments/packing/bin_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/bin_pack/env.py` & `jumanji-0.2.2/jumanji/environments/packing/bin_pack/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,38 +19,40 @@
 import jax
 import jax.numpy as jnp
 import matplotlib
 from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.packing.bin_pack import env_viewer
 from jumanji.environments.packing.bin_pack.generator import Generator, RandomGenerator
 from jumanji.environments.packing.bin_pack.reward import DenseReward, RewardFn
 from jumanji.environments.packing.bin_pack.space import Space
 from jumanji.environments.packing.bin_pack.types import (
     EMS,
     Item,
     Location,
     Observation,
     State,
     item_fits_in_item,
     item_from_space,
     item_volume,
     space_from_item_and_location,
 )
+from jumanji.environments.packing.bin_pack.viewer import BinPackViewer
 from jumanji.tree_utils import tree_add_element, tree_slice
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
 class BinPack(Environment[State]):
     """Problem of 3D bin packing, where a set of items have to be placed in a 3D container with the
-    goal of maximizing its volume utilization. We use the Empty Maximal Space (EMS) formulation
-    of this problem. An EMS is a 3D-rectangular space that lives inside the container and has the
-    following properties:
+    goal of maximizing its volume utilization. This environment only supports 1 bin, meaning it is
+    equivalent to the 3D-knapsack problem. We use the Empty Maximal Space (EMS) formulation of this
+    problem. An EMS is a 3D-rectangular space that lives inside the container and has the following
+    properties:
         - It does not intersect any items, and it is not fully included into any other EMSs.
         - It is defined by 2 3D-points, hence 6 coordinates (x1, x2, y1, y2, z1, z2),
         the first point corresponding to its bottom-left location while the second defining its
         top-right corner.
 
     - observation: `Observation`
         - ems: `EMS` tree of jax arrays (float if `normalize_dimensions` else int32) each of
@@ -113,15 +115,15 @@
     def __init__(
         self,
         generator: Optional[Generator] = None,
         obs_num_ems: int = 70,
         reward_fn: Optional[RewardFn] = None,
         normalize_dimensions: bool = True,
         debug: bool = False,
-        render_mode: str = "human",
+        viewer: Optional[Viewer[State]] = None,
     ):
         """Instantiates a `BinPack` environment.
 
         Args:
             generator: `Generator` whose `__call__` instantiates an environment
                 instance. Implemented options are [`RandomGenerator`, `ToyGenerator`,
                 `CSVGenerator`]. Defaults to `RandomGenerator` that generates up to 30 items maximum
@@ -137,22 +139,22 @@
                 an episode is the volume utilization of the container. Defaults to `DenseReward`.
             normalize_dimensions: if True, the observation is normalized (float) along each
                 dimension into a unit cubic container. If False, the observation is returned in
                 millimeters, i.e. integers (for both items and EMSs). Default to True.
             debug: if True, will add to timestep.extras an `invalid_ems_from_env` field that checks
                 if an invalid EMS was created by the environment, which should not happen. Computing
                 this metric slows down the environment. Default to False.
-            render_mode: string that defines the mode of rendering.
-                Choices are ["human, "rgb"], defaults to "human".
+            viewer: `Viewer` used for rendering. Defaults to `BinPackViewer` with "human" render
+                mode.
         """
         self.generator = generator or RandomGenerator(max_num_items=30, max_num_ems=100)
         self.obs_num_ems = obs_num_ems
         self.reward_fn = reward_fn or DenseReward()
         self.normalize_dimensions = normalize_dimensions
-        self._env_viewer = env_viewer.BinPackViewer("BinPack", render_mode)
+        self._viewer = viewer or BinPackViewer("BinPack", render_mode="human")
         self.debug = debug
 
     def __repr__(self) -> str:
         return "\n".join(
             [
                 "BinPack environment:",
                 f" - generator: {self.generator}",
@@ -353,15 +355,15 @@
 
     def render(self, state: State) -> Optional[NDArray]:
         """Render the given state of the environment.
 
         Args:
             state: State object containing the current dynamics of the environment.
         """
-        return self._env_viewer.render(state)
+        return self._viewer.render(state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
@@ -372,23 +374,23 @@
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
             animation.FuncAnimation: the animation object that was created.
         """
-        return self._env_viewer.animate(states, interval, save_path)
+        return self._viewer.animate(states, interval, save_path)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self._env_viewer.close()
+        self._viewer.close()
 
     def _make_observation_and_extras(
         self, state: State
     ) -> Tuple[State, Observation, Dict]:
         """Computes the observation and the environment metrics to include in `timestep.extras`. Also
         updates the `action_mask` and `sorted_ems_indexes` in the state. The observation is obtained
         by selecting a subset of all EMSs, namely the `obs_num_ems` largest ones.
```

### Comparing `jumanji-0.2.1/jumanji/environments/packing/bin_pack/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/packing/bin_pack/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 import mpl_toolkits.mplot3d.art3d
 import mpl_toolkits.mplot3d.axes3d
 import numpy as np
 from numpy.typing import NDArray
 
 import jumanji.environments
 from jumanji.environments.packing.bin_pack.types import State, item_from_space
+from jumanji.viewer import Viewer
 
 
-class BinPackViewer:
+class BinPackViewer(Viewer):
     FONT_STYLE = "monospace"
     FIGURE_SIZE = (6.0, 6.0)
 
     def __init__(self, name: str, render_mode: str = "human") -> None:
         """Viewer for the `BinPack` environment.
 
         Args:
```

### Comparing `jumanji-0.2.1/jumanji/environments/packing/bin_pack/generator.py` & `jumanji-0.2.2/jumanji/environments/packing/bin_pack/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/bin_pack/reward.py` & `jumanji-0.2.2/jumanji/environments/packing/bin_pack/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/bin_pack/space.py` & `jumanji-0.2.2/jumanji/environments/packing/bin_pack/space.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/bin_pack/types.py` & `jumanji-0.2.2/jumanji/environments/packing/bin_pack/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/job_shop/__init__.py` & `jumanji-0.2.2/jumanji/environments/packing/job_shop/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/job_shop/env.py` & `jumanji-0.2.2/jumanji/environments/packing/job_shop/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 
 from typing import Any, Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import matplotlib
+from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.packing.job_shop.env_viewer import JobShopViewer
 from jumanji.environments.packing.job_shop.generator import Generator, RandomGenerator
 from jumanji.environments.packing.job_shop.types import Observation, State
+from jumanji.environments.packing.job_shop.viewer import JobShopViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
 class JobShop(Environment[State]):
     """The Job Shop Scheduling Problem, as described in [1], is one of the best known
     combinatorial optimization problems. We are given `num_jobs` jobs, each consisting
     of at most `max_num_ops` ops, which need to be processed on `num_machines` machines.
     Each operation (op) has a specific machine that it needs to be processed on and a
@@ -83,40 +85,44 @@
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
-    def __init__(self, generator: Optional[Generator] = None):
+    def __init__(
+        self,
+        generator: Optional[Generator] = None,
+        viewer: Optional[Viewer[State]] = None,
+    ):
         """Instantiate a `JobShop` environment.
 
         Args:
             generator: `Generator` whose `__call__` instantiates an environment instance.
                 Implemented options are ['ToyGenerator', 'RandomGenerator'].
                 Defaults to `RandomGenerator` with 20 jobs, 10 machines, up to 8 ops
                 for any given job, and a max operation duration of 6.
+            viewer: `Viewer` used for rendering. Defaults to `JobShopViewer`.
         """
-        default_generator = RandomGenerator(
+        self.generator = generator or RandomGenerator(
             num_jobs=20,
             num_machines=10,
             max_num_ops=8,
             max_op_duration=6,
         )
-        self.generator = generator or default_generator
         self.num_jobs = self.generator.num_jobs
         self.num_machines = self.generator.num_machines
         self.max_num_ops = self.generator.max_num_ops
         self.max_op_duration = self.generator.max_op_duration
 
         # Define the "job id" of a no-op action as the number of jobs
         self.no_op_idx = self.num_jobs
 
         # Create viewer used for rendering
-        self._env_viewer = JobShopViewer(
+        self._viewer = viewer or JobShopViewer(
             "JobShop",
             self.num_jobs,
             self.num_machines,
             self.max_num_ops,
             self.max_op_duration,
         )
 
@@ -424,30 +430,30 @@
             action_spec: a `specs.MultiDiscreteArray` spec.
         """
         return specs.MultiDiscreteArray(
             num_values=jnp.full(self.num_machines, self.num_jobs + 1, jnp.int32),
             name="action",
         )
 
-    def render(self, state: State) -> None:
+    def render(self, state: State) -> Optional[NDArray]:
         """Render the given state of the environment. This rendering shows which job (or no-op)
         is running on each machine for the current time step and previous time steps.
 
         Args:
             state: `State` object containing the current environment state.
         """
-        return self._env_viewer.render(state)
+        return self._viewer.render(state)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self._env_viewer.close()
+        self._viewer.close()
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
@@ -458,15 +464,15 @@
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
             animation.FuncAnimation: the animation object that was created.
         """
-        return self._env_viewer.animate(states, interval, save_path)
+        return self._viewer.animate(states, interval, save_path)
 
     def _observation_from_state(self, state: State) -> Observation:
         """Converts a job shop environment state to an observation.
 
         Args:
             state: `State` object containing the dynamics of the environment.
```

### Comparing `jumanji-0.2.1/jumanji/environments/packing/job_shop/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/packing/job_shop/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import matplotlib.animation
 import matplotlib.cm
 import matplotlib.pyplot as plt
 import numpy as np
 
 import jumanji.environments
 from jumanji.environments.packing.job_shop.types import State
+from jumanji.viewer import Viewer
 
 
-class JobShopViewer:
+class JobShopViewer(Viewer):
     FIGURE_SIZE = (15.0, 10.0)
     COLORMAP_NAME = "hsv"
 
     def __init__(
         self,
         name: str,
         num_jobs: int,
```

### Comparing `jumanji-0.2.1/jumanji/environments/packing/job_shop/generator.py` & `jumanji-0.2.2/jumanji/environments/packing/job_shop/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/job_shop/types.py` & `jumanji-0.2.2/jumanji/environments/packing/job_shop/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/knapsack/__init__.py` & `jumanji-0.2.2/jumanji/environments/packing/knapsack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/knapsack/env.py` & `jumanji-0.2.2/jumanji/environments/packing/knapsack/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 import jax
 import jax.numpy as jnp
 import matplotlib
 from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.packing.knapsack.env_viewer import KnapsackViewer
 from jumanji.environments.packing.knapsack.reward import DenseReward, RewardFn
 from jumanji.environments.packing.knapsack.types import Observation, State
+from jumanji.environments.packing.knapsack.viewer import KnapsackViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
 class Knapsack(Environment[State]):
     """Knapsack environment as described in [1].
 
     - observation: Observation
         - weights: jax array (float) of shape (num_items,)
@@ -81,35 +82,35 @@
     """
 
     def __init__(
         self,
         num_items: int = 50,
         total_budget: float = 12.5,
         reward_fn: Optional[RewardFn] = None,
-        render_mode: str = "human",
+        viewer: Optional[Viewer[State]] = None,
     ):
         """Instantiates a `Knapsack` environment.
 
         Args:
             num_items: the number of items in the environment. Defaults to 50.
             total_budget: the capacity of the knapsack. Defaults to 12.5.
             reward_fn: `RewardFn` whose `__call__` method computes the reward of an environment
                 transition. The function must compute the reward based on the current state,
                 the chosen action, the next state and whether the action is valid.
                 Implemented options are [`DenseReward`, `SparseReward`]. Defaults to `DenseReward`.
-            render_mode: string that defines the mode of rendering.
-                Choices are ["human, "rgb"], defaults to "human".
+            viewer: `Viewer` used for rendering. Defaults to `KnapsackViewer` with "human" render
+                mode.
         """
 
         self.num_items = num_items
         self.total_budget = total_budget
         self.reward_fn = reward_fn or DenseReward()
-        self.env_viewer = KnapsackViewer(
+        self._viewer = viewer or KnapsackViewer(
             name="Knapsack",
-            render_mode=render_mode,
+            render_mode="human",
             total_budget=total_budget,
         )
 
     def __repr__(self) -> str:
         return (
             f"Knapsack environment with {self.num_items} items "
             f"and a total budget of {self.total_budget}."
@@ -238,15 +239,15 @@
     def render(self, state: State) -> Optional[NDArray]:
         """Render the environment state, displaying which items have been picked so far,
         their value, and the remaining budget.
 
         Args:
             state: the environment state to be rendered.
         """
-        return self.env_viewer.render(state)
+        return self._viewer.render(state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
@@ -257,23 +258,23 @@
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
             animation.FuncAnimation: the animation object that was created.
         """
-        return self.env_viewer.animate(states, interval, save_path)
+        return self._viewer.animate(states, interval, save_path)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self.env_viewer.close()
+        self._viewer.close()
 
     def _update_state(self, state: State, action: chex.Numeric) -> State:
         """Updates the state of the environment.
 
         Args:
             state: State object containing the dynamics of the environment.
             action: index of the next item to take.
```

### Comparing `jumanji-0.2.1/jumanji/environments/packing/knapsack/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/packing/knapsack/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import matplotlib.animation
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.typing import NDArray
 
 import jumanji.environments
 from jumanji.environments.packing.knapsack.types import State
+from jumanji.viewer import Viewer
 
 
-class KnapsackViewer:
+class KnapsackViewer(Viewer):
     FIGURE_SIZE = (5.0, 5.0)
 
     def __init__(
         self, name: str, render_mode: str = "human", total_budget: float = 2.0
     ) -> None:
         """Viewer for the `Knapsack` environment.
```

### Comparing `jumanji-0.2.1/jumanji/environments/packing/knapsack/reward.py` & `jumanji-0.2.2/jumanji/environments/packing/knapsack/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/packing/knapsack/types.py` & `jumanji-0.2.2/jumanji/environments/packing/knapsack/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/__init__.py` & `jumanji-0.2.2/jumanji/environments/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cleaner/__init__.py` & `jumanji-0.2.2/jumanji/environments/routing/cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cleaner/constants.py` & `jumanji-0.2.2/jumanji/environments/routing/cleaner/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cleaner/env.py` & `jumanji-0.2.2/jumanji/environments/routing/cleaner/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 import jax.numpy as jnp
 import matplotlib
 from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
 from jumanji.environments.routing.cleaner.constants import CLEAN, DIRTY, MOVES, WALL
-from jumanji.environments.routing.cleaner.env_viewer import CleanerViewer
 from jumanji.environments.routing.cleaner.generator import Generator, RandomGenerator
 from jumanji.environments.routing.cleaner.types import Observation, State
+from jumanji.environments.routing.cleaner.viewer import CleanerViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
 class Cleaner(Environment[State]):
     """A JAX implementation of the 'Cleaner' game where multiple agents have to clean all tiles of
     a maze.
 
     - observation: `Observation`
@@ -77,41 +78,43 @@
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        num_agents: int = 3,
         generator: Optional[Generator] = None,
         time_limit: Optional[int] = None,
-        render_mode: str = "human",
         penalty_per_timestep: float = 0.5,
+        viewer: Optional[Viewer[State]] = None,
     ) -> None:
         """Instantiates a `Cleaner` environment.
 
         Args:
             num_agents: number of agents. Defaults to 3.
             time_limit: max number of steps in an episode. Defaults to `num_rows * num_cols`.
             generator: `Generator` whose `__call__` instantiates an environment instance.
                 Implemented options are [`RandomGenerator`]. Defaults to `RandomGenerator` with
-                `num_rows=10` and `num_cols=10`.
-            render_mode: the mode for visualising the environment, can be "human" or "rgb_array".
+                `num_rows=10`, `num_cols=10` and `num_agents=3`.
+            viewer: `Viewer` used for rendering. Defaults to `CleanerViewer` with "human" render
+                mode.
             penalty_per_timestep: the penalty returned at each timestep in the reward.
         """
-        self.num_agents = num_agents
-        self.generator = generator or RandomGenerator(num_rows=10, num_cols=10)
+        self.generator = generator or RandomGenerator(
+            num_rows=10, num_cols=10, num_agents=3
+        )
+        self.num_agents = self.generator.num_agents
         self.num_rows = self.generator.num_rows
         self.num_cols = self.generator.num_cols
         self.grid_shape = (self.num_rows, self.num_cols)
         self.time_limit = time_limit or (self.num_rows * self.num_cols)
         self.penalty_per_timestep = penalty_per_timestep
 
         # Create viewer used for rendering
-        self._env_viewer = CleanerViewer("Cleaner", render_mode)
+        self._viewer = viewer or CleanerViewer("Cleaner", render_mode="human")
 
     def __repr__(self) -> str:
         return (
             f"Cleaner(\n"
             f"\tnum_rows={self.num_rows!r},\n"
             f"\tnum_cols={self.num_cols!r},\n"
             f"\tnum_agents={self.num_agents!r}, \n"
@@ -171,30 +174,21 @@
             key: random key used to reset the environment.
 
         Returns:
             state: `State` object corresponding to the new state of the environment after a reset.
             timestep: `TimeStep` object corresponding to the first timestep returned by the
                 environment after a reset.
         """
-        key, subkey = jax.random.split(key)
-
         # Agents start in upper left corner
         agents_locations = jnp.zeros((self.num_agents, 2), int)
 
-        grid = self.generator(subkey)
-        # Clean the tile in upper left corner
-        grid = self._clean_tiles_containing_agents(grid, agents_locations)
+        state = self.generator(key)
 
-        state = State(
-            grid=grid,
-            agents_locations=agents_locations,
-            action_mask=self._compute_action_mask(grid, agents_locations),
-            step_count=jnp.array(0, jnp.int32),
-            key=key,
-        )
+        # Create the action mask and update the state
+        state.action_mask = self._compute_action_mask(state.grid, agents_locations)
 
         observation = self._observation_from_state(state)
 
         extras = self._compute_extras(state)
         timestep = restart(observation, extras)
 
         return state, timestep
@@ -263,15 +257,15 @@
 
     def render(self, state: State) -> Optional[NDArray]:
         """Render the given state of the environment.
 
         Args:
             state: `State` object containing the current environment state.
         """
-        return self._env_viewer.render(state)
+        return self._viewer.render(state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
@@ -282,23 +276,23 @@
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
             animation.FuncAnimation: the animation object that was created.
         """
-        return self._env_viewer.animate(states, interval, save_path)
+        return self._viewer.animate(states, interval, save_path)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self._env_viewer.close()
+        self._viewer.close()
 
     def _compute_reward(self, prev_state: State, state: State) -> chex.Array:
         """Compute the reward by counting the number of tiles which changed from previous state.
 
         Since walls and dirty tiles do not change, counting the tiles which changed since previeous
         step is the same as counting the tiles which were cleaned.
         """
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cleaner/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/routing/cleaner/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cleaner/generator.py` & `jumanji-0.2.2/jumanji/environments/routing/cleaner/generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,67 +10,88 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import abc
 
 import chex
+import jax
 import jax.numpy as jnp
-from typing_extensions import TypeAlias
 
 from jumanji.environments.commons.maze_utils import maze_generation
-from jumanji.environments.routing.cleaner.constants import DIRTY, WALL
-
-Maze: TypeAlias = chex.Array
+from jumanji.environments.routing.cleaner.constants import CLEAN, DIRTY, WALL
+from jumanji.environments.routing.cleaner.types import State
 
 
 class Generator(abc.ABC):
-    def __init__(self, num_rows: int, num_cols: int):
-        """Interface for maze generation for the `Cleaner` environment.
+    def __init__(self, num_rows: int, num_cols: int, num_agents: int) -> None:
+        """Interface for instance generation for the `Cleaner` environment.
 
         Args:
-            num_rows: the width of the maze to create.
-            num_cols: the length of the maze to create.
+            num_rows: the width of the grid to create.
+            num_cols: the length of the grid to create.
+            num_agents: the number of agents.
         """
         self.num_rows = num_rows
         self.num_cols = num_cols
+        self.num_agents = num_agents
 
     @abc.abstractmethod
-    def __call__(self, key: chex.PRNGKey) -> Maze:
+    def __call__(self, key: chex.PRNGKey) -> State:
         """Generate a problem instance for the `Cleaner` environment.
 
         Args:
             key: random key.
 
         Returns:
-            A `Maze` representing a problem instance.
+            An initial `State` representing a problem instance.
         """
 
 
 class RandomGenerator(Generator):
-    def __init__(self, num_rows: int, num_cols: int) -> None:
-        super(RandomGenerator, self).__init__(num_rows=num_rows, num_cols=num_cols)
+    def __init__(self, num_rows: int, num_cols: int, num_agents: int) -> None:
+        super(RandomGenerator, self).__init__(
+            num_rows=num_rows, num_cols=num_cols, num_agents=num_agents
+        )
 
-    def __call__(self, key: chex.PRNGKey) -> Maze:
-        """Generate a random maze.
+    def __call__(self, key: chex.PRNGKey) -> State:
+        """Generate a random instance of the cleaner environment.
 
         This method relies on the `generate_maze` method from the `maze_generation` module to
         generate a maze. This generated maze has its own specific values to represent empty tiles
         and walls. Here, they are replaced respectively with DIRTY and WALL to match the values
         of the cleaner environment.
 
         Args:
             key: the Jax random number generation key.
 
         Returns:
-            maze: the generated maze.
+            state: the generated state.
         """
-        maze = maze_generation.generate_maze(self.num_rows, self.num_cols, key)
-        return self._adapt_values(maze)
+        generator_key, state_key = jax.random.split(key)
+        maze = maze_generation.generate_maze(
+            self.num_rows, self.num_cols, generator_key
+        )
+
+        grid = self._adapt_values(maze)
+
+        # Agents start in upper left corner
+        agents_locations = jnp.zeros((self.num_agents, 2), jnp.int32)
+
+        # Clean the tile in upper left corner
+        grid = grid.at[0, 0].set(CLEAN)
+
+        return State(
+            grid=grid,
+            agents_locations=agents_locations,
+            action_mask=None,
+            step_count=jnp.array(0, jnp.int32),
+            key=state_key,
+        )
 
-    def _adapt_values(self, maze: Maze) -> Maze:
+    def _adapt_values(self, maze: chex.Array) -> chex.Array:
         """Adapt the values of the maze from maze_generation to agent cleaner."""
         maze = jnp.where(maze == maze_generation.EMPTY, DIRTY, maze)
         # This line currently doesn't do anything, but avoid breaking this function if either of
         # maze_generation.WALL or WALL is changed.
         maze = jnp.where(maze == maze_generation.WALL, WALL, maze)
         return maze
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cleaner/types.py` & `jumanji-0.2.2/jumanji/environments/routing/cleaner/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, NamedTuple
+from typing import TYPE_CHECKING, NamedTuple, Optional
 
 import chex
 import jax.numpy as jnp
 
 if TYPE_CHECKING:
     from dataclasses import dataclass
 else:
@@ -33,16 +33,16 @@
     action_mask: boolean array specifying, for each agent, which action
         (up, right, down, left) is legal.
     step_count: the number of steps elapsed since the beginning of the episode.
     key: random key used for auto-reset.
     """
 
     grid: chex.Array  # (num_rows, num_cols)
-    agents_locations: chex.Array  # (num_agent, 2)
-    action_mask: chex.Array  # (num_agent, 4)
+    agents_locations: chex.Array  # (num_agents, 2)
+    action_mask: Optional[chex.Array]  # (num_agents, 4)
     step_count: jnp.int32  # ()
     key: chex.PRNGKey  # (2,)
 
 
 class Observation(NamedTuple):
     """The observation that the agent sees.
 
@@ -51,10 +51,10 @@
     agents_locations: array which specifies the x and y coordinates of every agent.
     action_mask: boolean array specifying, for each agent, which action
         (up, right, down, left) is legal.
     step_count: the number of steps elapsed since the beginning of the episode.
     """
 
     grid: chex.Array  # (num_rows, num_cols)
-    agents_locations: chex.Array  # (num_agent, 2)
-    action_mask: chex.Array  # (num_agent, 4)
+    agents_locations: chex.Array  # (num_agents, 2)
+    action_mask: chex.Array  # (num_agents, 4)
     step_count: jnp.int32  # ()
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/__init__.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/constants.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/env.py` & `jumanji-0.2.2/jumanji/environments/routing/cvrp/env.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,401 +8,371 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Dict, Optional, Sequence, Tuple
+from typing import Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import matplotlib
-from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.routing.connector.constants import (
-    AGENT_INITIAL_VALUE,
-    NOOP,
-    PATH,
-)
-from jumanji.environments.routing.connector.env_viewer import ConnectorViewer
-from jumanji.environments.routing.connector.generator import (
-    Generator,
-    UniformRandomGenerator,
-)
-from jumanji.environments.routing.connector.reward import DenseRewardFn, RewardFn
-from jumanji.environments.routing.connector.types import Agent, Observation, State
-from jumanji.environments.routing.connector.utils import (
-    connected_or_blocked,
-    get_agent_grid,
-    get_correction_mask,
-    is_valid_position,
-    move_agent,
-    move_position,
-    switch_perspective,
-)
+from jumanji.environments.routing.cvrp.constants import DEPOT_IDX
+from jumanji.environments.routing.cvrp.reward import DenseReward, RewardFn
+from jumanji.environments.routing.cvrp.types import Observation, State
+from jumanji.environments.routing.cvrp.viewer import CVRPViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
-class Connector(Environment[State]):
-    """The `Connector` environment is a multi-agent gridworld problem where each agent must connect a
-    start to a target. However, when moving through this gridworld the agent leaves an impassable
-    trail behind it. Therefore, agents must connect to their targets without overlapping the routes
-    taken by any other agent.
-
-    - observation - `Observation`
-        - action mask: jax array (bool) of shape (num_agents, 5).
-        - step_count: jax array (int32) of shape ()
-            the current episode step.
-        - grid: jax array (int32) of shape (num_agents, size, size)
-            - each 2d array (size, size) along axis 0 is the agent's local observation.
-            - agents have ids from 0 to (num_agents - 1)
-            - with 2 agents you might have a grid like this:
-              4 0 1
-              5 0 1
-              6 3 2
-              which means agent 1 has moved from the top right of the grid down and is currently in
-              the bottom right corner and is aiming to get to the middle bottom cell. Agent 2
-              started in the top left and moved down once towards its target in the bottom left.
-
-              This would just be agent 0's view, the numbers would be flipped for agent 1's view.
-              So the full observation would be of shape (2, 3, 3).
-
-    - action: jax array (int32) of shape (num_agents,):
-        - can take the values [0,1,2,3,4] which correspond to [No Op, Up, Right, Down, Left].
-        - each value in the array corresponds to an agent's action.
-
-    - reward: jax array (float) of shape ():
-        - dense: each agent is given 1.0 if it connects on that step, otherwise 0.0. Additionally,
-            each agent that has not connected receives a penalty reward of -0.03.
-
-    - episode termination: if an agent can't move, or the time limit is reached, or the agent
-        connects to its target, it is considered done. Once all agents are done, the episode
-        terminates. The timestep discounts are of shape (num_agents,).
-
-    - state: State:
-        - key: jax PRNG key used to randomly spawn agents and targets.
-        - grid: jax array (int32) of shape (size, size) which corresponds to agent 0's observation.
-        - step_count: jax array (int32) of shape () number of steps elapsed in the current episode.
+class CVRP(Environment[State]):
+    """Capacitated Vehicle Routing Problem (CVRP) environment as described in [1].
+
+    - observation: `Observation`
+        - coordinates: jax array (float) of shape (num_nodes + 1, 2)
+            the coordinates of each node and the depot.
+        - demands: jax array (float) of shape (num_nodes + 1,)
+            the associated cost of each node and the depot (0.0 for the depot).
+        - unvisited_nodes: jax array (bool) of shape (num_nodes + 1,)
+            indicates nodes that remain to be visited.
+        - position: jax array (int32) of shape ()
+            the index of the last visited node.
+        - trajectory: jax array (int32) of shape (2 * num_nodes,)
+            array of node indices defining the route (set to DEPOT_IDX if not filled yet).
+        - capacity: jax array (float) of shape ()
+            the current capacity of the vehicle.
+        - action_mask: jax array (bool) of shape (num_nodes + 1,)
+            binary mask (False/True <--> invalid/valid action).
+
+    - action: jax array (int32) of shape ()
+        [0, ..., num_nodes] -> node to visit. 0 corresponds to visiting the depot.
+
+    - reward: jax array (float) of shape (), could be either:
+        - dense: the negative distance between the current node and the chosen next node to go to.
+            For the last node, it also includes the distance to the depot to complete the tour.
+        - sparse: the negative tour length at the end of the episode. The tour length is defined
+            as the sum of the distances between consecutive nodes.
+        In both cases, the reward is a large negative penalty of `-2 * num_nodes * sqrt(2)` if the
+        action is invalid, e.g. a previously selected node other than the depot is selected again.
+
+    - episode termination:
+        - if no action can be performed, i.e. all nodes have been visited.
+        - if an invalid action is taken, i.e. a previously visited city other than the depot is
+            chosen.
+
+    - state: `State`
+        - coordinates: jax array (float) of shape (num_nodes + 1, 2)
+            the coordinates of each node and the depot.
+        - demands: jax array (int32) of shape (num_nodes + 1,)
+            the associated cost of each node and the depot (0.0 for the depot).
+        - position: jax array (int32)
+            the index of the last visited node.
+        - capacity: jax array (int32)
+            the current capacity of the vehicle.
+        - visited_mask: jax array (bool) of shape (num_nodes + 1,)
+            binary mask (False/True <--> not visited/visited).
+        - trajectory: jax array (int32) of shape (2 * num_nodes,)
+            identifiers of the nodes that have been visited (set to DEPOT_IDX if not filled yet).
+        - num_visits: int32
+            number of actions that have been taken (i.e., unique visits).
+
+    [1] Toth P., Vigo D. (2014). "Vehicle routing: problems, methods, and applications".
 
     ```python
-    from jumanji.environments import Connector
-    env = Connector()
+    from jumanji.environments import CVRP
+    env = CVRP()
     key = jax.random.key(0)
     state, timestep = jax.jit(env.reset)(key)
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        generator: Optional[Generator] = None,
+        num_nodes: int = 20,
+        max_capacity: int = 30,
+        max_demand: int = 10,
         reward_fn: Optional[RewardFn] = None,
-        time_limit: int = 50,
-        render_mode: str = "human",
-    ) -> None:
-        """Create the `Connector` environment.
+        viewer: Optional[Viewer[State]] = None,
+    ):
+        """Instantiates a `CVRP` environment.
 
         Args:
-            generator: `Generator` whose `__call__` instantiates an environment instance.
-                Implemented options are [`UniformRandomGenerator`].
-                Defaults to `UniformRandomGenerator` with `grid_size=10` and `num_agents=5`.
-            reward_fn: class of type `RewardFn`, whose `__call__` is used as a reward function.
-                Implemented options are [`DenseRewardFn`]. Defaults to `DenseRewardFn`.
-            time_limit: the number of steps allowed before an episode terminates. Defaults to 50.
+            num_nodes: number of city nodes in the environment. Defaults to 20.
+            max_capacity: maximum capacity of the vehicle. Defaults to 30.
+            max_demand: maximum demand of each node. Defaults to 10.
+            reward_fn: `RewardFn` whose `__call__` method computes the reward of an environment
+                transition. The function must compute the reward based on the current state,
+                the chosen action, the next state and whether the action is valid.
+                Implemented options are [`DenseReward`, `SparseReward`]. Defaults to `DenseReward`.
+            viewer: `Viewer` used for rendering. Defaults to `CVRPViewer` with "human" render mode.
         """
-        self._generator = generator or UniformRandomGenerator(
-            grid_size=10, num_agents=5
+
+        if max_capacity < max_demand:
+            raise ValueError(
+                f"The demand associated with each node must be lower than the maximum capacity, "
+                f"hence the maximum capacity must be >= {max_demand}."
+            )
+        self.num_nodes = num_nodes
+        self.max_capacity = max_capacity
+        self.max_demand = max_demand
+        self.reward_fn = reward_fn or DenseReward()
+        self._viewer = viewer or CVRPViewer(
+            name="CVRP",
+            num_cities=self.num_nodes,
+            render_mode="human",
+        )
+
+    def __repr__(self) -> str:
+        return (
+            f"CVRP(num_nodes={self.num_nodes}, max_capacity={self.max_capacity}, "
+            f"max_demand={self.max_demand})"
         )
-        self._reward_fn = reward_fn or DenseRewardFn()
-        self.time_limit = time_limit
-        self.num_agents = self._generator.num_agents
-        self.grid_size = self._generator.grid_size
-        self._agent_ids = jnp.arange(self.num_agents)
-        self._renderer = ConnectorViewer("Connector", self.num_agents, render_mode)
 
     def reset(self, key: chex.PRNGKey) -> Tuple[State, TimeStep[Observation]]:
         """Resets the environment.
 
         Args:
-            key: used to randomly generate the connector grid.
+            key: used to randomly generate the coordinates.
 
         Returns:
-            state: `State` object corresponding to the new state of the environment.
-            timestep: `TimeStep` object corresponding to the initial environment timestep.
-        """
-        state = self._generator(key)
-
-        action_mask = jax.vmap(self._get_action_mask, (0, None))(
-            state.agents, state.grid
-        )
-        observation = Observation(
-            grid=self._obs_from_grid(state.grid),
-            action_mask=action_mask,
-            step_count=state.step_count,
-        )
-        extras = self._get_extras(state)
-        timestep = restart(
-            observation=observation, extras=extras, shape=(self.num_agents,)
+             state: `State` object corresponding to the new state of the environment.
+             timestep: `TimeStep` object corresponding to the first timestep returned by the
+                environment.
+        """
+        key, coordinates_key, demands_key = jax.random.split(key, 3)
+        coordinates = jax.random.uniform(
+            coordinates_key, (self.num_nodes + 1, 2), minval=0, maxval=1
+        )
+        demands = jax.random.randint(
+            demands_key, (self.num_nodes + 1,), minval=1, maxval=self.max_demand
+        )
+        demands = demands.at[DEPOT_IDX].set(0)
+        visited_mask = jnp.zeros(self.num_nodes + 1, dtype=bool).at[DEPOT_IDX].set(True)
+        state = State(
+            coordinates=coordinates,
+            demands=demands,
+            position=jnp.array(DEPOT_IDX, jnp.int32),
+            capacity=jnp.array(self.max_capacity, jnp.int32),
+            visited_mask=visited_mask,
+            trajectory=jnp.full(2 * self.num_nodes, DEPOT_IDX, jnp.int32),
+            num_total_visits=jnp.array(1, jnp.int32),
+            key=key,
         )
+        timestep = restart(observation=self._state_to_observation(state))
         return state, timestep
 
     def step(
-        self, state: State, action: chex.Array
+        self, state: State, action: chex.Numeric
     ) -> Tuple[State, TimeStep[Observation]]:
-        """Perform an environment step.
+        """Run one timestep of the environment's dynamics.
 
         Args:
-            state: State object containing the dynamics of the environment.
-            action: Array containing the actions to take for each agent.
-                - 0 no op
-                - 1 move up
-                - 2 move right
-                - 3 move down
-                - 4 move left
+            state: `State` object containing the dynamics of the environment.
+            action: jax array (int32) of shape () containing the index of the next node to visit.
 
         Returns:
-            state: `State` object corresponding to the next state of the environment.
-            timestep: `TimeStep` object corresponding the timestep returned by the environment.
+            state, timestep: next state of the environment and timestep to be observed.
         """
-        agents, grid = self._step_agents(state, action)
-        new_state = State(
-            grid=grid, step_count=state.step_count + 1, agents=agents, key=state.key
-        )
-
-        # Construct timestep: get observations, rewards, discounts
-        grids = self._obs_from_grid(grid)
-        reward = self._reward_fn(state, action, new_state)
-        action_mask = jax.vmap(self._get_action_mask, (0, None))(agents, grid)
-        observation = Observation(
-            grid=grids, action_mask=action_mask, step_count=new_state.step_count
-        )
-
-        dones = jax.vmap(connected_or_blocked)(agents, action_mask)
-        discount = jnp.asarray(jnp.logical_not(dones), dtype=float)
-        extras = self._get_extras(new_state)
+        node_demand = state.demands[action]
+        node_is_visited = state.visited_mask[action]
+        is_valid = ~node_is_visited & (state.capacity >= node_demand)
+
+        next_state = jax.lax.cond(
+            is_valid,
+            self._update_state,
+            lambda *_: state,
+            state,
+            action,
+        )
+
+        reward = self.reward_fn(state, action, next_state, is_valid)
+        observation = self._state_to_observation(next_state)
+
+        # Terminate if all nodes have been visited or the action is invalid.
+        is_done = next_state.visited_mask.all() | ~is_valid
+
         timestep = jax.lax.cond(
-            dones.all() | (new_state.step_count >= self.time_limit),
-            lambda: termination(
-                reward=reward,
-                observation=observation,
-                extras=extras,
-                shape=self.num_agents,
-            ),
-            lambda: transition(
-                reward=reward,
-                observation=observation,
-                discount=discount,
-                extras=extras,
-                shape=self.num_agents,
-            ),
-        )
-
-        return new_state, timestep
-
-    def _step_agents(
-        self, state: State, action: chex.Array
-    ) -> Tuple[Agent, chex.Array]:
-        """Steps all agents at the same time correcting for possible collisions.
+            is_done,
+            termination,
+            transition,
+            reward,
+            observation,
+        )
+        return next_state, timestep
 
-        If a collision occurs we place the agent with the lower `agent_id` in its previous position.
+    def observation_spec(self) -> specs.Spec[Observation]:
+        """Returns the observation spec.
 
         Returns:
-            Tuple: (agents, grid) after having applied each agents' action
+            Spec for the `Observation` whose fields are:
+            - coordinates: BoundedArray (float) of shape (num_nodes + 1, 2).
+            - demands: BoundedArray (float) of shape (num_nodes + 1,).
+            - unvisited_nodes: BoundedArray (bool) of shape (num_nodes + 1,).
+            - position: DiscreteArray (num_values = num_nodes + 1) of shape ().
+            - trajectory: BoundedArray (int32) of shape (2 * num_nodes,).
+            - capacity: BoundedArray (float) of shape ().
+            - action_mask: BoundedArray (bool) of shape (num_nodes + 1,).
         """
-        agent_ids = jnp.arange(self.num_agents)
-        # Step all agents at the same time (separately) and return all of the grids
-        agents, grids = jax.vmap(self._step_agent, in_axes=(0, None, 0))(
-            state.agents, state.grid, action
-        )
-
-        # Get grids with only values related to a single agent.
-        # For example: remove all other agents from agent 1's grid. Do this for all agents.
-        agent_grids = jax.vmap(get_agent_grid)(agent_ids, grids)
-        joined_grid = jnp.max(agent_grids, 0)  # join the grids
-
-        # Create a correction mask for possible collisions (see the docs of `get_correction_mask`)
-        correction_fn = jax.vmap(get_correction_mask, in_axes=(None, None, 0))
-        correction_masks, collided_agents = correction_fn(
-            state.grid, joined_grid, agent_ids
-        )
-        correction_mask = jnp.sum(correction_masks, 0)
-
-        # Correct state.agents
-        # Get the correct agents, either old agents (if collision) or new agents if no collision
-        agents = jax.vmap(
-            lambda collided, old_agent, new_agent: jax.lax.cond(
-                collided,
-                lambda: old_agent,
-                lambda: new_agent,
-            )
-        )(collided_agents, state.agents, agents)
-        # Create the new grid by fixing old one with correction mask and adding the obstacles
-        return agents, joined_grid + correction_mask
-
-    def _step_agent(
-        self, agent: Agent, grid: chex.Array, action: chex.Numeric
-    ) -> Tuple[Agent, chex.Array]:
-        """Moves the agent according to the given action if it is possible.
+        coordinates = specs.BoundedArray(
+            shape=(self.num_nodes + 1, 2),
+            minimum=0.0,
+            maximum=1.0,
+            dtype=float,
+            name="coordinates",
+        )
+        demands = specs.BoundedArray(
+            shape=(self.num_nodes + 1,),
+            minimum=0.0,
+            maximum=1.0,
+            dtype=float,
+            name="demands",
+        )
+        unvisited_nodes = specs.BoundedArray(
+            shape=(self.num_nodes + 1,),
+            dtype=bool,
+            minimum=False,
+            maximum=True,
+            name="unvisited_nodes",
+        )
+        position = specs.DiscreteArray(
+            self.num_nodes + 1, dtype=jnp.int32, name="position"
+        )
+        trajectory = specs.BoundedArray(
+            shape=(2 * self.num_nodes,),
+            minimum=0,
+            maximum=self.num_nodes + 1,
+            dtype=jnp.int32,
+            name="trajectory",
+        )
+        capacity = specs.BoundedArray(
+            shape=(), minimum=0.0, maximum=1.0, dtype=float, name="capacity"
+        )
+        action_mask = specs.BoundedArray(
+            shape=(self.num_nodes + 1,),
+            dtype=bool,
+            minimum=False,
+            maximum=True,
+            name="action_mask",
+        )
+        return specs.Spec(
+            Observation,
+            "ObservationSpec",
+            coordinates=coordinates,
+            demands=demands,
+            unvisited_nodes=unvisited_nodes,
+            position=position,
+            trajectory=trajectory,
+            capacity=capacity,
+            action_mask=action_mask,
+        )
+
+    def action_spec(self) -> specs.DiscreteArray:
+        """Returns the action spec.
 
         Returns:
-            Tuple: (agent, grid) after having applied the given action.
+            action_spec: a `specs.DiscreteArray` spec.
         """
-        new_pos = move_position(agent.position, action)
-
-        new_agent, new_grid = jax.lax.cond(
-            is_valid_position(grid, agent, new_pos) & (action != NOOP),
-            move_agent,
-            lambda *_: (agent, grid),
-            agent,
-            grid,
-            new_pos,
-        )
-
-        return new_agent, new_grid
-
-    def _obs_from_grid(self, grid: chex.Array) -> chex.Array:
-        """Gets the observation vector for all agents."""
-        return jax.vmap(switch_perspective, (None, 0, None))(
-            grid, self._agent_ids, self.num_agents
-        )
-
-    def _get_action_mask(self, agent: Agent, grid: chex.Array) -> chex.Array:
-        """Gets an agent's action mask."""
-        # Don't check action 0 because no-op is always valid
-        actions = jnp.arange(1, 5)
-
-        def is_valid_action(action: int) -> chex.Array:
-            agent_pos = move_position(agent.position, action)
-            return is_valid_position(grid, agent, agent_pos)
-
-        mask = jnp.ones(5, dtype=bool)
-        mask = mask.at[actions].set(jax.vmap(is_valid_action)(actions))
-        return mask
-
-    def _get_extras(self, state: State) -> Dict:
-        """Computes extras metrics to be return within the timestep."""
-        offset = AGENT_INITIAL_VALUE
-        total_path_length = jnp.sum((offset + (state.grid - offset) % 3) == PATH)
-        # Add agents' head
-        total_path_length += self.num_agents
-        extras = {
-            "num_connections": jnp.sum(state.agents.connected),
-            "ratio_connections": jnp.mean(state.agents.connected),
-            "total_path_length": total_path_length,
-        }
-        return extras
+        return specs.DiscreteArray(self.num_nodes + 1, name="action")
 
-    def render(self, state: State) -> Optional[NDArray]:
-        """Render the given state of the environment.
+    def render(self, state: State) -> Optional[chex.ArrayNumpy]:
+        """Render the given state of the environment. This rendering shows the layout of the tour so
+         far with the cities as circles, and the depot as a square.
 
         Args:
-            state: `State` object containing the current environment state.
+            state: environment state to render.
+
+        Returns:
+            rgb_array: the RGB image of the state as an array.
         """
-        return self._renderer.render(state.grid)
+        return self._viewer.render(state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
-        """Create an animation from a sequence of states.
+        """Creates an animated gif of the CVRP environment based on the sequence of states.
 
         Args:
-            states: sequence of `State` corresponding to subsequent timesteps.
+            states: sequence of environment states corresponding to consecutive timesteps.
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
-            animation that can export to gif, mp4, or render with HTML.
+            animation.FuncAnimation: the animation object that was created.
         """
-        grids = [state.grid for state in states]
-        return self._renderer.animate(grids, interval, save_path)
+        return self._viewer.animate(states, interval, save_path)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self._renderer.close()
-
-    def observation_spec(self) -> specs.Spec[Observation]:
-        """Specifications of the observation of the `Connector` environment.
-
-        Returns:
-            Spec for the `Observation` whose fields are:
-            - grid: BoundedArray (int32) of shape (num_agents, grid_size, grid_size).
-            - action_mask: BoundedArray (bool) of shape (num_agents, 5).
-            - step_count: BoundedArray (int32) of shape ().
-        """
-        grid = specs.BoundedArray(
-            shape=(self.num_agents, self.grid_size, self.grid_size),
-            dtype=jnp.int32,
-            name="grid",
-            minimum=0,
-            maximum=self.num_agents * 3 + AGENT_INITIAL_VALUE,
-        )
-        action_mask = specs.BoundedArray(
-            shape=(self.num_agents, 5),
-            dtype=bool,
-            minimum=False,
-            maximum=True,
-            name="action_mask",
-        )
-        step_count = specs.BoundedArray(
-            shape=(),
-            dtype=jnp.int32,
-            minimum=0,
-            maximum=self.time_limit,
-            name="step_count",
-        )
-        return specs.Spec(
-            Observation,
-            "ObservationSpec",
-            grid=grid,
-            action_mask=action_mask,
-            step_count=step_count,
-        )
+        self._viewer.close()
 
-    def action_spec(self) -> specs.MultiDiscreteArray:
-        """Returns the action spec for the Connector environment.
+    def _update_state(self, state: State, action: chex.Numeric) -> State:
+        """Updates the state of the environment.
 
-        5 actions: [0,1,2,3,4] -> [No Op, Up, Right, Down, Left]. Since this is a multi-agent
-        environment, the environment expects an array of actions of shape (num_agents,).
+        Args:
+            state: State object containing the dynamics of the environment.
+            action: int32, index of the next node to visit.
 
         Returns:
-            observation_spec: `MultiDiscreteArray` of shape (num_agents,).
+            state: State object corresponding to the new state of the environment.
         """
-        return specs.MultiDiscreteArray(
-            num_values=jnp.array([5] * self.num_agents),
-            dtype=jnp.int32,
-            name="action",
+        capacity = jax.lax.select(
+            action == DEPOT_IDX,
+            self.max_capacity,
+            state.capacity - state.demands[action],
+        )
+
+        # Set depot to False (valid to visit) since it can be visited multiple times
+        visited_mask = state.visited_mask.at[DEPOT_IDX].set(False)
+
+        return State(
+            coordinates=state.coordinates,
+            demands=state.demands,
+            position=action,
+            capacity=capacity,
+            visited_mask=visited_mask.at[action].set(True),
+            trajectory=state.trajectory.at[state.num_total_visits].set(action),
+            num_total_visits=state.num_total_visits + 1,
+            key=state.key,
         )
 
-    def reward_spec(self) -> specs.Array:
-        """
-        Returns:
-            reward_spec: a `specs.Array` spec of shape (num_agents,). One for each agent.
-        """
-        return specs.Array(shape=(self.num_agents,), dtype=float, name="reward")
+    def _state_to_observation(self, state: State) -> Observation:
+        """Converts a state into an observation.
+
+        Args:
+            state: `State` object containing the dynamics of the environment.
 
-    def discount_spec(self) -> specs.BoundedArray:
-        """
         Returns:
-            discount_spec: a `specs.Array` spec of shape (num_agents,). One for each agent
+            observation: `Observation` object containing the observation of the environment.
         """
-        return specs.BoundedArray(
-            shape=(self.num_agents,),
-            dtype=float,
-            minimum=0.0,
-            maximum=1.0,
-            name="discount",
+        # A node is not reachable if it has already been visited or if the vehicle does not have
+        # enough capacity to cover its demand.
+        action_mask = ~state.visited_mask & (state.capacity >= state.demands)
+
+        # The depot is reachable if we are not at it already.
+        action_mask = action_mask.at[DEPOT_IDX].set(state.position != DEPOT_IDX)
+
+        return Observation(
+            coordinates=state.coordinates,
+            demands=jnp.asarray(state.demands / self.max_capacity, float),
+            unvisited_nodes=~state.visited_mask,
+            position=state.position,
+            trajectory=state.trajectory,
+            capacity=jnp.asarray(state.capacity / self.max_capacity, float),
+            action_mask=action_mask,
         )
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 
 import jumanji.environments
 from jumanji.environments.routing.connector.utils import (
     get_agent_id,
     is_path,
     is_target,
 )
+from jumanji.viewer import Viewer
 
 
-class ConnectorViewer:
+class ConnectorViewer(Viewer):
     FIGURE_SIZE = (10.0, 10.0)
 
     def __init__(self, name: str, num_agents: int, render_mode: str = "human") -> None:
         """
         Viewer for a `Connector` environment.
 
         Args:
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/generator.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/reward.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/types.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/connector/utils.py` & `jumanji-0.2.2/jumanji/environments/routing/connector/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cvrp/__init__.py` & `jumanji-0.2.2/jumanji/environments/routing/cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cvrp/constants.py` & `jumanji-0.2.2/jumanji/environments/routing/cvrp/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cvrp/env.py` & `jumanji-0.2.2/jumanji/environments/routing/tsp/env.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,365 +14,288 @@
 
 from typing import Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import matplotlib
+from chex import PRNGKey
+from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.routing.cvrp.constants import DEPOT_IDX
-from jumanji.environments.routing.cvrp.env_viewer import CVRPViewer
-from jumanji.environments.routing.cvrp.reward import DenseReward, RewardFn
-from jumanji.environments.routing.cvrp.types import Observation, State
+from jumanji.environments.routing.tsp.reward import DenseReward, RewardFn
+from jumanji.environments.routing.tsp.types import Observation, State
+from jumanji.environments.routing.tsp.viewer import TSPViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
-class CVRP(Environment[State]):
-    """Capacitated Vehicle Routing Problem (CVRP) environment as described in [1].
+class TSP(Environment[State]):
+    """Traveling Salesman Problem (TSP) environment as described in [1].
 
-    - observation: `Observation`
-        - coordinates: jax array (float) of shape (num_nodes + 1, 2)
-            the coordinates of each node and the depot.
-        - demands: jax array (float) of shape (num_nodes + 1,)
-            the associated cost of each node and the depot (0.0 for the depot).
-        - unvisited_nodes: jax array (bool) of shape (num_nodes + 1,)
-            indicates nodes that remain to be visited.
-        - position: jax array (int32) of shape ()
-            the index of the last visited node.
-        - trajectory: jax array (int32) of shape (2 * num_nodes,)
-            array of node indices defining the route (set to DEPOT_IDX if not filled yet).
-        - capacity: jax array (float) of shape ()
-            the current capacity of the vehicle.
-        - action_mask: jax array (bool) of shape (num_nodes + 1,)
-            binary mask (False/True <--> invalid/valid action).
+    - observation: Observation
+        - coordinates: jax array (float) of shape (num_cities, 2)
+            the coordinates of each city.
+        - position: jax array (int32)  of shape ()
+            the index corresponding to the last visited city.
+        - trajectory: jax array (int32) of shape (num_cities,)
+            array of city indices defining the route (-1 --> not filled yet).
+        - action_mask: jax array (bool) of shape (num_cities,)
+            binary mask (False/True <--> illegal/legal <--> cannot be visited/can be visited).
 
     - action: jax array (int32) of shape ()
-        [0, ..., num_nodes] -> node to visit. 0 corresponds to visiting the depot.
+        [0, ..., num_cities - 1] -> city to visit.
 
     - reward: jax array (float) of shape (), could be either:
-        - dense: the negative distance between the current node and the chosen next node to go to.
-            For the last node, it also includes the distance to the depot to complete the tour.
+        - dense: the negative distance between the current city and the chosen next city to go to.
+            It is 0 for the first chosen city, and for the last city, it also includes the distance
+            to the initial city to complete the tour.
         - sparse: the negative tour length at the end of the episode. The tour length is defined
-            as the sum of the distances between consecutive nodes.
-        In both cases, the reward is a large negative penalty of `-2 * num_nodes * sqrt(2)` if the
-        action is invalid, e.g. a previously selected node other than the depot is selected again.
+            as the sum of the distances between consecutive cities. It is computed by starting at
+            the first city and ending there, after visiting all the cities.
+        In both cases, the reward is a large negative penalty of `-num_cities * sqrt(2)` if
+        the action is invalid, i.e. a previously selected city is selected again.
 
     - episode termination:
-        - if no action can be performed, i.e. all nodes have been visited.
-        - if an invalid action is taken, i.e. a previously visited city other than the depot is
-            chosen.
+        - if no action can be performed, i.e. all cities have been visited.
+        - if an invalid action is taken, i.e. an already visited city is chosen.
 
     - state: `State`
-        - coordinates: jax array (float) of shape (num_nodes + 1, 2)
-            the coordinates of each node and the depot.
-        - demands: jax array (int32) of shape (num_nodes + 1,)
-            the associated cost of each node and the depot (0.0 for the depot).
-        - position: jax array (int32)
-            the index of the last visited node.
-        - capacity: jax array (int32)
-            the current capacity of the vehicle.
-        - visited_mask: jax array (bool) of shape (num_nodes + 1,)
+        - coordinates: jax array (float) of shape (num_cities, 2)
+            the coordinates of each city.
+        - position: int32
+            the identifier (index) of the last visited city.
+        - visited_mask: jax array (bool) of shape (num_cities,)
             binary mask (False/True <--> not visited/visited).
-        - trajectory: jax array (int32) of shape (2 * num_nodes,)
-            identifiers of the nodes that have been visited (set to DEPOT_IDX if not filled yet).
-        - num_visits: int32
-            number of actions that have been taken (i.e., unique visits).
+        - trajectory: jax array (int32) of shape (num_cities,)
+            the identifiers of the cities that have been visited (-1 means that no city has been
+            visited yet at that time in the sequence).
+        - num_visited: int32
+            number of cities that have been visited.
 
-    [1] Toth P., Vigo D. (2014). "Vehicle routing: problems, methods, and applications".
+    [1] Kwon Y., Choo J., Kim B., Yoon I., Min S., Gwon Y. (2020). "POMO: Policy Optimization
+        with Multiple Optima for Reinforcement Learning".
 
     ```python
-    from jumanji.environments import CVRP
-    env = CVRP()
+    from jumanji.environments import TSP
+    env = TSP()
     key = jax.random.key(0)
     state, timestep = jax.jit(env.reset)(key)
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        num_nodes: int = 20,
-        max_capacity: int = 30,
-        max_demand: int = 10,
+        num_cities: int = 20,
         reward_fn: Optional[RewardFn] = None,
-        render_mode: str = "human",
+        viewer: Optional[Viewer[State]] = None,
     ):
-        """Instantiates a `CVRP` environment.
+        """Instantiates a `TSP` environment.
 
         Args:
-            num_nodes: number of city nodes in the environment. Defaults to 20.
-            max_capacity: maximum capacity of the vehicle. Defaults to 30.
-            max_demand: maximum demand of each node. Defaults to 10.
-            reward_fn: `RewardFn` whose `__call__` method computes the reward of an environment
+            num_cities: number of cities to visit. Defaults to 20.
+            reward_fn: RewardFn whose `__call__` method computes the reward of an environment
                 transition. The function must compute the reward based on the current state,
-                the chosen action, the next state and whether the action is valid.
+                the chosen action and the next state.
                 Implemented options are [`DenseReward`, `SparseReward`]. Defaults to `DenseReward`.
-            render_mode: string that defines the mode of rendering.
-                Choices are ["human, "rgb"], defaults to "human".
+            viewer: `Viewer` used for rendering. Defaults to `TSPViewer` with "human" render mode.
         """
 
-        if max_capacity < max_demand:
-            raise ValueError(
-                f"The demand associated with each node must be lower than the maximum capacity, "
-                f"hence the maximum capacity must be >= {max_demand}."
-            )
-        self.num_nodes = num_nodes
-        self.max_capacity = max_capacity
-        self.max_demand = max_demand
+        self.num_cities = num_cities
         self.reward_fn = reward_fn or DenseReward()
-        self._env_viewer = CVRPViewer(
-            name="CVRP",
-            num_cities=self.num_nodes,
-            render_mode=render_mode,
-        )
+        self._viewer = viewer or TSPViewer(name="TSP", render_mode="human")
 
     def __repr__(self) -> str:
-        return (
-            f"CVRP(num_nodes={self.num_nodes}, max_capacity={self.max_capacity}, "
-            f"max_demand={self.max_demand})"
-        )
+        return f"TSP environment with {self.num_cities} cities."
 
-    def reset(self, key: chex.PRNGKey) -> Tuple[State, TimeStep[Observation]]:
+    def reset(self, key: PRNGKey) -> Tuple[State, TimeStep[Observation]]:
         """Resets the environment.
 
         Args:
             key: used to randomly generate the coordinates.
 
         Returns:
-             state: `State` object corresponding to the new state of the environment.
-             timestep: `TimeStep` object corresponding to the first timestep returned by the
-                environment.
+            state: State object corresponding to the new state of the environment.
+            timestep: TimeStep object corresponding to the first timestep returned
+                by the environment.
         """
-        key, coordinates_key, demands_key = jax.random.split(key, 3)
+        key, sample_key = jax.random.split(key)
         coordinates = jax.random.uniform(
-            coordinates_key, (self.num_nodes + 1, 2), minval=0, maxval=1
+            sample_key, (self.num_cities, 2), minval=0, maxval=1
         )
-        demands = jax.random.randint(
-            demands_key, (self.num_nodes + 1,), minval=1, maxval=self.max_demand
-        )
-        demands = demands.at[DEPOT_IDX].set(0)
-        visited_mask = jnp.zeros(self.num_nodes + 1, dtype=bool).at[DEPOT_IDX].set(True)
         state = State(
             coordinates=coordinates,
-            demands=demands,
-            position=jnp.array(DEPOT_IDX, jnp.int32),
-            capacity=jnp.array(self.max_capacity, jnp.int32),
-            visited_mask=visited_mask,
-            trajectory=jnp.full(2 * self.num_nodes, DEPOT_IDX, jnp.int32),
-            num_total_visits=jnp.array(1, jnp.int32),
+            position=jnp.array(-1, jnp.int32),
+            visited_mask=jnp.zeros(self.num_cities, dtype=bool),
+            trajectory=jnp.full(self.num_cities, -1, jnp.int32),
+            num_visited=jnp.array(0, jnp.int32),
             key=key,
         )
         timestep = restart(observation=self._state_to_observation(state))
         return state, timestep
 
     def step(
         self, state: State, action: chex.Numeric
     ) -> Tuple[State, TimeStep[Observation]]:
         """Run one timestep of the environment's dynamics.
 
         Args:
             state: `State` object containing the dynamics of the environment.
-            action: jax array (int32) of shape () containing the index of the next node to visit.
+            action: `Array` containing the index of the next position to visit.
 
         Returns:
-            state, timestep: next state of the environment and timestep to be observed.
+            state: the next state of the environment.
+            timestep: the timestep to be observed.
         """
-        node_demand = state.demands[action]
-        node_is_visited = state.visited_mask[action]
-        is_valid = ~node_is_visited & (state.capacity >= node_demand)
-
+        is_valid = ~state.visited_mask[action]
         next_state = jax.lax.cond(
             is_valid,
             self._update_state,
             lambda *_: state,
             state,
             action,
         )
 
         reward = self.reward_fn(state, action, next_state, is_valid)
         observation = self._state_to_observation(next_state)
 
-        # Terminate if all nodes have been visited or the action is invalid.
-        is_done = next_state.visited_mask.all() | ~is_valid
-
+        # Terminate if all cities have been visited or the action is invalid
+        is_done = (next_state.num_visited == self.num_cities) | ~is_valid
         timestep = jax.lax.cond(
             is_done,
             termination,
             transition,
             reward,
             observation,
         )
         return next_state, timestep
 
     def observation_spec(self) -> specs.Spec[Observation]:
         """Returns the observation spec.
 
         Returns:
             Spec for the `Observation` whose fields are:
-            - coordinates: BoundedArray (float) of shape (num_nodes + 1, 2).
-            - demands: BoundedArray (float) of shape (num_nodes + 1,).
-            - unvisited_nodes: BoundedArray (bool) of shape (num_nodes + 1,).
-            - position: DiscreteArray (num_values = num_nodes + 1) of shape ().
-            - trajectory: BoundedArray (int32) of shape (2 * num_nodes,).
-            - capacity: BoundedArray (float) of shape ().
-            - action_mask: BoundedArray (bool) of shape (num_nodes + 1,).
+            - coordinates: BoundedArray (float) of shape (num_cities,).
+            - position: DiscreteArray (num_values = num_cities) of shape ().
+            - trajectory: BoundedArray (int32) of shape (num_cities,).
+            - action_mask: BoundedArray (bool) of shape (num_cities,).
         """
         coordinates = specs.BoundedArray(
-            shape=(self.num_nodes + 1, 2),
+            shape=(self.num_cities, 2),
             minimum=0.0,
             maximum=1.0,
             dtype=float,
             name="coordinates",
         )
-        demands = specs.BoundedArray(
-            shape=(self.num_nodes + 1,),
-            minimum=0.0,
-            maximum=1.0,
-            dtype=float,
-            name="demands",
-        )
-        unvisited_nodes = specs.BoundedArray(
-            shape=(self.num_nodes + 1,),
-            dtype=bool,
-            minimum=False,
-            maximum=True,
-            name="unvisited_nodes",
-        )
         position = specs.DiscreteArray(
-            self.num_nodes + 1, dtype=jnp.int32, name="position"
+            self.num_cities, dtype=jnp.int32, name="position"
         )
         trajectory = specs.BoundedArray(
-            shape=(2 * self.num_nodes,),
-            minimum=0,
-            maximum=self.num_nodes + 1,
+            shape=(self.num_cities,),
             dtype=jnp.int32,
+            minimum=-1,
+            maximum=self.num_cities - 1,
             name="trajectory",
         )
-        capacity = specs.BoundedArray(
-            shape=(), minimum=0.0, maximum=1.0, dtype=float, name="capacity"
-        )
         action_mask = specs.BoundedArray(
-            shape=(self.num_nodes + 1,),
+            shape=(self.num_cities,),
             dtype=bool,
             minimum=False,
             maximum=True,
             name="action_mask",
         )
         return specs.Spec(
             Observation,
             "ObservationSpec",
             coordinates=coordinates,
-            demands=demands,
-            unvisited_nodes=unvisited_nodes,
             position=position,
             trajectory=trajectory,
-            capacity=capacity,
             action_mask=action_mask,
         )
 
     def action_spec(self) -> specs.DiscreteArray:
         """Returns the action spec.
 
         Returns:
             action_spec: a `specs.DiscreteArray` spec.
         """
-        return specs.DiscreteArray(self.num_nodes + 1, name="action")
+        return specs.DiscreteArray(self.num_cities, name="action")
 
-    def render(self, state: State) -> Optional[chex.ArrayNumpy]:
-        """Render the given state of the environment. This rendering shows the layout of the tour so
-         far with the cities as circles, and the depot as a square.
+    def render(self, state: State) -> Optional[NDArray]:
+        """Render the given state of the environment. This rendering shows the layout of the cities
+        and the tour so far.
 
         Args:
-            state: environment state to render.
+            state: current environment state.
 
         Returns:
             rgb_array: the RGB image of the state as an array.
         """
-        return self._env_viewer.render(state)
+        return self._viewer.render(state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
-        """Creates an animated gif of the CVRP environment based on the sequence of states.
+        """Creates an animated gif of the `TSP` environment based on the sequence of states.
 
         Args:
             states: sequence of environment states corresponding to consecutive timesteps.
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
             animation.FuncAnimation: the animation object that was created.
         """
-        return self._env_viewer.animate(states, interval, save_path)
+        return self._viewer.animate(states, interval, save_path)
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self._env_viewer.close()
+        self._viewer.close()
 
     def _update_state(self, state: State, action: chex.Numeric) -> State:
-        """Updates the state of the environment.
+        """
+        Updates the state of the environment.
 
         Args:
             state: State object containing the dynamics of the environment.
-            action: int32, index of the next node to visit.
+            action: int32, index of the next position to visit.
 
         Returns:
             state: State object corresponding to the new state of the environment.
         """
-        capacity = jax.lax.select(
-            action == DEPOT_IDX,
-            self.max_capacity,
-            state.capacity - state.demands[action],
-        )
-
-        # Set depot to False (valid to visit) since it can be visited multiple times
-        visited_mask = state.visited_mask.at[DEPOT_IDX].set(False)
-
         return State(
             coordinates=state.coordinates,
-            demands=state.demands,
             position=action,
-            capacity=capacity,
-            visited_mask=visited_mask.at[action].set(True),
-            trajectory=state.trajectory.at[state.num_total_visits].set(action),
-            num_total_visits=state.num_total_visits + 1,
+            visited_mask=state.visited_mask.at[action].set(True),
+            trajectory=state.trajectory.at[state.num_visited].set(action),
+            num_visited=state.num_visited + 1,
             key=state.key,
         )
 
     def _state_to_observation(self, state: State) -> Observation:
         """Converts a state into an observation.
 
         Args:
             state: `State` object containing the dynamics of the environment.
 
         Returns:
             observation: `Observation` object containing the observation of the environment.
         """
-        # A node is not reachable if it has already been visited or if the vehicle does not have
-        # enough capacity to cover its demand.
-        action_mask = ~state.visited_mask & (state.capacity >= state.demands)
-
-        # The depot is reachable if we are not at it already.
-        action_mask = action_mask.at[DEPOT_IDX].set(state.position != DEPOT_IDX)
-
         return Observation(
             coordinates=state.coordinates,
-            demands=jnp.asarray(state.demands / self.max_capacity, float),
-            unvisited_nodes=~state.visited_mask,
             position=state.position,
             trajectory=state.trajectory,
-            capacity=jnp.asarray(state.capacity / self.max_capacity, float),
-            action_mask=action_mask,
+            action_mask=~state.visited_mask,
         )
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cvrp/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/routing/cvrp/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from chex import Array
 from numpy.typing import NDArray
 
 import jumanji.environments
 from jumanji.environments.routing.cvrp.types import State
+from jumanji.viewer import Viewer
 
 
-class CVRPViewer:
+class CVRPViewer(Viewer):
     FIGURE_SIZE = (10.0, 10.0)
     NODE_COLOUR = "black"
     COLORMAP_NAME = "hsv"
     NODE_SIZE = 150
     DEPOT_SIZE = 250
     ARROW_WIDTH = 0.004
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cvrp/reward.py` & `jumanji-0.2.2/jumanji/environments/routing/cvrp/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/cvrp/types.py` & `jumanji-0.2.2/jumanji/environments/routing/cvrp/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/maze/__init__.py` & `jumanji-0.2.2/jumanji/environments/routing/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/maze/constants.py` & `jumanji-0.2.2/jumanji/environments/routing/maze/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/maze/env.py` & `jumanji-0.2.2/jumanji/environments/routing/snake/env.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,347 +8,530 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, Sequence, Tuple
+from typing import Any, List, Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
+import matplotlib
 import matplotlib.animation
-from numpy.typing import NDArray
+import matplotlib.artist
+import matplotlib.pyplot as plt
+from matplotlib.patches import Circle, Rectangle
 
+import jumanji
+import jumanji.environments
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.routing.maze.constants import MOVES
-from jumanji.environments.routing.maze.env_viewer import MazeEnvViewer
-from jumanji.environments.routing.maze.generator import Generator, RandomGenerator
-from jumanji.environments.routing.maze.types import Observation, Position, State
+from jumanji.environments.routing.snake.types import Observation, Position, State
 from jumanji.types import TimeStep, restart, termination, transition
 
 
-class Maze(Environment[State]):
-    """A JAX implementation of a 2D Maze. The goal is to navigate the maze to find the target
-    position.
-
-    - observation:
-        - agent_position: current 2D Position of agent.
-        - target_position: 2D Position of target cell.
-        - walls: jax array (bool) of shape (num_rows, num_cols)
-            whose values are `True` where walls are and `False` for empty cells.
-        - action_mask: array (bool) of shape (4,)
-            defining the available actions in the current position.
-        - step_count: jax array (int32) of shape ()
-            step number of the episode.
+class Snake(Environment[State]):
+    """A JAX implementation of the 'Snake' game.
 
-    - action: jax array (int32) of shape () specifying which action to take: [0,1,2,3] correspond to
-        [Up, Right, Down, Left]. If an invalid action is taken, i.e. there is a wall blocking the
-        action, then no action (no-op) is taken.
-
-    - reward: jax array (float32) of shape (): 1 if the target is reached, 0 otherwise.
-
-    - episode termination (if any):
-        - agent reaches the target position.
-        - the time_limit is reached.
-
-    - state: State:
-        - agent_position: current 2D Position of agent.
-        - target_position: 2D Position of target cell.
-        - walls: jax array (bool) of shape (num_rows, num_cols)
-            whose values are `True` where walls are and `False` for empty cells.
-        - action_mask: array (bool) of shape (4,)
-            defining the available actions in the current position.
+    - observation: `Observation`
+        - grid: jax array (float) of shape (num_rows, num_cols, 5)
+            feature maps that include information about the fruit, the snake head, its body and
+            tail.
+            - body: 2D map with 1. where a body cell is present, else 0.
+            - head: 2D map with 1. where the snake's head is located, else 0.
+            - tail: 2D map with 1. where the snake's tail is located, else 0.
+            - fruit: 2D map with 1. where the fruit is located, else 0.
+            - norm_body_state: 2D map with a float between 0. and 1. for each body cell in the
+                decreasing order from head to tail.
+        - step_count: jax array (int32) of shape ()
+            current number of steps in the episode.
+        - action_mask: jax array (bool) of shape (4,)
+            array specifying which directions the snake can move in from its current position.
+
+    - action: jax array (int32) of shape()
+        [0,1,2,3] -> [Up, Right, Down, Left].
+
+    - reward: jax array (float) of shape ()
+        1.0 if a fruit is eaten, otherwise 0.0.
+
+    - episode termination:
+        - if no action can be performed, i.e. the snake is surrounded.
+        - if the time limit is reached.
+        - if an invalid action is taken, the snake exits the grid or bumps into itself.
+
+    - state: `State`
+        - body: jax array (bool) of shape (num_rows, num_cols)
+            array indicating the snake's body cells.
+        - body_state: jax array (int32) of shape (num_rows, num_cols)
+            array ordering the snake's body cells, in decreasing order from head to tail.
+        - head_position: `Position` (int32) of shape ()
+            position of the snake's head on the 2D grid.
+        - tail: jax array (bool) of shape (num_rows, num_cols)
+            array indicating the snake's tail.
+        - fruit_position: `Position` (int32) of shape ()
+            position of the fruit on the 2D grid.
+        - length: jax array (int32) of shape ()
+            current length of the snake.
         - step_count: jax array (int32) of shape ()
-            step number of the episode.
-        - key: random key (uint) of shape (2,).
+            current number of steps in the episode.
+        - action_mask: jax array (bool) of shape (4,)
+            array specifying which directions the snake can move in from its current position.
+        - key: jax array (uint32) of shape (2,)
+            random key used to sample a new fruit when one is eaten and used for auto-reset.
 
     ```python
-    from jumanji.environments import Maze
-    env = Maze()
+    from jumanji.environments import Snake
+    env = Snake()
     key = jax.random.key(0)
     state, timestep = jax.jit(env.reset)(key)
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
-    FIGURE_NAME = "Maze"
+    FIGURE_NAME = "Snake"
     FIGURE_SIZE = (6.0, 6.0)
+    MOVES = jnp.array([[-1, 0], [0, 1], [1, 0], [0, -1]], jnp.int32)
 
-    def __init__(
-        self,
-        generator: Optional[Generator] = None,
-        time_limit: Optional[int] = None,
-        render_mode: str = "human",
-    ) -> None:
-        """Instantiates a `Maze` environment.
+    def __init__(self, num_rows: int = 12, num_cols: int = 12, time_limit: int = 4000):
+        """Instantiates a `Snake` environment.
 
         Args:
-            generator: `Generator` whose `__call__` instantiates an environment instance.
-                Implemented options are [`ToyGenerator`, `RandomGenerator`].
-                Defaults to `RandomGenerator` with `num_rows=10` and `num_cols=10`.
-            time_limit: the time_limit of an episode, i.e. the maximum number of environment steps
-                before the episode terminates. By default, `time_limit = num_rows * num_cols`.
-            render_mode: the mode for visualising the environment, can be "human" or "rgb_array".
-        """
-        self.generator = generator or RandomGenerator(num_rows=10, num_cols=10)
-        self.num_rows = self.generator.num_rows
-        self.num_cols = self.generator.num_cols
-        self.shape = (self.num_rows, self.num_cols)
-        self.time_limit = time_limit or self.num_rows * self.num_cols
-
-        # Create viewer used for rendering
-        self._env_viewer = MazeEnvViewer("Maze", render_mode)
+            num_rows: number of rows of the 2D grid. Defaults to 12.
+            num_cols: number of columns of the 2D grid. Defaults to 12.
+            time_limit: time_limit of an episode, i.e. number of environment steps before
+                the episode ends. Defaults to 4000.
+        """
+        super().__init__()
+        self.num_rows = num_rows
+        self.num_cols = num_cols
+        self.board_shape = (num_rows, num_cols)
+        self.time_limit = time_limit
+
+        # You must store the created Animation in a variable that lives as long as the animation
+        # should run. Otherwise, the animation will get garbage-collected.
+        self._animation: Optional[matplotlib.animation.Animation] = None
 
     def __repr__(self) -> str:
         return "\n".join(
             [
-                "Maze environment:",
+                "Snake environment:",
                 f" - num_rows: {self.num_rows}",
                 f" - num_cols: {self.num_cols}",
                 f" - time_limit: {self.time_limit}",
-                f" - generator: {self.generator}",
             ]
         )
 
+    def reset(self, key: chex.PRNGKey) -> Tuple[State, TimeStep[Observation]]:
+        """Resets the environment.
+
+        Args:
+            key: random key used to sample the snake and fruit positions.
+
+        Returns:
+             state: `State` object corresponding to the new state of the environment.
+             timestep: `TimeStep` object corresponding to the first timestep returned by the
+                environment.
+        """
+        key, snake_key, fruit_key = jax.random.split(key, 3)
+        # Sample Snake's head position.
+        head_coordinates = jax.random.randint(
+            snake_key,
+            shape=(2,),
+            minval=jnp.zeros(2, int),
+            maxval=jnp.array(self.board_shape),
+        )
+        head_position = Position(*tuple(head_coordinates))
+
+        body = jnp.zeros(self.board_shape, bool).at[tuple(head_position)].set(True)
+        tail = body
+        body_state = body.astype(jnp.int32)
+        fruit_position = self._sample_fruit_coord(body, fruit_key)
+        state = State(
+            key=key,
+            body=body,
+            body_state=body_state,
+            head_position=head_position,
+            tail=tail,
+            fruit_position=fruit_position,
+            length=jnp.array(1, jnp.int32),
+            step_count=jnp.array(0, jnp.int32),
+            action_mask=self._get_action_mask(head_position, body_state),
+        )
+        timestep = restart(observation=self._state_to_observation(state))
+        return state, timestep
+
+    def step(
+        self, state: State, action: chex.Numeric
+    ) -> Tuple[State, TimeStep[Observation]]:
+        """Run one timestep of the environment's dynamics.
+
+        Args:
+            state: `State` object containing the dynamics of the environment.
+            action: Array containing the action to take:
+                - 0: move up.
+                - 1: move to the right.
+                - 2: move down.
+                - 3: move to the left.
+
+        Returns:
+            state, timestep: next state of the environment and timestep to be observed.
+        """
+        is_valid = state.action_mask[action]
+        key, fruit_key = jax.random.split(state.key)
+
+        head_position = self._update_head_position(state.head_position, action)
+
+        fruit_eaten = head_position == state.fruit_position
+
+        length = state.length + fruit_eaten
+
+        body_state_without_head = jax.lax.select(
+            fruit_eaten,
+            state.body_state,
+            jnp.clip(state.body_state - 1, 0),
+        )
+        body_state = body_state_without_head.at[tuple(head_position)].set(length)
+
+        body = body_state > 0
+
+        tail = body_state == 1
+
+        fruit_position = jax.lax.cond(
+            fruit_eaten,
+            self._sample_fruit_coord,
+            lambda *_: state.fruit_position,
+            body,
+            fruit_key,
+        )
+        step_count = state.step_count + 1
+        next_state = State(
+            key=key,
+            body=body,
+            body_state=body_state,
+            head_position=head_position,
+            tail=tail,
+            fruit_position=fruit_position,
+            length=length,
+            step_count=state.step_count + 1,
+            action_mask=self._get_action_mask(head_position, body_state),
+        )
+
+        snake_completed = jnp.all(body)
+        done = ~is_valid | snake_completed | (step_count >= self.time_limit)
+
+        reward = jnp.asarray(fruit_eaten, float)
+        observation = self._state_to_observation(next_state)
+
+        timestep = jax.lax.cond(
+            done,
+            termination,
+            transition,
+            reward,
+            observation,
+        )
+        return next_state, timestep
+
     def observation_spec(self) -> specs.Spec[Observation]:
-        """Specifications of the observation of the `Maze` environment.
+        """Returns the observation spec.
 
         Returns:
             Spec for the `Observation` whose fields are:
-            - agent_position: tree of BoundedArray (int32) of shape ().
-            - target_position: tree of BoundedArray (int32) of shape ().
-            - walls: BoundedArray (bool) of shape (num_rows, num_cols).
-            - step_count: Array (int32) of shape ().
+            - grid: BoundedArray (float) of shape (num_rows, num_cols, 5).
+            - step_count: DiscreteArray (num_values = time_limit) of shape ().
             - action_mask: BoundedArray (bool) of shape (4,).
         """
-        agent_position = specs.Spec(
-            Position,
-            "PositionSpec",
-            row=specs.BoundedArray(
-                (), jnp.int32, 0, self.num_rows - 1, "row_coordinate"
-            ),
-            col=specs.BoundedArray(
-                (), jnp.int32, 0, self.num_cols - 1, "col_coordinate"
-            ),
+        grid = specs.BoundedArray(
+            shape=(self.num_rows, self.num_cols, 5),
+            minimum=0.0,
+            maximum=1.0,
+            dtype=float,
+            name="grid",
+        )
+        step_count = specs.DiscreteArray(
+            self.time_limit, dtype=jnp.int32, name="step_count"
         )
-        walls = specs.BoundedArray(
-            shape=(self.num_rows, self.num_cols),
+        action_mask = specs.BoundedArray(
+            shape=(4,),
             dtype=bool,
             minimum=False,
             maximum=True,
-            name="walls",
-        )
-        step_count = specs.Array((), jnp.int32, "step_count")
-        action_mask = specs.BoundedArray(
-            shape=(4,), dtype=bool, minimum=False, maximum=True, name="action_mask"
+            name="action_mask",
         )
         return specs.Spec(
             Observation,
             "ObservationSpec",
-            agent_position=agent_position,
-            target_position=agent_position,
-            walls=walls,
+            grid=grid,
             step_count=step_count,
             action_mask=action_mask,
         )
 
     def action_spec(self) -> specs.DiscreteArray:
         """Returns the action spec. 4 actions: [0,1,2,3] -> [Up, Right, Down, Left].
 
         Returns:
-            action_spec: discrete action space with 4 values.
+            action_spec: a `specs.DiscreteArray` spec.
         """
         return specs.DiscreteArray(4, name="action")
 
-    def reset(self, key: chex.PRNGKey) -> Tuple[State, TimeStep[Observation]]:
-        """Resets the environment by calling the instance generator for a new instance.
+    def _state_to_observation(self, state: State) -> Observation:
+        """Maps an environment state to an observation.
 
         Args:
-            key: random key used to reset the environment since it is stochastic.
+            state: `State` object containing the dynamics of the environment.
 
         Returns:
-            state: `State` object corresponding to the new state of the environment after a reset.
-            timestep: `TimeStep` object corresponding the first timestep returned by the environment
-                after a reset.
+            The observation derived from the state.
         """
-
-        key, maze_key, agent_key = jax.random.split(key, 3)
-
-        walls = self.generator(maze_key)
-
-        # Randomise agent start and target positions.
-        start_and_target_indices = jax.random.choice(
-            agent_key,
-            jnp.arange(self.num_rows * self.num_cols),
-            (2,),
-            replace=False,
-            p=~walls.flatten(),
-        )
-        (agent_row, target_row), (agent_col, target_col) = jnp.divmod(
-            start_and_target_indices, self.num_cols
+        body = state.body
+        head = jnp.zeros_like(body).at[tuple(state.head_position)].set(True)
+        tail = state.tail
+        fruit = jnp.zeros_like(body).at[tuple(state.fruit_position)].set(True)
+        norm_body_state = state.body_state / jnp.maximum(1, state.body_state.max())
+        grid = jnp.concatenate(
+            jax.tree_util.tree_map(
+                lambda x: x[..., None], [body, head, tail, fruit, norm_body_state]
+            ),
+            axis=-1,
+            dtype=float,
         )
 
-        agent_position = Position(row=agent_row, col=agent_col)
-        target_position = Position(row=target_row, col=target_col)
-
-        # Build the state.
-        state = State(
-            agent_position=agent_position,
-            target_position=target_position,
-            walls=walls,
-            action_mask=self._compute_action_mask(walls, agent_position),
-            key=key,
-            step_count=jnp.array(0, jnp.int32),
+        return Observation(
+            grid=grid,
+            step_count=state.step_count,
+            action_mask=state.action_mask,
         )
 
-        # Generate the observation from the environment state.
-        observation = self._observation_from_state(state)
-
-        # Return a restart timestep whose step type is FIRST.
-        timestep = restart(observation)
+    def _sample_fruit_coord(
+        self,
+        body: chex.Array,
+        key: chex.PRNGKey,
+    ) -> Position:
+        """Sample the coordinates of a new fruit at a location where the snake is not.
 
-        return state, timestep
+        Args:
+            body: array indicating the snake's body cells.
+            key: random key to generate a random fruit position.
 
-    def step(
-        self, state: State, action: chex.Array
-    ) -> Tuple[State, TimeStep[Observation]]:
+        Returns:
+            Position(row, col) corresponding to the new fruit coordinates.
         """
-        Run one timestep of the environment's dynamics.
+        fruit_index = jax.random.choice(
+            key,
+            jnp.arange(self.num_rows * self.num_cols),
+            p=~body.flatten(),
+        )
+        row, col = jnp.divmod(fruit_index, self.num_cols)
+        return Position(row=row, col=col)
 
-        If an action is invalid, the agent does not move, i.e. the episode does not
-        automatically terminate.
+    def _get_action_mask(
+        self,
+        head_position: Position,
+        body_state: chex.Array,
+    ) -> chex.Array:
+        """Checks whether the episode is over or not.
 
         Args:
-            state: State object containing the dynamics of the environment.
-            action: (int32) specifying which action to take: [0,1,2,3] correspond to
-                [Up, Right, Down, Left]. If an invalid action is taken, i.e. there is a wall
-                blocking the action, then no action (no-op) is taken.
+            head_position: Position of the snake's head.
+            body_state: array ordering the snake's body cells.
 
         Returns:
-            state: the next state of the environment.
-            timestep: the next timestep to be observed.
+            action_mask: array (bool) of shape (4,).
         """
-        # If the chosen action is invalid, i.e. blocked by a wall, overwrite it to no-op.
-        action = jax.lax.select(state.action_mask[action], action, 4)
 
-        # Take the action in the environment:  up, right, down, or left
-        # Remember the walls coordinates: (0,0) is top left.
-        agent_position = jax.lax.switch(
-            action,
-            [
-                lambda position: Position(position.row - 1, position.col),  # Up
-                lambda position: Position(position.row, position.col + 1),  # Right
-                lambda position: Position(position.row + 1, position.col),  # Down
-                lambda position: Position(position.row, position.col - 1),  # Left
-                lambda position: position,  # No-op
-            ],
-            state.agent_position,
-        )
-
-        # Generate action mask to keep in the state for the next step and
-        # to provide to the agent in the observation.
-        action_mask = self._compute_action_mask(state.walls, agent_position)
-
-        # Build the state.
-        state = State(
-            agent_position=agent_position,
-            target_position=state.target_position,
-            walls=state.walls,
-            action_mask=action_mask,
-            key=state.key,
-            step_count=state.step_count + 1,
-        )
-        # Generate the observation from the environment state.
-        observation = self._observation_from_state(state)
-
-        # Check if the episode terminates (i.e. done is True).
-        no_actions_available = ~jnp.any(action_mask)
-        target_reached = state.agent_position == state.target_position
-        time_limit_exceeded = state.step_count >= self.time_limit
+        def is_valid(move: chex.Array) -> chex.Array:
+            new_head_position = head_position + Position(*tuple(move))
+            outside_board = (
+                (new_head_position.row < 0)
+                | (new_head_position.row >= self.num_rows)
+                | (new_head_position.col < 0)
+                | (new_head_position.col >= self.num_cols)
+            )
+            body_state_without_head = jnp.clip(body_state - 1, 0)
+            head_bumps_body = body_state_without_head[tuple(new_head_position)] > 0
+            return ~outside_board & ~head_bumps_body
 
-        done = no_actions_available | target_reached | time_limit_exceeded
+        action_mask = jax.vmap(is_valid)(self.MOVES)
+        return action_mask
 
-        # Compute the reward.
-        reward = jnp.array(state.agent_position == state.target_position, float)
+    def _update_head_position(
+        self, head_position: Position, action: chex.Numeric
+    ) -> Position:
+        """Give the new head position after taking an action.
 
-        # Return either a MID or a LAST timestep depending on done.
-        timestep = jax.lax.cond(
-            done,
-            termination,
-            transition,
-            reward,
-            observation,
-        )
-        return state, timestep
+        Args:
+            head_position: `Position` of the snake's head.
+            action: integer that tells in which direction to go.
 
-    def _compute_action_mask(
-        self, walls: chex.Array, agent_position: Position
-    ) -> chex.Array:
-        """Compute the action mask.
-        An action is considered invalid if it leads to a WALL or goes outside of the maze.
+        Returns:
+            New head position after taking the action.
         """
+        # Possible moves are: Up, Right, Down, Left.
+        row_move, col_move = self.MOVES[action]
+        move_position = Position(row=row_move, col=col_move)
+        next_head_position = Position(*tuple(head_position)) + move_position
+        return next_head_position
 
-        def is_move_valid(agent_position: Position, move: chex.Array) -> chex.Array:
-            x, y = jnp.array([agent_position.row, agent_position.col]) + move
-            return (
-                (x >= 0)
-                & (x < self.num_cols)
-                & (y >= 0)
-                & (y < self.num_rows)
-                & ~(walls[x, y])
-            )
-
-        # vmap over the moves.
-        action_mask = jax.vmap(is_move_valid, in_axes=(None, 0))(agent_position, MOVES)
+    def render(self, state: State) -> None:
+        """Render frames of the environment for a given state using matplotlib.
 
-        return action_mask
+        Args:
+            state: State object containing the current dynamics of the environment.
 
-    def _observation_from_state(self, state: State) -> Observation:
-        """Create an observation from the state of the environment."""
-        return Observation(
-            agent_position=state.agent_position,
-            target_position=state.target_position,
-            walls=state.walls,
-            step_count=state.step_count,
-            action_mask=state.action_mask,
-        )
+        """
+        self._clear_display()
+        fig, ax = self._get_fig_ax()
+        self._draw(ax, state)
+        self._update_display(fig)
 
-    def render(self, state: State) -> Optional[NDArray]:
-        """Render the given state of the environment.
+    def close(self) -> None:
+        """Perform any necessary cleanup.
 
-        Args:
-            state: `State` object containing the current environment state.
+        Environments will automatically :meth:`close()` themselves when
+        garbage collected or when the program exits.
         """
-        return self._env_viewer.render(state)
+        plt.close(self.FIGURE_NAME)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
-        """Creates an animated gif of the `Maze` environment based on the sequence of states.
+        """Create an animation from a sequence of states.
 
         Args:
-            states: sequence of environment states corresponding to consecutive timesteps.
+            states: sequence of `State` corresponding to subsequent timesteps.
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
-            animation.FuncAnimation: the animation object that was created.
+            Animation object that can be saved as a GIF, MP4, or rendered with HTML.
         """
-        return self._env_viewer.animate(states, interval, save_path)
-
-    def close(self) -> None:
-        """Perform any necessary cleanup.
+        fig, ax = plt.subplots(num=f"{self.FIGURE_NAME}Anim", figsize=self.FIGURE_SIZE)
+        self._draw_board(ax)
+        plt.close(fig)
+
+        patches: List[matplotlib.patches.Patch] = []
+
+        def make_frame(state: State) -> Any:
+            while patches:
+                patches.pop().remove()
+            patches.extend(self._create_entities(state))
+            for patch in patches:
+                ax.add_patch(patch)
+
+        # Create the animation object.
+        matplotlib.rc("animation", html="jshtml")
+        self._animation = matplotlib.animation.FuncAnimation(
+            fig,
+            make_frame,
+            frames=states,
+            interval=interval,
+        )
+
+        # Save the animation as a gif.
+        if save_path:
+            self._animation.save(save_path)
+
+        return self._animation
+
+    def _get_fig_ax(self) -> Tuple[plt.Figure, plt.Axes]:
+        exists = plt.fignum_exists(self.FIGURE_NAME)
+        if exists:
+            fig = plt.figure(self.FIGURE_NAME)
+            ax = fig.get_axes()[0]
+        else:
+            fig = plt.figure(self.FIGURE_NAME, figsize=self.FIGURE_SIZE)
+            fig.set_tight_layout({"pad": False, "w_pad": 0.0, "h_pad": 0.0})
+            if not plt.isinteractive():
+                fig.show()
+            ax = fig.add_subplot()
+        return fig, ax
+
+    def _draw(self, ax: plt.Axes, state: State) -> None:
+        ax.clear()
+        self._draw_board(ax)
+        for patch in self._create_entities(state):
+            ax.add_patch(patch)
+
+    def _draw_board(self, ax: plt.Axes) -> None:
+        # Draw the square box that delimits the board.
+        ax.axis("off")
+        ax.plot([0, 0], [0, self.num_rows], "-k", lw=2)
+        ax.plot([0, self.num_cols], [self.num_rows, self.num_rows], "-k", lw=2)
+        ax.plot([self.num_cols, self.num_cols], [self.num_rows, 0], "-k", lw=2)
+        ax.plot([self.num_cols, 0], [0, 0], "-k", lw=2)
+
+    def _create_entities(self, state: State) -> List[matplotlib.patches.Patch]:
+        """Loop over the different cells and draws corresponding shapes in the ax object."""
+        patches = []
+        linewidth = (
+            min(
+                n * size
+                for n, size in zip((self.num_rows, self.num_cols), self.FIGURE_SIZE)
+            )
+            / 44.0
+        )
+        cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
+            "", ["yellowgreen", "forestgreen"]
+        )
+        for row in range(self.num_rows):
+            for col in range(self.num_cols):
+                if state.body_state[row, col]:
+                    body_cell_patch = Rectangle(
+                        (col, self.num_rows - 1 - row),
+                        1,
+                        1,
+                        edgecolor=cmap(1),
+                        facecolor=cmap(state.body_state[row, col] / state.length),
+                        fill=True,
+                        lw=linewidth,
+                    )
+                    patches.append(body_cell_patch)
+        head_patch = Circle(
+            (
+                state.head_position[1] + 0.5,
+                self.num_rows - 1 - state.head_position[0] + 0.5,
+            ),
+            0.3,
+            edgecolor=cmap(0.5),
+            facecolor=cmap(0),
+            fill=True,
+            lw=linewidth,
+        )
+        patches.append(head_patch)
+        fruit_patch = Circle(
+            (
+                state.fruit_position[1] + 0.5,
+                self.num_rows - 1 - state.fruit_position[0] + 0.5,
+            ),
+            0.2,
+            edgecolor="brown",
+            facecolor="lightcoral",
+            fill=True,
+            lw=linewidth,
+        )
+        patches.append(fruit_patch)
+        return patches
+
+    def _update_display(self, fig: plt.Figure) -> None:
+        if plt.isinteractive():
+            # Required to update render when using Jupyter Notebook.
+            fig.canvas.draw()
+            if jumanji.environments.is_colab():
+                plt.show(self.FIGURE_NAME)
+        else:
+            # Required to update render when not using Jupyter Notebook.
+            fig.canvas.draw_idle()
+            fig.canvas.flush_events()
+
+    def _clear_display(self) -> None:
+        if jumanji.environments.is_colab():
+            import IPython.display
 
-        Environments will automatically :meth:`close()` themselves when
-        garbage collected or when the program exits.
-        """
-        self._env_viewer.close()
+            IPython.display.clear_output(True)
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/maze/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/routing/maze/viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Sequence
 
+import chex
 import matplotlib
 from numpy.typing import NDArray
 
-from jumanji.environments.commons.maze_utils.maze_generation import Maze
 from jumanji.environments.commons.maze_utils.maze_rendering import MazeViewer
 from jumanji.environments.routing.maze.types import State
+from jumanji.viewer import Viewer
 
 EMPTY = 0
 WALL = 1
 
 
 class MazeEnvViewer(MazeViewer):
     AGENT = 2
@@ -31,15 +32,20 @@
     COLORS = {
         EMPTY: [1, 1, 1],  # White
         WALL: [0, 0, 0],  # Black
         AGENT: [0, 1, 0],  # Green
         TARGET: [1, 0, 0],  # Red
     }
 
-    def __init__(self, name: str, render_mode: str = "human") -> None:
+    def __init__(
+        self,
+        name: str,
+        render_mode: str = "human",
+        viewer: Optional[Viewer[State]] = None,
+    ) -> None:
         """Viewer for the Maze environment.
 
         Args:
             name: the window name to be used when initialising the matplotlib window.
             render_mode: the mode used to render the environment. Must be one of:
                 - "human": render the environment on screen.
                 - "rgb_array": return a numpy array frame representing the environment.
@@ -71,11 +77,11 @@
 
         Returns:
             Animation that can be saved as a GIF, MP4, or rendered with HTML.
         """
         mazes = [self._overlay_agent_and_target(state) for state in states]
         return super().animate(mazes, interval, save_path)
 
-    def _overlay_agent_and_target(self, state: State) -> Maze:
+    def _overlay_agent_and_target(self, state: State) -> chex.Array:
         maze = state.walls.astype(int)
         maze = maze.at[tuple(state.agent_position)].set(self.AGENT)
         return maze.at[tuple(state.target_position)].set(self.TARGET)
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/maze/generator.py` & `jumanji-0.2.2/jumanji/environments/routing/maze/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import abc
 
 import chex
 import jax.numpy as jnp
-from typing_extensions import TypeAlias
 
 from jumanji.environments.commons.maze_utils import maze_generation
 
-Maze: TypeAlias = chex.Array
-
 
 class Generator(abc.ABC):
     def __init__(self, num_rows: int, num_cols: int):
         """Interface for maze generator.
 
         Args:
             num_rows: the width of the maze to create.
             num_cols: the length of the maze to create.
         """
         self.num_rows = num_rows
         self.num_cols = num_cols
 
     @abc.abstractmethod
-    def __call__(self, key: chex.PRNGKey) -> Maze:
+    def __call__(self, key: chex.PRNGKey) -> chex.Array:
         """Generate a problem instance.
 
         Args:
             key: random key.
 
         Returns:
             A `Maze` representing a problem instance.
@@ -47,29 +44,29 @@
 
 class ToyGenerator(Generator):
     """Generate a hardcoded 5x5 toy maze."""
 
     def __init__(self) -> None:
         super(ToyGenerator, self).__init__(num_rows=5, num_cols=5)
 
-    def __call__(self, key: chex.PRNGKey) -> Maze:
+    def __call__(self, key: chex.PRNGKey) -> chex.Array:
         walls = jnp.ones((self.num_rows, self.num_cols), bool)
         walls = walls.at[0, :].set((False, True, False, False, False))
         walls = walls.at[1, :].set((False, True, False, True, True))
         walls = walls.at[2, :].set((False, True, False, False, False))
         walls = walls.at[3, :].set((False, False, False, True, True))
         walls = walls.at[4, :].set((False, False, False, False, False))
         return walls
 
 
 class RandomGenerator(Generator):
     def __init__(self, num_rows: int, num_cols: int) -> None:
         super(RandomGenerator, self).__init__(num_rows=num_rows, num_cols=num_cols)
 
-    def __call__(self, key: chex.PRNGKey) -> Maze:
+    def __call__(self, key: chex.PRNGKey) -> chex.Array:
         """Generate a random maze.
 
         This method relies on the `generate_maze` method from the `maze_generation` module to
         generate a maze.
 
         Args:
             key: the Jax random number generation key.
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/maze/types.py` & `jumanji-0.2.2/jumanji/environments/routing/maze/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/snake/__init__.py` & `jumanji-0.2.2/jumanji/environments/routing/snake/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/snake/types.py` & `jumanji-0.2.2/jumanji/environments/routing/snake/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/tsp/__init__.py` & `jumanji-0.2.2/jumanji/environments/routing/tsp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/tsp/env.py` & `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/env.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,289 +13,246 @@
 # limitations under the License.
 
 from typing import Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
-import matplotlib
-from chex import PRNGKey
+import matplotlib.animation
 from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
-from jumanji.environments.routing.tsp.env_viewer import TSPViewer
-from jumanji.environments.routing.tsp.reward import DenseReward, RewardFn
-from jumanji.environments.routing.tsp.types import Observation, State
+from jumanji.environments.logic.rubiks_cube.constants import (
+    DEFAULT_STICKER_COLORS,
+    Face,
+)
+from jumanji.environments.logic.rubiks_cube.generator import (
+    Generator,
+    ScramblingGenerator,
+)
+from jumanji.environments.logic.rubiks_cube.reward import RewardFn, SparseRewardFn
+from jumanji.environments.logic.rubiks_cube.types import Observation, State
+from jumanji.environments.logic.rubiks_cube.utils import (
+    flatten_action,
+    is_solved,
+    rotate_cube,
+)
+from jumanji.environments.logic.rubiks_cube.viewer import RubiksCubeViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
-class TSP(Environment[State]):
-    """Traveling Salesman Problem (TSP) environment as described in [1].
+class RubiksCube(Environment[State]):
+    """A JAX implementation of the Rubik's Cube with a configurable cube size (by default, 3) and
+    number of scrambles at reset.
 
-    - observation: Observation
-        - coordinates: jax array (float) of shape (num_cities, 2)
-            the coordinates of each city.
-        - position: jax array (int32)  of shape ()
-            the index corresponding to the last visited city.
-        - trajectory: jax array (int32) of shape (num_cities,)
-            array of city indices defining the route (-1 --> not filled yet).
-        - action_mask: jax array (bool) of shape (num_cities,)
-            binary mask (False/True <--> illegal/legal <--> cannot be visited/can be visited).
-
-    - action: jax array (int32) of shape ()
-        [0, ..., num_cities - 1] -> city to visit.
-
-    - reward: jax array (float) of shape (), could be either:
-        - dense: the negative distance between the current city and the chosen next city to go to.
-            It is 0 for the first chosen city, and for the last city, it also includes the distance
-            to the initial city to complete the tour.
-        - sparse: the negative tour length at the end of the episode. The tour length is defined
-            as the sum of the distances between consecutive cities. It is computed by starting at
-            the first city and ending there, after visiting all the cities.
-        In both cases, the reward is a large negative penalty of `-num_cities * sqrt(2)` if
-        the action is invalid, i.e. a previously selected city is selected again.
+    - observation: `Observation`
+        - cube: jax array (int8) of shape (6, cube_size, cube_size):
+            each cell contains the index of the corresponding colour of the sticker in the scramble.
+        - step_count: jax array (int32) of shape ():
+            specifies how many timesteps have elapsed since environment reset.
+
+    - action:
+        multi discrete array containing the move to perform (face, depth, and direction).
+
+    - reward: jax array (float) of shape ():
+        by default, 1.0 if cube is solved, otherwise 0.0.
 
     - episode termination:
-        - if no action can be performed, i.e. all cities have been visited.
-        - if an invalid action is taken, i.e. an already visited city is chosen.
+        if either the cube is solved or a time limit is reached.
 
     - state: `State`
-        - coordinates: jax array (float) of shape (num_cities, 2)
-            the coordinates of each city.
-        - position: int32
-            the identifier (index) of the last visited city.
-        - visited_mask: jax array (bool) of shape (num_cities,)
-            binary mask (False/True <--> not visited/visited).
-        - trajectory: jax array (int32) of shape (num_cities,)
-            the identifiers of the cities that have been visited (-1 means that no city has been
-            visited yet at that time in the sequence).
-        - num_visited: int32
-            number of cities that have been visited.
-
-    [1] Kwon Y., Choo J., Kim B., Yoon I., Min S., Gwon Y. (2020). "POMO: Policy Optimization
-        with Multiple Optima for Reinforcement Learning".
+        - cube: jax array (int8) of shape (6, cube_size, cube_size):
+            each cell contains the index of the corresponding colour of the sticker in the scramble.
+        - step_count: jax array (int32) of shape ():
+            specifies how many timesteps have elapsed since environment reset.
+        - key: jax array (uint) of shape (2,) used for seeding the sampling for scrambling on
+            reset.
 
     ```python
-    from jumanji.environments import TSP
-    env = TSP()
+    from jumanji.environments import RubiksCube
+    env = RubiksCube()
     key = jax.random.key(0)
     state, timestep = jax.jit(env.reset)(key)
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        num_cities: int = 20,
+        generator: Optional[Generator] = None,
+        time_limit: int = 200,
         reward_fn: Optional[RewardFn] = None,
-        render_mode: str = "human",
+        viewer: Optional[Viewer[State]] = None,
     ):
-        """Instantiates a `TSP` environment.
+        """Instantiate a `RubiksCube` environment.
 
         Args:
-            num_cities: number of cities to visit. Defaults to 20.
-            reward_fn: RewardFn whose `__call__` method computes the reward of an environment
-                transition. The function must compute the reward based on the current state,
-                the chosen action and the next state.
-                Implemented options are [`DenseReward`, `SparseReward`]. Defaults to `DenseReward`.
-            render_mode: string that defines the mode of rendering.
-                Choices are ["human, "rgb"], defaults to "human".
-        """
-
-        self.num_cities = num_cities
-        self.reward_fn = reward_fn or DenseReward()
-        self._env_viewer = TSPViewer(name="TSP", render_mode=render_mode)
-
-    def __repr__(self) -> str:
-        return f"TSP environment with {self.num_cities} cities."
+            generator: `Generator` used to generate problem instances on environment reset.
+                Implemented options are [`ScramblingGenerator`]. Defaults to `ScramblingGenerator`,
+                with 100 scrambles on reset.
+                The generator will contain an attribute `cube_size`, corresponding to the number of
+                cubies to an edge, and defaulting to 3.
+            time_limit: the number of steps allowed before an episode terminates. Defaults to 200.
+            reward_fn: `RewardFn` whose `__call__` method computes the reward given the new state.
+                Implemented options are [`SparseRewardFn`]. Defaults to `SparseRewardFn`, giving a
+                reward of 1.0 if the cube is solved or otherwise 0.0.
+            viewer: `Viewer` to support rendering and animation methods.
+                Implemented options are [`RubiksCubeViewer`]. Defaults to `RubiksCubeViewer`.
+        """
+        if time_limit <= 0:
+            raise ValueError(
+                f"The time_limit must be positive, but received time_limit={time_limit}"
+            )
+        self.time_limit = time_limit
+        self.reward_function = reward_fn or SparseRewardFn()
+        self.generator = generator or ScramblingGenerator(
+            cube_size=3,
+            num_scrambles_on_reset=100,
+        )
+        self._viewer = viewer or RubiksCubeViewer(
+            sticker_colors=DEFAULT_STICKER_COLORS, cube_size=self.generator.cube_size
+        )
 
-    def reset(self, key: PRNGKey) -> Tuple[State, TimeStep[Observation]]:
+    def reset(self, key: chex.PRNGKey) -> Tuple[State, TimeStep[Observation]]:
         """Resets the environment.
 
         Args:
-            key: used to randomly generate the coordinates.
+            key: needed for scramble.
 
         Returns:
-            state: State object corresponding to the new state of the environment.
-            timestep: TimeStep object corresponding to the first timestep returned
-                by the environment.
+            state: `State` corresponding to the new state of the environment.
+            timestep: `TimeStep` corresponding to the first timestep returned by the
+                environment.
         """
-        key, sample_key = jax.random.split(key)
-        coordinates = jax.random.uniform(
-            sample_key, (self.num_cities, 2), minval=0, maxval=1
-        )
-        state = State(
-            coordinates=coordinates,
-            position=jnp.array(-1, jnp.int32),
-            visited_mask=jnp.zeros(self.num_cities, dtype=bool),
-            trajectory=jnp.full(self.num_cities, -1, jnp.int32),
-            num_visited=jnp.array(0, jnp.int32),
-            key=key,
-        )
-        timestep = restart(observation=self._state_to_observation(state))
+        state = self.generator(key)
+        observation = self._state_to_observation(state=state)
+        timestep = restart(observation=observation)
         return state, timestep
 
     def step(
-        self, state: State, action: chex.Numeric
+        self, state: State, action: chex.Array
     ) -> Tuple[State, TimeStep[Observation]]:
         """Run one timestep of the environment's dynamics.
 
         Args:
             state: `State` object containing the dynamics of the environment.
-            action: `Array` containing the index of the next position to visit.
+            action: `Array` of shape (3,) indicating the face to move, depth of the move, and the
+                amount to move by.
 
         Returns:
-            state: the next state of the environment.
-            timestep: the timestep to be observed.
+            next_state: `State` corresponding to the next state of the environment.
+            next_timestep: `TimeStep` corresponding to the timestep returned by the environment.
         """
-        is_valid = ~state.visited_mask[action]
-        next_state = jax.lax.cond(
-            is_valid,
-            self._update_state,
-            lambda *_: state,
-            state,
-            action,
-        )
-
-        reward = self.reward_fn(state, action, next_state, is_valid)
-        observation = self._state_to_observation(next_state)
-
-        # Terminate if all cities have been visited or the action is invalid
-        is_done = (next_state.num_visited == self.num_cities) | ~is_valid
-        timestep = jax.lax.cond(
-            is_done,
+        flattened_action = flatten_action(
+            unflattened_action=action, cube_size=self.generator.cube_size
+        )
+        cube = rotate_cube(
+            cube=state.cube,
+            flattened_action=flattened_action,
+        )
+        step_count = state.step_count + 1
+        next_state = State(
+            cube=cube,
+            step_count=step_count,
+            key=state.key,
+        )
+        reward = self.reward_function(state=next_state)
+        solved = is_solved(cube)
+        done = (step_count >= self.time_limit) | solved
+        next_observation = self._state_to_observation(state=next_state)
+        next_timestep = jax.lax.cond(
+            done,
             termination,
             transition,
             reward,
-            observation,
+            next_observation,
         )
-        return next_state, timestep
+        return next_state, next_timestep
 
     def observation_spec(self) -> specs.Spec[Observation]:
-        """Returns the observation spec.
+        """Specifications of the observation of the `RubiksCube` environment.
 
         Returns:
-            Spec for the `Observation` whose fields are:
-            - coordinates: BoundedArray (float) of shape (num_cities,).
-            - position: DiscreteArray (num_values = num_cities) of shape ().
-            - trajectory: BoundedArray (int32) of shape (num_cities,).
-            - action_mask: BoundedArray (bool) of shape (num_cities,).
-        """
-        coordinates = specs.BoundedArray(
-            shape=(self.num_cities, 2),
-            minimum=0.0,
-            maximum=1.0,
-            dtype=float,
-            name="coordinates",
-        )
-        position = specs.DiscreteArray(
-            self.num_cities, dtype=jnp.int32, name="position"
+            Spec containing all the specifications for all the `Observation` fields:
+             - cube: BoundedArray (jnp.int8) of shape (num_faces, cube_size, cube_size).
+             - step_count: BoundedArray (jnp.int32) of shape ().
+        """
+        cube = specs.BoundedArray(
+            shape=(len(Face), self.generator.cube_size, self.generator.cube_size),
+            dtype=jnp.int8,
+            minimum=0,
+            maximum=len(Face) - 1,
+            name="cube",
         )
-        trajectory = specs.BoundedArray(
-            shape=(self.num_cities,),
+        step_count = specs.BoundedArray(
+            shape=(),
             dtype=jnp.int32,
-            minimum=-1,
-            maximum=self.num_cities - 1,
-            name="trajectory",
-        )
-        action_mask = specs.BoundedArray(
-            shape=(self.num_cities,),
-            dtype=bool,
-            minimum=False,
-            maximum=True,
-            name="action_mask",
+            minimum=0,
+            maximum=self.time_limit,
+            name="step_count",
         )
         return specs.Spec(
             Observation,
             "ObservationSpec",
-            coordinates=coordinates,
-            position=position,
-            trajectory=trajectory,
-            action_mask=action_mask,
+            cube=cube,
+            step_count=step_count,
         )
 
-    def action_spec(self) -> specs.DiscreteArray:
-        """Returns the action spec.
+    def action_spec(self) -> specs.MultiDiscreteArray:
+        """Returns the action spec. An action is composed of 3 elements that range in: 6 faces, each
+        with cube_size//2 possible depths, and 3 possible directions.
 
         Returns:
-            action_spec: a `specs.DiscreteArray` spec.
+            action_spec: `MultiDiscreteArray` object.
         """
-        return specs.DiscreteArray(self.num_cities, name="action")
+        return specs.MultiDiscreteArray(
+            num_values=jnp.array(
+                [len(Face), self.generator.cube_size // 2, 3], jnp.int32
+            ),
+            name="action",
+            dtype=jnp.int32,
+        )
+
+    def _state_to_observation(self, state: State) -> Observation:
+        return Observation(cube=state.cube, step_count=state.step_count)
 
     def render(self, state: State) -> Optional[NDArray]:
-        """Render the given state of the environment. This rendering shows the layout of the cities
-        and the tour so far.
+        """Renders the current state of the cube.
 
         Args:
-            state: current environment state.
-
-        Returns:
-            rgb_array: the RGB image of the state as an array.
+            state: the current state to be rendered.
         """
-        return self._env_viewer.render(state)
+        return self._viewer.render(state=state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
-        """Creates an animated gif of the `TSP` environment based on the sequence of states.
+        """Creates an animated gif of the cube based on the sequence of states.
 
         Args:
-            states: sequence of environment states corresponding to consecutive timesteps.
-            interval: delay between frames in milliseconds, default to 200.
+            states: a list of `State` objects representing the sequence of game states.
+            interval: the delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
             animation.FuncAnimation: the animation object that was created.
         """
-        return self._env_viewer.animate(states, interval, save_path)
+        return self._viewer.animate(
+            states=states, interval=interval, save_path=save_path
+        )
 
     def close(self) -> None:
         """Perform any necessary cleanup.
 
         Environments will automatically :meth:`close()` themselves when
         garbage collected or when the program exits.
         """
-        self._env_viewer.close()
-
-    def _update_state(self, state: State, action: chex.Numeric) -> State:
-        """
-        Updates the state of the environment.
-
-        Args:
-            state: State object containing the dynamics of the environment.
-            action: int32, index of the next position to visit.
-
-        Returns:
-            state: State object corresponding to the new state of the environment.
-        """
-        return State(
-            coordinates=state.coordinates,
-            position=action,
-            visited_mask=state.visited_mask.at[action].set(True),
-            trajectory=state.trajectory.at[state.num_visited].set(action),
-            num_visited=state.num_visited + 1,
-            key=state.key,
-        )
-
-    def _state_to_observation(self, state: State) -> Observation:
-        """Converts a state into an observation.
-
-        Args:
-            state: `State` object containing the dynamics of the environment.
-
-        Returns:
-            observation: `Observation` object containing the observation of the environment.
-        """
-        return Observation(
-            coordinates=state.coordinates,
-            position=state.position,
-            trajectory=state.trajectory,
-            action_mask=~state.visited_mask,
-        )
+        self._viewer.close()
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/tsp/env_viewer.py` & `jumanji-0.2.2/jumanji/environments/routing/tsp/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import matplotlib.animation
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.typing import NDArray
 
 import jumanji.environments
 from jumanji.environments.routing.tsp.types import State
+from jumanji.viewer import Viewer
 
 
-class TSPViewer:
+class TSPViewer(Viewer):
     FIGURE_SIZE = (10.0, 10.0)
     NODE_COLOUR = "dimgray"
     NODE_SIZE = 150
     ARROW_WIDTH = 0.004
 
     def __init__(self, name: str, render_mode: str = "human") -> None:
         """Viewer for the TSP environment.
```

### Comparing `jumanji-0.2.1/jumanji/environments/routing/tsp/reward.py` & `jumanji-0.2.2/jumanji/environments/routing/tsp/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/environments/routing/tsp/types.py` & `jumanji-0.2.2/jumanji/environments/routing/tsp/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/registration.py` & `jumanji-0.2.2/jumanji/registration.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/specs.py` & `jumanji-0.2.2/jumanji/specs.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/testing/__init__.py` & `jumanji-0.2.2/jumanji/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/testing/env_not_smoke.py` & `jumanji-0.2.2/jumanji/testing/env_not_smoke.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/testing/fakes.py` & `jumanji-0.2.2/jumanji/testing/fakes.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/testing/pytrees.py` & `jumanji-0.2.2/jumanji/testing/pytrees.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/__init__.py` & `jumanji-0.2.2/jumanji/training/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/agents/__init__.py` & `jumanji-0.2.2/jumanji/training/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/agents/a2c/__init__.py` & `jumanji-0.2.2/jumanji/training/agents/a2c/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/agents/a2c/a2c_agent.py` & `jumanji-0.2.2/jumanji/training/agents/a2c/a2c_agent.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/agents/base.py` & `jumanji-0.2.2/jumanji/training/agents/base.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/agents/random/__init__.py` & `jumanji-0.2.2/jumanji/training/agents/random/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/agents/random/random_agent.py` & `jumanji-0.2.2/jumanji/training/agents/random/random_agent.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/evaluator.py` & `jumanji-0.2.2/jumanji/training/evaluator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/loggers.py` & `jumanji-0.2.2/jumanji/training/loggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     def write(
         self,
         data: Dict[str, Any],
         label: Optional[str] = None,
         env_steps: Optional[int] = None,
     ) -> None:
         if env_steps is not None:
-            env_steps_str = f"Env steps: {env_steps:.2e} | "
+            env_steps_str = f"Env Steps: {env_steps:.2e} | "
         else:
             env_steps_str = ""
         label_str = f"{label.replace('_', ' ').title()} >> " if label else ""
         logging.info(label_str + env_steps_str + self._format_values(data))
 
 
 class ListLogger(Logger):
```

### Comparing `jumanji-0.2.1/jumanji/training/networks/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/base.py` & `jumanji-0.2.2/jumanji/training/networks/base.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/bin_pack/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/bin_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/bin_pack/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/bin_pack/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/bin_pack/random.py` & `jumanji-0.2.2/jumanji/training/networks/bin_pack/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/cleaner/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/cleaner/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/cleaner/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/cleaner/random.py` & `jumanji-0.2.2/jumanji/training/networks/cleaner/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/connector/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/connector/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/connector/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/connector/random.py` & `jumanji-0.2.2/jumanji/training/networks/connector/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/cvrp/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/cvrp/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/cvrp/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/cvrp/random.py` & `jumanji-0.2.2/jumanji/training/networks/cvrp/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/distribution.py` & `jumanji-0.2.2/jumanji/training/networks/distribution.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/game_2048/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/game_2048/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/game_2048/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/game_2048/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/game_2048/random.py` & `jumanji-0.2.2/jumanji/training/networks/game_2048/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/job_shop/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/job_shop/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/job_shop/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/job_shop/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/job_shop/random.py` & `jumanji-0.2.2/jumanji/training/networks/job_shop/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/knapsack/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/knapsack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/knapsack/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/knapsack/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/knapsack/random.py` & `jumanji-0.2.2/jumanji/training/networks/knapsack/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/masked_categorical_random.py` & `jumanji-0.2.2/jumanji/training/networks/masked_categorical_random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/maze/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/maze/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/maze/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/maze/random.py` & `jumanji-0.2.2/jumanji/training/networks/maze/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/minesweeper/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/minesweeper/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/minesweeper/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/minesweeper/actor_critic.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,36 +36,36 @@
     board_embed_dim: int,
     board_conv_channels: Sequence[int],
     board_kernel_shape: int,
     num_mines_embed_dim: int,
     final_layer_dims: Sequence[int],
 ) -> ActorCriticNetworks:
     """Make actor-critic networks for the `Minesweeper` environment."""
-    board_height = minesweeper.num_rows
-    board_width = minesweeper.num_cols
+    board_num_rows = minesweeper.num_rows
+    board_num_cols = minesweeper.num_cols
     vocab_size = 1 + PATCH_SIZE**2  # unexplored, or 0, 1, ..., 8
 
     parametric_action_distribution = FactorisedActionSpaceParametricDistribution(
         action_spec_num_values=np.asarray(minesweeper.action_spec().num_values)
     )
     policy_network = make_network_cnn(
         vocab_size=vocab_size,
-        board_height=board_height,
-        board_width=board_width,
+        board_num_rows=board_num_rows,
+        board_num_cols=board_num_cols,
         board_embed_dim=board_embed_dim,
         board_conv_channels=board_conv_channels,
         board_kernel_shape=board_kernel_shape,
         num_mines_embed_dim=num_mines_embed_dim,
         final_layer_dims=final_layer_dims,
         critic=False,
     )
     value_network = make_network_cnn(
         vocab_size=vocab_size,
-        board_height=board_height,
-        board_width=board_width,
+        board_num_rows=board_num_rows,
+        board_num_cols=board_num_cols,
         board_embed_dim=board_embed_dim,
         board_conv_channels=board_conv_channels,
         board_kernel_shape=board_kernel_shape,
         num_mines_embed_dim=num_mines_embed_dim,
         final_layer_dims=final_layer_dims,
         critic=True,
     )
@@ -74,16 +74,16 @@
         value_network=value_network,
         parametric_action_distribution=parametric_action_distribution,
     )
 
 
 def make_network_cnn(
     vocab_size: int,
-    board_height: int,
-    board_width: int,
+    board_num_rows: int,
+    board_num_cols: int,
     board_embed_dim: int,
     board_conv_channels: Sequence[int],
     board_kernel_shape: int,
     num_mines_embed_dim: int,
     final_layer_dims: Sequence[int],
     critic: bool,
 ) -> FeedForwardNetwork:
@@ -102,17 +102,17 @@
                 hk.Embed(vocab_size=vocab_size, embed_dim=board_embed_dim),
                 *[layer for conv_layer in conv_layers for layer in conv_layer],
             ]
         )
         x = board_embedder(observation.board + 1)
         num_mines_embedder = hk.Linear(num_mines_embed_dim)
         y = num_mines_embedder(
-            observation.num_mines[:, None] / (board_height * board_width)
+            observation.num_mines[:, None] / (board_num_rows * board_num_cols)
         )[:, None, None, :]
-        y = jnp.tile(y, [1, board_height, board_width, 1])
+        y = jnp.tile(y, [1, board_num_rows, board_num_cols, 1])
         output = jnp.concatenate([x, y], axis=-1)
         final_layers = hk.nets.MLP((*final_layer_dims, 1))
         output = jnp.squeeze(final_layers(output), axis=-1)
         if critic:
             return jnp.mean(output, axis=(-1, -2))
         else:
             masked_logits = jnp.where(
```

### Comparing `jumanji-0.2.1/jumanji/training/networks/minesweeper/random.py` & `jumanji-0.2.2/jumanji/training/networks/minesweeper/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/parametric_distribution.py` & `jumanji-0.2.2/jumanji/training/networks/parametric_distribution.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/postprocessor.py` & `jumanji-0.2.2/jumanji/training/networks/postprocessor.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/protocols.py` & `jumanji-0.2.2/jumanji/training/networks/protocols.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/rubiks_cube/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/rubiks_cube/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/rubiks_cube/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/rubiks_cube/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/rubiks_cube/random.py` & `jumanji-0.2.2/jumanji/training/networks/rubiks_cube/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/snake/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/snake/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/snake/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/snake/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/snake/random.py` & `jumanji-0.2.2/jumanji/training/networks/snake/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/transformer_block.py` & `jumanji-0.2.2/jumanji/training/networks/transformer_block.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/tsp/__init__.py` & `jumanji-0.2.2/jumanji/training/networks/tsp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/tsp/actor_critic.py` & `jumanji-0.2.2/jumanji/training/networks/tsp/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/networks/tsp/random.py` & `jumanji-0.2.2/jumanji/training/networks/tsp/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/setup_train.py` & `jumanji-0.2.2/jumanji/training/setup_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from typing import Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import optax
 from omegaconf import DictConfig
@@ -47,29 +48,14 @@
     TerminalLogger,
 )
 from jumanji.training.networks.actor_critic import ActorCriticNetworks
 from jumanji.training.networks.protocols import RandomPolicy
 from jumanji.training.types import ActingState, TrainingState
 from jumanji.wrappers import MultiToSingleWrapper, VmapAutoResetWrapper
 
-ENV_FACTORY = {
-    "bin_pack": BinPack,
-    "cvrp": CVRP,
-    "tsp": TSP,
-    "snake": Snake,
-    "rubiks_cube": RubiksCube,
-    "minesweeper": Minesweeper,
-    "knapsack": Knapsack,
-    "job_shop": JobShop,
-    "game_2048": Game2048,
-    "cleaner": Cleaner,
-    "maze": Maze,
-    "connector": Connector,
-}
-
 
 def setup_logger(cfg: DictConfig) -> Logger:
     logger: Logger
     if cfg.logger.type == "tensorboard":
         logger = TensorboardLogger(
             name=cfg.logger.name, save_checkpoint=cfg.logger.save_checkpoint
         )
```

### Comparing `jumanji-0.2.1/jumanji/training/timer.py` & `jumanji-0.2.2/jumanji/training/timer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/train.py` & `jumanji-0.2.2/jumanji/training/train.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/types.py` & `jumanji-0.2.2/jumanji/training/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/training/utils.py` & `jumanji-0.2.2/jumanji/training/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/tree_utils.py` & `jumanji-0.2.2/jumanji/tree_utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/types.py` & `jumanji-0.2.2/jumanji/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji/version.py` & `jumanji-0.2.2/jumanji/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `jumanji-0.2.1/jumanji/wrappers.py` & `jumanji-0.2.2/jumanji/wrappers.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/jumanji.egg-info/PKG-INFO` & `jumanji-0.2.2/jumanji.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumanji
-Version: 0.2.1
+Version: 0.2.2
 Summary: A suite of diverse and challenging RL environments in JAX
 Home-page: https://github.com/instadeepai/jumanji/
 Author: InstaDeep
 Author-email: hello@instadeep.com
 License: Apache 2.0
 Keywords: reinforcement-learning python jax
 Classifier: Development Status :: 4 - Beta
@@ -232,32 +232,33 @@
 @software{jumanji2023github,
   author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
         and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
         Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
         and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
   title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
   url = {https://github.com/instadeepai/jumanji},
-  version = {0.2.1},
+  version = {0.2.2},
   year = {2023},
 }
 ```
 
 
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
 
 - 🤖 [Qdax](https://github.com/adaptive-intelligent-robotics/QDax) is a library to accelerate
 Quality-Diversity and neuro-evolution algorithms through hardware accelerators and parallelization.
+- 🌳 [Evojax](https://github.com/google/evojax) provides tools to enable neuroevolution algorithms
+to work with neural networks running across multiple TPU/GPUs.
 - 🦾 [Brax](https://github.com/google/brax) is a differentiable physics engine that simulates
 environments made up of rigid bodies, joints, and actuators.
 - 🏋️‍ [Gymnax](https://github.com/RobertTLange/gymnax) implements classic environments including
 classic control, bsuite, MinAtar and a collection of meta RL tasks.
-- 🌳 [Evojax](https://github.com/google/evojax) provides tools to enable neuroevolution algorithms
-to work with neural networks running across multiple TPU/GPUs.
-
+- 🎲 [Pgx](https://github.com/sotetsuk/pgx) provides classic board game environments like
+Backgammon, Shogi, and Go.
 
 ## Acknowledgements 🙏
 
 The development of this library was supported with Cloud TPUs
 from Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC) 🌤.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jumanji Version: 0.2.1 Summary: A suite of diverse
+Metadata-Version: 2.1 Name: jumanji Version: 0.2.2 Summary: A suite of diverse
 and challenging RL environments in JAX Home-page: https://github.com/
 instadeepai/jumanji/ Author: InstaDeep Author-email: hello@instadeep.com
 License: Apache 2.0 Keywords: reinforcement-learning python jax Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -164,22 +164,24 @@
 guidelines. ## Citing Jumanji âï¸ If you use Jumanji in your work, please
 cite the library using: ``` @software{jumanji2023github, author = {ClÃ©ment
 Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz and Vincent Coyette
 and Paul Duckworth and Daniel Furelos-Blanco and Nathan Grinsztajn and Tristan
 Kalloniatis and Victor Le and Omayma Mahjoub and Laurence Midgley and Shikha
 Surana and Cemlyn Waters and Alexandre Laterre}, title = {Jumanji: a Suite of
 Diverse and Challenging Reinforcement Learning Environments in JAX}, url =
-{https://github.com/instadeepai/jumanji}, version = {0.2.1}, year = {2023}, }
+{https://github.com/instadeepai/jumanji}, version = {0.2.2}, year = {2023}, }
 ``` ## See Also ð Other works have embraced the approach of writing RL
 environments in JAX. In particular, we suggest users check out the following
 sister repositories: - ð¤ [Qdax](https://github.com/adaptive-intelligent-
 robotics/QDax) is a library to accelerate Quality-Diversity and neuro-evolution
-algorithms through hardware accelerators and parallelization. - ð¦¾ [Brax]
-(https://github.com/google/brax) is a differentiable physics engine that
-simulates environments made up of rigid bodies, joints, and actuators. -
+algorithms through hardware accelerators and parallelization. - ð³ [Evojax]
+(https://github.com/google/evojax) provides tools to enable neuroevolution
+algorithms to work with neural networks running across multiple TPU/GPUs. -
+ð¦¾ [Brax](https://github.com/google/brax) is a differentiable physics engine
+that simulates environments made up of rigid bodies, joints, and actuators. -
 ðï¸â [Gymnax](https://github.com/RobertTLange/gymnax) implements classic
 environments including classic control, bsuite, MinAtar and a collection of
-meta RL tasks. - ð³ [Evojax](https://github.com/google/evojax) provides tools
-to enable neuroevolution algorithms to work with neural networks running across
-multiple TPU/GPUs. ## Acknowledgements ð The development of this library was
-supported with Cloud TPUs from Google's [TPU Research Cloud](https://
-sites.research.google/trc/about/) (TRC) ð¤.
+meta RL tasks. - ð² [Pgx](https://github.com/sotetsuk/pgx) provides classic
+board game environments like Backgammon, Shogi, and Go. ## Acknowledgements
+ð The development of this library was supported with Cloud TPUs from
+Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC)
+ð¤.
```

### Comparing `jumanji-0.2.1/jumanji.egg-info/SOURCES.txt` & `jumanji-0.2.2/jumanji.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 jumanji/env.py
 jumanji/py.typed
 jumanji/registration.py
 jumanji/specs.py
 jumanji/tree_utils.py
 jumanji/types.py
 jumanji/version.py
+jumanji/viewer.py
 jumanji/wrappers.py
 jumanji.egg-info/PKG-INFO
 jumanji.egg-info/SOURCES.txt
 jumanji.egg-info/dependency_links.txt
 jumanji.egg-info/not-zip-safe
 jumanji.egg-info/requires.txt
 jumanji.egg-info/top_level.txt
@@ -24,83 +25,87 @@
 jumanji/environments/commons/maze_utils/__init__.py
 jumanji/environments/commons/maze_utils/maze_generation.py
 jumanji/environments/commons/maze_utils/maze_rendering.py
 jumanji/environments/commons/maze_utils/stack.py
 jumanji/environments/logic/__init__.py
 jumanji/environments/logic/game_2048/__init__.py
 jumanji/environments/logic/game_2048/env.py
-jumanji/environments/logic/game_2048/env_viewer.py
 jumanji/environments/logic/game_2048/types.py
 jumanji/environments/logic/game_2048/utils.py
+jumanji/environments/logic/game_2048/viewer.py
 jumanji/environments/logic/minesweeper/__init__.py
 jumanji/environments/logic/minesweeper/constants.py
 jumanji/environments/logic/minesweeper/done.py
 jumanji/environments/logic/minesweeper/env.py
+jumanji/environments/logic/minesweeper/generator.py
 jumanji/environments/logic/minesweeper/reward.py
 jumanji/environments/logic/minesweeper/types.py
 jumanji/environments/logic/minesweeper/utils.py
+jumanji/environments/logic/minesweeper/viewer.py
 jumanji/environments/logic/rubiks_cube/__init__.py
 jumanji/environments/logic/rubiks_cube/constants.py
 jumanji/environments/logic/rubiks_cube/env.py
+jumanji/environments/logic/rubiks_cube/generator.py
 jumanji/environments/logic/rubiks_cube/reward.py
 jumanji/environments/logic/rubiks_cube/types.py
 jumanji/environments/logic/rubiks_cube/utils.py
+jumanji/environments/logic/rubiks_cube/viewer.py
 jumanji/environments/packing/__init__.py
 jumanji/environments/packing/bin_pack/__init__.py
 jumanji/environments/packing/bin_pack/env.py
-jumanji/environments/packing/bin_pack/env_viewer.py
 jumanji/environments/packing/bin_pack/generator.py
 jumanji/environments/packing/bin_pack/reward.py
 jumanji/environments/packing/bin_pack/space.py
 jumanji/environments/packing/bin_pack/types.py
+jumanji/environments/packing/bin_pack/viewer.py
 jumanji/environments/packing/job_shop/__init__.py
 jumanji/environments/packing/job_shop/env.py
-jumanji/environments/packing/job_shop/env_viewer.py
 jumanji/environments/packing/job_shop/generator.py
 jumanji/environments/packing/job_shop/types.py
+jumanji/environments/packing/job_shop/viewer.py
 jumanji/environments/packing/knapsack/__init__.py
 jumanji/environments/packing/knapsack/env.py
-jumanji/environments/packing/knapsack/env_viewer.py
 jumanji/environments/packing/knapsack/reward.py
 jumanji/environments/packing/knapsack/types.py
+jumanji/environments/packing/knapsack/viewer.py
 jumanji/environments/routing/__init__.py
 jumanji/environments/routing/cleaner/__init__.py
 jumanji/environments/routing/cleaner/constants.py
 jumanji/environments/routing/cleaner/env.py
-jumanji/environments/routing/cleaner/env_viewer.py
 jumanji/environments/routing/cleaner/generator.py
 jumanji/environments/routing/cleaner/types.py
+jumanji/environments/routing/cleaner/viewer.py
 jumanji/environments/routing/connector/__init__.py
 jumanji/environments/routing/connector/constants.py
 jumanji/environments/routing/connector/env.py
-jumanji/environments/routing/connector/env_viewer.py
 jumanji/environments/routing/connector/generator.py
 jumanji/environments/routing/connector/reward.py
 jumanji/environments/routing/connector/types.py
 jumanji/environments/routing/connector/utils.py
+jumanji/environments/routing/connector/viewer.py
 jumanji/environments/routing/cvrp/__init__.py
 jumanji/environments/routing/cvrp/constants.py
 jumanji/environments/routing/cvrp/env.py
-jumanji/environments/routing/cvrp/env_viewer.py
 jumanji/environments/routing/cvrp/reward.py
 jumanji/environments/routing/cvrp/types.py
+jumanji/environments/routing/cvrp/viewer.py
 jumanji/environments/routing/maze/__init__.py
 jumanji/environments/routing/maze/constants.py
 jumanji/environments/routing/maze/env.py
-jumanji/environments/routing/maze/env_viewer.py
 jumanji/environments/routing/maze/generator.py
 jumanji/environments/routing/maze/types.py
+jumanji/environments/routing/maze/viewer.py
 jumanji/environments/routing/snake/__init__.py
 jumanji/environments/routing/snake/env.py
 jumanji/environments/routing/snake/types.py
 jumanji/environments/routing/tsp/__init__.py
 jumanji/environments/routing/tsp/env.py
-jumanji/environments/routing/tsp/env_viewer.py
 jumanji/environments/routing/tsp/reward.py
 jumanji/environments/routing/tsp/types.py
+jumanji/environments/routing/tsp/viewer.py
 jumanji/testing/__init__.py
 jumanji/testing/env_not_smoke.py
 jumanji/testing/fakes.py
 jumanji/testing/pytrees.py
 jumanji/training/__init__.py
 jumanji/training/evaluator.py
 jumanji/training/loggers.py
```

### Comparing `jumanji-0.2.1/jumanji.egg-info/requires.txt` & `jumanji-0.2.2/jumanji.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/pyproject.toml` & `jumanji-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/setup.cfg` & `jumanji-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.1/setup.py` & `jumanji-0.2.2/setup.py`

 * *Files identical despite different names*

