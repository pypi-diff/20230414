# Comparing `tmp/ipyparallel-8.6.0.tar.gz` & `tmp/ipyparallel-8.6.1.tar.gz`

## Comparing `ipyparallel-8.6.0.tar` & `ipyparallel-8.6.1.tar`

### file list

```diff
@@ -1,295 +1,295 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.coveragerc
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.eslintignore
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.eslintrc.js
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.flake8
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.mailmap
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.prettierignore
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/asv.conf.json
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/install.json
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/package.json
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/readthedocs.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/tsconfig.eslint.json
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/tsconfig.json
--rw-r--r--   0        0        0   202459 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/yarn.lock
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.binder/jupyter_config.json
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.binder/postBuild
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.binder/requirements.txt
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv.conf.json
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv_normal.sh
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv_quick.sh
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv_runner.py
--rw-r--r--   0        0        0   182323 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/async_benchmark.ipynb
--rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmark_result.py
--rw-r--r--   0        0        0   669564 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmark_results.ipynb
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/cluster_start.py
--rw-r--r--   0        0        0    79070 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/depth_benchmark.ipynb
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/engines_test.py
--rwxr-xr-x   0        0        0     5486 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/gcloud_setup.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/instance_setup.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/logger.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling_initial_results.ipynb
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling_latest_results.ipynb
--rw-r--r--   0        0        0   160310 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/push_benchmarks.ipynb
--rw-r--r--   0        0        0   862420 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/scheduler_benchmarks.ipynb
--rw-r--r--   0        0        0   147522 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/throughtput_benchmarks.ipynb
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/testing.py
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/throughput.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/utils.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/explore/control_flow.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/explore/scheduler.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-16.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-32.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-64.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-96.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/profiling_code.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/profiling_code_runner.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/view_profiling_results.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/benchmarks.json
--rw-r--r--   0        0        0    16442 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json
--rw-r--r--   0        0        0    32378 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json
--rw-r--r--   0        0        0    36602 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json
--rw-r--r--   0        0        0    49624 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json
--rw-r--r--   0        0        0    70610 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/Dockerfile
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/docker-compose.yaml
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/entrypoint.sh
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/slurm.conf
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/ssh/Dockerfile
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/ssh/docker-compose.yaml
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/ssh/ipcluster_config.py
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/Makefile
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/make.bat
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/requirements.txt
--rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/changelog.md
--rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/conf.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/index.md
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/links.txt
--rw-r--r--   0        0        0   234426 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/_static/IPyParallel-MPI-Example.png
--rw-r--r--   0        0        0    69226 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/_static/basic.mp4
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/api/ipyparallel.rst
--rw-r--r--   0        0        0    26434 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Cluster API.ipynb
--rw-r--r--   0        0        0   279116 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Data Publication API.ipynb
--rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Futures.ipynb
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Index.ipynb
--rw-r--r--   0        0        0    67353 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb
--rw-r--r--   0        0        0    62592 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb
--rw-r--r--   0        0        0   165516 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Monte Carlo Options.ipynb
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Parallel Decorator and map.ipynb
--rw-r--r--   0        0        0  3554371 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Parallel Magics.ipynb
--rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Using Dill.ipynb
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Using MPI with IPython Parallel.ipynb
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/customresults.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/dagdeps.py
--rw-r--r--   0        0        0    42291 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/dask.ipynb
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/dependencies.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/fetchparse.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/iopubwatcher.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/itermapresult.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/joblib.ipynb
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/nwmerge.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/phistogram.py
--rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/progress.ipynb
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/task_mod.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/task_profiler.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/throughput.py
--rw-r--r--   0        0        0   329806 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/visualizing-tasks.ipynb
--rw-r--r--   0        0        0   439979 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/Broadcast view.ipynb
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/Dockerfile
--rw-r--r--   0        0        0    69566 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/MPI Broadcast.ipynb
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/docker-compose.yaml
--rw-r--r--   0        0        0    84423 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/memmap Broadcast.ipynb
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/pwordfreq.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/wordfreq.py
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/bintree.py
--rwxr-xr-x   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/bintree_script.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/communicator.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/interengine.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/pi/parallelpi.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/pi/pidigits.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipy
--rw-r--r--   0        0        0    45443 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipynb
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/rmt/rmtkernel.py
--rwxr-xr-x   0        0        0    19532 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/RectPartitioner.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/communicator.py
--rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave-mpi.py
--rwxr-xr-x   0        0        0     7405 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave.py
--rwxr-xr-x   0        0        0    11642 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/wavesolver.py
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/connections.md
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/dag_dependencies.md
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/db.md
--rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/details.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/index.md
--rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/launchers.md
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/messages.md
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/mpi.md
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/security.md
--rw-r--r--   0        0        0    32144 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/allconnections.png
--rw-r--r--   0        0        0   303213 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/allconnections.svg
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.pdf
--rw-r--r--   0        0        0   202436 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.png
--rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.png
--rw-r--r--   0        0        0   283962 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.svg
--rw-r--r--   0        0        0    38554 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/hbfade.png
--rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/iopubfade.png
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.png
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.svg
--rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.png
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.svg
--rw-r--r--   0        0        0    30974 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.png
--rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.svg
--rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/notiffade.png
--rw-r--r--   0        0        0    41180 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.png
--rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.svg
--rw-r--r--   0        0        0    38260 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/queryfade.png
--rw-r--r--   0        0        0    40459 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/queuefade.png
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/simpledag.pdf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/simpledag.png
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/asyncresult.md
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/demos.md
--rw-r--r--   0        0        0    23931 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/direct.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/index.md
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/intro.md
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/magics.md
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/process.md
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/task.md
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.pdf
--rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.png
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.pdf
--rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.png
--rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.pdf
--rw-r--r--   0        0        0    50744 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.png
--rw-r--r--   0        0        0   128061 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.pdf
--rw-r--r--   0        0        0   115825 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.png
--rw-r--r--   0        0        0    41799 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.pdf
--rw-r--r--   0        0        0    36727 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.png
--rw-r--r--   0        0        0    74773 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.pdf
--rw-r--r--   0        0        0    73675 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.png
--rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/wideView.png
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/__init__.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/_async.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/_version.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/datapub.py
--rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/error.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/joblib.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/logger.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/traitlets.py
--rw-r--r--   0        0        0    23239 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/baseapp.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/ipclusterapp.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/ipcontrollerapp.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/ipengineapp.py
--rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/iploggerapp.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/launcher.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/logwatcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/__init__.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/_joblib.py
--rw-r--r--   0        0        0    42102 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/asyncresult.py
--rw-r--r--   0        0        0    91902 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/client.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/futures.py
--rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/magics.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/map.py
--rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/remotefunction.py
--rw-r--r--   0        0        0    54129 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/view.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/__main__.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/_winhpcjob.py
--rwxr-xr-x   0        0        0    23629 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/app.py
--rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/cluster.py
--rw-r--r--   0        0        0    84108 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/launcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/__main__.py
--rwxr-xr-x   0        0        0    44147 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/app.py
--rw-r--r--   0        0        0     8820 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/broadcast_scheduler.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/dependency.py
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/dictdb.py
--rwxr-xr-x   0        0        0    10768 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/heartmonitor.py
--rw-r--r--   0        0        0    55731 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/hub.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/mongodb.py
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/scheduler.py
--rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/sqlitedb.py
--rw-r--r--   0        0        0    27127 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/task_scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/__main__.py
--rwxr-xr-x   0        0        0    33960 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/app.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/datapub.py
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/kernel.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/log.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/nanny.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/package.json
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/schemas/ipyparallel-labextension/plugin.json
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js
--rw-r--r--   0        0        0    25407 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/remoteEntry.1bb490d7217e637c4abe.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/style.js
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/__init__.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/base.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/handlers.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/install.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/static/clusterlist.css
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/static/clusterlist.js
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/static/main.js
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/__init__.py
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/canning.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/codeutil.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/serialize.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/_test_startup_crash.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/clienttest.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/conftest.py
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_apps.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_async.py
--rw-r--r--   0        0        0    18324 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_asyncresult.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_canning.py
--rw-r--r--   0        0        0    24230 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_client.py
--rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_cluster.py
--rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_db.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_dependency.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_executor.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_joblib.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_launcher.py
--rw-r--r--   0        0        0     8908 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_lbview.py
--rw-r--r--   0        0        0    18314 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_magics.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_mongodb.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_mpi.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_remotefunction.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_serialize.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_slurm.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_ssh.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_util.py
--rw-r--r--   0        0        0    29722 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_view.py
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_view_broadcast.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/jupyter-config/jupyter_notebook_config.d/ipyparallel.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/jupyter-config/jupyter_server_config.d/ipyparallel.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/jupyter-config/nbconfig/tree.d/ipyparallel.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/webpack.config.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/schema/plugin.json
--rw-r--r--   0        0        0    23367 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/clusters.tsx
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/commands.ts
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/dialog.tsx
--rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/index.ts
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/sidebar.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/svg.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/code-dark.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/code-light.svg
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/index.css
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/logo.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.gitignore
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/COPYING.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/hatch_build.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.coveragerc
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.eslintignore
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.eslintrc.js
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.flake8
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.mailmap
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.prettierignore
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/asv.conf.json
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/install.json
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/package.json
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/readthedocs.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/tsconfig.json
+-rw-r--r--   0        0        0   202459 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/yarn.lock
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.binder/jupyter_config.json
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.binder/postBuild
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.binder/requirements.txt
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv.conf.json
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv_normal.sh
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv_quick.sh
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv_runner.py
+-rw-r--r--   0        0        0   182323 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/async_benchmark.ipynb
+-rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmark_result.py
+-rw-r--r--   0        0        0   669564 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmark_results.ipynb
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/cluster_start.py
+-rw-r--r--   0        0        0    79070 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/depth_benchmark.ipynb
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/engines_test.py
+-rwxr-xr-x   0        0        0     5486 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/gcloud_setup.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/instance_setup.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/logger.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling_initial_results.ipynb
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling_latest_results.ipynb
+-rw-r--r--   0        0        0   160310 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/push_benchmarks.ipynb
+-rw-r--r--   0        0        0   862420 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/scheduler_benchmarks.ipynb
+-rw-r--r--   0        0        0   147522 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/throughtput_benchmarks.ipynb
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/testing.py
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/throughput.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/utils.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/explore/control_flow.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/explore/scheduler.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-16.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-32.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-64.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-96.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/profiling_code.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/profiling_code_runner.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/view_profiling_results.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/benchmarks.json
+-rw-r--r--   0        0        0    16442 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json
+-rw-r--r--   0        0        0    32378 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json
+-rw-r--r--   0        0        0    36602 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json
+-rw-r--r--   0        0        0    49624 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json
+-rw-r--r--   0        0        0    70610 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/Dockerfile
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/docker-compose.yaml
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/entrypoint.sh
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/slurm.conf
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/ssh/Dockerfile
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/ssh/docker-compose.yaml
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/ssh/ipcluster_config.py
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/Makefile
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/make.bat
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0    17267 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/changelog.md
+-rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/conf.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/index.md
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/links.txt
+-rw-r--r--   0        0        0   234426 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/_static/IPyParallel-MPI-Example.png
+-rw-r--r--   0        0        0    69226 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/_static/basic.mp4
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/api/ipyparallel.rst
+-rw-r--r--   0        0        0    26434 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Cluster API.ipynb
+-rw-r--r--   0        0        0   279116 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Data Publication API.ipynb
+-rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Futures.ipynb
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Index.ipynb
+-rw-r--r--   0        0        0    67353 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb
+-rw-r--r--   0        0        0    62592 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb
+-rw-r--r--   0        0        0   165516 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Monte Carlo Options.ipynb
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Parallel Decorator and map.ipynb
+-rw-r--r--   0        0        0  3554371 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Parallel Magics.ipynb
+-rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Using Dill.ipynb
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Using MPI with IPython Parallel.ipynb
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/customresults.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/dagdeps.py
+-rw-r--r--   0        0        0    42291 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/dask.ipynb
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/dependencies.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/fetchparse.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/iopubwatcher.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/itermapresult.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/joblib.ipynb
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/nwmerge.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/phistogram.py
+-rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/progress.ipynb
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/task_mod.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/task_profiler.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/throughput.py
+-rw-r--r--   0        0        0   329806 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/visualizing-tasks.ipynb
+-rw-r--r--   0        0        0   439979 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/Broadcast view.ipynb
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/Dockerfile
+-rw-r--r--   0        0        0    69566 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/MPI Broadcast.ipynb
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/docker-compose.yaml
+-rw-r--r--   0        0        0    84423 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/memmap Broadcast.ipynb
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/pwordfreq.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/wordfreq.py
+-rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/bintree.py
+-rwxr-xr-x   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/bintree_script.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/communicator.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/interengine.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/pi/parallelpi.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/pi/pidigits.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipy
+-rw-r--r--   0        0        0    45443 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipynb
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/rmt/rmtkernel.py
+-rwxr-xr-x   0        0        0    19532 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/RectPartitioner.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/communicator.py
+-rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave-mpi.py
+-rwxr-xr-x   0        0        0     7405 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave.py
+-rwxr-xr-x   0        0        0    11642 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/wavesolver.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/connections.md
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/dag_dependencies.md
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/db.md
+-rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/details.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/index.md
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/launchers.md
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/messages.md
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/mpi.md
+-rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/security.md
+-rw-r--r--   0        0        0    32144 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/allconnections.png
+-rw-r--r--   0        0        0   303213 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/allconnections.svg
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.pdf
+-rw-r--r--   0        0        0   202436 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.png
+-rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.png
+-rw-r--r--   0        0        0   283962 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.svg
+-rw-r--r--   0        0        0    38554 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/hbfade.png
+-rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/iopubfade.png
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.png
+-rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.svg
+-rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.png
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.svg
+-rw-r--r--   0        0        0    30974 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.png
+-rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.svg
+-rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/notiffade.png
+-rw-r--r--   0        0        0    41180 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.png
+-rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.svg
+-rw-r--r--   0        0        0    38260 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/queryfade.png
+-rw-r--r--   0        0        0    40459 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/queuefade.png
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/simpledag.pdf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/simpledag.png
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/asyncresult.md
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/demos.md
+-rw-r--r--   0        0        0    23931 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/direct.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/index.md
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/intro.md
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/magics.md
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/process.md
+-rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/task.md
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.pdf
+-rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.png
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.pdf
+-rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.png
+-rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.pdf
+-rw-r--r--   0        0        0    50744 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.png
+-rw-r--r--   0        0        0   128061 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.pdf
+-rw-r--r--   0        0        0   115825 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.png
+-rw-r--r--   0        0        0    41799 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.pdf
+-rw-r--r--   0        0        0    36727 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.png
+-rw-r--r--   0        0        0    74773 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.pdf
+-rw-r--r--   0        0        0    73675 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.png
+-rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/wideView.png
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/__init__.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/_async.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/_version.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/datapub.py
+-rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/error.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/joblib.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/logger.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/traitlets.py
+-rw-r--r--   0        0        0    23239 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/baseapp.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/ipclusterapp.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/ipcontrollerapp.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/ipengineapp.py
+-rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/iploggerapp.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/launcher.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/logwatcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/__init__.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/_joblib.py
+-rw-r--r--   0        0        0    42109 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/asyncresult.py
+-rw-r--r--   0        0        0    91891 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/client.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/futures.py
+-rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/magics.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/map.py
+-rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/remotefunction.py
+-rw-r--r--   0        0        0    54129 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/view.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/__main__.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/_winhpcjob.py
+-rwxr-xr-x   0        0        0    23629 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/app.py
+-rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/cluster.py
+-rw-r--r--   0        0        0    84108 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/launcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/__main__.py
+-rwxr-xr-x   0        0        0    44147 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/app.py
+-rw-r--r--   0        0        0     8820 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/broadcast_scheduler.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/dependency.py
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/dictdb.py
+-rwxr-xr-x   0        0        0    10768 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/heartmonitor.py
+-rw-r--r--   0        0        0    55731 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/hub.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/mongodb.py
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/scheduler.py
+-rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/sqlitedb.py
+-rw-r--r--   0        0        0    27127 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/task_scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/__main__.py
+-rwxr-xr-x   0        0        0    33960 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/app.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/datapub.py
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/kernel.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/log.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/nanny.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/package.json
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/schemas/ipyparallel-labextension/plugin.json
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js
+-rw-r--r--   0        0        0    25407 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js
+-rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/remoteEntry.f5bc00ef0248261af0b1.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/style.js
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/__init__.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/base.py
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/handlers.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/install.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/static/clusterlist.css
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/static/clusterlist.js
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/static/main.js
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/__init__.py
+-rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/canning.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/codeutil.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/serialize.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/_test_startup_crash.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/clienttest.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/conftest.py
+-rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_apps.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_async.py
+-rw-r--r--   0        0        0    19138 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_asyncresult.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_canning.py
+-rw-r--r--   0        0        0    24230 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_client.py
+-rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_cluster.py
+-rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_db.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_dependency.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_executor.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_joblib.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_launcher.py
+-rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_lbview.py
+-rw-r--r--   0        0        0    19042 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_magics.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_mongodb.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_mpi.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_remotefunction.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_serialize.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_slurm.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_ssh.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_util.py
+-rw-r--r--   0        0        0    29736 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_view.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_view_broadcast.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/jupyter-config/jupyter_notebook_config.d/ipyparallel.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/jupyter-config/jupyter_server_config.d/ipyparallel.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/jupyter-config/nbconfig/tree.d/ipyparallel.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/webpack.config.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/schema/plugin.json
+-rw-r--r--   0        0        0    23367 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/clusters.tsx
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/commands.ts
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/dialog.tsx
+-rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/index.ts
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/sidebar.ts
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/svg.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/code-dark.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/code-light.svg
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/index.css
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/logo.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.gitignore
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/COPYING.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/hatch_build.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/PKG-INFO
```

