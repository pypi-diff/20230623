# Comparing `tmp/ape-foundry-0.6.8.tar.gz` & `tmp/ape-foundry-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-foundry-0.6.8.tar", last modified: Thu May 18 18:15:26 2023, max compression
+gzip compressed data, was "ape-foundry-0.6.9.tar", last modified: Tue Jun 13 15:26:33 2023, max compression
```

## Comparing `ape-foundry-0.6.8.tar` & `ape-foundry-0.6.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/ape_foundry/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.405429 ape-foundry-0.6.8/ape_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.405429 ape-foundry-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.405429 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/reverts_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.409430 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/RevertsContractVy.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.897358 ape-foundry-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.885358 ape-foundry-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.885358 ape-foundry-0.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.889358 ape-foundry-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-13 15:26:33.897358 ape-foundry-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.889358 ape-foundry-0.6.9/ape_foundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/ape_foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/ape_foundry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/ape_foundry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31693 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/ape_foundry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/ape_foundry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 15:26:33.000000 ape-foundry-0.6.9/ape_foundry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.889358 ape-foundry-0.6.9/ape_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-13 15:26:33.000000 ape-foundry-0.6.9/ape_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-13 15:26:33.000000 ape-foundry-0.6.9/ape_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:26:33.000000 ape-foundry-0.6.9/ape_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:26:33.000000 ape-foundry-0.6.9/ape_foundry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-13 15:26:33.000000 ape-foundry-0.6.9/ape_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 15:26:33.000000 ape-foundry-0.6.9/ape_foundry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 15:26:33.897358 ape-foundry-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.889358 ape-foundry-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.885358 ape-foundry-0.6.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.885358 ape-foundry-0.6.9/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.885358 ape-foundry-0.6.9/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.889358 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.885358 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.897358 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.897358 ape-foundry-0.6.9/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:26:33.897358 ape-foundry-0.6.9/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-13 15:25:31.000000 ape-foundry-0.6.9/tests/test_trace.py
```

### Comparing `ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/bug.md` & `ape-foundry-0.6.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/feature.md` & `ape-foundry-0.6.9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/work-item.md` & `ape-foundry-0.6.9/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/.github/release-drafter.yml` & `ape-foundry-0.6.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/.github/workflows/codeql.yml` & `ape-foundry-0.6.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/.github/workflows/commitlint.yaml` & `ape-foundry-0.6.9/.github/workflows/commitlint.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-foundry-0.6.8/.github/workflows/prtitle.yaml` & `ape-foundry-0.6.9/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-foundry-0.6.8/.github/workflows/publish.yaml` & `ape-foundry-0.6.9/.github/workflows/publish.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
 
     - name: Build
```

### Comparing `ape-foundry-0.6.8/.github/workflows/stale-prs.yml` & `ape-foundry-0.6.9/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/.github/workflows/test.yaml` & `ape-foundry-0.6.9/.github/workflows/test.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Install Foundry
           uses: foundry-rs/foundry-toolchain@v1
           with:
@@ -103,14 +103,14 @@
 #
 #        steps:
 #        - uses: actions/checkout@v3
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v4
 #          with:
-#              python-version: 3.8
+#              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-foundry-0.6.8/.gitignore` & `ape-foundry-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/.pre-commit-config.yaml` & `ape-foundry-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/CONTRIBUTING.md` & `ape-foundry-0.6.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/LICENSE` & `ape-foundry-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/README.md` & `ape-foundry-0.6.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 Foundry network provider plugin for Ape.
 Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
@@ -71,15 +71,14 @@
 
 ```yaml
 foundry:
   fork:
     ethereum:
       mainnet:
         upstream_provider: alchemy
-
 ```
 
 Otherwise, it defaults to the default mainnet provider plugin.
 You can also specify a `block_number` and `evm_version`.
 
 If the block number is specified, but no EVM version is specified, it is automatically set based on the block height for known networks.
 
@@ -95,7 +94,43 @@
 
 ```yaml
 foundry:
   host: https://anvil.example.com
 ```
 
 Now, instead of launching a local process, it will attempt to connect to the remote anvil node and use this plugin as the ape interface.
