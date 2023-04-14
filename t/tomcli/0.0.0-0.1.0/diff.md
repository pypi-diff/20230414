# Comparing `tmp/tomcli-0.0.0.tar.gz` & `tmp/tomcli-0.1.0.tar.gz`

## Comparing `tomcli-0.0.0.tar` & `tomcli-0.1.0.tar`

### file list

```diff
@@ -1,90 +1,161 @@
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 tomcli-0.0.0/NEWS.md
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 tomcli-0.0.0/noxfile.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 tomcli-0.0.0/ruff.toml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tomcli-0.0.0/.builds/nox-lint.yml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tomcli-0.0.0/.builds/nox.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tomcli-0.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tomcli-0.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tomcli-0.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomcli-0.0.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 tomcli-0.0.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/138cd2ffd9a72fa1
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/17032b34c3539c33
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/182adab4e5a8e026
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/191bd3e667e65878
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/1cae0246f47a51e6
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/242872c45603caf
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/25f3447aeaf90609
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/2b63439cd5af3054
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/343c17d86941be6d
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/34e1ab478d40a9f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/3bd00a94f33fcfb6
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/3f58ceb8ff490785
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/41414cb33223f426
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/47990969b0816c19
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/4ee7b8cdcbae7088
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/52052331ac998de4
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/53b770c79f3eb823
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/60cd4b8318ff3584
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/6746594f55461582
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/6b2cd9174eb27a0b
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/6ca2f2fc9012834d
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/6e1805a0b2587263
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/76586ca86e26121c
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/78d76edde2035610
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/7c61d90fd1d2157e
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/7daa321bf9a53c19
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/8a402591edeaa7cd
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/8c07c91f8542951d
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/8cbb3cc218d2ac4e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/9077c3459649e893
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/92dba4109cb7630e
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/937b28c1e8bec5db
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/997ed1b7b1b436bc
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/9a95a18da5948a17
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/9fb39b3a808d7699
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/a29416463f58d4c8
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/a893c04545a27cb5
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/ac3bb96a02e8e6e
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/b0498287d2c842b7
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/b92653f4ad1ae939
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/bb5da1dd2b74eb4a
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/bbbc901adcc3cdce
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/d605b54ed8ac564b
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/db1c6b1a34a124cf
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/dc0a1dabe7469cc9
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/dc597330036fdb6b
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/dccc2bf75292b03c
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/e9947e79394d7105
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/e9a66483d5236f84
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/ebc90afe0dc2f9c9
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/ee43000363d5572
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.0.0/.ruff_cache/content/fc383bcf580fd858
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/d_0cdc8f8d5ab5d777___init___py.html
--rw-r--r--   0        0        0    40651 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/d_1f8b6c189908f960___init___py.html
--rw-r--r--   0        0        0    22243 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/d_1f8b6c189908f960_get_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 tomcli-0.0.0/htmlcov/style.css
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.0.0/src/tomcli/__init__.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 tomcli-0.0.0/src/tomcli/toml.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomcli-0.0.0/src/tomcli/cli/__init__.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.0.0/src/tomcli/cli/get.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tomcli-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tomcli-0.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tomcli-0.0.0/tests/test_tomcli_get.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tomcli-0.0.0/.gitignore
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tomcli-0.0.0/README.md
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tomcli-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomcli-0.0.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 tomcli-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 tomcli-0.1.0/NEWS.md
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 tomcli-0.1.0/noxfile.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 tomcli-0.1.0/ruff.toml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 tomcli-0.1.0/tomcli.spec
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox-lint.yml
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox-mockbuild-36.yml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox-mockbuild.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox.yml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 tomcli-0.1.0/.copr/Makefile
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/102ae904ce423ecb
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/132a3334bcb697d4
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/138cd2ffd9a72fa1
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/16cf683684086e42
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/17032b34c3539c33
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/182adab4e5a8e026
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/191bd3e667e65878
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/195fac077159fecb
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/1cae0246f47a51e6
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/1ed1e9bc14a8e947
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/21b095e72d064d0b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/228428ef6c55f9b4
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/242872c45603caf
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/25f3447aeaf90609
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/26fd5f1a8357f894
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/2b63439cd5af3054
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/33669fbc3402d0a1
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/343c17d86941be6d
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/34e1ab478d40a9f3
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3622d24d03165106
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3bd00a94f33fcfb6
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3c9f99f371b068bd
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3f58ceb8ff490785
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4053dc61d6f25547
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/41414cb33223f426
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4308237c7c08ba51
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4553072f09555c43
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/47990969b0816c19
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4888e119c62fc817
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4a7642a70dda40d5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4d0ebeb74dea6e4b
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4dbd6c78c25046fa
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4ee7b8cdcbae7088
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/51d60f70e1c125ab
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/52052331ac998de4
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/53b770c79f3eb823
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/550a149458063685
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/567b69da99e997a2
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/597c305794afb3f8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/60cd4b8318ff3584
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/657ba086a2498dbf
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6746594f55461582
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/674c74015bfddf43
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6786b37a5221b5ca
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6b2cd9174eb27a0b
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6b3a3867f95ee3d2
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6c2e1ccb7af019ae
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6ca2f2fc9012834d
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6e1805a0b2587263
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6e75d02f45e0b6fb
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6fe881ef0238e47f
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/72b1b7c696d63174
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7504488c70d0af41
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/76586ca86e26121c
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/78d76edde2035610
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7a8936c6cc6300fc
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7c61d90fd1d2157e
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7daa321bf9a53c19
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/868e7acfe2fb4ddd
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8a402591edeaa7cd
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8c07c91f8542951d
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8cbb3cc218d2ac4e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8f65f16675aa2609
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9077c3459649e893
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9121b1d341614163
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/92cc94298f42a9ca
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/92dba4109cb7630e
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/937b28c1e8bec5db
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/997ed1b7b1b436bc
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/99d43425a9401b4
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9a95a18da5948a17
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9d5dbdd0a8f1e60
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9fb39b3a808d7699
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a27d76782310c1d1
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a29416463f58d4c8
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a86f2775c1a8a107
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a893c04545a27cb5
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ac3bb96a02e8e6e
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b0498287d2c842b7
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b3930246cf024275
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b5d7fd139b8e8a0e
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b92653f4ad1ae939
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bab378b835e02eca
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bb5da1dd2b74eb4a
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bbbc901adcc3cdce
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bca2376011140193
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/c5e9cf82f769cc55
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/d16f80d852d45e0f
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/d605b54ed8ac564b
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/db1c6b1a34a124cf
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/dc0a1dabe7469cc9
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/dc597330036fdb6b
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/dccc2bf75292b03c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/de5d7f1c9f277e6e
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/defb66c7533f1af0
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e4f9058a88b51681
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e86563f1db503e0a
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e9947e79394d7105
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e9a66483d5236f84
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ebc4eaabfb6b1a87
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ebc90afe0dc2f9c9
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ee43000363d5572
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ee5eab6a18e8f319
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ef2b9c6d0e28e698
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f14acfbd1d4b990e
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f24f2f95e29bfcd4
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f4fbc527411366a3
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f7ab763b6cbfb8c
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f91fb7119f181aad
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/fc383bcf580fd858
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/fcc03fa280ebd898
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 tomcli-0.1.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_0cdc8f8d5ab5d777___init___py.html
+-rw-r--r--   0        0        0    57283 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960___init___py.html
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960__util_py.html
+-rw-r--r--   0        0        0    19997 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_get_py.html
+-rw-r--r--   0        0        0    34226 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_set_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/style.css
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/__init__.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/toml.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/_util.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/get.py
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/set.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_tomcli_get.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_tomcli_set.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_data/pyproject.toml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_data/test1.toml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tomcli-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tomcli-0.1.0/README.md
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tomcli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomcli-0.1.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 tomcli-0.1.0/PKG-INFO
```

### Comparing `tomcli-0.0.0/CONTRIBUTING.md` & `tomcli-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/ruff.toml` & `tomcli-0.1.0/ruff.toml`

 * *Files 13% similar despite different names*