### Comparing `ipyparallel-8.6.0/.eslintrc.js` & `ipyparallel-8.6.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/.flake8` & `ipyparallel-8.6.1/.flake8`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/.mailmap` & `ipyparallel-8.6.1/.mailmap`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/.pre-commit-config.yaml` & `ipyparallel-8.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/CONTRIBUTING.md` & `ipyparallel-8.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/package.json` & `ipyparallel-8.6.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'8.6.1'"}*

```diff
@@ -91,9 +91,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.6.0"
+    "version": "8.6.1"
 }
```

### Comparing `ipyparallel-8.6.0/tsconfig.json` & `ipyparallel-8.6.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/yarn.lock` & `ipyparallel-8.6.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/.binder/postBuild` & `ipyparallel-8.6.1/.binder/postBuild`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/.github/workflows/release.yml` & `ipyparallel-8.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/.github/workflows/test.yml` & `ipyparallel-8.6.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/asv_runner.py` & `ipyparallel-8.6.1/benchmarks/asv_runner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/async_benchmark.ipynb` & `ipyparallel-8.6.1/benchmarks/async_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/benchmark_result.py` & `ipyparallel-8.6.1/benchmarks/benchmark_result.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/benchmark_results.ipynb` & `ipyparallel-8.6.1/benchmarks/benchmark_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/cluster_start.py` & `ipyparallel-8.6.1/benchmarks/cluster_start.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/depth_benchmark.ipynb` & `ipyparallel-8.6.1/benchmarks/depth_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/gcloud_setup.py` & `ipyparallel-8.6.1/benchmarks/gcloud_setup.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/instance_setup.py` & `ipyparallel-8.6.1/benchmarks/instance_setup.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/logger.py` & `ipyparallel-8.6.1/benchmarks/logger.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/profiling_initial_results.ipynb` & `ipyparallel-8.6.1/benchmarks/profiling_initial_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/profiling_latest_results.ipynb` & `ipyparallel-8.6.1/benchmarks/profiling_latest_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/push_benchmarks.ipynb` & `ipyparallel-8.6.1/benchmarks/push_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/scheduler_benchmarks.ipynb` & `ipyparallel-8.6.1/benchmarks/scheduler_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/throughtput_benchmarks.ipynb` & `ipyparallel-8.6.1/benchmarks/throughtput_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/benchmarks/throughput.py` & `ipyparallel-8.6.1/benchmarks/benchmarks/throughput.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/benchmarks/utils.py` & `ipyparallel-8.6.1/benchmarks/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/explore/control_flow.py` & `ipyparallel-8.6.1/benchmarks/explore/control_flow.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/profiling/profiling_code.py` & `ipyparallel-8.6.1/benchmarks/profiling/profiling_code.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/profiling/profiling_code_runner.py` & `ipyparallel-8.6.1/benchmarks/profiling/profiling_code_runner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/profiling/view_profiling_results.py` & `ipyparallel-8.6.1/benchmarks/profiling/view_profiling_results.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/results/benchmarks.json` & `ipyparallel-8.6.1/benchmarks/results/benchmarks.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json` & `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json` & `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json` & `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json` & `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json` & `ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json` & `ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ci/slurm/Dockerfile` & `ipyparallel-8.6.1/ci/slurm/Dockerfile`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ci/slurm/docker-compose.yaml` & `ipyparallel-8.6.1/ci/slurm/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ci/slurm/slurm.conf` & `ipyparallel-8.6.1/ci/slurm/slurm.conf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ci/ssh/Dockerfile` & `ipyparallel-8.6.1/ci/ssh/Dockerfile`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ci/ssh/ipcluster_config.py` & `ipyparallel-8.6.1/ci/ssh/ipcluster_config.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/Makefile` & `ipyparallel-8.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/make.bat` & `ipyparallel-8.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/changelog.md` & `ipyparallel-8.6.1/docs/source/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 # Changelog
 
 Changes in IPython Parallel
 
 ## 8.6
 
