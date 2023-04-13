# Comparing `tmp/ape-foundry-0.6.6.tar.gz` & `tmp/ape-foundry-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-foundry-0.6.6.tar", last modified: Tue Apr 11 14:47:15 2023, max compression
+gzip compressed data, was "ape-foundry-0.6.7.tar", last modified: Thu Apr 13 22:24:43 2023, max compression
```

## Comparing `ape-foundry-0.6.6.tar` & `ape-foundry-0.6.7.tar`

### file list

```diff
@@ -1,129 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-11 14:47:15.397011 ape-foundry-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/ape_foundry/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26360 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/ape_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 14:47:15.397011 ape-foundry-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.389011 ape-foundry-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.389011 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/ape_foundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.667888 ape-foundry-0.6.7/ape_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.667888 ape-foundry-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.667888 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_trace.py
```

### Comparing `ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/bug.md` & `ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/feature.md` & `ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/work-item.md` & `ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/release-drafter.yml` & `ape-foundry-0.6.7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/workflows/codeql.yml` & `ape-foundry-0.6.7/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/workflows/commitlint.yaml` & `ape-foundry-0.6.7/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/workflows/prtitle.yaml` & `ape-foundry-0.6.7/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/workflows/publish.yaml` & `ape-foundry-0.6.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/workflows/stale-prs.yml` & `ape-foundry-0.6.7/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.github/workflows/test.yaml` & `ape-foundry-0.6.7/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.gitignore` & `ape-foundry-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/.pre-commit-config.yaml` & `ape-foundry-0.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/CONTRIBUTING.md` & `ape-foundry-0.6.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/LICENSE` & `ape-foundry-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/PKG-INFO` & `ape-foundry-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.6.6
+Version: 0.6.7
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-foundry-0.6.6/README.md` & `ape-foundry-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/ape_foundry/__init__.py` & `ape-foundry-0.6.7/ape_foundry/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/ape_foundry/constants.py` & `ape-foundry-0.6.7/ape_foundry/constants.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/ape_foundry/exceptions.py` & `ape-foundry-0.6.7/ape_foundry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/ape_foundry/provider.py` & `ape-foundry-0.6.7/ape_foundry/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 import shutil
 from bisect import bisect_right
 from copy import copy
+from itertools import tee
 from pathlib import Path
 from subprocess import PIPE, call
