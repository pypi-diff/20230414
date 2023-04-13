# Comparing `tmp/ape-hardhat-0.6.3.tar.gz` & `tmp/ape-hardhat-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-hardhat-0.6.3.tar", last modified: Tue Apr 11 14:33:49 2023, max compression
+gzip compressed data, was "ape-hardhat-0.6.4.tar", last modified: Thu Apr 13 22:08:51 2023, max compression
```

## Comparing `ape-hardhat-0.6.3.tar` & `ape-hardhat-0.6.4.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.997008 ape-hardhat-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.973008 ape-hardhat-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.973008 ape-hardhat-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.977008 ape-hardhat-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-11 14:33:48.997008 ape-hardhat-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.977008 ape-hardhat-0.6.3/ape_hardhat/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/ape_hardhat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/ape_hardhat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/ape_hardhat/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/ape_hardhat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 14:33:48.000000 ape-hardhat-0.6.3/ape_hardhat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.977008 ape-hardhat-0.6.3/ape_hardhat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-11 14:33:48.000000 ape-hardhat-0.6.3/ape_hardhat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-11 14:33:48.000000 ape-hardhat-0.6.3/ape_hardhat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:33:48.000000 ape-hardhat-0.6.3/ape_hardhat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:33:48.000000 ape-hardhat-0.6.3/ape_hardhat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-11 14:33:48.000000 ape-hardhat-0.6.3/ape_hardhat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 14:33:48.000000 ape-hardhat-0.6.3/ape_hardhat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/hardhat.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-11 14:33:48.997008 ape-hardhat-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.981008 ape-hardhat-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.973008 ape-hardhat-0.6.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.973008 ape-hardhat-0.6.3/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.973008 ape-hardhat-0.6.3/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.981008 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.973008 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.993008 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.997008 ape-hardhat-0.6.3/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:33:48.997008 ape-hardhat-0.6.3/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-04-11 14:32:47.000000 ape-hardhat-0.6.3/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/ape_hardhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/ape_hardhat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/hardhat.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.777949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_trace.py
```

### Comparing `ape-hardhat-0.6.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/release-drafter.yml` & `ape-hardhat-0.6.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/workflows/codeql.yml` & `ape-hardhat-0.6.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/workflows/commit.yaml` & `ape-hardhat-0.6.4/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/workflows/prtitle.yaml` & `ape-hardhat-0.6.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/workflows/publish.yaml` & `ape-hardhat-0.6.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/workflows/stale-prs.yml` & `ape-hardhat-0.6.4/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.github/workflows/test.yaml` & `ape-hardhat-0.6.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.gitignore` & `ape-hardhat-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/.pre-commit-config.yaml` & `ape-hardhat-0.6.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-hardhat-0.6.3/CONTRIBUTING.md` & `ape-hardhat-0.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/LICENSE` & `ape-hardhat-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/PKG-INFO` & `ape-hardhat-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.6.3
+Version: 0.6.4
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-hardhat-0.6.3/README.md` & `ape-hardhat-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/ape_hardhat/__init__.py` & `ape-hardhat-0.6.4/ape_hardhat/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/ape_hardhat/exceptions.py` & `ape-hardhat-0.6.4/ape_hardhat/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/ape_hardhat/provider.py` & `ape-hardhat-0.6.4/ape_hardhat/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Web3Provider,
 )
 from ape.exceptions import (
     ContractLogicError,
     OutOfGasError,
     ProviderError,
     SubprocessError,
+    TransactionError,
     VirtualMachineError,
 )
 from ape.logging import logger
 from ape.types import AddressType, CallTreeNode, ContractCode, SnapshotID, TraceFrame
 from ape.utils import cached_property
 from ape_test import Config as TestConfig
 from eth_utils import is_0x_prefixed, is_hex, to_hex
@@ -466,42 +467,52 @@
             amount_hex_str = to_hex(int(amount))
         elif isinstance(amount, int) or isinstance(amount, bytes):
             amount_hex_str = to_hex(amount)
 
         self._make_request("hardhat_setBalance", [account, amount_hex_str])
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
-        txn = kwargs.get("txn")
         if not len(exception.args):
-            return VirtualMachineError(base_err=exception, txn=txn)
+            return VirtualMachineError(base_err=exception, **kwargs)
 
         err_data = exception.args[0]
 
         message = err_data if isinstance(err_data, str) else str(err_data.get("message"))
         if not message:
-            return VirtualMachineError(base_err=exception, txn=txn)
+            return VirtualMachineError(base_err=exception, **kwargs)
+
         elif message.startswith("execution reverted: "):
             message = message.replace("execution reverted: ", "")
 
         if message.startswith(_REVERT_REASON_PREFIX):
             message = message.replace(_REVERT_REASON_PREFIX, "").strip("'")
-            return ContractLogicError(revert_message=message, txn=txn)
+            err = ContractLogicError(revert_message=message, **kwargs)
+            return self.compiler_manager.enrich_error(err)
 
         elif _NO_REASON_REVERT_MESSAGE in message:
-            return ContractLogicError(txn=txn)
+            err = ContractLogicError(**kwargs)
+            return self.compiler_manager.enrich_error(err)
 
         elif message == "Transaction ran out of gas":
-            return OutOfGasError(txn=txn)
+            return OutOfGasError(**kwargs)
 
         elif "reverted with an unrecognized custom error" in message and "(return data:" in message:
             # Happens during custom Solidity exceptions.
             message = message.split("(return data:")[-1].rstrip("/)").strip()
-            return ContractLogicError(revert_message=message, txn=txn)
+            err = ContractLogicError(revert_message=message, **kwargs)
+            enriched_error = self.compiler_manager.enrich_error(err)
+
+            if enriched_error.message == TransactionError.DEFAULT_MESSAGE:
+                # Since input data is always missing, and to preserve backwards compat,
+                # use the selector as the message still.
+                enriched_error.message = message
+
+            return enriched_error
 
