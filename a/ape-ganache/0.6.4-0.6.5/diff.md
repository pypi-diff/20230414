# Comparing `tmp/ape-ganache-0.6.4.tar.gz` & `tmp/ape-ganache-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ganache-0.6.4.tar", last modified: Tue Apr 11 14:42:01 2023, max compression
+gzip compressed data, was "ape-ganache-0.6.5.tar", last modified: Thu Apr 13 22:18:44 2023, max compression
```

## Comparing `ape-ganache-0.6.4.tar` & `ape-ganache-0.6.5.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.451766 ape-ganache-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.427765 ape-ganache-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.427765 ape-ganache-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.431765 ape-ganache-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-11 14:42:01.451766 ape-ganache-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.431765 ape-ganache-0.6.4/ape_ganache/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/ape_ganache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/ape_ganache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/ape_ganache/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/ape_ganache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 14:42:01.000000 ape-ganache-0.6.4/ape_ganache/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.431765 ape-ganache-0.6.4/ape_ganache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-11 14:42:01.000000 ape-ganache-0.6.4/ape_ganache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-11 14:42:01.000000 ape-ganache-0.6.4/ape_ganache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:42:01.000000 ape-ganache-0.6.4/ape_ganache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:42:01.000000 ape-ganache-0.6.4/ape_ganache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-11 14:42:01.000000 ape-ganache-0.6.4/ape_ganache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 14:42:01.000000 ape-ganache-0.6.4/ape_ganache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 14:42:01.451766 ape-ganache-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.435765 ape-ganache-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.423765 ape-ganache-0.6.4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.423765 ape-ganache-0.6.4/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.423765 ape-ganache-0.6.4/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.439766 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)    33359 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28199 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.423765 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.451766 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.451766 ape-ganache-0.6.4/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:01.451766 ape-ganache-0.6.4/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-11 14:41:11.000000 ape-ganache-0.6.4/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.421451 ape-ganache-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-13 22:18:44.421451 ape-ganache-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/ape_ganache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/ape_ganache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/ape_ganache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/ape_ganache/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/ape_ganache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:18:44.000000 ape-ganache-0.6.5/ape_ganache/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.413451 ape-ganache-0.6.5/ape_ganache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-13 22:18:44.000000 ape-ganache-0.6.5/ape_ganache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-04-13 22:18:44.000000 ape-ganache-0.6.5/ape_ganache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:18:44.000000 ape-ganache-0.6.5/ape_ganache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:18:44.000000 ape-ganache-0.6.5/ape_ganache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-13 22:18:44.000000 ape-ganache-0.6.5/ape_ganache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 22:18:44.000000 ape-ganache-0.6.5/ape_ganache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 22:18:44.421451 ape-ganache-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.413451 ape-ganache-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.413451 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33359 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28199 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.409451 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.421451 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.421451 ape-ganache-0.6.5/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:18:44.421451 ape-ganache-0.6.5/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-13 22:17:54.000000 ape-ganache-0.6.5/tests/test_trace.py
```

### Comparing `ape-ganache-0.6.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-ganache-0.6.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-ganache-0.6.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ganache-0.6.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/release-drafter.yml` & `ape-ganache-0.6.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/workflows/codeql.yml` & `ape-ganache-0.6.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/workflows/commit.yaml` & `ape-ganache-0.6.5/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/workflows/prtitle.yaml` & `ape-ganache-0.6.5/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/workflows/publish.yaml` & `ape-ganache-0.6.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/workflows/stale-prs.yml` & `ape-ganache-0.6.5/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.github/workflows/test.yaml` & `ape-ganache-0.6.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.gitignore` & `ape-ganache-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/.pre-commit-config.yaml` & `ape-ganache-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/CONTRIBUTING.md` & `ape-ganache-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/LICENSE` & `ape-ganache-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/PKG-INFO` & `ape-ganache-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ganache
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-ganache: Ape network provider for Ganache
 Home-page: https://github.com/ApeWorX/ape-ganache
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-ganache-0.6.4/README.md` & `ape-ganache-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/ape_ganache/__init__.py` & `ape-ganache-0.6.5/ape_ganache/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/ape_ganache/exceptions.py` & `ape-ganache-0.6.5/ape_ganache/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/ape_ganache/provider.py` & `ape-ganache-0.6.5/ape_ganache/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 import shutil
 from enum import Enum