+### 8.6.1
+
+([full changelog](https://github.com/ipython/ipyparallel/compare/8.6.0...8.6.1))
+
+### Bugs fixed
+
+- avoid errors when engine id cannot be identified [#793](https://github.com/ipython/ipyparallel/pull/793) ([@minrk](https://github.com/minrk))
+- Disable variable expansion in %px [#792](https://github.com/ipython/ipyparallel/pull/792) ([@minrk](https://github.com/minrk))
+- fix wait_interactive(return_when=FIRST_EXCEPTION) when there are no errors [#790](https://github.com/ipython/ipyparallel/pull/790) ([@minrk](https://github.com/minrk))
+
 ### 8.6.0
 
 A tiny release fixing issues seen building notebooks with jupyter-book.
 
 ([full changelog](https://github.com/ipython/ipyparallel/compare/8.5.1...8.6.0))
 
 - Fix KeyError on parent_header when streaming output with %%px
```

### Comparing `ipyparallel-8.6.0/docs/source/conf.py` & `ipyparallel-8.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/index.md` & `ipyparallel-8.6.1/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/links.txt` & `ipyparallel-8.6.1/docs/source/links.txt`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/_static/IPyParallel-MPI-Example.png` & `ipyparallel-8.6.1/docs/source/_static/IPyParallel-MPI-Example.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/_static/basic.mp4` & `ipyparallel-8.6.1/docs/source/_static/basic.mp4`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/api/ipyparallel.rst` & `ipyparallel-8.6.1/docs/source/api/ipyparallel.rst`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Cluster API.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Cluster API.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Data Publication API.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Data Publication API.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Futures.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Futures.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Index.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Index.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Monte Carlo Options.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Monte Carlo Options.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Parallel Decorator and map.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Parallel Decorator and map.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Parallel Magics.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Parallel Magics.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Using Dill.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Using Dill.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/Using MPI with IPython Parallel.ipynb` & `ipyparallel-8.6.1/docs/source/examples/Using MPI with IPython Parallel.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/customresults.py` & `ipyparallel-8.6.1/docs/source/examples/customresults.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/dagdeps.py` & `ipyparallel-8.6.1/docs/source/examples/dagdeps.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/dask.ipynb` & `ipyparallel-8.6.1/docs/source/examples/dask.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/dependencies.py` & `ipyparallel-8.6.1/docs/source/examples/dependencies.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/fetchparse.py` & `ipyparallel-8.6.1/docs/source/examples/fetchparse.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/iopubwatcher.py` & `ipyparallel-8.6.1/docs/source/examples/iopubwatcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/itermapresult.py` & `ipyparallel-8.6.1/docs/source/examples/itermapresult.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/joblib.ipynb` & `ipyparallel-8.6.1/docs/source/examples/joblib.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/nwmerge.py` & `ipyparallel-8.6.1/docs/source/examples/nwmerge.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/phistogram.py` & `ipyparallel-8.6.1/docs/source/examples/phistogram.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/progress.ipynb` & `ipyparallel-8.6.1/docs/source/examples/progress.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/task_profiler.py` & `ipyparallel-8.6.1/docs/source/examples/task_profiler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/throughput.py` & `ipyparallel-8.6.1/docs/source/examples/throughput.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/visualizing-tasks.ipynb` & `ipyparallel-8.6.1/docs/source/examples/visualizing-tasks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/broadcast/Broadcast view.ipynb` & `ipyparallel-8.6.1/docs/source/examples/broadcast/Broadcast view.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/broadcast/MPI Broadcast.ipynb` & `ipyparallel-8.6.1/docs/source/examples/broadcast/MPI Broadcast.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/broadcast/docker-compose.yaml` & `ipyparallel-8.6.1/docs/source/examples/broadcast/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/broadcast/memmap Broadcast.ipynb` & `ipyparallel-8.6.1/docs/source/examples/broadcast/memmap Broadcast.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/pwordfreq.py` & `ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/pwordfreq.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/wordfreq.py` & `ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/wordfreq.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/interengine/bintree.py` & `ipyparallel-8.6.1/docs/source/examples/interengine/bintree.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/interengine/bintree_script.py` & `ipyparallel-8.6.1/docs/source/examples/interengine/bintree_script.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/interengine/communicator.py` & `ipyparallel-8.6.1/docs/source/examples/interengine/communicator.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/interengine/interengine.py` & `ipyparallel-8.6.1/docs/source/examples/interengine/interengine.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/pi/parallelpi.py` & `ipyparallel-8.6.1/docs/source/examples/pi/parallelpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/pi/pidigits.py` & `ipyparallel-8.6.1/docs/source/examples/pi/pidigits.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipy` & `ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipy`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipynb` & `ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/rmt/rmtkernel.py` & `ipyparallel-8.6.1/docs/source/examples/rmt/rmtkernel.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/wave2D/RectPartitioner.py` & `ipyparallel-8.6.1/docs/source/examples/wave2D/RectPartitioner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/wave2D/communicator.py` & `ipyparallel-8.6.1/docs/source/examples/wave2D/communicator.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave-mpi.py` & `ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave-mpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave.py` & `ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/examples/wave2D/wavesolver.py` & `ipyparallel-8.6.1/docs/source/examples/wave2D/wavesolver.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/connections.md` & `ipyparallel-8.6.1/docs/source/reference/connections.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/dag_dependencies.md` & `ipyparallel-8.6.1/docs/source/reference/dag_dependencies.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/db.md` & `ipyparallel-8.6.1/docs/source/reference/db.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/details.md` & `ipyparallel-8.6.1/docs/source/reference/details.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/launchers.md` & `ipyparallel-8.6.1/docs/source/reference/launchers.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/messages.md` & `ipyparallel-8.6.1/docs/source/reference/messages.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/mpi.md` & `ipyparallel-8.6.1/docs/source/reference/mpi.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/security.md` & `ipyparallel-8.6.1/docs/source/reference/security.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/allconnections.png` & `ipyparallel-8.6.1/docs/source/reference/figs/allconnections.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/allconnections.svg` & `ipyparallel-8.6.1/docs/source/reference/figs/allconnections.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.pdf` & `ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.png` & `ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.png` & `ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.svg` & `ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/hbfade.png` & `ipyparallel-8.6.1/docs/source/reference/figs/hbfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/iopubfade.png` & `ipyparallel-8.6.1/docs/source/reference/figs/iopubfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.png` & `ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.svg` & `ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.png` & `ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.svg` & `ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.png` & `ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.svg` & `ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/notiffade.png` & `ipyparallel-8.6.1/docs/source/reference/figs/notiffade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.png` & `ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.svg` & `ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/queryfade.png` & `ipyparallel-8.6.1/docs/source/reference/figs/queryfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/queuefade.png` & `ipyparallel-8.6.1/docs/source/reference/figs/queuefade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/simpledag.pdf` & `ipyparallel-8.6.1/docs/source/reference/figs/simpledag.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/reference/figs/simpledag.png` & `ipyparallel-8.6.1/docs/source/reference/figs/simpledag.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/asyncresult.md` & `ipyparallel-8.6.1/docs/source/tutorial/asyncresult.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/demos.md` & `ipyparallel-8.6.1/docs/source/tutorial/demos.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/direct.md` & `ipyparallel-8.6.1/docs/source/tutorial/direct.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/intro.md` & `ipyparallel-8.6.1/docs/source/tutorial/intro.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/magics.md` & `ipyparallel-8.6.1/docs/source/tutorial/magics.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/process.md` & `ipyparallel-8.6.1/docs/source/tutorial/process.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/task.md` & `ipyparallel-8.6.1/docs/source/tutorial/task.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.pdf` & `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.png` & `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.pdf` & `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.png` & `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.pdf` & `ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.png` & `ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.pdf` & `ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.png` & `ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.pdf` & `ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.png` & `ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.pdf` & `ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.png` & `ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/docs/source/tutorial/figs/wideView.png` & `ipyparallel-8.6.1/docs/source/tutorial/figs/wideView.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/__init__.py` & `ipyparallel-8.6.1/ipyparallel/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/_async.py` & `ipyparallel-8.6.1/ipyparallel/_async.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/_version.py` & `ipyparallel-8.6.1/ipyparallel/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-__version__ = "8.6.0"
+__version__ = "8.6.1"
 
 # matches tbump regex in pyproject.toml
 _version_regex = re.compile(
     r'''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `ipyparallel-8.6.0/ipyparallel/error.py` & `ipyparallel-8.6.1/ipyparallel/error.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/joblib.py` & `ipyparallel-8.6.1/ipyparallel/joblib.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/traitlets.py` & `ipyparallel-8.6.1/ipyparallel/traitlets.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/util.py` & `ipyparallel-8.6.1/ipyparallel/util.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/apps/baseapp.py` & `ipyparallel-8.6.1/ipyparallel/apps/baseapp.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/apps/iploggerapp.py` & `ipyparallel-8.6.1/ipyparallel/apps/iploggerapp.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/apps/logwatcher.py` & `ipyparallel-8.6.1/ipyparallel/apps/logwatcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/client/_joblib.py` & `ipyparallel-8.6.1/ipyparallel/client/_joblib.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/client/asyncresult.py` & `ipyparallel-8.6.1/ipyparallel/client/asyncresult.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             display(er)
 
         if ip is None:
             return
 
         if msg_type == 'display_data':
             msg_content = msg['content']
-            _raw_text('[output:%i]' % eid)
+            _raw_text(f'[output:{eid}]')
             self._republish_displaypub(msg_content, eid)
 
     @contextmanager
     def stream_output(self):
         """Stream output for this result as it arrives.
 
         Returns a context manager, during which output is streamed.
@@ -574,17 +574,17 @@
         if self._single_result:
             results = [results]
         engine_ids = [md['engine_id'] for md in self._metadata]
 
         rdict = {}
         for engine_id, result in zip(engine_ids, results):
             if engine_id in rdict:
+                n_jobs = engine_ids.count(engine_id)
                 raise ValueError(
-                    "Cannot build dict, %i jobs ran on engine #%i"
-                    % (engine_ids.count(engine_id), engine_id)
+                    f"Cannot build dict, {n_jobs} jobs ran on engine #{engine_id}"
                 )
             else:
                 rdict[engine_id] = result
 
         return rdict
 
     @property
@@ -872,15 +872,15 @@
             if return_when is None:
                 finished = wait_result
             else:
                 done, pending = wait_result
                 if return_when == FIRST_COMPLETED:
                     finished = bool(done)
                 elif return_when == FIRST_EXCEPTION:
-                    finished = any(not ar._success for ar in done)
+                    finished = (not pending) or any(not ar._success for ar in done)
                 else:
                     raise ValueError(f"Unrecognized return_when={return_when!r}")
 
         progress_bar.update(self.progress - progress_bar.n)
         progress_bar.close()
 
     def _republish_displaypub(self, content, eid):
@@ -985,40 +985,40 @@
         targets = self.engine_id
 
         if groupby == "engine":
             for eid, stdout, stderr, outputs, r, execute_result in zip(
                 targets, stdouts, stderrs, output_lists, results, execute_results
             ):
                 if not result_only:
-                    self._display_stream(stdout, '[stdout:%i] ' % eid)
-                    self._display_stream(stderr, '[stderr:%i] ' % eid, file=sys.stderr)
+                    self._display_stream(stdout, f'[stdout:{eid}] ')
+                    self._display_stream(stderr, f'[stderr:{eid}] ', file=sys.stderr)
 
                 if get_ipython() is None:
                     # displaypub is meaningless outside IPython
                     continue
 
                 if (outputs and not result_only) or execute_result is not None:
-                    _raw_text('[output:%i]' % eid)
+                    _raw_text(f'[output:{eid}]')
 
                 if not result_only:
                     for output in outputs:
                         self._republish_displaypub(output, eid)
 
                 if execute_result is not None:
                     display(r)
 
         elif groupby in ('type', 'order'):
             if not result_only:
                 # republish stdout:
                 for eid, stdout in zip(targets, stdouts):
-                    self._display_stream(stdout, '[stdout:%i] ' % eid)
+                    self._display_stream(stdout, f'[stdout:{eid}] ')
 
                 # republish stderr:
                 for eid, stderr in zip(targets, stderrs):
-                    self._display_stream(stderr, '[stderr:%i] ' % eid, file=sys.stderr)
+                    self._display_stream(stderr, f'[stderr:{eid}] ', file=sys.stderr)
 
             if get_ipython() is None:
                 # displaypub is meaningless outside IPython
                 return
 
             if not result_only:
                 if groupby == 'order':
@@ -1026,21 +1026,21 @@
                         eid: outputs for eid, outputs in zip(targets, output_lists)
                     }
                     N = max(len(outputs) for outputs in output_lists)
                     for i in range(N):
                         for eid in targets:
                             outputs = output_dict[eid]
                             if len(outputs) >= N:
-                                _raw_text('[output:%i]' % eid)
+                                _raw_text(f'[output:{eid}]')
                                 self._republish_displaypub(outputs[i], eid)
                 else:
                     # republish displaypub output
                     for eid, outputs in zip(targets, output_lists):
                         if outputs:
-                            _raw_text('[output:%i]' % eid)
+                            _raw_text(f'[output:{eid}]')
                         for output in outputs:
                             self._republish_displaypub(output, eid)
 
             # finally, add execute_result:
             for eid, r, execute_result in zip(targets, results, execute_results):
                 if execute_result is not None:
                     display(r)
```

### Comparing `ipyparallel-8.6.0/ipyparallel/client/client.py` & `ipyparallel-8.6.1/ipyparallel/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         if '\n' in text_out and not text_out.startswith('\n'):
             # add newline for multiline reprs
             text_out = '\n' + text_out
 
         return ''.join(
             [
                 out,
-                'Out[%i:%i]: ' % (self.metadata['engine_id'], self.execution_count),
+                f"Out[{self.metadata['engine_id']}:{self.execution_count}]: ",
                 normal,
                 text_out,
             ]
         )
 
     def _repr_pretty_(self, p, cycle):
         p.text(self._plaintext())
@@ -503,15 +503,15 @@
             'task',
             'mux',
             'iopub',
             'notification',
             'registration',
             'broadcast',
         ):
-            cfg[key] = cfg['interface'] + ':%i' % cfg[key]
+            cfg[key] = f"{cfg['interface']}:{cfg[key]}"
 
         url = cfg['registration']
 
         if location is not None and addr == localhost():
             # location specified, and connection is expected to be local
             location_ip = util.ip_for_host(location)
 
@@ -705,15 +705,15 @@
                 targets = self._ids
             else:
                 raise TypeError("%r not valid str target, must be 'all'" % (targets))
         elif isinstance(targets, int):
             if targets < 0:
                 targets = self.ids[targets]
             if targets not in self._ids:
-                raise IndexError("No such engine: %i" % targets)
+                raise IndexError(f"No such engine: {targets}")
             targets = [targets]
 
         if isinstance(targets, slice):
             indices = list(range(len(self._ids))[targets])
             ids = self.ids
             targets = [ids[i] for i in indices]
```

### Comparing `ipyparallel-8.6.0/ipyparallel/client/futures.py` & `ipyparallel-8.6.1/ipyparallel/client/futures.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/client/magics.py` & `ipyparallel-8.6.1/ipyparallel/client/magics.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 import inspect
 import re
 import sys
 from textwrap import dedent
 
 from IPython.core import magic_arguments
 from IPython.core.error import UsageError
-from IPython.core.magic import Magics
+from IPython.core.magic import Magics, no_var_expand
 
 import ipyparallel as ipp
 
 from .. import error
 
 # -----------------------------------------------------------------------------
 # Definitions of magic functions for use with IPython
@@ -337,14 +337,15 @@
         if args.save_name:
             self.shell.user_ns[args.save_name] = self.last_result
             return
 
         self.last_result.get()
         self.last_result.display_outputs(groupby=args.groupby)
 
+    @no_var_expand
     def px(self, line=''):
         """Executes the given python command in parallel.
 
         Examples
         --------
         ::
```

### Comparing `ipyparallel-8.6.0/ipyparallel/client/map.py` & `ipyparallel-8.6.1/ipyparallel/client/map.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/client/remotefunction.py` & `ipyparallel-8.6.1/ipyparallel/client/remotefunction.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/client/view.py` & `ipyparallel-8.6.1/ipyparallel/client/view.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/cluster/_winhpcjob.py` & `ipyparallel-8.6.1/ipyparallel/cluster/_winhpcjob.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/cluster/app.py` & `ipyparallel-8.6.1/ipyparallel/cluster/app.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/cluster/cluster.py` & `ipyparallel-8.6.1/ipyparallel/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/cluster/launcher.py` & `ipyparallel-8.6.1/ipyparallel/cluster/launcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/app.py` & `ipyparallel-8.6.1/ipyparallel/controller/app.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/broadcast_scheduler.py` & `ipyparallel-8.6.1/ipyparallel/controller/broadcast_scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/dependency.py` & `ipyparallel-8.6.1/ipyparallel/controller/dependency.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/dictdb.py` & `ipyparallel-8.6.1/ipyparallel/controller/dictdb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/heartmonitor.py` & `ipyparallel-8.6.1/ipyparallel/controller/heartmonitor.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/hub.py` & `ipyparallel-8.6.1/ipyparallel/controller/hub.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/mongodb.py` & `ipyparallel-8.6.1/ipyparallel/controller/mongodb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/scheduler.py` & `ipyparallel-8.6.1/ipyparallel/controller/scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/sqlitedb.py` & `ipyparallel-8.6.1/ipyparallel/controller/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/controller/task_scheduler.py` & `ipyparallel-8.6.1/ipyparallel/controller/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/engine/app.py` & `ipyparallel-8.6.1/ipyparallel/engine/app.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/engine/datapub.py` & `ipyparallel-8.6.1/ipyparallel/engine/datapub.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/engine/kernel.py` & `ipyparallel-8.6.1/ipyparallel/engine/kernel.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/engine/log.py` & `ipyparallel-8.6.1/ipyparallel/engine/log.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/engine/nanny.py` & `ipyparallel-8.6.1/ipyparallel/engine/nanny.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/labextension/package.json` & `ipyparallel-8.6.1/ipyparallel/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9715277777777778%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f5bc00ef0248261af0b1.js'}}",*

 * * "'version'": "'8.6.1'"}*

```diff
@@ -49,15 +49,15 @@
         "lab/schema/*.json",
         "lab/style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ipython/ipyparallel",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1bb490d7217e637c4abe.js"
+            "load": "static/remoteEntry.f5bc00ef0248261af0b1.js"
         },
         "extension": true,
         "outputDir": "ipyparallel/labextension",
         "schemaDir": "lab/schema",
         "webpackConfig": "lab/webpack.config.js"
     },
     "keywords": [
@@ -95,9 +95,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.6.0"
+    "version": "8.6.1"
 }
```

### Comparing `ipyparallel-8.6.0/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig` & `ipyparallel-8.6.1/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'8.6.1'"}*

```diff
@@ -91,9 +91,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.6.0"
+    "version": "8.6.1"
 }
```

### Comparing `ipyparallel-8.6.0/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js` & `ipyparallel-8.6.1/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js` & `ipyparallel-8.6.1/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/labextension/static/remoteEntry.1bb490d7217e637c4abe.js` & `ipyparallel-8.6.1/ipyparallel/labextension/static/remoteEntry.f5bc00ef0248261af0b1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -108,15 +108,15 @@
                         (!i || !i.loaded && (!n != !i.eager ? n : l > i.from)) && (a[r] = {
                             get: t,
                             from: l,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (i("@lumino/polling", "1.11.4", (() => Promise.all([w.e(114), w.e(60)]).then((() => () => w(114))))), i("ipyparallel-labextension", "8.6.0", (() => Promise.all([w.e(60), w.e(592)]).then((() => () => w(592)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@lumino/polling", "1.11.4", (() => Promise.all([w.e(114), w.e(60)]).then((() => () => w(114))))), i("ipyparallel-labextension", "8.6.1", (() => Promise.all([w.e(60), w.e(592)]).then((() => () => w(592)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `ipyparallel-8.6.0/ipyparallel/labextension/static/third-party-licenses.json` & `ipyparallel-8.6.1/ipyparallel/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/nbextension/base.py` & `ipyparallel-8.6.1/ipyparallel/nbextension/base.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/nbextension/handlers.py` & `ipyparallel-8.6.1/ipyparallel/nbextension/handlers.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/nbextension/install.py` & `ipyparallel-8.6.1/ipyparallel/nbextension/install.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/nbextension/static/clusterlist.js` & `ipyparallel-8.6.1/ipyparallel/nbextension/static/clusterlist.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/nbextension/static/main.js` & `ipyparallel-8.6.1/ipyparallel/nbextension/static/main.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/serialize/__init__.py` & `ipyparallel-8.6.1/ipyparallel/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/serialize/canning.py` & `ipyparallel-8.6.1/ipyparallel/serialize/canning.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/serialize/codeutil.py` & `ipyparallel-8.6.1/ipyparallel/serialize/codeutil.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/serialize/serialize.py` & `ipyparallel-8.6.1/ipyparallel/serialize/serialize.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/__init__.py` & `ipyparallel-8.6.1/ipyparallel/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/clienttest.py` & `ipyparallel-8.6.1/ipyparallel/tests/clienttest.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                 return
             time.sleep(0.1)
         if not f():
             print("Warning: Awaited condition never arrived")
 
     test_timeout = 30
 
-    def setup(self):
+    def setup_method(self):
         self.context = zmq.Context.instance()
         if hasattr(signal, 'SIGALRM'):
             # use sigalarm for test timeout
             def _sigalarm(sig, frame):
                 raise TimeoutError(
                     f"test did not finish in {self.test_timeout} seconds"
                 )
@@ -186,15 +186,15 @@
 
         self.client = self.connect_client()
         # start every test with clean engine namespaces:
         self.client.clear(block=True)
         self.base_engine_count = len(self.client.ids)
         self.engines = []
 
-    def teardown(self):
+    def teardown_method(self):
         if len(self.client):
             self.client[:].use_pickle()
 
         # self.client.clear(block=True)
         # close fds:
         for e in filter(lambda e: e.poll() is not None, launchers):
             launchers.remove(e)
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/conftest.py` & `ipyparallel-8.6.1/ipyparallel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_apps.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_async.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_asyncresult.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_asyncresult.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return n
 
 
 def echo(x):
     return x
 
 
-class AsyncResultTest(ClusterTestCase):
+class TestAsyncResult(ClusterTestCase):
     def test_single_result_view(self):
         """various one-target views get the right value for single_result"""
         eid = self.client.ids[-1]
         ar = self.client[eid].apply_async(lambda: 42)
         assert ar.get() == 42
         ar = self.client[[eid]].apply_async(lambda: 42)
         assert ar.get() == [42]
@@ -395,15 +395,15 @@
     def test_wait_for_send(self):
         view = self.client[-1]
         view.track = True
         with pytest.raises(TimeoutError):
             # this test can fail if the send happens too quickly
             # e.g. the IO thread takes control for too long,
             # so run the test a few times
-            for i in range(3):
+            for i in range(10):
                 if i > 0:
                     print("Retrying test_wait_for_send")
                 data = os.urandom(10 * 1024 * 1024)
                 ar = view.apply_async(lambda x: x, data)
                 ar.wait_for_send(0)
         ar.wait_for_send(10)
 
@@ -513,14 +513,41 @@
         first_done = done.pop()
         assert first_done.msg_ids == amr.msg_ids[:1]
         assert amr.wait(timeout=10) == True
         done, pending = amr.wait(timeout=0, return_when=ipp.FIRST_EXCEPTION)
         assert pending == set()
         assert len(done) == len(amr)
 
+    def test_wait_interactive_first_exception(self):
+        dv = self.client[:]
+
+        ar = dv.apply_async(time.sleep, 0.2)
+        ar.wait_interactive(return_when=ipp.FIRST_EXCEPTION)
+        assert ar.done()
+
+        def fail(i):
+            print(i)
+            import time
+
+            if i == 0:
+                print(1 / i)
+            time.sleep(1)
+            return i
+
+        amr = dv.map_async(fail, range(len(dv)))
+        tic = time.perf_counter()
+        amr.wait_interactive(timeout=5, return_when=ipp.FIRST_EXCEPTION)
+        toc = time.perf_counter()
+        assert toc - tic < 4
+        done, pending = amr.wait(timeout=0, return_when=ipp.FIRST_EXCEPTION)
+        assert done
+        assert len(done) == 1
+        first_done = done.pop()
+        assert first_done.msg_ids == amr.msg_ids[:1]
+
     def test_progress(self):
         dv = self.client[:]
         amr = dv.map_async(time.sleep, [0.2] * 2 * len(dv))
         assert len(amr) == len(dv) * 2
         assert amr.progress == 0
         amr.wait_interactive()
         assert amr.progress == len(amr)
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_canning.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_canning.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_client.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_cluster.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_db.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_dependency.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 
 mixed = list(map(str, range(10)))
 completed = list(map(str, range(0, 10, 2)))
 failed = list(map(str, range(1, 10, 2)))
 
 
-class DependencyTest(ClusterTestCase):
-    def setup(self):
-        super().setup()
+class TestDependency(ClusterTestCase):
+    def setup_method(self):
+        super().setup_method()
         self.user_ns = {'__builtins__': __builtins__}
         self.view = self.client.load_balanced_view()
         self.dview = self.client[-1]
         self.succeeded = set(map(str, range(0, 25, 2)))
         self.failed = set(map(str, range(1, 25, 2)))
 
     def assertMet(self, dep):
@@ -43,15 +43,15 @@
 
     def assertUnreachable(self, dep):
         assert dep.unreachable(
             self.succeeded, self.failed
         ), "Dependency should be unreachable"
 
     def assertReachable(self, dep):
-        assert dep.unreachable(
+        assert not dep.unreachable(
             self.succeeded, self.failed
         ), "Dependency should be reachable"
 
     def cancan(self, f):
         """decorator to pass through canning into self.user_ns"""
         return uncan(can(f), self.user_ns)
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_executor.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return n
 
 
 def echo(x):
     return x
 
 
-class AsyncResultTest(ClusterTestCase):
+class TestExecutor(ClusterTestCase):
     def test_client_executor(self):
         executor = self.client.executor()
         assert isinstance(executor.view, LoadBalancedView)
         f = executor.submit(lambda x: 2 * x, 5)
         r = f.result()
         assert r == 10
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_joblib.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_joblib.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 
 def neg(x):
     return -1 * x
 
 
 class TestJobLib(ClusterTestCase):
-    def setup(self):
+    def setup_method(self):
         if not have_joblib:
             pytest.skip("Requires joblib >= 0.10")
-        super().setup()
+        super().setup_method()
         add_engines(1, total=True)
 
     def test_default_backend(self):
         """ipyparallel.register_joblib_backend() registers default backend"""
         ipp.register_joblib_backend()
         with mock.patch.object(ipp.Client, "__new__", lambda *a, **kw: self.client):
             p = Parallel(backend='ipyparallel')
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_launcher.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_lbview.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_lbview.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import ipyparallel as ipp
 from ipyparallel import error
 
 from .clienttest import ClusterTestCase, crash, raises_remote
 
 
 class TestLoadBalancedView(ClusterTestCase):
-    def setup(self):
-        super().setup()
+    def setup_method(self):
+        super().setup_method()
         self.view = self.client.load_balanced_view()
 
     def test_z_crash(self):
         """test graceful handling of engine death (balanced)"""
         self.add_engines(1)
         ar = self.view.apply_async(crash)
         with raises_remote(error.EngineError):
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_magics.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_magics.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,37 @@
             ip.run_line_magic(
                 'px', 'import sys,time;print(a);sys.stdout.flush();time.sleep(0.2)'
             )
         assert '[stdout:' in io.stdout
         assert '\n\n' not in io.stdout
         assert io.stdout.rstrip().endswith('10')
 
+    def test_px_var_expand(self):
+        ip = get_ipython()
+        v = self.client[-1:]
+        v.activate()
+        v.block = True
+        ip.user_ns['x'] = 'client'
+        v['x'] = 'engine'
+        ip.run_line_magic('px', 'y=f"{x}"')
+        assert v['y'] == ["engine"]
+
+    def test_cell_px_var_expand(self):
+        ip = get_ipython()
+        v = self.client[-1:]
+        v.activate()
+        v.block = True
+        ip.user_ns['x'] = 'client'
+        v['x'] = 'engine'
+        ip.user_ns["out_name"] = "theoutput"
+        ip.run_cell_magic('px', '-o {out_name}', 'y=f"{x}"')
+        assert v['y'] == ["engine"]
+        assert "theoutput" in ip.user_ns
+        assert isinstance(ip.user_ns["theoutput"], ipp.AsyncResult)
+
     def _check_generated_stderr(self, stderr, n):
         expected = [
             r'\[stderr:\d+\]',
             '^stderr$',
             '^stderr2$',
         ] * n
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_mongodb.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_mpi.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_remotefunction.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_remotefunction.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_serialize.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_slurm.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_slurm.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_ssh.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_util.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_view.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 )
 
 point = namedtuple("point", "x y")
 
 
 @pytest.mark.usefixtures('ipython')
 class TestView(ClusterTestCase):
-    def setup(self):
+    def setup_method(self):
         # On Win XP, wait for resource cleanup, else parallel test group fails
         if platform.system() == "Windows" and platform.win32_ver()[0] == "XP":
             # 1 sec fails. 1.5 sec seems ok. Using 2 sec for margin of safety
             time.sleep(2)
-        super().setup()
+        super().setup_method()
 
     def test_z_crash_mux(self):
         """test graceful handling of engine death (direct)"""
         self.add_engines(1)
         self.minimum_engines(2)
         eid = self.client.ids[-1]
         view = self.client[-2:]
```

### Comparing `ipyparallel-8.6.0/ipyparallel/tests/test_view_broadcast.py` & `ipyparallel-8.6.1/ipyparallel/tests/test_view_broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 needs_map = pytest.mark.xfail(reason="map not yet implemented")
 
 
 @pytest.mark.usefixtures('ipython')
 class TestBroadcastView(test_view.TestView):
     is_coalescing = False
 
-    def setup(self):
-        super().setup()
+    def setup_method(self):
+        super().setup_method()
         self._broadcast_view_used = False
         # use broadcast view for direct API
         real_direct_view = self.client.real_direct_view = self.client.direct_view
 
         def broadcast_or_direct(targets):
             if isinstance(targets, int):
                 return real_direct_view(targets)
```

### Comparing `ipyparallel-8.6.0/lab/src/clusters.tsx` & `ipyparallel-8.6.1/lab/src/clusters.tsx`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/lab/src/commands.ts` & `ipyparallel-8.6.1/lab/src/commands.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/lab/src/dialog.tsx` & `ipyparallel-8.6.1/lab/src/dialog.tsx`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/lab/src/index.ts` & `ipyparallel-8.6.1/lab/src/index.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/lab/src/sidebar.ts` & `ipyparallel-8.6.1/lab/src/sidebar.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/lab/style/index.css` & `ipyparallel-8.6.1/lab/style/index.css`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/lab/style/logo.svg` & `ipyparallel-8.6.1/lab/style/logo.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/COPYING.md` & `ipyparallel-8.6.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/README.md` & `ipyparallel-8.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/hatch_build.py` & `ipyparallel-8.6.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.0/pyproject.toml` & `ipyparallel-8.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "jupyterlab>=3.0.0,==3.*",
   "hatchling>=0.25"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ipyparallel"
-version = "8.6.0"
+version = "8.6.1"
 authors = [{name = "IPython Development Team", email = "ipython-dev@scipy.org"}]
 license = {file = "COPYING.md"}
 readme = "README.md"
 description = "Interactive Parallel Computing with IPython"
 keywords = [
     "Interactive",
     "Interpreter",
@@ -141,15 +141,15 @@
 ]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/jupyterhub/jupyterhub"
 
 [tool.tbump.version]
-current = "8.6.0"
+current = "8.6.1"
 
 # pep440 regex
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
```

### Comparing `ipyparallel-8.6.0/PKG-INFO` & `ipyparallel-8.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyparallel
-Version: 8.6.0
+Version: 8.6.1
 Summary: Interactive Parallel Computing with IPython
 Project-URL: Homepage, https://ipython.org
 Author-email: IPython Development Team <ipython-dev@scipy.org>
 License: # Licensing terms
         
         Traitlets is adapted from enthought.traits, Copyright (c) Enthought, Inc.,
         under the terms of the Modified BSD License.
```