```diff
@@ -30,10 +30,12 @@
     "B008",
     # Allow overwriting loop variable
     "PLW2901",
 ]
 [per-file-ignores]
 "tests/*" = ["ARG"]
 "noxfile.py" = ["ARG"]
+"src/tomcli/cli/*" = ["UP"]
 
 [isort]
 required-imports = ["from __future__ import annotations"]
+known-first-party = ["tomcli"]
```

### Comparing `tomcli-0.0.0/.ruff_cache/content/17032b34c3539c33` & `tomcli-0.1.0/.ruff_cache/content/17032b34c3539c33`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/182adab4e5a8e026` & `tomcli-0.1.0/.ruff_cache/content/182adab4e5a8e026`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/191bd3e667e65878` & `tomcli-0.1.0/.ruff_cache/content/191bd3e667e65878`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/242872c45603caf` & `tomcli-0.1.0/.ruff_cache/content/242872c45603caf`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/2b63439cd5af3054` & `tomcli-0.1.0/.ruff_cache/content/1ed1e9bc14a8e947`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/343c17d86941be6d` & `tomcli-0.1.0/.ruff_cache/content/343c17d86941be6d`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/41414cb33223f426` & `tomcli-0.1.0/.ruff_cache/content/41414cb33223f426`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/6ca2f2fc9012834d` & `tomcli-0.1.0/.ruff_cache/content/6ca2f2fc9012834d`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/78d76edde2035610` & `tomcli-0.1.0/.ruff_cache/content/78d76edde2035610`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/7c61d90fd1d2157e` & `tomcli-0.1.0/.ruff_cache/content/7c61d90fd1d2157e`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/7daa321bf9a53c19` & `tomcli-0.1.0/.ruff_cache/content/7daa321bf9a53c19`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/937b28c1e8bec5db` & `tomcli-0.1.0/.ruff_cache/content/2b63439cd5af3054`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/9a95a18da5948a17` & `tomcli-0.1.0/.ruff_cache/content/9a95a18da5948a17`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/.ruff_cache/content/a893c04545a27cb5` & `tomcli-0.1.0/.ruff_cache/content/a893c04545a27cb5`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/htmlcov/coverage_html.js` & `tomcli-0.1.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/htmlcov/d_0cdc8f8d5ab5d777___init___py.html` & `tomcli-0.1.0/htmlcov/d_0cdc8f8d5ab5d777___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_1f8b6c189908f960___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-13 04:07 +0300
+            created at 2023-04-13 11:39 +0300
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,23 +85,23 @@
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="str">CLI for working with TOML files. Pronounced "tohm-clee."</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.0.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.0.0.post0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_1f8b6c189908f960___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-13 04:07 +0300
+            created at 2023-04-13 11:39 +0300
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,23 +7,23 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 3 statements   3 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-13 04:07 +0300
+at 2023-04-13 11:39 +0300
 
 
 1# Copyright (C) 2023 Maxwell G <maxwell@gtmx.me> 
 2# 
 3# SPDX-License-Identifier: MIT 
 4 
 5""" 
 6CLI for working with TOML files. Pronounced "tohm-clee." 
 7""" 
 8from __future__ import annotations 
 9 