+from itertools import tee
 from pathlib import Path
 from subprocess import PIPE, Popen
 from typing import Dict, Iterator, List, Literal, Optional, Union, cast
 
 from ape.api import (
     ImpersonatedAccount,
     PluginConfig,
@@ -357,51 +358,72 @@
         # Strange bug in Ganache where sub-calls REVERT trickles to the top-level
         # CALL when it is not supposed to. Reset `failed`.
         evm_call.failed = receipt.failed
 
         return self._create_call_tree_node(evm_call, txn_hash=txn_hash)
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
-        txn = kwargs.get("txn")
         if not len(exception.args):
-            return VirtualMachineError(base_err=exception, txn=txn)
+            return VirtualMachineError(base_err=exception, **kwargs)
 
+        ganache_prefix = "VM Exception while processing transaction: "
         err_data = exception.args[0]
         if isinstance(err_data, dict):
             message = str(err_data.get("message"))
+
+            if err_data.get("data", {}).get("hash") and message == f"{ganache_prefix}revert":
+                txn_hash = err_data.get("data", {}).get("hash")
+                data = {}
+
+                if "trace" in kwargs:
+                    kwargs["trace"], new_trace = tee(kwargs["trace"])
+                    data = list(new_trace)[-1].raw
+
+                else:
+                    try:
+                        data = list(self.get_transaction_trace(txn_hash))[-1].raw
+                    except Exception:
+                        pass
+
+                if data.get("op") == "REVERT":
+                    err_selector_and_inputs = "".join([x[2:] for x in data["memory"][4:]])
+                    if err_selector_and_inputs:
+                        message = f"{ganache_prefix}0x{err_selector_and_inputs}"
+
         elif isinstance(err_data, str):
             # The message is already extract during gas estimation
             message = str(err_data)
         else:
-            return VirtualMachineError(base_err=exception, txn=txn)
+            return VirtualMachineError(base_err=exception, **kwargs)
 
         if not message:
-            return VirtualMachineError(base_err=exception, txn=txn)
+            return VirtualMachineError(base_err=exception, **kwargs)
 
         # Handle `ContactLogicError` similarly to other providers in `ape`.
         # by stripping off the unnecessary prefix that ganache has on reverts.
-        ganache_prefix = "VM Exception while processing transaction: "
         prefixes = (f"execution reverted: {ganache_prefix}", ganache_prefix)
         is_revert = False
         for prefix in prefixes:
             if message.startswith(prefix):
                 message = message.replace(prefix, "")
                 is_revert = True
                 break
 
         if not is_revert:
-            return VirtualMachineError(message, txn=txn)
+            return VirtualMachineError(message, **kwargs)
 
-        elif message == "revert":
-            return ContractLogicError(txn=txn)
+        if message == "revert":
+            err = ContractLogicError(**kwargs)
+            return self.compiler_manager.enrich_error(err)
 
         elif message.startswith("revert "):
             message = message.replace("revert ", "")
 
-        return ContractLogicError(revert_message=message, txn=txn)
+        err = ContractLogicError(revert_message=message, **kwargs)
+        return self.compiler_manager.enrich_error(err)
 
     def unlock_account(self, address: AddressType) -> bool:
         self._make_request("evm_addAccount", [address, ""])
         return self._make_request("personal_unlockAccount", [address, "", 9999999999])
 
 
 class GanacheForkProvider(GanacheProvider):
```

### Comparing `ape-ganache-0.6.4/ape_ganache.egg-info/PKG-INFO` & `ape-ganache-0.6.5/ape_ganache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ganache
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-ganache: Ape network provider for Ganache
 Home-page: https://github.com/ApeWorX/ape-ganache
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-ganache-0.6.4/ape_ganache.egg-info/SOURCES.txt` & `ape-ganache-0.6.5/ape_ganache.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 tests/test_fork_provider.py
 tests/test_gas_report.py
 tests/test_provider.py
 tests/test_trace.py
 tests/data/contracts/ethereum/local/contract_a.json
 tests/data/contracts/ethereum/local/contract_b.json
 tests/data/contracts/ethereum/local/contract_c.json
+tests/data/contracts/ethereum/local/has_error.json
 tests/data/contracts/ethereum/local/solidity_contract.json
 tests/data/contracts/ethereum/local/token_a.json
 tests/data/contracts/ethereum/local/token_b.json
 tests/data/contracts/ethereum/local/vyper_contract.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
@@ -104,9 +105,10 @@
 tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
 tests/data/python/pytest_test_conftest.py
 tests/data/python/pytest_tests.py
+tests/data/sources/HasError.sol
 tests/data/sources/TokenA.vy
 tests/data/sources/TokenB.vy
```

### Comparing `ape-ganache-0.6.4/ape_ganache.egg-info/requires.txt` & `ape-ganache-0.6.5/ape_ganache.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-eth-ape<0.7,>=0.6.7
-evm-trace>=0.1.0a14
+eth-ape<0.7,>=0.6.8
+evm-trace
 hexbytes
 web3
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
```

### Comparing `ape-ganache-0.6.4/pyproject.toml` & `ape-ganache-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/setup.py` & `ape-ganache-0.6.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-ganache",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.7,<0.7",
-        "evm-trace>=0.1.0a14",
+        "eth-ape>=0.6.8,<0.7",
+        "evm-trace",  # Use same version as eth-ape
         "hexbytes",  # Use same version as eth-ape
         "web3",  # Use same version as eth-ape
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_ganache"],
     license="Apache-2.0",
```

### Comparing `ape-ganache-0.6.4/tests/ape-config.yaml` & `ape-ganache-0.6.5/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/conftest.py` & `ape-ganache-0.6.5/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from ape_ganache import GanacheProvider
 
 # NOTE: Ensure that we don't use local paths for the DATA FOLDER
 ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "data" / "contracts"
+LOCAL_CONTRACTS_PATH = BASE_CONTRACTS_PATH / "ethereum" / "local"
 NAME = "ganache"
 
 # Needed to test tracing support in core `ape test` command.
 pytest_plugins = ["pytester"]
 MAINNET_FORK_PORT = 9001
 GOERLI_FORK_PORT = 9002
 
@@ -107,35 +108,49 @@
 
 
 @pytest.fixture(scope="session")
 def networks():
     return ape.networks
 
 
-@pytest.fixture(params=("solidity", "vyper"))
-def raw_contract_type(request):
-    path = BASE_CONTRACTS_PATH / "ethereum" / "local" / f"{request.param}_contract.json"
-    return path.read_text()
+@pytest.fixture
+def get_contract_type():
+    def fn(name: str) -> ContractType:
+        return ContractType.parse_file(LOCAL_CONTRACTS_PATH / f"{name}.json")
 
+    return fn
 
-@pytest.fixture
-def contract_type(raw_contract_type) -> ContractType:
-    return ContractType.parse_raw(raw_contract_type)
+
+@pytest.fixture(params=("solidity", "vyper"))
+def contract_type(request, get_contract_type) -> ContractType:
+    name = f"{request.param}_contract"
+    return get_contract_type(name)
 
 
 @pytest.fixture
 def contract_container(contract_type) -> ContractContainer:
     return ContractContainer(contract_type=contract_type)
 
 
 @pytest.fixture
 def contract_instance(owner, contract_container, connected_provider):
     return owner.deploy(contract_container)
 
 
+@pytest.fixture
+def error_contract_container(get_contract_type):
+    ct = get_contract_type("has_error")
+    return ContractContainer(ct)
+
+
+@pytest.fixture
+def error_contract(owner, error_contract_container):
+    return owner.deploy(error_contract_container)
+
+
 @pytest.fixture(scope="session")
 def sender(accounts):
     return accounts[0]
 
 
 @pytest.fixture(scope="session")
 def receiver(accounts):
@@ -144,14 +159,19 @@
 
 @pytest.fixture(scope="session")
 def owner(accounts):
     return accounts[2]
 
 
 @pytest.fixture(scope="session")
+def not_owner(accounts):
+    return accounts[3]
+
+
+@pytest.fixture(scope="session")
 def local_network_api(networks):
     return networks.ethereum.local
 
 
 @pytest.fixture
 def connected_provider(name, networks, local_network_api):
     with networks.ethereum.local.use_provider(name) as provider:
```

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/local/contract_a.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/local/contract_b.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/local/contract_c.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/local/token_a.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/local/token_b.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-ganache-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/python/pytest_tests.py` & `ape-ganache-0.6.5/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/sources/TokenA.vy` & `ape-ganache-0.6.5/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/data/sources/TokenB.vy` & `ape-ganache-0.6.5/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/expected_traces.py` & `ape-ganache-0.6.5/tests/expected_traces.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 LOCAL_TRACE = r"""
-Call trace for
-'0x([A-Fa-f0-9]{64})'
+Call trace for '0x([A-Fa-f0-9]{64})'
 tx\.origin=0x[a-fA-F0-9]{40}
 ContractA\.methodWithoutArguments\(\) -> 0x00..5174 \[\d+ gas\]
 ├── SYMBOL\.methodB1\(lolol="ice-cream", dynamo=36\)
 │   ├── ContractC\.getSomeList\(\) -> \[
 │   │     3425311345134513461345134534531452345,
 │   │     111344445534535353,
 │   │     993453434534534534534977788884443333
 │   │   \]
 │   └── ContractC\.methodC1\(windows95="simpler", jamaica=36, cardinal=ContractA\)
 ├── SYMBOL\.callMe\(blue=tx.origin\) -> tx\.origin
 ├── SYMBOL\.methodB2\(trombone=tx.origin\)
-│   ├── ContractC\.paperwork\(ContractA\) -> \(os="simpler", country=36,
-│   │   wings=ContractA\)
+│   ├── ContractC\.paperwork\(ContractA\) -> \(os="simpler", country=36, wings=ContractA\)
 │   ├── ContractC\.methodC1\(windows95="simpler", jamaica=0, cardinal=ContractC\)
 │   ├── ContractC\.methodC2\(\)
 │   └── ContractC\.methodC2\(\)
 ├── ContractC\.addressToValue\(tx\.origin\) -> 0
 ├── SYMBOL\.bandPractice\(tx\.origin\) -> 0
 ├── SYMBOL\.methodB1\(lolol="lemondrop", dynamo=0\)
 │   ├── ContractC\.getSomeList\(\) -> \[
@@ -31,16 +29,15 @@
     │     3425311345134513461345134534531452345,
     │     111344445534535353,
     │     993453434534534534534977788884443333
     │   \]
     └── ContractC\.methodC1\(windows95="simpler", jamaica=111, cardinal=ContractA\)
 """
 MAINNET_FAIL_TRACE_FIRST_10_LINES = r"""
-Call trace for
-'0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d'
+Call trace for '0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d'
 reverted with message: "UNIV3R: min return"
 tx\.origin=0xd2f91C13e2D7ABbA4408Cd3D86285b7835524ad7
 AggregationRouterV4\.uniswapV3Swap\(
   amount=12851675475480000000000,
   minReturn=4205588148,
   pools=\[
     682631518358379038160760928734868612545194078373,
@@ -55,25 +52,36 @@
     │   ├── UniswapV3Pool\.token0\(\) -> FiatTokenProxy
     │   ├── UniswapV3Pool\.token1\(\) -> WETH
     │   ├── UniswapV3Pool\.fee\(\) -> 500
     │   └── WETH\.transfer\(dst=UniswapV3Pool, wad=2098831888913057968\) -> True
     └── WETH\.balanceOf\(UniswapV3Pool\) -> 68359883632315875514968
 """
 MAINNET_TRACE_FIRST_10_LINES = r"""
-Call trace for
-'0xb7d7f1d5ce7743e821d3026647df486f517946ef1342a1ae93c96e4a8016eab7'
+Call trace for '0xb7d7f1d5ce7743e821d3026647df486f517946ef1342a1ae93c96e4a8016eab7'
 tx\.origin=0x5668EAd1eDB8E2a4d724C8fb9cB5fFEabEB422dc
 DSProxy\.execute\(_target=LoanShifterTaker, _data=0x35\.\.0000\) -> "" \[1249147 gas\]
 └── \(delegate\) LoanShifterTaker\.moveLoan\(
       _exchangeData=\[
         0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE,
         ZERO_ADDRESS,
         0,
         0,
 """
+MAINNET_TRACE_LAST_10_LINES = r"""
+    │                   └── LendingRateOracle\.getMarketBorrowRate\(_asset=DAI\) ->
+    │                       35000000000000000000000000
+    ├── DSProxy\.authority\(\) -> DSGuard
+    ├── DSGuard\.forbid\(src=LoanShifterReceiver, dst=DSProxy, sig=0x1c\.\.0000\)
+    └── DefisaverLogger\.Log\(
+          _contract=DSProxy,
+          _caller=tx\.origin,
+          _logName="LoanShifter",
+          _data=0x00\.\.0000
+        \)
+"""
 LOCAL_GAS_REPORT = r"""
  +ContractA Gas
 
   Method +Times called +Min. +Max. +Mean +Median
  ─+
   methodWithoutArguments +1 +\d+ +\d+ +\d+ + \d+
 """
```

### Comparing `ape-ganache-0.6.4/tests/test_fork_provider.py` & `ape-ganache-0.6.5/tests/test_fork_provider.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/test_gas_report.py` & `ape-ganache-0.6.5/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `ape-ganache-0.6.4/tests/test_provider.py` & `ape-ganache-0.6.5/tests/test_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,7 +173,15 @@
 
     # Ensure can use impersonated accounts.
     other_account = accounts[0]
     other_account.transfer(impersonated_account, "1 ETH")
     assert impersonated_account.balance == int(1e18)
     receipt = impersonated_account.transfer(accounts[0], "0.5 ETH")
     assert not receipt.failed
+
+
+def test_revert_error(error_contract, not_owner):
+    """
+    Test matching a revert custom Solidity error.
+    """
+    with pytest.raises(error_contract.Unauthorized):
+        error_contract.withdraw(sender=not_owner)
```

### Comparing `ape-ganache-0.6.4/tests/test_trace.py` & `ape-ganache-0.6.5/tests/test_trace.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 import re
 import shutil
+import tempfile
 from pathlib import Path
 from typing import List
 
 import pytest
 from ape.contracts import ContractContainer
 from ethpm_types import ContractType
 
 from .expected_traces import (
     LOCAL_GAS_REPORT,
     LOCAL_TRACE,
     MAINNET_FAIL_TRACE_FIRST_10_LINES,
     MAINNET_FAIL_TRACE_LAST_10_LINES,
     MAINNET_TRACE_FIRST_10_LINES,
+    MAINNET_TRACE_LAST_10_LINES,
 )
 
 MAINNET_FAIL_TXN_HASH = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
 MAINNET_TXN_HASH = "0xb7d7f1d5ce7743e821d3026647df486f517946ef1342a1ae93c96e4a8016eab7"
 EXPECTED_MAP = {
-    MAINNET_TXN_HASH: (MAINNET_TRACE_FIRST_10_LINES,),
-    MAINNET_FAIL_TXN_HASH: (
-        MAINNET_FAIL_TRACE_FIRST_10_LINES,
-        MAINNET_FAIL_TRACE_LAST_10_LINES,
-    ),
+    MAINNET_TXN_HASH: (MAINNET_TRACE_FIRST_10_LINES, MAINNET_TRACE_LAST_10_LINES),
+    MAINNET_FAIL_TXN_HASH: (MAINNET_FAIL_TRACE_FIRST_10_LINES, MAINNET_FAIL_TRACE_LAST_10_LINES),
 }
 BASE_CONTRACTS_PATH = Path(__file__).parent / "data" / "contracts" / "ethereum"
 
 
 @pytest.fixture
 def captrace(capsys):
     class CapTrace:
-        def read_trace(self, expected_start: str):
-            lines = capsys.readouterr().out.splitlines()
+        def read_trace(self, expected_start: str, file=None):
+            lines = file.readlines() if file else capsys.readouterr().out.splitlines()
             start_index = 0
             for index, line in enumerate(lines):
-                if line.strip() == expected_start:
+                if line.strip().startswith(expected_start):
                     start_index = index
                     break
 
             return lines[start_index:]
 
     return CapTrace()
 
@@ -79,47 +78,71 @@
     return contract_a.methodWithoutArguments(sender=owner)
 
 
 def test_local_transaction_traces(local_receipt, captrace):
     # NOTE: Strange bug in Rich where we can't use sys.stdout for testing tree output.
     # And we have to write to a file, close it, and then re-open it to see output.
     def run_test():
-        local_receipt.show_trace()
-        lines = captrace.read_trace("Call trace for")
+        with tempfile.TemporaryDirectory() as temp_dir:
+            temp_file = Path(temp_dir) / "temp"
+
+            with open(temp_file, "w") as file:
+                local_receipt.show_trace(file=file)
+
+            with open(temp_file, "r") as file:
+                lines = captrace.read_trace("Call trace for", file=file)
+
         assert_rich_output(lines, LOCAL_TRACE)
 
     run_test()
 
     # Verify can happen more than once.
     run_test()
 
 
 def test_local_transaction_gas_report(local_receipt, captrace):
     def run_test():
-        local_receipt.show_gas_report()
-        lines = captrace.read_trace("ContractA Gas")
-        assert_rich_output(lines, LOCAL_GAS_REPORT)
+        with tempfile.TemporaryDirectory() as temp_dir:
+            temp_file = Path(temp_dir) / "temp"
+
+            with open(temp_file, "w") as file:
+                local_receipt.show_gas_report(file=file)
+
+            with open(temp_file, "r") as file:
+                lines = captrace.read_trace("ContractA Gas", file=file)
+
+            assert_rich_output(lines, LOCAL_GAS_REPORT)
 
     run_test()
 
     # Verify can happen more than once.
     run_test()
 
 
 @pytest.mark.manual
 def test_mainnet_transaction_traces(mainnet_receipt, captrace):
-    mainnet_receipt.show_trace()
-    lines = captrace.read_trace("Call trace for")
-    expected_beginning = EXPECTED_MAP[mainnet_receipt.txn_hash][0]
-    actual_beginning = lines[:10]
-    assert_rich_output(actual_beginning, expected_beginning)
-
-    # NOTE: Currently, the end of the first mainnet trace does not work
-    # It randomly cuts off in Ganache because of bug. Thus, we are currently
-    # only comparing the first 10 lines.
+    with tempfile.TemporaryDirectory() as temp_dir:
+        temp_file = Path(temp_dir) / "temp"
+
+        with open(temp_file, "w") as file:
+            mainnet_receipt.show_trace(file=file)
+
+        with open(temp_file, "r") as file:
+            lines = captrace.read_trace("Call trace for", file=file)
+
+        expected_beginning, expected_ending = EXPECTED_MAP[mainnet_receipt.txn_hash]
+        actual_beginning = lines[:10]
+        actual_ending = lines[-10:]
+        assert_rich_output(actual_beginning, expected_beginning)
+
+        if mainnet_receipt.txn_hash != MAINNET_TXN_HASH:
+            # NOTE: Currently, the end of the first mainnet trace does not work
+            # It randomly cuts off in Ganache because of bug. Thus, we are currently
+            # only comparing the first 10 lines.
+            assert_rich_output(actual_ending, expected_ending)
 
 
 def assert_rich_output(rich_capture: List[str], expected: str):
     expected_lines = [x.rstrip() for x in expected.splitlines() if x.rstrip()]
     actual_lines = [x.rstrip() for x in rich_capture if x.rstrip()]
     assert actual_lines, "No output."
     output = "\n".join(actual_lines)
```