-        return VirtualMachineError(message)
+        return VirtualMachineError(message, **kwargs)
 
 
 class HardhatForkProvider(HardhatProvider):
     """
     A Hardhat provider that uses ``--fork``, like:
     ``npx hardhat node --fork <upstream-provider-url>``.
```

### Comparing `ape-hardhat-0.6.3/ape_hardhat.egg-info/PKG-INFO` & `ape-hardhat-0.6.4/ape_hardhat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.6.3
+Version: 0.6.4
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-hardhat-0.6.3/ape_hardhat.egg-info/SOURCES.txt` & `ape-hardhat-0.6.4/ape_hardhat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,9 +106,10 @@
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

### Comparing `ape-hardhat-0.6.3/ape_hardhat.egg-info/requires.txt` & `ape-hardhat-0.6.4/ape_hardhat.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-eth-ape<0.7,>=0.6.7
+eth-ape<0.7,>=0.6.8
 evm-trace
 hexbytes
 web3
 
 [dev]
 pytest>=6.0
 pytest-mock
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-alchemy
 ape-polygon
 rich
-black>=22.12.0
-mypy==0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-PyYAML
 types-setuptools
 types-requests
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 setuptools
@@ -37,21 +37,21 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
 [lint]
-black>=22.12.0
-mypy==0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-PyYAML
 types-setuptools
 types-requests
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 
 [release]
 setuptools
 setuptools-scm
```

### Comparing `ape-hardhat-0.6.3/pyproject.toml` & `ape-hardhat-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/setup.py` & `ape-hardhat-0.6.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "ape-alchemy",  # Needed for forked-network tests
         "ape-polygon",  # Needed to make sure polygon works
         "rich",  # Needed for trace tests
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy==0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-PyYAML",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed for mypy typeshed
         "types-requests",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
         "Sphinx>=3.4.3,<4",  # Documentation generator
         "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
@@ -67,15 +67,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-hardhat",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.7,<0.7",
+        "eth-ape>=0.6.8,<0.7",
         "evm-trace",  # Use same version as eth-ape
         "hexbytes",  # Use same version as eth-ape
         "web3",  # Use same version as eth-ape
     ],
     python_requires=">=3.8,<3.11",
     extras_require=extras_require,
     py_modules=["ape_hardhat"],
```

### Comparing `ape-hardhat-0.6.3/tests/ape-config.yaml` & `ape-hardhat-0.6.4/tests/ape-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   request_timeout: 29
   fork_request_timeout: 360
 
   fork:
     ethereum:
       mainnet:
         upstream_provider: alchemy
-        block_number: 15776634
+        block_number: 17040366
       goerli:
         upstream_provider: alchemy
         block_number: 7849922
       sepolia:
         upstream_provider: alchemy
         block_number: 3091950
```

### Comparing `ape-hardhat-0.6.3/tests/conftest.py` & `ape-hardhat-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/contract_a.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/contract_b.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/contract_c.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/has_error.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/has_error.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7256944444444444%*

 * *Differences: {"'abi'": "{1: {'inputs': [OrderedDict([('internalType', 'address'), ('name', 'addr'), ('type', "*

 * *          "'address')]), OrderedDict([('internalType', 'uint256'), ('name', 'counter'), ('type', "*

 * *          "'uint256')])]}, insert: [(0, OrderedDict([('inputs', [OrderedDict([('internalType', "*

 * *          "'address'), ('name', 'foo'), ('type', 'address')])]), ('name', 'OtherError'), ('type', "*

 * *          "'error')]))]}",*

 * * "'deploymentBytecode'": "{'bytecode': "*

 * *                         "'0x608060405260008054600 […]*

```diff
@@ -1,34 +1,57 @@
 {
     "abi": [
         {
-            "inputs": [],
+            "inputs": [
+                {
+                    "internalType": "address",
+                    "name": "foo",
+                    "type": "address"
+                }
+            ],
+            "name": "OtherError",
+            "type": "error"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "address",
+                    "name": "addr",
+                    "type": "address"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "counter",
+                    "type": "uint256"
+                }
+            ],
             "name": "Unauthorized",
             "type": "error"
         },
         {
             "inputs": [],
             "name": "withdraw",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
     "contractName": "HasError",
     "deploymentBytecode": {
-        "bytecode": "0x6080604052600080546001600160a01b0319163317905534801561002257600080fd5b5060d0806100316000396000f3fe6080604052348015600f57600080fd5b506004361060285760003560e01c80633ccfd60b14602d575b600080fd5b60336035565b005b6000546001600160a01b03163314605e576040516282b42960e81b815260040160405180910390fd5b600080546040516001600160a01b03909116914780156108fc02929091818181858888f193505050501580156097573d6000803e3d6000fd5b5056fea2646970667358221220468a2879368e6d2aa4ab94427e98c665c9b1e891a664a4ab8c3c90d1f43bfd7764736f6c63430008130033"
+        "bytecode": "0x6080604052600080546001600160a01b0319163317905534801561002257600080fd5b5060fd806100316000396000f3fe6080604052348015600f57600080fd5b506004361060285760003560e01c80633ccfd60b14602d575b600080fd5b60336035565b005b6000546001600160a01b03163314606d5760405163da47202360e01b8152336004820152607b60248201526044015b60405180910390fd5b33608b576040516366441a6560e11b81523360048201526024016064565b600080546040516001600160a01b03909116914780156108fc02929091818181858888f1935050505015801560c4573d6000803e3d6000fd5b5056fea2646970667358221220ba2c63b5e17021933e79c5cd42e5f3aeb4661c4cf4176013d4b4ac57e35955b264736f6c63430008130033"
     },
     "devdoc": {
         "kind": "dev",
         "methods": {},
         "version": 1
     },
     "runtimeBytecode": {
-        "bytecode": "0x6080604052600080546001600160a01b0319163317905534801561002257600080fd5b5060d0806100316000396000f3fe6080604052348015600f57600080fd5b506004361060285760003560e01c80633ccfd60b14602d575b600080fd5b60336035565b005b6000546001600160a01b03163314605e576040516282b42960e81b815260040160405180910390fd5b600080546040516001600160a01b03909116914780156108fc02929091818181858888f193505050501580156097573d6000803e3d6000fd5b5056fea2646970667358221220468a2879368e6d2aa4ab94427e98c665c9b1e891a664a4ab8c3c90d1f43bfd7764736f6c63430008130033"
+        "bytecode": "0x6080604052600080546001600160a01b0319163317905534801561002257600080fd5b5060fd806100316000396000f3fe6080604052348015600f57600080fd5b506004361060285760003560e01c80633ccfd60b14602d575b600080fd5b60336035565b005b6000546001600160a01b03163314606d5760405163da47202360e01b8152336004820152607b60248201526044015b60405180910390fd5b33608b576040516366441a6560e11b81523360048201526024016064565b600080546040516001600160a01b03909116914780156108fc02929091818181858888f1935050505015801560c4573d6000803e3d6000fd5b5056fea2646970667358221220ba2c63b5e17021933e79c5cd42e5f3aeb4661c4cf4176013d4b4ac57e35955b264736f6c63430008130033"
     },
-    "sourceId": "HasError.sol",
+    "sourceId": "has_error.json",
+    "sourcemap": "144:342:3:-:0;;;168:43;;;-1:-1:-1;;;;;;168:43:3;200:10;168:43;;;144:342;;;;;;;;;;;;;;;;",
     "userdoc": {
         "kind": "user",
         "methods": {},
         "version": 1
     }
 }
```

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/token_a.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/token_b.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/python/pytest_tests.py` & `ape-hardhat-0.6.4/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/sources/TokenA.vy` & `ape-hardhat-0.6.4/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/data/sources/TokenB.vy` & `ape-hardhat-0.6.4/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/expected_traces.py` & `ape-hardhat-0.6.4/tests/expected_traces.py`

 * *Files 9% similar despite different names*

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
@@ -55,16 +52,15 @@
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
```

### Comparing `ape-hardhat-0.6.3/tests/test_fork_provider.py` & `ape-hardhat-0.6.4/tests/test_fork_provider.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/test_gas_report.py` & `ape-hardhat-0.6.4/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.3/tests/test_provider.py` & `ape-hardhat-0.6.4/tests/test_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,22 @@
     with pytest.raises(ContractLogicError, match="Transaction failed."):
         contract_instance.setNumber(5, sender=owner)
 
 
 def test_contract_revert_custom_exception(owner, get_contract_type, accounts):
     ct = get_contract_type("has_error")
     contract = owner.deploy(ContractContainer(ct))
-    with pytest.raises(ContractLogicError, match="0x82b42900"):
+
+    # Hex match for backwards compat.
+    # Will support the same custom
+    with pytest.raises(contract.Unauthorized) as err:
         contract.withdraw(sender=accounts[7])
 
+    assert err.value.inputs == {"addr": accounts[7].address, "counter": 123}
+
 
 def test_transaction_contract_as_sender(contract_instance, connected_provider):
     # Set balance so test wouldn't normally fail from lack of funds
     connected_provider.set_balance(contract_instance.address, "1000 ETH")
 
     with pytest.raises(ContractLogicError, match="!authorized"):
         # Task failed successfully
```

### Comparing `ape-hardhat-0.6.3/tests/test_trace.py` & `ape-hardhat-0.6.4/tests/test_trace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import shutil
+import tempfile
 from pathlib import Path
 from typing import List
 
 import pytest
 from ape.contracts import ContractContainer
 from ethpm_types import ContractType
 
@@ -24,19 +25,19 @@
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
 
@@ -76,46 +77,67 @@
 
 
 @pytest.mark.fork
 def test_local_transaction_traces(local_receipt, captrace):
     # NOTE: Strange bug in Rich where we can't use sys.stdout for testing tree output.
     # And we have to write to a file, close it, and then re-open it to see output.
     def run_test():
-        local_receipt.show_trace()
-        lines = captrace.read_trace("Call trace for")
-        assert_rich_output(lines, LOCAL_TRACE)
+        with tempfile.TemporaryDirectory() as temp_dir:
+            temp_file = Path(temp_dir) / "temp"
+
+            with open(temp_file, "w") as file:
+                local_receipt.show_trace(file=file)
+
+            with open(temp_file, "r") as file:
+                lines = captrace.read_trace("Call trace for", file=file)
+
+            assert_rich_output(lines, LOCAL_TRACE)
 
     run_test()
 
     # Verify can happen more than once.
     run_test()
 
 
 @pytest.mark.fork
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
-    expected_beginning, expected_ending = EXPECTED_MAP[mainnet_receipt.txn_hash]
-    actual_beginning = lines[:10]
-    actual_ending = lines[-10:]
-    assert_rich_output(actual_beginning, expected_beginning)
-    assert_rich_output(actual_ending, expected_ending)
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
+        assert_rich_output(actual_ending, expected_ending)
 
 
 def assert_rich_output(rich_capture: List[str], expected: str):
     expected_lines = [x.rstrip() for x in expected.splitlines() if x.rstrip()]
     actual_lines = [x.rstrip() for x in rich_capture if x.rstrip()]
     assert actual_lines, "No output."
     output = "\n".join(actual_lines)
```