-10__version__ = "0.0.0" 
+10__version__ = "0.0.0.post0" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-13 04:07 +0300
+at 2023-04-13 11:39 +0300
```

### Comparing `tomcli-0.0.0/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html` & `tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_set_py.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/tomcli/toml.py: 68%</title>
+    <title>Coverage for src/tomcli/cli/set.py: 71%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/tomcli/toml.py</b>:
-            <span class="pc_cov">68%</span>
+            <span class="text">Coverage for </span><b>src/tomcli/cli/set.py</b>:
+            <span class="pc_cov">71%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">72 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">49<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">23<span class="text"> missing</span></button>
+            <span class="text">68 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">48<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">20<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_1f8b6c189908f960_get_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_0cdc8f8d5ab5d777_toml_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-13 04:07 +0300
+            created at 2023-04-13 11:39 +0300
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,164 +80,119 @@
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># Copyright (C) 2023 Maxwell G &lt;maxwell@gtmx.me></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">contextlib</span> <span class="key">import</span> <span class="nam">contextmanager</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">enum</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">io</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span><span class="op">.</span><span class="nam">abc</span> <span class="key">import</span> <span class="nam">Iterator</span><span class="op">,</span> <span class="nam">Mapping</span><span class="op">,</span> <span class="nam">MutableMapping</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">types</span> <span class="key">import</span> <span class="nam">ModuleType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">IO</span><span class="op">,</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># ruff: noqa: UP007</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">dataclasses</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span><span class="op">.</span><span class="nam">abc</span> <span class="key">import</span> <span class="nam">Mapping</span><span class="op">,</span> <span class="nam">MutableMapping</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">typer</span> <span class="key">import</span> <span class="nam">Argument</span><span class="op">,</span> <span class="nam">Context</span><span class="op">,</span> <span class="nam">Exit</span><span class="op">,</span> <span class="nam">Option</span><span class="op">,</span> <span class="nam">Typer</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">class</span> <span class="nam">Reader</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    Libraries to use for deserializing TOML</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="nam">tomcli</span><span class="op">.</span><span class="nam">cli</span><span class="op">.</span><span class="nam">_util</span> <span class="key">import</span> <span class="nam">_std_cm</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">from</span> <span class="nam">tomcli</span><span class="op">.</span><span class="nam">toml</span> <span class="key">import</span> <span class="nam">Reader</span><span class="op">,</span> <span class="nam">Writer</span><span class="op">,</span> <span class="nam">dump</span><span class="op">,</span> <span class="nam">load</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="nam">app</span> <span class="op">=</span> <span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">TOMLLIB</span> <span class="op">=</span> <span class="str">"tomllib"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">TOMLKIT</span> <span class="op">=</span> <span class="str">"tomlkit"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">class</span> <span class="nam">Writer</span><span class="op">(</span><span class="nam">enum</span><span class="op">.</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    Libraries to use for serializing TOML</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="nam">TOMLI_W</span> <span class="op">=</span> <span class="str">"tomli_w"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="nam">TOMLKIT</span> <span class="op">=</span> <span class="str">"tomlkit"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="nam">DEFAULT_READER</span> <span class="op">=</span> <span class="nam">Reader</span><span class="op">.</span><span class="nam">TOMLKIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="nam">DEFAULT_WRITER</span> <span class="op">=</span> <span class="nam">Writer</span><span class="op">.</span><span class="nam">TOMLKIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="nam">NEEDS_STR</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Writer</span> <span class="op">|</span> <span class="nam">Reader</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="nam">Writer</span><span class="op">.</span><span class="nam">TOMLKIT</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="key">def</span> <span class="nam">get_part</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">selector</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">if</span> <span class="nam">selector</span> <span class="op">==</span> <span class="str">"."</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">cur</span> <span class="op">=</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">parts</span> <span class="op">=</span> <span class="nam">selector</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">idx</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span><span class="op">,</span> <span class="nam">part</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">parts</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: B007</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="nam">cur</span> <span class="op">=</span> <span class="nam">cur</span><span class="op">[</span><span class="nam">part</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">except</span> <span class="op">(</span><span class="nam">IndexError</span><span class="op">,</span> <span class="nam">KeyError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">up_to</span> <span class="op">=</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">parts</span><span class="op">[</span><span class="op">:</span> <span class="nam">idx</span> <span class="op">+</span> <span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="str">f"Invalid selector {selector!r}: could not find {up_to!r}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">raise</span> <span class="nam">Exit</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span> <span class="key">from</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">return</span> <span class="nam">cur</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="nam">AVAILABLE_READERS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">Reader</span><span class="op">,</span> <span class="nam">ModuleType</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="nam">AVAILABLE_WRITERS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">Writer</span><span class="op">,</span> <span class="nam">ModuleType</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span><span class="op">[</span><span class="op">:</span><span class="num">2</span><span class="op">]</span> <span class="op">>=</span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">AVAILABLE_READERS</span><span class="op">[</span><span class="nam">Reader</span><span class="op">.</span><span class="nam">TOMLLIB</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">import</span> <span class="nam">tomli</span> <span class="key">as</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">AVAILABLE_READERS</span><span class="op">[</span><span class="nam">Reader</span><span class="op">.</span><span class="nam">TOMLLIB</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomli_w</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">AVAILABLE_WRITERS</span><span class="op">[</span><span class="nam">Writer</span><span class="op">.</span><span class="nam">TOMLI_W</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tomli_w</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="key">except</span> <span class="nam">ImportError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t"><span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="nam">AVAILABLE_READERS</span><span class="op">[</span><span class="nam">Reader</span><span class="op">.</span><span class="nam">TOMLKIT</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">AVAILABLE_WRITERS</span><span class="op">[</span><span class="nam">Writer</span><span class="op">.</span><span class="nam">TOMLKIT</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="op">@</span><span class="nam">contextmanager</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="key">def</span> <span class="nam">_get_stream</span><span class="op">(</span><span class="nam">fp</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">,</span> <span class="nam">backend</span><span class="op">:</span> <span class="nam">Reader</span> <span class="op">|</span> <span class="nam">Writer</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Iterator</span><span class="op">[</span><span class="nam">IO</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">if</span> <span class="nam">backend</span> <span class="key">in</span> <span class="nam">NEEDS_STR</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">fp</span><span class="op">.</span><span class="nam">flush</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">io</span><span class="op">.</span><span class="nam">TextIOWrapper</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="str">"utf-8"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="key">yield</span> <span class="nam">wrapper</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">finally</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="nam">wrapper</span><span class="op">.</span><span class="nam">flush</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">wrapper</span><span class="op">.</span><span class="nam">detach</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="key">yield</span> <span class="nam">fp</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t"><span class="key">def</span> <span class="nam">load</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="nam">fp</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="nam">prefered_reader</span><span class="op">:</span> <span class="nam">Reader</span> <span class="op">=</span> <span class="nam">DEFAULT_READER</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="nam">allow_fallback</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">    Parse a bytes stream containing TOML data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="str">    Parameters:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="str">        fp:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="str">            A bytes stream that supports `.read()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="str">        prefered_reader:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">            A [`Reader`][tomcli.toml.Reader] to use for parsing the TOML document</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="str">        allow_fallback:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="str">            Whether to fallback to another Reader if `prefered_reader` is unavailable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">AVAILABLE_READERS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">missing</span> <span class="op">=</span> <span class="str">", "</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">module</span><span class="op">.</span><span class="nam">value</span> <span class="key">for</span> <span class="nam">module</span> <span class="key">in</span> <span class="nam">Reader</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ModuleNotFoundError</span><span class="op">(</span><span class="str">f"None of the following were found: {missing}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="key">if</span> <span class="nam">prefered_reader</span> <span class="key">in</span> <span class="nam">AVAILABLE_READERS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">with</span> <span class="nam">_get_stream</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="nam">prefered_reader</span><span class="op">)</span> <span class="key">as</span> <span class="nam">wrapper</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">            <span class="key">return</span> <span class="nam">AVAILABLE_READERS</span><span class="op">[</span><span class="nam">prefered_reader</span><span class="op">]</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">wrapper</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="key">elif</span> <span class="key">not</span> <span class="nam">allow_fallback</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ModuleNotFoundError</span><span class="op">(</span><span class="str">f"No module named {prefered_reader.value!r}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="nam">reader</span><span class="op">,</span> <span class="nam">mod</span> <span class="op">=</span> <span class="nam">next</span><span class="op">(</span><span class="nam">iter</span><span class="op">(</span><span class="nam">AVAILABLE_READERS</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">with</span> <span class="nam">_get_stream</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="nam">reader</span><span class="op">)</span> <span class="key">as</span> <span class="nam">wrapper</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="key">return</span> <span class="nam">mod</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">wrapper</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="key">def</span> <span class="nam">dump</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">Mapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="nam">fp</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">    <span class="nam">prefered_writer</span><span class="op">:</span> <span class="nam">Writer</span> <span class="op">=</span> <span class="nam">DEFAULT_WRITER</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">    <span class="nam">allow_fallback</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">    Serialize an object to TOML and write it to a binary stream</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="str">    Parameters:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="str">        fp:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t"><span class="str">            A bytes stream that supports `.write()`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="str">        prefered_writer:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="str">            A [`Writer`][tomcli.toml.Writer] to use for serializing the Python</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t"><span class="str">            object</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">        allow_fallback:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">            Whether to fallback to another Writer if `prefered_writer` is unavailable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">AVAILABLE_WRITERS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="nam">missing</span> <span class="op">=</span> <span class="str">", "</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">module</span><span class="op">.</span><span class="nam">value</span> <span class="key">for</span> <span class="nam">module</span> <span class="key">in</span> <span class="nam">Writer</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ModuleNotFoundError</span><span class="op">(</span><span class="str">f"None of the following were found: {missing}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="key">if</span> <span class="nam">prefered_writer</span> <span class="key">in</span> <span class="nam">AVAILABLE_WRITERS</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="key">with</span> <span class="nam">_get_stream</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="nam">prefered_writer</span><span class="op">)</span> <span class="key">as</span> <span class="nam">wrapper</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">            <span class="key">return</span> <span class="nam">AVAILABLE_WRITERS</span><span class="op">[</span><span class="nam">prefered_writer</span><span class="op">]</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">wrapper</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="key">elif</span> <span class="key">not</span> <span class="nam">allow_fallback</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ModuleNotFoundError</span><span class="op">(</span><span class="str">f"No module named {prefered_writer.value!r}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">writer</span><span class="op">,</span> <span class="nam">mod</span> <span class="op">=</span> <span class="nam">next</span><span class="op">(</span><span class="nam">iter</span><span class="op">(</span><span class="nam">AVAILABLE_WRITERS</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">    <span class="key">with</span> <span class="nam">_get_stream</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="nam">writer</span><span class="op">)</span> <span class="key">as</span> <span class="nam">wrapper</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="key">return</span> <span class="nam">mod</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">wrapper</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="op">@</span><span class="nam">dataclasses</span><span class="op">.</span><span class="nam">dataclass</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">class</span> <span class="nam">ModderCtx</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">out</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">reader</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">writer</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">allow_fallback_r</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="nam">allow_fallback_w</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">def</span> <span class="nam">set_default_rw</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">reader</span><span class="op">:</span> <span class="nam">Reader</span><span class="op">,</span> <span class="nam">writer</span><span class="op">:</span> <span class="nam">Writer</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">reader</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">reader</span> <span class="op">=</span> <span class="nam">reader</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">allow_fallback_r</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">writer</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">writer</span> <span class="op">=</span> <span class="nam">writer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">allow_fallback_w</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">def</span> <span class="nam">load</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">with</span> <span class="nam">_std_cm</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">path</span><span class="op">,</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">.</span><span class="nam">buffer</span><span class="op">,</span> <span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="key">return</span> <span class="nam">load</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">reader</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">allow_fallback_r</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">def</span> <span class="nam">dump</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">__data</span><span class="op">:</span> <span class="nam">Mapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="key">with</span> <span class="nam">_std_cm</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">out</span><span class="op">,</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">buffer</span><span class="op">,</span> <span class="str">"wb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">dump</span><span class="op">(</span><span class="nam">__data</span><span class="op">,</span> <span class="nam">fp</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">writer</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">allow_fallback_w</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">callback</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="key">def</span> <span class="nam">callback</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="nam">ctx</span><span class="op">:</span> <span class="nam">Context</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="nam">output</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="nam">Option</span><span class="op">(</span><span class="key">None</span><span class="op">,</span> <span class="str">"-o"</span><span class="op">,</span> <span class="str">"--output"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="nam">reader</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">Reader</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="nam">writer</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">Writer</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="nam">ctx</span><span class="op">.</span><span class="nam">obj</span> <span class="op">=</span> <span class="nam">ModderCtx</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">output</span> <span class="key">or</span> <span class="nam">path</span><span class="op">,</span> <span class="nam">reader</span><span class="op">,</span> <span class="nam">writer</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="str">"del"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t"><span class="key">def</span> <span class="nam">delete</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="nam">ctx</span><span class="op">:</span> <span class="nam">Context</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">selector</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="nam">modder</span><span class="op">:</span> <span class="nam">ModderCtx</span> <span class="op">=</span> <span class="nam">ctx</span><span class="op">.</span><span class="nam">find_object</span><span class="op">(</span><span class="nam">ModderCtx</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="nam">modder</span><span class="op">.</span><span class="nam">set_default_rw</span><span class="op">(</span><span class="nam">Reader</span><span class="op">.</span><span class="nam">TOMLKIT</span><span class="op">,</span> <span class="nam">Writer</span><span class="op">.</span><span class="nam">TOMLKIT</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">modder</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">if</span> <span class="nam">selector</span> <span class="op">==</span> <span class="str">"."</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="key">raise</span> <span class="nam">Exit</span><span class="op">(</span><span class="str">"Thank you for your patronage, but we won't delete the whole file."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="nam">parts</span> <span class="op">=</span> <span class="nam">selector</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="nam">idx</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="nam">cur</span> <span class="op">=</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span><span class="op">,</span> <span class="nam">part</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">parts</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="key">if</span> <span class="nam">idx</span> <span class="op">+</span> <span class="num">1</span> <span class="op">==</span> <span class="nam">len</span><span class="op">(</span><span class="nam">parts</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">                <span class="key">del</span> <span class="nam">cur</span><span class="op">[</span><span class="nam">part</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="nam">cur</span> <span class="op">=</span> <span class="nam">cur</span><span class="op">[</span><span class="nam">part</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">except</span> <span class="op">(</span><span class="nam">IndexError</span><span class="op">,</span> <span class="nam">KeyError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">up_to</span> <span class="op">=</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">parts</span><span class="op">[</span><span class="op">:</span> <span class="nam">idx</span> <span class="op">+</span> <span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="str">f"Invalid selector {selector!r}: could not find {up_to!r}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="key">raise</span> <span class="nam">Exit</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span> <span class="key">from</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="nam">modder</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_1f8b6c189908f960_get_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_0cdc8f8d5ab5d777_toml_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-13 04:07 +0300
+            created at 2023-04-13 11:39 +0300
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,166 +1,121 @@
 