-from typing import Any, Dict, Iterator, List, Literal, Optional, Union, cast
+from typing import Any, Dict, Iterator, List, Literal, Optional, Tuple, Union, cast
 
 from ape.api import (
     BlockAPI,
     PluginConfig,
     ReceiptAPI,
     SubprocessProvider,
     TestProviderAPI,
@@ -31,14 +32,15 @@
 from eth_typing import HexStr
 from eth_utils import add_0x_prefix, is_0x_prefixed, is_hex, to_checksum_address, to_hex
 from evm_trace import CallType, ParityTraceList
 from evm_trace import TraceFrame as EvmTraceFrame
 from evm_trace import get_calltree_from_geth_trace, get_calltree_from_parity_trace
 from hexbytes import HexBytes
 from web3 import HTTPProvider, Web3
+from web3.exceptions import ContractLogicError as Web3ContractLogicError
 from web3.exceptions import ExtraDataLengthError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 from web3.middleware import geth_poa_middleware
 from web3.middleware.validation import MAX_EXTRADATA_LENGTH
 from web3.types import TxParams
 
 from ape_foundry.constants import EVM_VERSION_BY_NETWORK
@@ -426,17 +428,15 @@
 
         # The user is requesting information related to a call's trace,
         # such as gas usage data.
 
         if "type" in arguments[0] and isinstance(arguments[0]["type"], int):
             arguments[0]["type"] = to_hex(arguments[0]["type"])
 
-        result = self._make_request("debug_traceCall", arguments)
-        trace_data = result.get("structLogs", [])
-        trace_frames = (EvmTraceFrame(**f) for f in trace_data)
+        result, trace_frames = self._trace_call(arguments)
         return_value = HexBytes(result["returnValue"])
         root_node_kwargs = {
             "gas_cost": result.get("gas", 0),
             "address": txn.receiver,
             "calldata": txn.data,
             "value": txn.value,
             "call_type": CallType.CALL,
@@ -467,14 +467,19 @@
 
         if show_trace:
             call_tree = call_tree.enrich(use_symbol_for_tokens=True)
             self.chain_manager._reports.show_trace(call_tree)
 
         return return_value
 
+    def _trace_call(self, arguments: List[Any]) -> Tuple[Dict, Iterator[EvmTraceFrame]]:
+        result = self._make_request("debug_traceCall", arguments)
+        trace_data = result.get("structLogs", [])
+        return result, (EvmTraceFrame(**f) for f in trace_data)
+
     def get_balance(self, address: str) -> int:
         if hasattr(address, "address"):
             address = address.address
 
         result = self._make_request("eth_getBalance", [address, "latest"])
         if not result:
             raise ProviderError(f"Failed to get balance for account '{address}'.")
@@ -482,15 +487,17 @@
         return int(result, 16) if isinstance(result, str) else result
 
     def get_transaction_trace(self, txn_hash: str) -> Iterator[TraceFrame]:
         for trace in self._get_transaction_trace(txn_hash):
             yield self._create_trace_frame(trace)
 
     def _get_transaction_trace(self, txn_hash: str) -> Iterator[EvmTraceFrame]:
-        result = self._make_request("debug_traceTransaction", [txn_hash, {"stepsTracing": True}])
+        result = self._make_request(
+            "debug_traceTransaction", [txn_hash, {"stepsTracing": True, "enableMemory": True}]
+        )
         frames = result.get("structLogs", [])
         for frame in frames:
             yield EvmTraceFrame(**frame)
 
     def get_call_tree(self, txn_hash: str) -> CallTreeNode:
         raw_trace_list = self._make_request("trace_transaction", [txn_hash])
         trace_list = ParityTraceList.parse_obj(raw_trace_list)
@@ -498,46 +505,69 @@
         if not trace_list:
             raise ProviderError(f"No trace found for transaction '{txn_hash}'")
 
         evm_call = get_calltree_from_parity_trace(trace_list)
         return self._create_call_tree_node(evm_call, txn_hash=txn_hash)
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
-        txn = kwargs.get("txn")
         if not len(exception.args):
-            return VirtualMachineError(base_err=exception, txn=txn)
+            return VirtualMachineError(base_err=exception, **kwargs)
 
         err_data = exception.args[0]
         message = str(err_data.get("message")) if isinstance(err_data, dict) else err_data
 
         if not message:
-            return VirtualMachineError(base_err=exception, txn=txn)
+            return VirtualMachineError(base_err=exception, **kwargs)
 
         # Handle `ContactLogicError` similarly to other providers in `ape`.
         # by stripping off the unnecessary prefix that foundry has on reverts.
         foundry_prefix = (
             "Error: VM Exception while processing transaction: reverted with reason string "
         )
         if message.startswith(foundry_prefix):
             message = message.replace(foundry_prefix, "").strip("'")
-            return ContractLogicError(revert_message=message, txn=txn)
+            err = ContractLogicError(revert_message=message, **kwargs)
+            return self.compiler_manager.enrich_error(err)
+
+        elif "Transaction reverted without a reason string" in message:
+            err = ContractLogicError(**kwargs)
+            return self.compiler_manager.enrich_error(err)
+
+        elif message.lower() == "execution reverted":
+            err = ContractLogicError(**kwargs)
+
+            if isinstance(exception, Web3ContractLogicError):
+                # Check for custom error.
+                data = {}
+                if "trace" in kwargs:
+                    kwargs["trace"], new_trace = tee(kwargs["trace"])
+                    data = list(new_trace)[-1].raw
+
+                elif "txn" in kwargs:
+                    try:
+                        txn_hash = kwargs["txn"].txn_hash.hex()
+                        data = list(self.get_transaction_trace(txn_hash))[-1].raw
+                    except Exception:
+                        pass
+
+                if data.get("op") == "REVERT":
+                    custom_err = "".join([x[2:] for x in data["memory"][4:]])
+                    if custom_err:
+                        err.message = f"0x{custom_err}"
 
-        elif (
-            "Transaction reverted without a reason string" in message
-            or message.lower() == "execution reverted"
-        ):
-            return ContractLogicError(txn=txn)
+            return self.compiler_manager.enrich_error(err)
 
         elif message == "Transaction ran out of gas":
-            return OutOfGasError(txn=txn)
+            return OutOfGasError(**kwargs)
 
         elif message.startswith("execution reverted: "):
-            return ContractLogicError(message.replace("execution reverted: ", "").strip(), txn=txn)
+            err = ContractLogicError(message.replace("execution reverted: ", "").strip(), **kwargs)
+            return self.compiler_manager.enrich_error(err)
 
-        return VirtualMachineError(message, txn=txn)
+        return VirtualMachineError(message, **kwargs)
 
     def set_block_gas_limit(self, gas_limit: int) -> bool:
         return self._make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
 
     def set_code(self, address: AddressType, code: ContractCode) -> bool:
         if isinstance(code, bytes):
             code = code.hex()
@@ -560,15 +590,19 @@
 
         txn_dict.pop("chainId", None)
         arguments[0] = txn_dict
 
         try:
             result = self._make_request("eth_call", arguments)
         except Exception as err:
-            raise self.get_virtual_machine_error(err) from err
+            trace = (self._create_trace_frame(x) for x in self._trace_call(arguments)[1])
+            contract_address = arguments[0]["to"]
+            raise self.get_virtual_machine_error(
+                err, trace=trace, contract_address=contract_address
+            ) from err
 
         return HexBytes(result)
 
 
 class FoundryForkProvider(FoundryProvider):
     """
     A Foundry provider that uses ``--fork``, like:
```

### Comparing `ape-foundry-0.6.6/ape_foundry.egg-info/PKG-INFO` & `ape-foundry-0.6.7/ape_foundry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.6.6
+Version: 0.6.7
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-foundry-0.6.6/ape_foundry.egg-info/SOURCES.txt` & `ape-foundry-0.6.7/ape_foundry.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 tests/test_fork_provider.py
 tests/test_gas_report.py
 tests/test_provider.py
 tests/test_trace.py
 tests/data/contracts/ethereum/local/contract_a.json
 tests/data/contracts/ethereum/local/contract_b.json
 tests/data/contracts/ethereum/local/contract_c.json
+tests/data/contracts/ethereum/local/has_error.json
+tests/data/contracts/ethereum/local/reverts_contract.json
 tests/data/contracts/ethereum/local/solidity_contract.json
 tests/data/contracts/ethereum/local/token_a.json
 tests/data/contracts/ethereum/local/token_b.json
 tests/data/contracts/ethereum/local/vyper_contract.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
@@ -105,9 +107,11 @@
 tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
 tests/data/python/pytest_test_conftest.py
 tests/data/python/pytest_tests.py
+tests/data/sources/HasError.sol
+tests/data/sources/RevertsContractVy.vy
 tests/data/sources/TokenA.vy
 tests/data/sources/TokenB.vy
```

### Comparing `ape-foundry-0.6.6/ape_foundry.egg-info/requires.txt` & `ape-foundry-0.6.7/ape_foundry.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-eth-ape<0.7,>=0.6.7
-evm-trace>=0.1.0a13
+eth-ape<0.7,>=0.6.8
+evm-trace
 hexbytes
 web3
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
```

### Comparing `ape-foundry-0.6.6/pyproject.toml` & `ape-foundry-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/setup.py` & `ape-foundry-0.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-foundry",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.7,<0.7",
-        "evm-trace>=0.1.0a13",
+        "eth-ape>=0.6.8,<0.7",
+        "evm-trace",  # Use same version as eth-ape
         "hexbytes",  # Use same version as eth-ape
         "web3",  # Use same version as eth-ape
     ],
     python_requires=">=3.8,<3.11",
     extras_require=extras_require,
     py_modules=["ape_foundry"],
     license="Apache-2.0",
```

### Comparing `ape-foundry-0.6.6/tests/ape-config.yaml` & `ape-foundry-0.6.7/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/conftest.py` & `ape-foundry-0.6.7/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from ape_foundry import FoundryProvider
 
 # NOTE: Ensure that we don't use local paths for the DATA FOLDER
 ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "data" / "contracts"
+LOCAL_CONTRACTS_PATH = BASE_CONTRACTS_PATH / "ethereum" / "local"
 NAME = "foundry"
 
 # Needed to test tracing support in core `ape test` command.
 pytest_plugins = ["pytester"]
 MAINNET_FORK_PORT = 9001
 GOERLI_FORK_PORT = 9002
 
@@ -107,35 +108,55 @@
 
 
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
+@pytest.fixture
+def reverts_contract(owner):
+    path = LOCAL_CONTRACTS_PATH / "reverts_contract.json"
+    return owner.deploy(ContractContainer(ContractType.parse_file(path)))
+
+
 @pytest.fixture(scope="session")
 def sender(accounts):
     return accounts[0]
 
 
 @pytest.fixture(scope="session")
 def receiver(accounts):
@@ -144,14 +165,19 @@
 
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

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_a.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_b.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_c.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_a.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_b.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/python/pytest_tests.py` & `ape-foundry-0.6.7/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/sources/TokenA.vy` & `ape-foundry-0.6.7/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/data/sources/TokenB.vy` & `ape-foundry-0.6.7/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/expected_traces.py` & `ape-foundry-0.6.7/tests/expected_traces.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,86 @@
 LOCAL_TRACE = r"""
-Call trace for
-'0x([A-Fa-f0-9]{64})'
+Call trace for '0x([A-Fa-f0-9]{64})'
 tx\.origin=0x[a-fA-F0-9]{40}
 ContractA\.methodWithoutArguments\(\) -> 0x00..5174 \[\d+ gas\]
 ├── SYMBOL\.methodB1\(lolol="ice-cream", dynamo=36\) \[\d+ gas\]
 │   ├── ContractC\.getSomeList\(\) -> \[
 │   │     3425311345134513461345134534531452345,
 │   │     111344445534535353,
 │   │     993453434534534534534977788884443333
 │   │   \] \[\d+ gas\]
-│   └── ContractC\.methodC1\(windows95="simpler", jamaica=36, cardinal=ContractA\)
-│       \[\d+ gas\]
+│   └── ContractC\.methodC1\(windows95="simpler", jamaica=36, cardinal=ContractA\) \[\d+ gas\]
 ├── SYMBOL\.callMe\(blue=tx.origin\) -> tx\.origin \[\d+ gas\]
 ├── SYMBOL\.methodB2\(trombone=tx.origin\) \[\d+ gas\]
-│   ├── ContractC\.paperwork\(ContractA\) -> \(os="simpler", country=36,
-│   │   wings=ContractA\) \[\d+ gas\]
-│   ├── ContractC\.methodC1\(windows95="simpler", jamaica=0, cardinal=ContractC\)
-│   │   \[\d+ gas\]
+│   ├── ContractC\.paperwork\(ContractA\) -> \(os="simpler", country=36, wings=ContractA\) \[\d+ gas\]
+│   ├── ContractC\.methodC1\(windows95="simpler", jamaica=0, cardinal=ContractC\) \[\d+ gas\]
 │   ├── ContractC\.methodC2\(\) \[\d+ gas\]
 │   └── ContractC\.methodC2\(\) \[\d+ gas\]
 ├── ContractC\.addressToValue\(tx\.origin\) -> 0 \[\d+ gas\]
 ├── SYMBOL\.bandPractice\(tx\.origin\) -> 0 \[\d+ gas\]
 ├── SYMBOL\.methodB1\(lolol="lemondrop", dynamo=0\) \[\d+ gas\]
 │   ├── ContractC\.getSomeList\(\) -> \[
 │   │     3425311345134513461345134534531452345,
 │   │     111344445534535353,
 │   │     993453434534534534534977788884443333
 │   │   \] \[\d+ gas\]
-│   └── ContractC.methodC1\(windows95="simpler", jamaica=0, cardinal=ContractA\)
-│       \[\d+ gas\]
+│   └── ContractC.methodC1\(windows95="simpler", jamaica=0, cardinal=ContractA\) \[\d+ gas\]
 └── SYMBOL\.methodB1\(lolol="snitches_get_stiches", dynamo=111\) \[\d+ gas\]
     ├── ContractC\.getSomeList\(\) -> \[
     │     3425311345134513461345134534531452345,
     │     111344445534535353,
     │     993453434534534534534977788884443333
     │   \] \[\d+ gas\]
-    └── ContractC\.methodC1\(windows95="simpler", jamaica=111, cardinal=ContractA\)
-        \[\d+ gas\]
+    └── ContractC\.methodC1\(windows95="simpler", jamaica=111, cardinal=ContractA\) \[\d+ gas\]
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
     5789604461865809771178549250512551984713807685540901737341300416798777562476
 """
 MAINNET_FAIL_TRACE_LAST_10_LINES = r"""
+    ├── AggregationRouterV4\.uniswapV3SwapCallback\(
     │     amount0Delta=-4192051335,
     │     amount1Delta=2098831888913057968,
     │     0x00\.\.097d
     │   \) \[9861 gas\]
     │   ├── UniswapV3Pool.token0\(\) -> FiatTokenProxy \[266 gas\]
     │   ├── UniswapV3Pool\.token1\(\) -> WETH \[308 gas\]
     │   ├── UniswapV3Pool\.fee\(\) -> 500 \[251 gas\]
-    │   └── WETH\.transfer\(dst=UniswapV3Pool, wad=2098831888913057968\) -> True
-    │       \[6062 gas\]
+    │   └── WETH\.transfer\(dst=UniswapV3Pool, wad=2098831888913057968\) -> True \[6062 gas\]
     └── WETH\.balanceOf\(UniswapV3Pool\) -> 68359883632315875514968 \[534 gas\]
 """
 MAINNET_TRACE_FIRST_10_LINES = r"""
-Call trace for
-'0xb7d7f1d5ce7743e821d3026647df486f517946ef1342a1ae93c96e4a8016eab7'
+Call trace for '0xb7d7f1d5ce7743e821d3026647df486f517946ef1342a1ae93c96e4a8016eab7'
 tx\.origin=0x5668EAd1eDB8E2a4d724C8fb9cB5fFEabEB422dc
 DSProxy\.execute\(_target=LoanShifterTaker, _data=0x35\.\.0000\) -> "" \[\d+ gas\]
 └── \(delegate\) LoanShifterTaker\.moveLoan\(
       _exchangeData=\[
         0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE,
         ZERO_ADDRESS,
         0,
         0,
 """
 MAINNET_TRACE_LAST_10_LINES = r"""
+    │                   └── LendingRateOracle\.getMarketBorrowRate\(_asset=DAI\) ->
     │                       35000000000000000000000000 \[1164 gas\]
     ├── DSProxy\.authority\(\) -> DSGuard \[1291 gas\]
-    ├── DSGuard\.forbid\(src=LoanShifterReceiver, dst=DSProxy, sig=0x1c\.\.0000\)
-    │   \[5253 gas\]
+    ├── DSGuard\.forbid\(src=LoanShifterReceiver, dst=DSProxy, sig=0x1c\.\.0000\) \[5253 gas\]
     └── DefisaverLogger\.Log\(
           _contract=DSProxy,
           _caller=tx\.origin,
           _logName="LoanShifter",
           _data=0x00\.\.0000
-        \)
+        \) \[6057 gas\]
 """
 LOCAL_GAS_REPORT = r"""
  +ContractA Gas
 
   Method +Times called +Min. +Max. +Mean +Median
  ─+
   methodWithoutArguments +1 +\d+ +\d+ +\d+ + \d+
```

### Comparing `ape-foundry-0.6.6/tests/test_fork_provider.py` & `ape-foundry-0.6.7/tests/test_fork_provider.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/test_gas_report.py` & `ape-foundry-0.6.7/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.6/tests/test_provider.py` & `ape-foundry-0.6.7/tests/test_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import tempfile
 from pathlib import Path
 
 import pytest
 from ape.exceptions import ContractLogicError
+from ape.pytest.contextmanagers import RevertsContextManager as reverts
 from ape.types import CallTreeNode, TraceFrame
 from evm_trace import CallType
 from hexbytes import HexBytes
 
 from ape_foundry.exceptions import FoundryProviderError
 from ape_foundry.provider import FOUNDRY_CHAIN_ID
 
@@ -138,14 +139,27 @@
 
 def test_revert(sender, contract_instance):
     # 'sender' is not the owner so it will revert (with a message)
     with pytest.raises(ContractLogicError, match="!authorized"):
         contract_instance.setNumber(6, sender=sender)
 
 
+def test_revert_dev_string_check(sender, reverts_contract):
+    with reverts(dev_message="dev: one"):
+        reverts_contract.revertStrings(1, sender=sender)
+
+    with reverts(dev_message="dev: error"):
+        reverts_contract.revertStrings(2, sender=sender)
+
+
+def test_revert_dev_string_check_call(sender, reverts_contract):
+    with reverts(dev_message="dev: one"):
+        reverts_contract.revertStringsCall(1)
+
+
 def test_contract_revert_no_message(owner, contract_instance):
     # The Contract raises empty revert when setting number to 5.
     with pytest.raises(ContractLogicError, match="Transaction failed."):
         contract_instance.setNumber(5, sender=owner)
 
 
 def test_transaction_contract_as_sender(
@@ -186,7 +200,15 @@
 
 def test_get_receipt(connected_provider, contract_instance, owner):
     receipt = contract_instance.setAddress(owner.address, sender=owner)
     actual = connected_provider.get_receipt(receipt.txn_hash)
     assert receipt.txn_hash == actual.txn_hash
     assert actual.receiver == contract_instance.address
     assert actual.sender == receipt.sender
+
+
+def test_revert_error(error_contract, not_owner):
+    """
+    Test matching a revert custom Solidity error.
+    """
+    with pytest.raises(error_contract.Unauthorized):
+        error_contract.withdraw(sender=not_owner)
```

### Comparing `ape-foundry-0.6.6/tests/test_trace.py` & `ape-foundry-0.6.7/tests/test_trace.py`

 * *Files 17% similar despite different names*

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
 
@@ -75,45 +76,64 @@
     return contract_a.methodWithoutArguments(sender=owner)
 
 
 def test_local_transaction_traces(local_receipt, captrace):
     # NOTE: Strange bug in Rich where we can't use sys.stdout for testing tree output.
     # And we have to write to a file, close it, and then re-open it to see output.
     def run_test():
-        local_receipt.show_trace()
-        lines = captrace.read_trace("Call trace for")
-        assert_rich_output(lines, LOCAL_TRACE)
+        with tempfile.TemporaryDirectory() as temp_dir:
+            # Use a tempfile to avoid terminal inconsistencies affecting output.
+            file_path = Path(temp_dir) / "temp"
+            with open(file_path, "w") as file:
+                local_receipt.show_trace(file=file)
+
+            with open(file_path, "r") as file:
+                lines = captrace.read_trace("Call trace for", file=file)
+                assert_rich_output(lines, LOCAL_TRACE)
 
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