+
+## Impersonate Accounts
+
+You can impersonate accounts using the `ape-foundry` plugin.
+To impersonate an account, do the following:
+
+```python
+import pytest
+
+@pytest.fixture
+def whale(accounts):
+    return accounts["example.eth"]
+```
+
+To transact, your impersonated account must have a balance.
+You can achieve this by using a forked network and impersonating an account with a balance.
+Alternatively, you can set your node's base fee and priority fee to `0`.
+
+To programtically set an account's balance, do the following:
+
+```python
+from ape import accounts
+
+account = accounts["example.eth"]
+account.balance = "1000 ETH"  # This calls `anvil_setBalance` under-the-hood.
+```
+
+## Base Fee and Priority Fee
+
+Configure your node's base fee and priority fee using the `ape-config.yaml` file.
+
+```yaml
+foundry:
+  base_fee: 0
+  priority_fee: 0
+```
```

### Comparing `ape-foundry-0.6.8/ape_foundry/__init__.py` & `ape-foundry-0.6.9/ape_foundry/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/ape_foundry/constants.py` & `ape-foundry-0.6.9/ape_foundry/constants.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/ape_foundry/exceptions.py` & `ape-foundry-0.6.9/ape_foundry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/ape_foundry/provider.py` & `ape-foundry-0.6.9/ape_foundry/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,18 @@
     """
 
     # Retry strategy configs, try increasing these if you're getting FoundrySubprocessError
     request_timeout: int = 30
     fork_request_timeout: int = 300
     process_attempts: int = 0
 
+    # RPC defaults
+    base_fee: int = 0
+    priority_fee: int = 0
+
     # For setting the values in --fork and --fork-block-number command arguments.
     # Used only in FoundryForkProvider.
     # Mapping of ecosystem_name => network_name => FoundryForkConfig
     fork: Dict[str, Dict[str, FoundryForkConfig]] = {}
 
     class Config:
         extra = "allow"
@@ -102,14 +106,18 @@
         return list(self.account_manager.test_accounts._impersonated_accounts)
 
     @property
     def mnemonic(self) -> str:
         return self._test_config.mnemonic
 
     @property
+    def base_fee(self) -> int:
+        return self.config.base_fee
+
+    @property
     def number_of_accounts(self) -> int:
         return self._test_config.number_of_accounts
 
     @property
     def process_name(self) -> str:
         return "anvil"
 
@@ -159,29 +167,33 @@
         if self._host is None:
             self._host = self.config.host or f"http://127.0.0.1:{DEFAULT_PORT}"
 
         return self._host
 
     @property
     def priority_fee(self) -> int:
-        return self.conversion_manager.convert("2 gwei", int)
+        return self.config.priority_fee
 
     @property
     def is_connected(self) -> bool:
         if self._host in ("auto", None):
             # Hasn't tried yet.
             return False
 
         self._set_web3()
         return self._web3 is not None
 
     @cached_property
     def _test_config(self) -> TestConfig:
         return cast(TestConfig, self.config_manager.get_config("test"))
 
+    @property
+    def auto_mine(self) -> bool:
+        return self._make_request("anvil_getAutomine", [])
+
     def connect(self):
         """
         Start the foundry process and verify it's up and accepting connections.
         **NOTE**: Must set port before calling 'super().connect()'.
         """
 
         warning = "`port` setting is deprecated. Please use `host` key that includes the port."
@@ -351,14 +363,16 @@
             "--mnemonic",
             self.mnemonic,
             "--accounts",
             f"{self.number_of_accounts}",
             "--derivation-path",
             "m/44'/60'/0'",
             "--steps-tracing",
+            "--block-base-fee-per-gas",
+            f"{self.config.base_fee}",
         ]
 
     def set_balance(self, account: AddressType, amount: Union[int, float, str, bytes]):
         is_str = isinstance(amount, str)
         _is_hex = False if not is_str else is_0x_prefixed(str(amount))
         is_key_word = is_str and len(str(amount).split(" ")) > 1
         if is_key_word:
@@ -394,14 +408,19 @@
         result = self._make_request("evm_revert", [snapshot_id])
         return result is True
 
     def unlock_account(self, address: AddressType) -> bool:
         self._make_request("anvil_impersonateAccount", [address])
         return True
 
+    def relock_account(self, address: AddressType):
+        self._make_request("anvil_stopImpersonatingAccount", [address])
+        if address in self.account_manager.test_accounts._impersonated_accounts:
+            del self.account_manager.test_accounts._impersonated_accounts[address]
+
     def send_transaction(self, txn: TransactionAPI) -> ReceiptAPI:
         """
         Creates a new message call transaction or a contract creation
         for signed transactions.
         """
         sender = txn.sender
         if sender:
@@ -411,41 +430,46 @@
             # Allow for an unsigned transaction
             sender = cast(AddressType, sender)  # We know it's checksummed at this point.
             txn = self.prepare_transaction(txn)
             original_code = HexBytes(self.get_code(sender))
             if original_code:
                 self.set_code(sender, "")
 
-            try:
-                txn_dict = txn.dict()
-                if isinstance(txn_dict.get("type"), int):
-                    txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
+            txn_dict = txn.dict()
+            if isinstance(txn_dict.get("type"), int):
+                txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
 
-                tx_params = cast(TxParams, txn_dict)
+            tx_params = cast(TxParams, txn_dict)
+            try:
                 txn_hash = self.web3.eth.send_transaction(tx_params)
-
             except ValueError as err:
-                raise self.get_virtual_machine_error(err) from err
+                raise self.get_virtual_machine_error(err, txn=txn) from err
+
             finally:
                 if original_code:
                     self.set_code(sender, original_code.hex())
         else:
             try:
                 txn_hash = self.web3.eth.send_raw_transaction(txn.serialize_transaction())
             except ValueError as err:
                 vm_err = self.get_virtual_machine_error(err, txn=txn)
 
                 if "nonce too low" in str(vm_err):
                     # Add additional nonce information
                     new_err_msg = f"Nonce '{txn.nonce}' is too low"
                     raise VirtualMachineError(
-                        new_err_msg, base_err=vm_err.base_err, code=vm_err.code
+                        new_err_msg,
+                        base_err=vm_err.base_err,
+                        code=vm_err.code,
+                        txn=txn,
+                        source_traceback=vm_err.source_traceback,
+                        trace=vm_err.trace,
+                        contract_address=vm_err.contract_address,
                     )
 
-                vm_err.txn = txn
                 raise vm_err from err
 
         receipt = self.get_receipt(
             txn_hash.hex(),
             required_confirmations=(
                 txn.required_confirmations
                 if txn.required_confirmations is not None
@@ -464,16 +488,15 @@
             # NOTE: For some reason, `nonce` can't be in the txn params or else it fails.
             if "nonce" in txn_params:
                 del txn_params["nonce"]
 
             try:
                 self.web3.eth.call(txn_params)
             except Exception as err:
-                vm_err = self.get_virtual_machine_error(err, txn=txn)
-                vm_err.txn = txn
+                vm_err = self.get_virtual_machine_error(err, txn=receipt)
                 raise vm_err from err
 
         logger.info(f"Confirmed {receipt.txn_hash} (total fees paid = {receipt.total_fees_paid})")
         self.chain_manager.history.append(receipt)
         return receipt
 
     def send_call(self, txn: TransactionAPI, **kwargs: Any) -> bytes:
@@ -617,15 +640,15 @@
                 if data.get("op") == "REVERT":
                     custom_err = "".join([x[2:] for x in data["memory"][4:]])
                     if custom_err:
                         err.message = f"0x{custom_err}"
 
             return self.compiler_manager.enrich_error(err)
 
-        elif message == "Transaction ran out of gas":
+        elif message == "Transaction ran out of gas" or "OutOfGas" in message:
             return OutOfGasError(**kwargs)
 
         elif message.startswith("execution reverted: "):
             err = ContractLogicError(message.replace("execution reverted: ", "").strip(), **kwargs)
             return self.compiler_manager.enrich_error(err)
 
         elif isinstance(exception, ContractCustomError):
```

### Comparing `ape-foundry-0.6.8/ape_foundry.egg-info/SOURCES.txt` & `ape-foundry-0.6.9/ape_foundry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/ape_foundry.egg-info/requires.txt` & `ape-foundry-0.6.9/ape_foundry.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/pyproject.toml` & `ape-foundry-0.6.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-foundry-0.6.8/setup.py` & `ape-foundry-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,9 +90,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_a.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_b.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_c.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/has_error.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/reverts_contract.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/reverts_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_a.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_b.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-foundry-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/python/pytest_tests.py` & `ape-foundry-0.6.9/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/sources/RevertsContractVy.vy` & `ape-foundry-0.6.9/tests/data/sources/RevertsContractVy.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/sources/TokenA.vy` & `ape-foundry-0.6.9/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/data/sources/TokenB.vy` & `ape-foundry-0.6.9/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/expected_traces.py` & `ape-foundry-0.6.9/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/test_fork_provider.py` & `ape-foundry-0.6.9/tests/test_fork_provider.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/test_gas_report.py` & `ape-foundry-0.6.9/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.8/tests/test_provider.py` & `ape-foundry-0.6.9/tests/test_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tempfile
 from pathlib import Path
 
 import pytest
+from ape.api.accounts import ImpersonatedAccount
 from ape.exceptions import ContractLogicError
 from ape.pytest.contextmanagers import RevertsContextManager as reverts
 from ape.types import CallTreeNode, TraceFrame
 from evm_trace import CallType
 from hexbytes import HexBytes
 
 from ape_foundry.provider import FOUNDRY_CHAIN_ID
@@ -86,18 +87,29 @@
 
     connected_provider.revert(snap)
     block_3 = connected_provider.get_block("latest")
     assert block_1.number == block_3.number
     assert block_1.hash == block_3.hash
 
 
-def test_unlock_account(connected_provider, accounts):
+def test_unlock_account(connected_provider, contract_a, accounts):
     actual = connected_provider.unlock_account(TEST_WALLET_ADDRESS)
     assert actual is True
 
+    # Tell Anvil we no longer want this unlocked.
+    connected_provider.relock_account(TEST_WALLET_ADDRESS)
+
+    # Unlock using the more public API.
+    acct = accounts[TEST_WALLET_ADDRESS]
+    assert isinstance(acct, ImpersonatedAccount)
+
+    # Ensure can transact.
+    receipt = contract_a.methodWithoutArguments(sender=acct)
+    assert not receipt.failed
+
 
 def test_get_transaction_trace(connected_provider, contract_instance, owner):
     receipt = contract_instance.setNumber(10, sender=owner)
 
     # Indirectly calls `connected_provider.get_transaction_trace()`
     frame_data = list(receipt.trace)
     assert frame_data
@@ -204,12 +216,31 @@
     """
     Test matching a revert custom Solidity error.
     """
     with pytest.raises(error_contract.Unauthorized):
         error_contract.withdraw(sender=not_owner)
 
 
+def test_revert_error_using_impersonated_account(error_contract, accounts, connected_provider):
+    """
+    Show that when a failure occurs when a txn is sent by an impersonated
+    account, that everything still works.
+    """
+    acct = accounts[TEST_WALLET_ADDRESS]
+    acct.balance = "1000 ETH"
+    with pytest.raises(error_contract.Unauthorized):
+        error_contract.withdraw(sender=acct)
+
+
 def test_host(temp_config, networks):
     data = {"foundry": {"host": "https://example.com"}}
     with temp_config(data):
         provider = networks.ethereum.local.get_provider("foundry")
         assert provider.uri == "https://example.com"
+
+
+def test_base_fee(connected_provider):
+    assert connected_provider.base_fee == 0
+
+
+def test_automine(connected_provider):
+    assert connected_provider.auto_mine is True
```

### Comparing `ape-foundry-0.6.8/tests/test_trace.py` & `ape-foundry-0.6.9/tests/test_trace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import re
 import shutil
 import tempfile
 from pathlib import Path
 from typing import List
 
 import pytest
-from ape.contracts import ContractContainer
-from ethpm_types import ContractType
 
 from .expected_traces import (
     LOCAL_GAS_REPORT,
     LOCAL_TRACE,
     MAINNET_FAIL_TRACE_FIRST_10_LINES,
     MAINNET_FAIL_TRACE_LAST_10_LINES,
     MAINNET_TRACE_FIRST_10_LINES,
@@ -52,30 +50,14 @@
     params=(MAINNET_TXN_HASH, MAINNET_FAIL_TXN_HASH),
 )
 def mainnet_receipt(request, mainnet_fork_provider):
     return mainnet_fork_provider.get_receipt(request.param)
 
 
 @pytest.fixture
-def contract_a(owner, connected_provider):
-    base_path = BASE_CONTRACTS_PATH / "local"
-
-    def get_contract_type(suffix: str) -> ContractType:
-        return ContractType.parse_file(base_path / f"contract_{suffix}.json")
-
-    contract_c = owner.deploy(ContractContainer(get_contract_type("c")))
-    contract_b = owner.deploy(ContractContainer(get_contract_type("b")), contract_c.address)
-    contract_a = owner.deploy(
-        ContractContainer(get_contract_type("a")), contract_b.address, contract_c.address
-    )
-
-    return contract_a
-
-
-@pytest.fixture
 def local_receipt(contract_a, owner):
     return contract_a.methodWithoutArguments(sender=owner)
 
 
 def test_local_transaction_traces(local_receipt, captrace):
     # NOTE: Strange bug in Rich where we can't use sys.stdout for testing tree output.
     # And we have to write to a file, close it, and then re-open it to see output.
```