-****** Coverage for src/tomcli/toml.py: 68% ******
+****** Coverage for src/tomcli/cli/set.py: 71% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 72 statements   49 run 23 missing 0 excluded *****
+***** 68 statements   48 run 20 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-13 04:07 +0300
+at 2023-04-13 11:39 +0300
 
 
 1# Copyright (C) 2023 Maxwell G <maxwell@gtmx.me> 
 2# 
 3# SPDX-License-Identifier: MIT 
 4 
-5from __future__ import annotations 
-6from contextlib import contextmanager 
-7 
-8import enum 
-9import io 
-10import sys 
-11from collections.abc import Iterator, Mapping, MutableMapping 
-12from types import ModuleType 
-13from typing import IO, Any, BinaryIO 
-14 
+5# ruff: noqa: UP007 
+6 
+7from __future__ import annotations 
+8 
+9import dataclasses 
+10from collections.abc import Mapping, MutableMapping 
+11import sys 
+12from typing import Any, Optional 
+13 
+14from typer import Argument, Context, Exit, Option, Typer 
 15 
-16class Reader(enum.Enum): 
-17 """ 
-18 Libraries to use for deserializing TOML 
-19 """ 
+16from tomcli.cli._util import _std_cm 
+17from tomcli.toml import Reader, Writer, dump, load 
+18 
+19app = Typer() 
 20 
-21 TOMLLIB = "tomllib" 
-22 TOMLKIT = "tomlkit" 
-23 
-24 
-25class Writer(enum.Enum): 
-26 """ 
-27 Libraries to use for serializing TOML 
-28 """ 
-29 
-30 TOMLI_W = "tomli_w" 
-31 TOMLKIT = "tomlkit" 
-32 
-33 
-34DEFAULT_READER = Reader.TOMLKIT 
-35DEFAULT_WRITER = Writer.TOMLKIT 
-36NEEDS_STR: tuple[Writer | Reader] = [Writer.TOMLKIT] 
+21 
+22def get_part(data: MutableMapping[str, Any], selector: str) -> Any: 
+23 if selector == ".": 
+24 return data 
+25 
+26 cur = data 
+27 parts = selector.split(".") 
+28 idx = 0 
+29 try: 
+30 for idx, part in enumerate(parts): # noqa: B007 
+31 cur = cur[part] 
+32 except (IndexError, KeyError): 
+33 up_to = ".".join(parts[: idx + 1]) 
+34 msg = f"Invalid selector {selector!r}: could not find {up_to!r}" 
+35 raise Exit(msg) from None 
+36 return cur 
 37 
-38AVAILABLE_READERS: dict[Reader, ModuleType] = {} 
-39AVAILABLE_WRITERS: dict[Writer, ModuleType] = {} 
-40 
-41if sys.version_info[:2] >= (3, 11): 
-42 import tomllib 
-43 
-44 AVAILABLE_READERS[Reader.TOMLLIB] = tomllib 
-45else: 
-46 try: 
-47 import tomli as tomllib 
-48 except ImportError: 
-49 pass 
-50 else: 
-51 AVAILABLE_READERS[Reader.TOMLLIB] = tomllib 
-52 
-53try: 
-54 import tomli_w 
-55except ImportError: 
-56 pass 
-57else: 
-58 AVAILABLE_WRITERS[Writer.TOMLI_W] = tomli_w 
-59 
-60try: 
-61 import tomlkit 
-62except ImportError: 
-63 pass 
-64else: 
-65 AVAILABLE_READERS[Reader.TOMLKIT] = tomlkit 
-66 AVAILABLE_WRITERS[Writer.TOMLKIT] = tomlkit 
-67 
-68 
-69@contextmanager 
-70def _get_stream(fp: BinaryIO, backend: Reader | Writer) -> Iterator[IO[Any]]:
- 
-71 if backend in NEEDS_STR: 
-72 fp.flush() 
-73 wrapper = io.TextIOWrapper(fp, "utf-8") 
-74 try: 
-75 yield wrapper 
-76 finally: 
-77 wrapper.flush() 
-78 wrapper.detach() 
-79 else: 
-80 yield fp 
-81 
-82 
-83def load( 
-84 fp: BinaryIO, 
-85 /, 
-86 prefered_reader: Reader = DEFAULT_READER, 
-87 allow_fallback: bool = True, 
-88) -> MutableMapping[str, Any]: 
-89 """ 
-90 Parse a bytes stream containing TOML data 
-91 
-92 Parameters: 
-93 fp: 
-94 A bytes stream that supports `.read() 
-95 prefered_reader: 
-96 A [`Reader`][tomcli.toml.Reader] to use for parsing the TOML document 
-97 allow_fallback: 
-98 Whether to fallback to another Reader if `prefered_reader` is unavailable 
-99 """ 
-100 if not AVAILABLE_READERS: 
-101 missing = ", ".join(module.value for module in Reader) 
-102 raise ModuleNotFoundError(f"None of the following were found: {missing}") 
-103 
-104 if prefered_reader in AVAILABLE_READERS: 
-105 with _get_stream(fp, prefered_reader) as wrapper: 
-106 return AVAILABLE_READERS[prefered_reader].load(wrapper) 
-107 elif not allow_fallback: 
-108 raise ModuleNotFoundError(f"No module named {prefered_reader.value!r}") 
-109 
-110 reader, mod = next(iter(AVAILABLE_READERS.items())) 
-111 with _get_stream(fp, reader) as wrapper: 
-112 return mod.load(wrapper) 
-113 
-114 
-115def dump( 
-116 data: Mapping[str, Any], 
-117 fp: BinaryIO, 
-118 /, 
-119 prefered_writer: Writer = DEFAULT_WRITER, 
-120 allow_fallback: bool = True, 
-121) -> None: 
-122 """ 
-123 Serialize an object to TOML and write it to a binary stream 
-124 
-125 Parameters: 
-126 fp: 
-127 A bytes stream that supports `.write()` 
-128 prefered_writer: 
-129 A [`Writer`][tomcli.toml.Writer] to use for serializing the Python 
-130 object 
-131 allow_fallback: 
-132 Whether to fallback to another Writer if `prefered_writer` is unavailable 
-133 """ 
-134 if not AVAILABLE_WRITERS: 
-135 missing = ", ".join(module.value for module in Writer) 
-136 raise ModuleNotFoundError(f"None of the following were found: {missing}") 
-137 
-138 if prefered_writer in AVAILABLE_WRITERS: 
-139 with _get_stream(fp, prefered_writer) as wrapper: 
-140 return AVAILABLE_WRITERS[prefered_writer].dump(data, wrapper) 
-141 elif not allow_fallback: 
-142 raise ModuleNotFoundError(f"No module named {prefered_writer.value!r}") 
-143 
-144 writer, mod = next(iter(AVAILABLE_WRITERS.items())) 
-145 with _get_stream(fp, writer) as wrapper: 
-146 return mod.dump(data, wrapper) 
+38 
+39@dataclasses.dataclass() 
+40class ModderCtx: 
+41 path: str 
+42 out: str 
+43 reader: str | None = None 
+44 writer: str | None = None 
+45 allow_fallback_r: bool = True 
+46 allow_fallback_w: bool = True 
+47 
+48 def set_default_rw(self, reader: Reader, writer: Writer): 
+49 if self.reader is None: 
+50 self.reader = reader 
+51 else: 
+52 self.allow_fallback_r = False 
+53 if self.writer is None: 
+54 self.writer = writer 
+55 else: 
+56 self.allow_fallback_w = False 
+57 
+58 def load(self) -> MutableMapping[str, Any]: 
+59 with _std_cm(self.path, sys.stdin.buffer, "rb") as fp: 
+60 return load(fp, self.reader, self.allow_fallback_r) 
+61 
+62 def dump(self, __data: Mapping[str, Any]) -> None: 
+63 with _std_cm(self.out, sys.stdout.buffer, "wb") as fp: 
+64 dump(__data, fp, self.writer, self.allow_fallback_w) 
+65 
+66 
+67@app.callback() 
+68def callback( 
+69 ctx: Context, 
+70 path: str = Argument(...), 
+71 output: Optional[str] = Option(None, "-o", "--output"), 
+72 reader: Optional[Reader] = None, 
+73 writer: Optional[Writer] = None, 
+74): 
+75 ctx.obj = ModderCtx(path, output or path, reader, writer) 
+76 
+77 
+78@app.command(name="del") 
+79def delete( 
+80 ctx: Context, 
+81 selector: str = Argument(...), 
+82): 
+83 modder: ModderCtx = ctx.find_object(ModderCtx) 
+84 modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT) 
+85 data = modder.load() 
+86 if selector == ".": 
+87 raise Exit("Thank you for your patronage, but we won't delete the whole
+file.") 
+88 parts = selector.split(".") 
+89 idx = 0 
+90 cur = data 
+91 try: 
+92 for idx, part in enumerate(parts): 
+93 if idx + 1 == len(parts): 
+94 del cur[part] 
+95 break 
+96 cur = cur[part] 
+97 except (IndexError, KeyError): 
+98 up_to = ".".join(parts[: idx + 1]) 
+99 msg = f"Invalid selector {selector!r}: could not find {up_to!r}" 
+100 raise Exit(msg) from None 
+101 modder.dump(data) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-13 04:07 +0300
+at 2023-04-13 11:39 +0300
```

### Comparing `tomcli-0.0.0/htmlcov/d_1f8b6c189908f960___init___py.html` & `tomcli-0.1.0/htmlcov/d_1f8b6c189908f960___init___py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/htmlcov/d_1f8b6c189908f960_get_py.html` & `tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_get_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/tomcli/cli/get.py: 95%</title>
+    <title>Coverage for src/tomcli/cli/get.py: 97%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/tomcli/cli/get.py</b>:
-            <span class="pc_cov">95%</span>
+            <span class="pc_cov">97%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">40 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">38<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">2<span class="text"> missing</span></button>
+            <span class="text">34 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">33<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">1<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_1f8b6c189908f960___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_1f8b6c189908f960__util_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_0cdc8f8d5ab5d777_toml_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_1f8b6c189908f960_set_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-13 04:07 +0300
+            created at 2023-04-13 11:39 +0300
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,80 +80,73 @@
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># Copyright (C) 2023 Maxwell G &lt;maxwell@gtmx.me></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># ruff: noqa: UP007</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span><span class="op">.</span><span class="nam">abc</span> <span class="key">import</span> <span class="nam">Iterable</span><span class="op">,</span> <span class="nam">Mapping</span><span class="op">,</span> <span class="nam">MutableMapping</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">contextlib</span> <span class="key">import</span> <span class="nam">contextmanager</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">BinaryIO</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">typer</span> <span class="key">import</span> <span class="nam">Argument</span><span class="op">,</span> <span class="nam">Exit</span><span class="op">,</span> <span class="nam">Typer</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">tomcli</span><span class="op">.</span><span class="nam">toml</span> <span class="key">import</span> <span class="nam">Reader</span><span class="op">,</span> <span class="nam">Writer</span><span class="op">,</span> <span class="nam">dump</span><span class="op">,</span> <span class="nam">load</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">app</span> <span class="op">=</span> <span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span><span class="op">.</span><span class="nam">abc</span> <span class="key">import</span> <span class="nam">Iterable</span><span class="op">,</span> <span class="nam">Mapping</span><span class="op">,</span> <span class="nam">MutableMapping</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typer</span> <span class="key">import</span> <span class="nam">Argument</span><span class="op">,</span> <span class="nam">Exit</span><span class="op">,</span> <span class="nam">Typer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="nam">tomcli</span><span class="op">.</span><span class="nam">cli</span><span class="op">.</span><span class="nam">_util</span> <span class="key">import</span> <span class="nam">_std_cm</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="nam">tomcli</span><span class="op">.</span><span class="nam">toml</span> <span class="key">import</span> <span class="nam">Reader</span><span class="op">,</span> <span class="nam">Writer</span><span class="op">,</span> <span class="nam">dump</span><span class="op">,</span> <span class="nam">load</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">def</span> <span class="nam">get_part</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">selector</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">/</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="key">if</span> <span class="nam">selector</span> <span class="op">==</span> <span class="str">"."</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">cur</span> <span class="op">=</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">parts</span> <span class="op">=</span> <span class="nam">selector</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">idx</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span><span class="op">,</span> <span class="nam">part</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">parts</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: B007</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">cur</span> <span class="op">=</span> <span class="nam">cur</span><span class="op">[</span><span class="nam">part</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">except</span> <span class="op">(</span><span class="nam">IndexError</span><span class="op">,</span> <span class="nam">KeyError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">up_to</span> <span class="op">=</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">parts</span><span class="op">[</span><span class="op">:</span> <span class="nam">idx</span> <span class="op">+</span> <span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="str">f"Invalid selector {selector!r}: could not find {up_to!r}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">raise</span> <span class="nam">Exit</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span> <span class="key">from</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">return</span> <span class="nam">cur</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="op">@</span><span class="nam">contextmanager</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="key">def</span> <span class="nam">_std_cm</span><span class="op">(</span><span class="nam">path</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">dash_stream</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">mode</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Iterable</span><span class="op">[</span><span class="nam">BinaryIO</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">if</span> <span class="nam">str</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span> <span class="op">==</span> <span class="str">"-"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">yield</span> <span class="nam">dash_stream</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">mode</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">yield</span> <span class="nam">fp</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="key">def</span> <span class="nam">get</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">selector</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Argument</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">reader</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">Reader</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">writer</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">Writer</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">allow_fallback_r</span> <span class="op">=</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">reader</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">allow_fallback_w</span> <span class="op">=</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">writer</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">reader</span> <span class="op">=</span> <span class="nam">reader</span> <span class="key">or</span> <span class="nam">Reader</span><span class="op">.</span><span class="nam">TOMLKIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="nam">writer</span> <span class="op">=</span> <span class="nam">writer</span> <span class="key">or</span> <span class="nam">Writer</span><span class="op">.</span><span class="nam">TOMLKIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">with</span> <span class="nam">_std_cm</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">.</span><span class="nam">buffer</span><span class="op">,</span> <span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">load</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="nam">reader</span><span class="op">,</span> <span class="nam">allow_fallback_r</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">selected</span> <span class="op">=</span> <span class="nam">get_part</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">selector</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">selected</span><span class="op">,</span> <span class="nam">Mapping</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">dump</span><span class="op">(</span><span class="nam">selected</span><span class="op">,</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">buffer</span><span class="op">,</span> <span class="nam">writer</span><span class="op">,</span> <span class="nam">allow_fallback_w</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="nam">selected</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="nam">app</span> <span class="op">=</span> <span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="key">def</span> <span class="nam">get_part</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">selector</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="key">if</span> <span class="nam">selector</span> <span class="op">==</span> <span class="str">"."</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">cur</span> <span class="op">=</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">parts</span> <span class="op">=</span> <span class="nam">selector</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">idx</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span><span class="op">,</span> <span class="nam">part</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">parts</span><span class="op">)</span><span class="op">:</span>  <span class="com"># noqa: B007</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="nam">cur</span> <span class="op">=</span> <span class="nam">cur</span><span class="op">[</span><span class="nam">part</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="key">except</span> <span class="op">(</span><span class="nam">IndexError</span><span class="op">,</span> <span class="nam">KeyError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">up_to</span> <span class="op">=</span> <span class="str">"."</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">parts</span><span class="op">[</span><span class="op">:</span> <span class="nam">idx</span> <span class="op">+</span> <span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="str">f"Invalid selector {selector!r}: could not find {up_to!r}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">raise</span> <span class="nam">Exit</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span> <span class="key">from</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">return</span> <span class="nam">cur</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="key">def</span> <span class="nam">get</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="nam">path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Argument</span><span class="op">(</span><span class="op">...</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="nam">selector</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Argument</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">reader</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">Reader</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">writer</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">Writer</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">allow_fallback_r</span> <span class="op">=</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">reader</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="nam">allow_fallback_w</span> <span class="op">=</span> <span class="nam">bool</span><span class="op">(</span><span class="nam">writer</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">reader</span> <span class="op">=</span> <span class="nam">reader</span> <span class="key">or</span> <span class="nam">Reader</span><span class="op">.</span><span class="nam">TOMLKIT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">writer</span> <span class="op">=</span> <span class="nam">writer</span> <span class="key">or</span> <span class="nam">Writer</span><span class="op">.</span><span class="nam">TOMLKIT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">with</span> <span class="nam">_std_cm</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">.</span><span class="nam">buffer</span><span class="op">,</span> <span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">fp</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">load</span><span class="op">(</span><span class="nam">fp</span><span class="op">,</span> <span class="nam">reader</span><span class="op">,</span> <span class="nam">allow_fallback_r</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">selected</span> <span class="op">=</span> <span class="nam">get_part</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">selector</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">selected</span><span class="op">,</span> <span class="nam">Mapping</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">dump</span><span class="op">(</span><span class="nam">selected</span><span class="op">,</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdout</span><span class="op">.</span><span class="nam">buffer</span><span class="op">,</span> <span class="nam">writer</span><span class="op">,</span> <span class="nam">allow_fallback_w</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="nam">selected</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_1f8b6c189908f960___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_1f8b6c189908f960__util_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_0cdc8f8d5ab5d777_toml_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_1f8b6c189908f960_set_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-13 04:07 +0300
+            created at 2023-04-13 11:39 +0300
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,81 +1,74 @@
 
-****** Coverage for src/tomcli/cli/get.py: 95% ******
+****** Coverage for src/tomcli/cli/get.py: 97% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 40 statements   38 run 2 missing 0 excluded *****
+***** 34 statements   33 run 1 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-13 04:07 +0300
+at 2023-04-13 11:39 +0300
 
 
 1# Copyright (C) 2023 Maxwell G <maxwell@gtmx.me> 
 2# 
 3# SPDX-License-Identifier: MIT 
 4 
-5from __future__ import annotations 
+5# ruff: noqa: UP007 
 6 
-7import sys 
-8from collections.abc import Iterable, Mapping, MutableMapping 
-9from contextlib import contextmanager 
-10from typing import Any, BinaryIO, Optional 
-11 
-12from typer import Argument, Exit, Typer 
-13 
-14from tomcli.toml import Reader, Writer, dump, load 
-15 
-16app = Typer() 
+7from __future__ import annotations 
+8 
+9import sys 
+10from collections.abc import Iterable, Mapping, MutableMapping 
+11from typing import Any, Optional 
+12 
+13from typer import Argument, Exit, Typer 
+14 
+15from tomcli.cli._util import _std_cm 
+16from tomcli.toml import Reader, Writer, dump, load 
 17 
-18 
-19def get_part(data: MutableMapping[str, Any], selector: str, /) -> Any: 
-20 if selector == ".": 
-21 return data 
-22 
-23 cur = data 
-24 parts = selector.split(".") 
-25 idx = 0 
-26 try: 
-27 for idx, part in enumerate(parts): # noqa: B007 
-28 cur = cur[part] 
-29 except (IndexError, KeyError): 
-30 up_to = ".".join(parts[: idx + 1]) 
-31 msg = f"Invalid selector {selector!r}: could not find {up_to!r}" 
-32 raise Exit(msg) from None 
-33 return cur 
-34 
-35 
-36@contextmanager 
-37def _std_cm(path: str, dash_stream: str, mode: str) -> Iterable[BinaryIO]: 
-38 if str(path) == "-": 
-39 yield dash_stream 
-40 else: 
-41 with open(path, mode) as fp: 
-42 yield fp 
-43 
-44 
-45@app.command() 
-46def get( 
-47 path: str = Argument(...), 
-48 selector: str = Argument("."), 
-49 reader: Optional[Reader] = None, 
-50 writer: Optional[Writer] = None, 
-51): 
-52 allow_fallback_r = bool(reader) 
-53 allow_fallback_w = bool(writer) 
-54 reader = reader or Reader.TOMLKIT 
-55 writer = writer or Writer.TOMLKIT 
-56 with _std_cm(path, sys.stdin.buffer, "rb") as fp: 
-57 data = load(fp, reader, allow_fallback_r) 
-58 selected = get_part(data, selector) 
-59 if isinstance(selected, Mapping): 
-60 dump(selected, sys.stdout.buffer, writer, allow_fallback_w) 
-61 else: 
-62 print(selected) 
+18app = Typer() 
+19 
+20 
+21def get_part(data: MutableMapping[str, Any], selector: str) -> Any: 
+22 if selector == ".": 
+23 return data 
+24 
+25 cur = data 
+26 parts = selector.split(".") 
+27 idx = 0 
+28 try: 
+29 for idx, part in enumerate(parts): # noqa: B007 
+30 cur = cur[part] 
+31 except (IndexError, KeyError): 
+32 up_to = ".".join(parts[: idx + 1]) 
+33 msg = f"Invalid selector {selector!r}: could not find {up_to!r}" 
+34 raise Exit(msg) from None 
+35 return cur 
+36 
+37 
+38@app.command() 
+39def get( 
+40 path: str = Argument(...), 
+41 selector: str = Argument("."), 
+42 reader: Optional[Reader] = None, 
+43 writer: Optional[Writer] = None, 
+44): 
+45 allow_fallback_r = bool(reader) 
+46 allow_fallback_w = bool(writer) 
+47 reader = reader or Reader.TOMLKIT 
+48 writer = writer or Writer.TOMLKIT 
+49 with _std_cm(path, sys.stdin.buffer, "rb") as fp: 
+50 data = load(fp, reader, allow_fallback_r) 
+51 selected = get_part(data, selector) 
+52 if isinstance(selected, Mapping): 
+53 dump(selected, sys.stdout.buffer, writer, allow_fallback_w) 
+54 else: 
+55 print(selected) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-13 04:07 +0300
+at 2023-04-13 11:39 +0300
```

### Comparing `tomcli-0.0.0/htmlcov/favicon_32.png` & `tomcli-0.1.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/htmlcov/keybd_closed.png` & `tomcli-0.1.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/htmlcov/keybd_open.png` & `tomcli-0.1.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/htmlcov/status.json` & `tomcli-0.1.0/htmlcov/status.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9501736111111111%*

 * *Differences: {"'files'": "{'d_0cdc8f8d5ab5d777___init___py': {'hash': '9f913b83bb3595f5de60faba988c7b4f'}, "*

 * *            "'d_1f8b6c189908f960_get_py': {'hash': 'd839cbd0f3985bb5b7eb6a80e177576e', 'index': "*

 * *            "{'nums': {insert: [(2, 34), (4, 1)], delete: [4, 2]}}}, 'd_0cdc8f8d5ab5d777_toml_py': "*

 * *            "{'hash': '35ae0cd56ea83d3bffda98dab7f07b37', 'index': {'nums': {insert: [(2, 96), (4, "*

 * *            "39)], delete: [4, 2]}}}, 'd_1f8b6c189908f960__util_py': OrderedDict([('hash', "*

 * *            "'7896638ac […]*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_0cdc8f8d5ab5d777___init___py": {
-            "hash": "3e46042d4fb5796b95f4e8e97e508327",
+            "hash": "9f913b83bb3595f5de60faba988c7b4f",
             "index": {
                 "html_filename": "d_0cdc8f8d5ab5d777___init___py.html",
                 "nums": [
                     0,
                     1,
                     3,
                     0,
@@ -14,23 +14,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/tomcli/__init__.py"
             }
         },
         "d_0cdc8f8d5ab5d777_toml_py": {
-            "hash": "157c8d88053e428f75e81dd5ebc3818d",
+            "hash": "35ae0cd56ea83d3bffda98dab7f07b37",
             "index": {
                 "html_filename": "d_0cdc8f8d5ab5d777_toml_py.html",
                 "nums": [
                     0,
                     1,
-                    72,
+                    96,
                     0,
-                    23,
+                    39,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/tomcli/toml.py"
             }
         },
@@ -47,29 +47,63 @@
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/tomcli/cli/__init__.py"
             }
         },
+        "d_1f8b6c189908f960__util_py": {
+            "hash": "7896638ac7169f49cc640372938a8d79",
+            "index": {
+                "html_filename": "d_1f8b6c189908f960__util_py.html",
+                "nums": [
+                    0,
+                    1,
+                    10,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0
+                ],
+                "relative_filename": "src/tomcli/cli/_util.py"
+            }
+        },
         "d_1f8b6c189908f960_get_py": {
-            "hash": "b4cbc21f417465980ff5dbcc9f2d273f",
+            "hash": "d839cbd0f3985bb5b7eb6a80e177576e",
             "index": {
                 "html_filename": "d_1f8b6c189908f960_get_py.html",
                 "nums": [
                     0,
                     1,
-                    40,
+                    34,
                     0,
-                    2,
+                    1,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/tomcli/cli/get.py"
             }
+        },
+        "d_1f8b6c189908f960_set_py": {
+            "hash": "365604a282fbc81ac49143bd015a2838",
+            "index": {
+                "html_filename": "d_1f8b6c189908f960_set_py.html",
+                "nums": [
+                    0,
+                    1,
+                    68,
+                    0,
+                    20,
+                    0,
+                    0,
+                    0
+                ],
+                "relative_filename": "src/tomcli/cli/set.py"
+            }
         }
     },
     "format": 2,
     "globals": "3b4539a26e342166afa5760b7aa37881",
     "version": "7.2.3"
 }
```

### Comparing `tomcli-0.0.0/htmlcov/style.css` & `tomcli-0.1.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/src/tomcli/toml.py` & `tomcli-0.1.0/src/tomcli/toml.py`

 * *Files 26% similar despite different names*

```diff
@@ -78,47 +78,54 @@
             wrapper.detach()
     else:
         yield fp
 
 
 def load(
     __fp: BinaryIO,
-    prefered_reader: Reader = DEFAULT_READER,
+    prefered_reader: Reader | None = None,
     allow_fallback: bool = True,
 ) -> MutableMapping[str, Any]:
     """
     Parse a bytes stream containing TOML data
 
     Parameters:
         __fp:
             A bytes stream that supports `.read(). Positional argument only.
         prefered_reader:
             A [`Reader`][tomcli.toml.Reader] to use for parsing the TOML document
         allow_fallback:
             Whether to fallback to another Reader if `prefered_reader` is unavailable
     """
+    prefered_reader = prefered_reader or DEFAULT_READER
     if not AVAILABLE_READERS:
         missing = ", ".join(module.value for module in Reader)
         raise ModuleNotFoundError(f"None of the following were found: {missing}")
 
     if prefered_reader in AVAILABLE_READERS:
-        with _get_stream(__fp, prefered_reader) as wrapper:
-            return AVAILABLE_READERS[prefered_reader].load(wrapper)
+        reader = prefered_reader
+        mod = AVAILABLE_READERS[reader]
     elif not allow_fallback:
         raise ModuleNotFoundError(f"No module named {prefered_reader.value!r}")
+    else:
+        reader, mod = next(iter(AVAILABLE_READERS.items()))
 
-    reader, mod = next(iter(AVAILABLE_READERS.items()))
-    with _get_stream(__fp, reader) as wrapper:
-        return mod.load(wrapper)
+    if hasattr(mod, "load"):
+        with _get_stream(__fp, reader) as wrapper:
+            return mod.load(wrapper)
+    # Older versions of tomlkit
+    else:
+        txt = __fp.read().decode("utf-8")
+        return mod.loads(txt)
 
 
 def dump(
     __data: Mapping[str, Any],
     __fp: BinaryIO,
-    prefered_writer: Writer = DEFAULT_WRITER,
+    prefered_writer: Writer | None = None,
     allow_fallback: bool = True,
 ) -> None:
     """
     Serialize an object to TOML and write it to a binary stream
 
     Parameters:
         __data:
@@ -127,20 +134,93 @@
             A bytes stream that supports `.write()`. Positional argument only.
         prefered_writer:
             A [`Writer`][tomcli.toml.Writer] to use for serializing the Python
             object
         allow_fallback:
             Whether to fallback to another Writer if `prefered_writer` is unavailable
     """
+    prefered_writer = prefered_writer or DEFAULT_WRITER
     if not AVAILABLE_WRITERS:
         missing = ", ".join(module.value for module in Writer)
         raise ModuleNotFoundError(f"None of the following were found: {missing}")
 
     if prefered_writer in AVAILABLE_WRITERS:
-        with _get_stream(__fp, prefered_writer) as wrapper:
-            return AVAILABLE_WRITERS[prefered_writer].dump(__data, wrapper)
+        writer = prefered_writer
+        mod = AVAILABLE_WRITERS[writer]
     elif not allow_fallback:
         raise ModuleNotFoundError(f"No module named {prefered_writer.value!r}")
+    else:
+        writer, mod = next(iter(AVAILABLE_WRITERS.items()))
+    if hasattr(mod, "dump"):
+        with _get_stream(__fp, writer) as wrapper:
+            return mod.dump(__data, wrapper)
+    # Older versions of tomlkit
+    else:
+        txt = mod.dumps(__data).encode("utf-8")
+        __fp.write(txt)
 
-    writer, mod = next(iter(AVAILABLE_WRITERS.items()))
-    with _get_stream(__fp, writer) as wrapper:
-        return mod.dump(__data, wrapper)
+
+def loads(
+    __data: str,
+    prefered_reader: Reader | None = None,
+    allow_fallback: bool = True,
+) -> MutableMapping[str, Any]:
+    """
+    Parse a string containing TOML data
+
+    Parameters:
+        __data:
+            A string containing TOML data. Positional argument only.
+        prefered_writer:
+            A [`Writer`][tomcli.toml.Writer] to use for serializing the Python
+            object
+        allow_fallback:
+            Whether to fallback to another Writer if `prefered_writer` is unavailable
+    """
+    prefered_reader = prefered_reader or DEFAULT_READER
+    reader: Reader
+    mod: ModuleType
+
+    if not AVAILABLE_READERS:
+        missing = ", ".join(module.value for module in Reader)
+        raise ModuleNotFoundError(f"None of the following were found: {missing}")
+
+    if prefered_reader in AVAILABLE_READERS:
+        reader = prefered_reader
+        mod = AVAILABLE_READERS[reader]
+    elif not allow_fallback:
+        raise ModuleNotFoundError(f"No module named {prefered_reader.value!r}")
+    else:
+        reader, mod = next(iter(AVAILABLE_READERS.items()))
+    return mod.loads(__data)
+
+
+def dumps(
+    __data: Mapping[str, Any],
+    prefered_writer: Writer | None = None,
+    allow_fallback: bool = True,
+) -> str:
+    """
+    Serialize an object to TOML and return it as a string
+
+    Parameters:
+        __data:
+            A Python object to serialize. Positional argument only.
+        prefered_writer:
+            A [`Writer`][tomcli.toml.Writer] to use for serializing the Python
+            object
+        allow_fallback:
+            Whether to fallback to another Writer if `prefered_writer` is unavailable
+    """
+    prefered_writer = prefered_writer or DEFAULT_WRITER
+    if not AVAILABLE_WRITERS:
+        missing = ", ".join(module.value for module in Writer)
+        raise ModuleNotFoundError(f"None of the following were found: {missing}")
+
+    if prefered_writer in AVAILABLE_WRITERS:
+        writer = prefered_writer
+        mod = AVAILABLE_WRITERS[writer]
+    elif not allow_fallback:
+        raise ModuleNotFoundError(f"No module named {prefered_writer.value!r}")
+    else:
+        writer, mod = next(iter(AVAILABLE_WRITERS.items()))
+    return mod.dump(__data)
```

### Comparing `tomcli-0.0.0/src/tomcli/cli/get.py` & `tomcli-0.1.0/src/tomcli/cli/get.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # SPDX-License-Identifier: MIT
 
 # ruff: noqa: UP007
 
 from __future__ import annotations
 
 import sys
-from collections.abc import Iterable, Mapping, MutableMapping
-from contextlib import contextmanager
-from typing import IO, Any, Optional
+from collections.abc import Mapping, MutableMapping
+from typing import Any, Optional
 
 from typer import Argument, Exit, Typer
 
+from tomcli.cli._util import _std_cm
 from tomcli.toml import Reader, Writer, dump, load
 
-app = Typer()
+app = Typer(context_settings=dict(help_option_names=["-h", "--help"]))
 
 
 def get_part(data: MutableMapping[str, Any], selector: str) -> Any:
     if selector == ".":
         return data
 
     cur = data
@@ -31,23 +31,14 @@
     except (IndexError, KeyError):
         up_to = ".".join(parts[: idx + 1])
         msg = f"Invalid selector {selector!r}: could not find {up_to!r}"
         raise Exit(msg) from None
     return cur
 
 
-@contextmanager
-def _std_cm(path: str, dash_stream: str, mode: str) -> Iterable[IO[Any]]:
-    if str(path) == "-":
-        yield dash_stream
-    else:
-        with open(path, mode) as fp:
-            yield fp
-
-
 @app.command()
 def get(
     path: str = Argument(...),
     selector: str = Argument("."),
     reader: Optional[Reader] = None,
     writer: Optional[Writer] = None,
 ):
```

### Comparing `tomcli-0.0.0/tests/test_tomcli_get.py` & `tomcli-0.1.0/tests/test_tomcli_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
 from pathlib import Path
 
 import typer
 import typer.testing
+
 from tomcli.cli.get import app
 
 HERE = Path(__file__).resolve().parent
 ROOT = HERE.parent
 
 
 def test_get_basic_dump(writer: str, reader: str):
@@ -49,20 +50,23 @@
         file,
         "build-system",
         f"--writer={writer}",
         f"--reader={reader}",
     ]
     ran = typer.testing.CliRunner().invoke(app, args)
     valid = [
-        """\
+        i.strip()
+        for i in (
+            """
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 """,
-        """\
+            """
 requires = [
     "hatchling",
 ]
 build-backend = "hatchling.build"
 """,
+        )
     ]
     assert ran.exit_code == 0
-    assert ran.stdout in valid
+    assert ran.stdout.strip() in valid
```

### Comparing `tomcli-0.0.0/pyproject.toml` & `tomcli-0.1.0/tests/test_data/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,17 @@
 dependencies = [
     "typer",
 ]
 
 [project.optional-dependencies]
 # User facing
 all = [
-    # For typer
-    "rich",
-    # Keep in sync with tomli and tomlkit extras.
+    "typer[all]",
+    # Keep in sync with tomlkit extra.
     # We can't use self-referntial extras in Fedora.
-    "tomli ; python_version<'3.11'",
-    "tomli_w",
     "tomlkit",
     #
 ]
 tomli = [
     "tomli ; python_version<'3.11'",
     "tomli_w",
 ]
@@ -76,10 +73,11 @@
 
 [project.urls]
 "Source code" = "https://git.sr.ht/~gotmax23/tomcli"
 "Mailing list" = "https://lists.sr.ht/~gotmax23/tomcli"
 
 [project.scripts]
 "tomcli-get" = "tomcli.cli.get:app"
+"tomcli-set" = "tomcli.cli.set:app"
 
 [tool.hatch.version]
 path = "src/tomcli/__init__.py"
```

### Comparing `tomcli-0.0.0/LICENSES/MIT.txt` & `tomcli-0.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `tomcli-0.0.0/PKG-INFO` & `tomcli-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcli
-Version: 0.0.0
+Version: 0.1.0
 Summary: CLI for working with TOML files. Pronounced "tohm-clee."
 Project-URL: Source code, https://git.sr.ht/~gotmax23/tomcli
 Project-URL: Mailing list, https://lists.sr.ht/~gotmax23/tomcli
 Author-email: Maxwell G <maxwell@gtmx.me>
 License-Expression: MIT
 License-File: LICENSES/MIT.txt
 Classifier: Development Status :: 3 - Alpha
@@ -15,27 +15,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: typer
 Provides-Extra: all
-Requires-Dist: rich; extra == 'all'
-Requires-Dist: tomli-w; extra == 'all'
-Requires-Dist: tomli; python_version < '3.11' and extra == 'all'
 Requires-Dist: tomlkit; extra == 'all'
+Requires-Dist: typer[all]; extra == 'all'
 Provides-Extra: codeqa
 Requires-Dist: reuse; extra == 'codeqa'
 Requires-Dist: ruff; extra == 'codeqa'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: nox>=2022.11.21; extra == 'dev'
+Requires-Dist: tomcli[all]; extra == 'dev'
 Requires-Dist: tomcli[codeqa]; extra == 'dev'
 Requires-Dist: tomcli[formatters]; extra == 'dev'
 Requires-Dist: tomcli[test]; extra == 'dev'
+Requires-Dist: tomcli[tomli]; extra == 'dev'
 Provides-Extra: formatters
 Requires-Dist: black; extra == 'formatters'
 Requires-Dist: ruff; extra == 'formatters'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Provides-Extra: tomli
 Requires-Dist: tomli-w; extra == 'tomli'
@@ -52,14 +52,18 @@
 SPDX-License-Identifier: MIT
 -->
 
 # tomcli
 
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/tomcli/commits/main.svg)](https://builds.sr.ht/~gotmax23/tomcli/commits/main?)
 
+[![copr build status][badge-copr]][link-copr] (gotmax23/tomcli)
+
+[![copr build status][badge-copr-dev]][link-copr-dev] (gotmax23/tomcli-dev)
+
 
 CLI for modifying toml files. Pronounced "tohm-clee."
 
 ## Links
 
 - [tomcli project hub](https://sr.ht/~gotmax23/tomcli)
 - [tomcli git.sr.ht repo](https://git.sr.ht/~gotmax23/tomcli)
@@ -74,7 +78,12 @@
 See [CONTRIBUTING.md](https://git.sr.ht/~gotmax23/tomcli/tree/main/item/CONTRIBUTING.md).
 
 ## License
 
 This repository is licensed under
 
     SPDX-License-Identifer: MIT
+
+[badge-copr]: https://copr.fedorainfracloud.org/coprs/gotmax23/tomcli/package/tomcli/status_image/last_build.png
+[link-copr]: https://copr.fedorainfracloud.org/coprs/gotmax23/tomcli/
+[badge-copr-dev]: https://copr.fedorainfracloud.org/coprs/gotmax23/tomcli-dev/package/tomcli/status_image/last_build.png
+[link-copr-dev]: https://copr.fedorainfracloud.org/coprs/gotmax23/tomcli-dev/
```

