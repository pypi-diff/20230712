# Comparing `tmp/btclib-2023.5.30.tar.gz` & `tmp/btclib-2023.7.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btclib-2023.5.30.tar", last modified: Tue Jun 13 15:49:25 2023, max compression
+gzip compressed data, was "btclib-2023.7.12.tar", last modified: Wed Jul 12 13:36:26 2023, max compression
```

## Comparing `btclib-2023.5.30.tar` & `btclib-2023.7.12.tar`

### file list

```diff
@@ -1,260 +1,293 @@
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:25.001772 btclib-2023.5.30/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      741 2023-02-07 11:12:07.000000 btclib-2023.5.30/.flake8
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      485 2023-02-07 11:12:07.000000 btclib-2023.5.30/.markdownlint.jsonc
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4894 2023-06-13 15:45:45.000000 btclib-2023.5.30/.pre-commit-config.yaml
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1657 2023-02-07 11:12:07.000000 btclib-2023.5.30/.sourcery.yaml
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      303 2022-07-04 10:37:33.000000 btclib-2023.5.30/AUTHORS.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      207 2022-07-04 10:37:33.000000 btclib-2023.5.30/CODE_OF_CONDUCT.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5855 2023-02-07 11:12:07.000000 btclib-2023.5.30/CONTRIBUTING.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      341 2023-02-07 11:12:07.000000 btclib-2023.5.30/COPYRIGHT
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    11354 2023-06-13 15:39:58.000000 btclib-2023.5.30/HISTORY.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1108 2023-02-07 11:12:07.000000 btclib-2023.5.30/LICENSE
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      943 2023-02-07 11:12:07.000000 btclib-2023.5.30/MANIFEST.in
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    10316 2023-06-13 15:49:25.001772 btclib-2023.5.30/PKG-INFO
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     8530 2023-02-07 11:12:07.000000 btclib-2023.5.30/README.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1371 2023-02-07 11:12:07.000000 btclib-2023.5.30/RELEASE.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      187 2023-02-07 11:12:07.000000 btclib-2023.5.30/SECURITY.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1639 2023-06-13 15:39:52.000000 btclib-2023.5.30/TODO.md
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.889772 btclib-2023.5.30/btclib/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      621 2023-06-13 15:39:58.000000 btclib-2023.5.30/btclib/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.889772 btclib-2023.5.30/btclib/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/_data/mainnet.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      600 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/_data/regtest.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/_data/testnet.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3823 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/alias.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3901 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/amount.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     6291 2023-06-13 15:39:58.000000 btclib-2023.5.30/btclib/b32.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4567 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/b58.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4308 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/base58.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5727 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bech32.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/bip32/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1380 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/__init__.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    16582 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/bip32.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3737 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/der_path.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5735 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/key_origin.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3879 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/slip132.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/block/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      515 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/block/__init__.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4968 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/block/block.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     7448 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/block/block_header.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/ec/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1553 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/ec/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4102 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_Brainpool.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3105 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_NIST.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2403 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_SEC2v1_insecure.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4233 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_SEC2v2.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     8771 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    25244 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve_group.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     8183 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve_group_2.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1727 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve_group_f.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2495 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/libsecp256k1.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3069 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/sec_point.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/ecc/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      633 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/__init__.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3593 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/bip340_nonce.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    14412 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/bms.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     6124 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/borromean.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2615 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/dh.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    19859 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/dsa.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4291 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/libsecp256k1.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3272 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/pedersen.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4441 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/rfc6979_nonce.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4466 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/sign_to_contract.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    15087 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/ssa.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      795 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/exceptions.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3089 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/hashes.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/mnemonic/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1389 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/mnemonic/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    13116 2022-07-04 10:37:33.000000 btclib-2023.5.30/btclib/mnemonic/_data/english.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    16033 2022-07-04 10:37:33.000000 btclib-2023.5.30/btclib/mnemonic/_data/italian.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5312 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/bip39.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5430 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/electrum.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    11856 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/entropy.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4287 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/mnemonic.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     9348 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/network.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4972 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/number_theory.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/psbt/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1237 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/psbt/__init__.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    20538 2023-05-11 14:15:22.000000 btclib-2023.5.30/btclib/psbt/psbt.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    16086 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/psbt/psbt_in.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5294 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/psbt/psbt_out.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4837 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/psbt/psbt_utils.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       27 2022-07-04 10:37:33.000000 btclib-2023.5.30/btclib/py.typed
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.901772 btclib-2023.5.30/btclib/script/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1565 2023-06-13 15:39:58.000000 btclib-2023.5.30/btclib/script/__init__.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    11000 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/script.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    17561 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/script_pub_key.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     9678 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/sig_hash.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5270 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/script/taproot.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2305 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/witness.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     7024 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/to_prv_key.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     7908 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/to_pub_key.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.901772 btclib-2023.5.30/btclib/tx/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      597 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/__init__.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3263 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/out_point.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    10363 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/tx.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4582 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/tx_in.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4045 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/tx_out.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     6075 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/utils.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1237 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/var_bytes.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2702 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/var_int.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.889772 btclib-2023.5.30/btclib.egg-info/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    10316 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/PKG-INFO
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5778 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/SOURCES.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)        1 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/dependency_links.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       20 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/requires.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)        7 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/top_level.txt
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.901772 btclib-2023.5.30/docs/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      638 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/Makefile
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1777 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/README.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      804 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/make.bat
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       43 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/requirements.txt
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.909772 btclib-2023.5.30/docs/source/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      788 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.bip32.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      491 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.block.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1088 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.ec.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1647 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.ecc.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      823 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.mnemonic.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      772 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.psbt.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2325 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      972 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.script.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      721 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.tx.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2148 2023-06-13 15:39:58.000000 btclib-2023.5.30/docs/source/conf.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      157 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/contributing_link.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      105 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/history_link.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      508 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/index.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       55 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/modules.rst
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      151 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/readme_link.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      153 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/security_link.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1380 2023-02-07 11:12:07.000000 btclib-2023.5.30/pyproject.toml
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      318 2023-02-07 11:12:07.000000 btclib-2023.5.30/readthedocs.yml
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      299 2023-02-07 11:12:07.000000 btclib-2023.5.30/requirements-dev.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       41 2023-02-07 11:12:07.000000 btclib-2023.5.30/requirements.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       38 2023-06-13 15:49:25.001772 btclib-2023.5.30/setup.cfg
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2705 2023-02-07 11:12:07.000000 btclib-2023.5.30/setup.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.913772 btclib-2023.5.30/tests/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1036 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/README.md
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      405 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.913772 btclib-2023.5.30/tests/_generated_files/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/_generated_files/mainnet.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      600 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/_generated_files/regtest.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/_generated_files/testnet.json
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/bip32/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      411 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/bip32/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3151 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/_data/bip32_invalid_keys.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5515 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/_data/bip32_test_vectors.json
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/bip32/_generated_files/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       73 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/bip32/_generated_files/key_origin.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      625 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/_generated_files/key_paths.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    14054 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_bip32.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5027 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_der_path.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5185 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_key_origin.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     9595 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_slip132.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/block/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      411 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.925772 btclib-2023.5.30/tests/block/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      215 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_1.bin
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      490 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_170.bin
--rw-rw-r--   0 kappa     (1000) kappa     (1000)   247533 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_200000.bin
--rw-rw-r--   0 kappa     (1000) kappa     (1000)   988519 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_481824.bin
--rw-rw-r--   0 kappa     (1000) kappa     (1000)   989323 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_481824_complete.bin
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.945772 btclib-2023.5.30/tests/block/_generated_files/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)  5738930 2023-05-11 14:09:55.000000 btclib-2023.5.30/tests/block/_generated_files/block_481824.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      419 2023-05-11 14:09:55.000000 btclib-2023.5.30/tests/block/_generated_files/block_header_481824.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    10561 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/test_block.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.949772 btclib-2023.5.30/tests/ec/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      408 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.949772 btclib-2023.5.30/tests/ec/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)   126364 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/_data/pubkey.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    15648 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    15426 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve_group.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4271 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve_group_2.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2179 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve_group_f.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4813 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_sec_point.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.953772 btclib-2023.5.30/tests/ecc/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      409 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.957772 btclib-2023.5.30/tests/ecc/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5161 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/ecc/_data/bip340_test_vectors.csv
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    50597 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/bms.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    89766 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/ecdsa_custom_nonce_sig.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    72463 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/ecdsa_sig.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    31685 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/rfc6979.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    27857 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_bms.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1484 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_borromean.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3887 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_der.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    29798 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_dh.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    13268 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_dsa.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2002 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_pedersen.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2925 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_rfc6979.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1508 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_sign_to_contract.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    25964 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_ssa.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.957772 btclib-2023.5.30/tests/mnemonic/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      414 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/mnemonic/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    12193 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/_data/bip39_test_vectors.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2751 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/_data/electrum_test_vectors.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    13116 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/mnemonic/_data/english.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    13108 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/mnemonic/_data/fakeenglish.txt
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3001 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_bip39.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5192 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_electrum.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    10689 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_entropy.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1952 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_mnemonic.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/psbt/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      410 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/psbt/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    29762 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/psbt/_data/bip174_test_vectors.json
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/psbt/_generated_files/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     8273 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/_generated_files/psbt.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2943 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/_generated_files/psbt_in.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      294 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/_generated_files/psbt_out.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    70300 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/test_psbt.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3597 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/test_psbt_in.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4404 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/test_psbt_out.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      736 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/test_psbt_utils.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       27 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/py.typed
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.965772 btclib-2023.5.30/tests/script/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      412 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.969772 btclib-2023.5.30/tests/script/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1648 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/_data/bip67_test_vectors.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)   210483 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/script/_data/sig_hash_legacy_test_vectors.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    29296 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/script/_data/taproot_test_vector.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)  9242563 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/_data/tapscript_test_vector.json
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.993772 btclib-2023.5.30/tests/script/_generated_files/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1100 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/script/_generated_files/witness.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     8330 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_script.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    23491 2023-06-13 15:39:58.000000 btclib-2023.5.30/tests/script/test_script_pub_key.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     8217 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_sig_hash_legacy.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     6958 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_sig_hash_segwitv0.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     8476 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_sig_hash_taproot.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4287 2023-06-13 15:39:58.000000 btclib-2023.5.30/tests/script/test_taproot.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4368 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_witness.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3719 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_amount.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    12411 2023-06-13 15:39:58.000000 btclib-2023.5.30/tests/test_b32.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    10234 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_b58.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3725 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_base58.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     6531 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_bech32.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      847 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_hashes.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2761 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_network.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3615 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_number_theory.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    11489 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_to_key.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     5844 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_to_prv_key.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     9749 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_to_pub_key.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3073 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_utils.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     2060 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_var_int.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.997772 btclib-2023.5.30/tests/tx/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      408 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/__init__.py
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.997772 btclib-2023.5.30/tests/tx/_data/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4740 2022-07-04 10:37:34.000000 btclib-2023.5.30/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin
-drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.997772 btclib-2023.5.30/tests/tx/_generated_files/
--rw-rw-r--   0 kappa     (1000) kappa     (1000)       98 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/out_point.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    12973 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/tx.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     1392 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/tx_in.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      289 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/tx_out.json
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3440 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_out_point.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)    20879 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_tx.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     4547 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_tx_in.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)     3558 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_tx_out.py
--rw-rw-r--   0 kappa     (1000) kappa     (1000)      409 2023-06-13 15:39:52.000000 btclib-2023.5.30/tox.ini
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.333846 btclib-2023.7.12/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      741 2023-07-01 10:07:28.000000 btclib-2023.7.12/.flake8
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      485 2023-07-01 10:07:28.000000 btclib-2023.7.12/.markdownlint.jsonc
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4894 2023-07-12 13:33:53.000000 btclib-2023.7.12/.pre-commit-config.yaml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1657 2023-07-01 10:07:28.000000 btclib-2023.7.12/.sourcery.yaml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      303 2020-05-23 17:12:05.000000 btclib-2023.7.12/AUTHORS.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      207 2022-02-10 09:44:49.000000 btclib-2023.7.12/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5855 2023-07-01 10:07:28.000000 btclib-2023.7.12/CONTRIBUTING.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      341 2023-07-01 10:07:28.000000 btclib-2023.7.12/COPYRIGHT
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11662 2023-07-12 13:33:53.000000 btclib-2023.7.12/HISTORY.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1108 2023-07-01 10:07:28.000000 btclib-2023.7.12/LICENSE
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      943 2023-07-01 10:07:28.000000 btclib-2023.7.12/MANIFEST.in
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10316 2023-07-12 13:36:26.333846 btclib-2023.7.12/PKG-INFO
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8530 2023-07-01 10:07:28.000000 btclib-2023.7.12/README.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1371 2023-07-01 10:07:28.000000 btclib-2023.7.12/RELEASE.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      187 2023-07-01 10:07:28.000000 btclib-2023.7.12/SECURITY.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1701 2023-07-12 06:07:20.000000 btclib-2023.7.12/TODO.md
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.301845 btclib-2023.7.12/btclib/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      620 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.301845 btclib-2023.7.12/btclib/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/_data/mainnet.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      600 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/_data/regtest.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/_data/testnet.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3889 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/alias.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3900 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/amount.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6290 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/b32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4573 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/b58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4307 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/base58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5726 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/bech32.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.301845 btclib-2023.7.12/btclib/bip32/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1379 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/bip32/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    16588 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/bip32/bip32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3736 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/bip32/der_path.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5734 2023-07-12 12:08:40.000000 btclib-2023.7.12/btclib/bip32/key_origin.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3878 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/bip32/slip132.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.301845 btclib-2023.7.12/btclib/block/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      514 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/block/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4977 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/block/block.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7439 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/block/block_header.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2109 2023-07-12 08:59:28.000000 btclib-2023.7.12/btclib/descriptors.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.301845 btclib-2023.7.12/btclib/ec/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1552 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ec/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.301845 btclib-2023.7.12/btclib/ec/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4102 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/ec/_data/ec_Brainpool.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3105 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/ec/_data/ec_NIST.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2403 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/ec/_data/ec_SEC2v1_insecure.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4233 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/ec/_data/ec_SEC2v2.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8770 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ec/curve.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    25198 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/ec/curve_group.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8178 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ec/curve_group_2.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1726 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ec/curve_group_f.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2494 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ec/libsecp256k1.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3068 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ec/sec_point.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/btclib/ecc/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      632 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3592 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/bip340_nonce.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    14411 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/bms.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6124 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/borromean.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2614 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/dh.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    20004 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/dsa.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4290 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/libsecp256k1.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3271 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/pedersen.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4440 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/rfc6979_nonce.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4453 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/sign_to_contract.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    15082 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/ecc/ssa.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      794 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/exceptions.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3272 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/hashes.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/btclib/mnemonic/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1388 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/mnemonic/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/btclib/mnemonic/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13116 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/mnemonic/_data/english.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    16033 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/mnemonic/_data/italian.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5307 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/mnemonic/bip39.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5429 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/mnemonic/electrum.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11851 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/mnemonic/entropy.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4286 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/mnemonic/mnemonic.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9347 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/network.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4967 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/number_theory.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/btclib/psbt/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1236 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/psbt/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    20658 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/psbt/psbt.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    22355 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/psbt/psbt_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8392 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/psbt/psbt_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11762 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/psbt/psbt_utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       27 2023-07-01 10:07:28.000000 btclib-2023.7.12/btclib/py.typed
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/btclib/script/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1564 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/btclib/script/engine/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6534 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/script/engine/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13148 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/script/engine/script.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13213 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/engine/script_op_codes.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8959 2023-07-12 13:33:53.000000 btclib-2023.7.12/btclib/script/engine/tapscript.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6195 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/op_codes_tapscript.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10989 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/script.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    18120 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/script_pub_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10412 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/sig_hash.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7934 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/taproot.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2304 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/script/witness.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7023 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/to_prv_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7907 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/to_pub_key.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/btclib/tx/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      596 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/tx/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3262 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/tx/out_point.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10659 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/tx/tx.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4581 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/tx/tx_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4044 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/tx/tx_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6074 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1236 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/var_bytes.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2701 2023-07-12 06:07:20.000000 btclib-2023.7.12/btclib/var_int.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.301845 btclib-2023.7.12/btclib.egg-info/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10316 2023-07-12 13:36:26.000000 btclib-2023.7.12/btclib.egg-info/PKG-INFO
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6797 2023-07-12 13:36:26.000000 btclib-2023.7.12/btclib.egg-info/SOURCES.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)        1 2023-07-12 13:36:26.000000 btclib-2023.7.12/btclib.egg-info/dependency_links.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       20 2023-07-12 13:36:26.000000 btclib-2023.7.12/btclib.egg-info/requires.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       28 2023-07-12 13:36:26.000000 btclib-2023.7.12/btclib.egg-info/top_level.txt
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.305846 btclib-2023.7.12/docs/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      638 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/Makefile
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1777 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/README.rst
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.293845 btclib-2023.7.12/docs/build/
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.293845 btclib-2023.7.12/docs/build/html/
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.309846 btclib-2023.7.12/docs/build/html/_sources/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      788 2022-02-10 18:57:40.000000 btclib-2023.7.12/docs/build/html/_sources/btclib.bip32.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2378 2022-02-10 18:57:40.000000 btclib-2023.7.12/docs/build/html/_sources/btclib.ecc.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      823 2022-02-10 18:57:40.000000 btclib-2023.7.12/docs/build/html/_sources/btclib.mnemonic.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      772 2022-02-10 18:57:40.000000 btclib-2023.7.12/docs/build/html/_sources/btclib.psbt.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2145 2022-02-10 18:57:40.000000 btclib-2023.7.12/docs/build/html/_sources/btclib.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      972 2022-02-19 16:23:39.000000 btclib-2023.7.12/docs/build/html/_sources/btclib.script.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1015 2022-02-10 18:57:40.000000 btclib-2023.7.12/docs/build/html/_sources/btclib.tx.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      189 2022-02-10 18:59:04.000000 btclib-2023.7.12/docs/build/html/_sources/index.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       55 2020-05-23 17:12:05.000000 btclib-2023.7.12/docs/build/html/_sources/modules.rst.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      804 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/make.bat
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       43 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/requirements.txt
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.309846 btclib-2023.7.12/docs/source/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      788 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.bip32.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      491 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.block.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1088 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.ec.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1647 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.ecc.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      823 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.mnemonic.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      772 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.psbt.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2325 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      756 2023-07-12 13:33:53.000000 btclib-2023.7.12/docs/source/btclib.script.engine.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1241 2023-07-12 13:33:53.000000 btclib-2023.7.12/docs/source/btclib.script.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      721 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/btclib.tx.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2147 2023-07-12 13:33:53.000000 btclib-2023.7.12/docs/source/conf.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      157 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/contributing_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      105 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/history_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      508 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/index.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       55 2020-05-23 17:12:05.000000 btclib-2023.7.12/docs/source/modules.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      151 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/readme_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      153 2023-07-01 10:07:28.000000 btclib-2023.7.12/docs/source/security_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1604 2023-07-12 06:07:20.000000 btclib-2023.7.12/pyproject.toml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      318 2023-07-01 10:07:28.000000 btclib-2023.7.12/readthedocs.yml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      299 2023-07-01 10:07:28.000000 btclib-2023.7.12/requirements-dev.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       41 2023-07-01 10:07:28.000000 btclib-2023.7.12/requirements.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       38 2023-07-12 13:36:26.333846 btclib-2023.7.12/setup.cfg
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2732 2023-07-12 13:33:53.000000 btclib-2023.7.12/setup.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.309846 btclib-2023.7.12/tests/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1036 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/README.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      404 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.309846 btclib-2023.7.12/tests/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3771 2023-07-12 08:59:28.000000 btclib-2023.7.12/tests/_data/descriptor_checksums.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.309846 btclib-2023.7.12/tests/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-07-12 12:11:35.000000 btclib-2023.7.12/tests/_generated_files/mainnet.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      600 2023-07-12 12:11:35.000000 btclib-2023.7.12/tests/_generated_files/regtest.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-07-12 12:11:35.000000 btclib-2023.7.12/tests/_generated_files/testnet.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.313846 btclib-2023.7.12/tests/bip32/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      410 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/bip32/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.313846 btclib-2023.7.12/tests/bip32/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3151 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/bip32/_data/bip32_invalid_keys.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5515 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/bip32/_data/bip32_test_vectors.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.313846 btclib-2023.7.12/tests/bip32/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       73 2023-07-12 12:11:35.000000 btclib-2023.7.12/tests/bip32/_generated_files/key_origin.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      625 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/bip32/_generated_files/key_paths.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    14921 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/bip32/test_bip32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5026 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/bip32/test_der_path.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5184 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/bip32/test_key_origin.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9594 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/bip32/test_slip132.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.313846 btclib-2023.7.12/tests/block/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      410 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/block/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.313846 btclib-2023.7.12/tests/block/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      215 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/block/_data/block_1.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      490 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/block/_data/block_170.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   247533 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/block/_data/block_200000.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   988519 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/block/_data/block_481824.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   989323 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/block/_data/block_481824_complete.bin
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.317846 btclib-2023.7.12/tests/block/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)  5738930 2023-07-12 12:11:43.000000 btclib-2023.7.12/tests/block/_generated_files/block_481824.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      419 2023-07-12 12:11:44.000000 btclib-2023.7.12/tests/block/_generated_files/block_header_481824.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10548 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/block/test_block.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.317846 btclib-2023.7.12/tests/ec/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      407 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ec/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.317846 btclib-2023.7.12/tests/ec/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   126364 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/ec/_data/pubkey.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    15647 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ec/test_curve.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    15425 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ec/test_curve_group.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4270 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ec/test_curve_group_2.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2178 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ec/test_curve_group_f.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4812 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ec/test_sec_point.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.321846 btclib-2023.7.12/tests/ecc/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      408 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.321846 btclib-2023.7.12/tests/ecc/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5161 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/ecc/_data/bip340_test_vectors.csv
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    50597 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/ecc/_data/bms.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    89766 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/ecc/_data/ecdsa_custom_nonce_sig.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    72463 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/ecc/_data/ecdsa_sig.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    31685 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/ecc/_data/rfc6979.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    27856 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_bms.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1483 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_borromean.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3886 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_der.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    29797 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_dh.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13267 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_dsa.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2001 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_pedersen.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2949 2023-07-12 13:33:53.000000 btclib-2023.7.12/tests/ecc/test_rfc6979.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1507 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_sign_to_contract.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    25963 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/ecc/test_ssa.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.321846 btclib-2023.7.12/tests/mnemonic/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      413 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/mnemonic/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.321846 btclib-2023.7.12/tests/mnemonic/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    12193 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/mnemonic/_data/bip39_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2751 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/mnemonic/_data/electrum_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13116 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/mnemonic/_data/english.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13108 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/mnemonic/_data/fakeenglish.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3000 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/mnemonic/test_bip39.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5191 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/mnemonic/test_electrum.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10683 2023-07-12 10:46:27.000000 btclib-2023.7.12/tests/mnemonic/test_entropy.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1951 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/mnemonic/test_mnemonic.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.321846 btclib-2023.7.12/tests/psbt/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      409 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/psbt/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.321846 btclib-2023.7.12/tests/psbt/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    29762 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/psbt/_data/bip174_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    12938 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/psbt/_data/bip371_test_vectors.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.321846 btclib-2023.7.12/tests/psbt/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9011 2023-07-12 12:11:36.000000 btclib-2023.7.12/tests/psbt/_generated_files/psbt.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3152 2023-07-12 12:11:36.000000 btclib-2023.7.12/tests/psbt/_generated_files/psbt_in.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      382 2023-07-12 12:11:36.000000 btclib-2023.7.12/tests/psbt/_generated_files/psbt_out.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    71517 2023-07-12 13:33:53.000000 btclib-2023.7.12/tests/psbt/test_psbt.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3596 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/psbt/test_psbt_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4403 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/psbt/test_psbt_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      735 2023-07-12 10:46:10.000000 btclib-2023.7.12/tests/psbt/test_psbt_utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       27 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/py.typed
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.325846 btclib-2023.7.12/tests/script/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      411 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.325846 btclib-2023.7.12/tests/script/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1648 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/script/_data/bip67_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   210483 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/script/_data/sig_hash_legacy_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    29296 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/script/_data/taproot_test_vector.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)  9242563 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/script/_data/tapscript_test_vector.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.329846 btclib-2023.7.12/tests/script/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1100 2023-07-12 12:11:36.000000 btclib-2023.7.12/tests/script/_generated_files/witness.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      967 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script/test_op_codes_taproot.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7918 2023-07-12 13:33:53.000000 btclib-2023.7.12/tests/script/test_script.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    23489 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script/test_script_pub_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8216 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script/test_sig_hash_legacy.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6957 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script/test_sig_hash_segwitv0.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8527 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script/test_sig_hash_taproot.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5731 2023-07-12 13:33:53.000000 btclib-2023.7.12/tests/script/test_taproot.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4367 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script/test_witness.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.329846 btclib-2023.7.12/tests/script_engine/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1657 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script_engine/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.329846 btclib-2023.7.12/tests/script_engine/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   215125 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script_engine/_data/script_tests.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    53413 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script_engine/_data/tx_invalid_legacy.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    85555 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script_engine/_data/tx_valid_legacy.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2860 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script_engine/test_script.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4787 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/script_engine/test_transactions.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3718 2023-07-12 10:53:32.000000 btclib-2023.7.12/tests/test_amount.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    12428 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_b32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10264 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_b58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3724 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_base58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6530 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_bech32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1510 2023-07-12 08:59:28.000000 btclib-2023.7.12/tests/test_descriptors.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      846 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_hashes.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2760 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_network.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3614 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_number_theory.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11488 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_to_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5843 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_to_prv_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9808 2023-07-12 13:33:53.000000 btclib-2023.7.12/tests/test_to_pub_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3072 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2059 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/test_var_int.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.333846 btclib-2023.7.12/tests/tx/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      407 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/tx/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.333846 btclib-2023.7.12/tests/tx/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4740 2023-07-01 10:07:28.000000 btclib-2023.7.12/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-07-12 13:36:26.333846 btclib-2023.7.12/tests/tx/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       98 2023-07-12 12:11:37.000000 btclib-2023.7.12/tests/tx/_generated_files/out_point.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    12973 2023-07-12 12:11:37.000000 btclib-2023.7.12/tests/tx/_generated_files/tx.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1392 2023-07-12 12:11:37.000000 btclib-2023.7.12/tests/tx/_generated_files/tx_in.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      289 2023-07-12 12:11:37.000000 btclib-2023.7.12/tests/tx/_generated_files/tx_out.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3439 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/tx/test_out_point.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    21028 2023-07-12 13:33:53.000000 btclib-2023.7.12/tests/tx/test_tx.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4546 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/tx/test_tx_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3557 2023-07-12 06:07:20.000000 btclib-2023.7.12/tests/tx/test_tx_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      437 2023-07-12 06:07:20.000000 btclib-2023.7.12/tox.ini
```

### Comparing `btclib-2023.5.30/.flake8` & `btclib-2023.7.12/.flake8`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/.pre-commit-config.yaml` & `btclib-2023.7.12/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -36,58 +36,58 @@
   - repo: https://github.com/leoll2/copyright_notice_precommit
     rev: 0.1.1
     hooks:
       - id: copyright-notice
         args: [--notice=COPYRIGHT]
         files: python
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
       - id: autoflake
         args:
           - --in-place
           - --expand-star-imports
           - --remove-all-unused-imports
           - --ignore-init-module-imports
           - --remove-duplicate-keys
           - --remove-unused-variables
           - --remove-rhs-for-unused-variables
         language: python
         types: [python]
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.6.0
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
         # exclude: *fixtures
         language: python
         types: [python]
-  - repo: https://github.com/pycqa/isort
+  - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (black profile, in place fixes)
         args: ["--profile", "black", "--filter-files"]
         language: python
         types: [python]
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.7.2
+    rev: v1.7.5
     hooks:
       - id: docformatter
         description: "Formats docstrings to follow PEP 257."
         language: python
         types: [python]
         args: ["--in-place"]
   - repo: https://github.com/DanielNoord/pydocstringformatter
     rev: v0.7.3
     hooks:
       - id: pydocstringformatter
         language: python
         types: [python]
-  - repo: https://github.com/pycqa/pydocstyle
+  - repo: https://github.com/PyCQA/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies: [tomli]
         language: python
         types: [python]
   - repo: https://github.com/asottile/yesqa
@@ -99,15 +99,15 @@
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         language: python
         types: [python]
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         name: black (in place fixes)
         # args: [--diff, --check]
         # It is recommended to specify the latest version of Python
         # supported by your project here, or alternatively use
         # pre-commit's default_language_version, see
@@ -133,25 +133,25 @@
         # B101, Test for use of assert
         # B311, Standard pseudo-random generators are not suitable
         #       for security/cryptographic purposes
         args: ["--skip", "B101,B311"]
         exclude: btclib
         language: python
         types: [python]
-  - repo: https://github.com/pycqa/pylint
+  - repo: https://github.com/PyCQA/pylint
     rev: v3.0.0a6
     hooks:
       - id: pylint
         args: [
             "--disable=E0401", # import-error
           ]
         language: python
         types: [python]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         language: python
         types: [python]
   - repo: https://github.com/mgedmin/check-manifest
     rev: "0.49"
     hooks:
```

### Comparing `btclib-2023.5.30/.sourcery.yaml` & `btclib-2023.7.12/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/CONTRIBUTING.md` & `btclib-2023.7.12/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/HISTORY.md` & `btclib-2023.7.12/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 # Release notes
 
 Notable changes to the codebase are documented here.
 
 Release names follow *[calendar versioning](https://calver.org/)*:
 full year, short month, short day (YYYY-M-D)
 
-## v2023.6 (work in progress, not released yet)
+## v2023.7.12
+
+This is the last release supporting py37.
 
 Major changes include:
 
-- TBD
+- added first draft implementation of descriptors
+- added first draft implementation of script engine
+- added taproot psbt fields
+- improved bip32 derivation (speeded-up, added one more test)
+- supported py3.12 with btclib_libsecp256k1
+- updated toolchain
 
 ## v2023.5.30
 
 Major changes include:
 
 - Fix circular import between ``script`` and ``b32``
 
@@ -40,14 +47,15 @@
 - added pre-commit hooks
 - adopted *mypy --strict* and *from \_\_future\_\_ import annotations*
 
 ## v2022.12.31
 
 Major changes include:
 
+- add support for PSBT's taproot fields (bip370)
 - added support for Python 3.11
 - fixed the OpenSSL 3.x RIPEMD160 issue in btclib/hashes.py
 - added CONTRIBUTING and SECURITY
 - solved issue #73
   [Re-import Tx subclasses into btclib.tx](https://github.com/btclib-org/btclib/issues/73)
 
 ## v2022.7.20
@@ -152,16 +160,16 @@
   bip32.deserialize(xkey), now it is bip32.BIP32KeyData.deserialize(xkey)
 - bip32: added str_from_bip32_path and bytes_from_bip32_path
 - bip3: made bip32 index an int (not bytes) to avoid byteorder ambiguity.
   Consequently, where previously it was xkey_dict\["index"\][0] < 0x80,
   now it is xkey_dict.index < 0x80000000
 - bip32: local "./" derivation, opposed to absolute "m/" derivation,
   is not available anymore
-- bip32: indexes_from_bip32_path now returns List[int] instead of
-  Tuple[List[bytes], bool] losing the "absolute derivation" bool
+- bip32: indexes_from_bip32_path now returns list[int] instead of
+  Tuple[list[bytes], bool] losing the "absolute derivation" bool
 - bms: serialize/deserialize have been renamed encode/decode as they
   include the base64 (de)encoding, not jut the plain (de)serialization
 - Block: fixed bug in difficulty calculation
 - introduced first beta version of HdKeyPaths, PartialSigs, PsbtIn,
   PsbtOut, and Psbt data classes and their associated helper functions
 - refactored Diffie-Hellman and ANSI-X9.63-KDF
 - introduced assorted elliptic curve point multiplication
```

### Comparing `btclib-2023.5.30/LICENSE` & `btclib-2023.7.12/LICENSE`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/MANIFEST.in` & `btclib-2023.7.12/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/PKG-INFO` & `btclib-2023.7.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btclib
-Version: 2023.5.30
+Version: 2023.7.12
 Summary: A library for 'bitcoin cryptography'
 Home-page: https://btclib.org
 Author: The btclib developers
 Author-email: devs@btclib.org
 License: MIT License
 Project-URL: Download, https://github.com/btclib-org/btclib/releases
 Project-URL: Documentation, https://btclib.readthedocs.io/
```

### Comparing `btclib-2023.5.30/README.md` & `btclib-2023.7.12/README.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/RELEASE.md` & `btclib-2023.7.12/RELEASE.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/TODO.md` & `btclib-2023.7.12/TODO.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,7 +35,11 @@
 - report test vectors from P. Todd's library
 - report trailing/leading blank trimming in Electrum message signing
 - report BIP39 whitespaces
 - SSA: ask about checking e=0
 - SSA: ask about why e=e(k), making impossible to select e, k indipendently
 - SSA: ask about benefit of removing 02/03 from pub_key
 - SSA: suggest better k
+
+- compare of dsa.rfc6979_and ssa.det_nonce_
+
+- refactor Psbt
```

### Comparing `btclib-2023.5.30/btclib/__init__.py` & `btclib-2023.7.12/btclib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """__init__ module for the btclib package."""
 
 name = "btclib"
-__version__ = "2023.5.30"
+__version__ = "2023.7.12"
 __author__ = "The btclib developers"
 __author_email__ = "devs@btclib.org"
 __copyright__ = "Copyright (C) 2017-2023 The btclib developers"
 __license__ = "MIT License"
```

### Comparing `btclib-2023.5.30/btclib/_data/mainnet.json` & `btclib-2023.7.12/btclib/_data/mainnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/_data/regtest.json` & `btclib-2023.7.12/btclib/_data/regtest.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/_data/testnet.json` & `btclib-2023.7.12/btclib/_data/testnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/alias.py` & `btclib-2023.7.12/btclib/alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Aliases.
 
 mypy aliases, documenting also coding input conventions.
 """
 from __future__ import annotations
 
 from io import BytesIO
-from typing import Any, Callable, Tuple, Union
+from typing import Any, Callable, List, Tuple, Union
 
 # Octets are a sequence of eight-bit bytes or a hex-string (not text string)
 #
 # hex-strings are strings that can be converted to bytes using bytes.fromhex,
 # e.g.:
 # "deadbeef"
 # "dead beef"
@@ -101,7 +100,10 @@
 
 # TODO add type hinting to script_tree
 # unfortunately recursive type hinting is not supported
 # https://github.com/python/mypy/issues/731
 # TaprootLeaf = Tuple[int, Script]
 # TaprootScriptTree = List[Union[Any, TaprootLeaf]]
 TaprootScriptTree = Any
+
+Command = Union[int, str, bytes]
+ScriptList = List[Command]
```

### Comparing `btclib-2023.5.30/btclib/amount.py` & `btclib-2023.7.12/btclib/amount.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Proper handling of monetary amounts.
 
 A BTC monetary amount can be expressed
 as number of satoshis (1 BTC is 100_000_000) or
 as Python Decimal with up to 8 digits, e.g. Decimal("0.12345678").
 
 Because of floating-point conversion issues
```

### Comparing `btclib-2023.5.30/btclib/b32.py` & `btclib-2023.7.12/btclib/b32.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-
 """SegWit address functions.
 
 Some of these functions were originally from
 https://github.com/sipa/bech32/tree/master/ref/python,
 with the following modifications:
 
 * moved bech32 stuff into bech32.py
```

### Comparing `btclib-2023.5.30/btclib/b58.py` & `btclib-2023.7.12/btclib/b58.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Base58 address and WIF functions.
 
 Base58 encoding of public keys and scripts as addresses, private keys as
 WIFs
 """
 from __future__ import annotations
 
 from btclib import b32
 from btclib.alias import Octets, String
 from btclib.base58 import b58decode, b58encode
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash160, sha256
 from btclib.network import NETWORKS, network_from_key_value
-from btclib.script import serialize
+from btclib.script.script import serialize
 from btclib.to_prv_key import PrvKey, prv_keyinfo_from_prv_key
 from btclib.to_pub_key import Key, pub_keyinfo_from_key
 from btclib.utils import bytes_from_octets
 
 
 def wif_from_prv_key(
     prv_key: PrvKey, network: str | None = None, compressed: bool | None = None
```

### Comparing `btclib-2023.5.30/btclib/base58.py` & `btclib-2023.7.12/btclib/base58.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Base58 encoding and decoding functions.
 
 Binary-to-text encoding schemes are used to transport binary data across
 channels designed to deal with textual data. In Bitcoin they are mostly
 used to represent large integers as alphanumeric text.
 
 Base58 is similar to Base64, which uses 10 digits, 26 lowercase characters,
```

### Comparing `btclib-2023.5.30/btclib/bech32.py` & `btclib-2023.7.12/btclib/bech32.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-
 """Bech32(m) encoding and decoding functions.
 
 BIP173: https://github.com/bitcoin/bips/blob/master/bip-0173.mediawiki
 
 This implementation of bech32 is originally from
 https://github.com/sipa/bech32/tree/master/ref/python,
 with the following modifications:
```

### Comparing `btclib-2023.5.30/btclib/bip32/__init__.py` & `btclib-2023.7.12/btclib/bip32/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.bip32."""
 
 from btclib.bip32.bip32 import (
     BIP32Key,
     BIP32KeyData,
     crack_prv_key,
     derive,
```

### Comparing `btclib-2023.5.30/btclib/bip32/bip32.py` & `btclib-2023.7.12/btclib/bip32/bip32.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """BIP32 Hierarchical Deterministic Wallet functions.
 
 A deterministic wallet is a hash-chain of private/public key pairs that
 derives from a single root, which is the only element requiring backup.
 Moreover, there are schemes where public keys can be calculated without
 accessing private keys.
 
@@ -305,51 +304,35 @@
             self.prv_key_int = 0
             self.pub_key_point = point_from_octets(self.key, ec)
 
         if check_validity:
             self.assert_valid()
 
 
-def __prv_key_derivation(xkey: _BIP32KeyData, index: int) -> None:
-    xkey.index = index
-    Q_bytes = bytes_from_point(mult(xkey.prv_key_int))
-    xkey.parent_fingerprint = hash160(Q_bytes)[:4]
-    hmac_ = (
-        hmac.new(
-            xkey.chain_code,
-            xkey.key + index.to_bytes(4, byteorder="big", signed=False),
-            "sha512",
-        ).digest()
-        if xkey.is_hardened
-        else hmac.new(
-            xkey.chain_code,
-            Q_bytes + index.to_bytes(4, byteorder="big", signed=False),
-            "sha512",
-        ).digest()
+def __prv_key_derivation(xkey: _BIP32KeyData, index: int, pub_key: bytes) -> None:
+    xb = (
+        xkey.key
+        if index >= 0x80000000
+        else pub_key or bytes_from_point(mult(xkey.prv_key_int))
     )
+    xb += index.to_bytes(4, byteorder="big", signed=False)
+    hmac_ = hmac.new(xkey.chain_code, xb, "sha512").digest()
     xkey.chain_code = hmac_[32:]
     offset = int.from_bytes(hmac_[:32], byteorder="big", signed=False)
     xkey.prv_key_int = (xkey.prv_key_int + offset) % ec.n
     xkey.key = b"\x00" + xkey.prv_key_int.to_bytes(32, byteorder="big", signed=False)
-    xkey.pub_key_point = INF
 
 
 def __pub_key_derivation(xkey: _BIP32KeyData, index: int) -> None:
-    xkey.index = index
-    xkey.parent_fingerprint = hash160(xkey.key)[:4]
-    hmac_ = hmac.new(
-        xkey.chain_code,
-        xkey.key + index.to_bytes(4, byteorder="big", signed=False),
-        "sha512",
-    ).digest()
+    xb = xkey.key + index.to_bytes(4, byteorder="big", signed=False)
+    hmac_ = hmac.new(xkey.chain_code, xb, "sha512").digest()
     xkey.chain_code = hmac_[32:]
     offset = int.from_bytes(hmac_[:32], byteorder="big", signed=False)
     xkey.pub_key_point = ec.add(xkey.pub_key_point, mult(offset))
     xkey.key = bytes_from_point(xkey.pub_key_point)
-    xkey.prv_key_int = 0
 
 
 def _derive(
     xkey: BIP32Key, der_path: BIP32DerPath, forced_version: Octets | None = None
 ) -> BIP32KeyData:
     if not isinstance(xkey, BIP32KeyData):
         xkey = BIP32KeyData.b58decode(xkey)
@@ -378,22 +361,30 @@
         fversion = bytes_from_octets(forced_version, 4)
         if fversion not in allowed_versions:
             err_msg = "invalid version forced on the extended key"
             err_msg += f"{hex_string(fversion)}"
             raise BTClibValueError(err_msg)
         xkey.version = fversion
 
-    if xkey.is_private:
-        for index in indexes:
-            __prv_key_derivation(xkey, index)
-    else:
-        if any(index >= 0x80000000 for index in indexes):
-            raise BTClibValueError("invalid hardened derivation from public key")
-        for index in indexes:
-            __pub_key_derivation(xkey, index)
+    if indexes:
+        if xkey.is_private:
+            for index in indexes[:-1]:
+                __prv_key_derivation(xkey, index, b"")
+            pub_key = bytes_from_point(mult(xkey.prv_key_int))
+            xkey.parent_fingerprint = hash160(pub_key)[:4]
+            __prv_key_derivation(xkey, indexes[-1], pub_key)
+        else:
+            if any(index >= 0x80000000 for index in indexes):
+                raise BTClibValueError("invalid hardened derivation from public key")
+            for index in indexes[:-1]:
+                __pub_key_derivation(xkey, index)
+            xkey.parent_fingerprint = hash160(xkey.key)[:4]
+            __pub_key_derivation(xkey, indexes[-1])
+
+        xkey.index = indexes[-1]
 
     return xkey
 
 
 def derive(
     xkey: BIP32Key, der_path: BIP32DerPath, forced_version: Octets | None = None
 ) -> str:
```

### Comparing `btclib-2023.5.30/btclib/bip32/der_path.py` & `btclib-2023.7.12/btclib/bip32/der_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """BIP32 derivation path and key origin.
 
 A BIP 32 derivation path can be represented as:
 
 - "m/44h/0'/1H/0/10" or "44h/0'/1H/0/10" string
 - sequence of integer indexes (even a single int)
 - bytes (multiples of 4-bytes index)
```

### Comparing `btclib-2023.5.30/btclib/bip32/key_origin.py` & `btclib-2023.7.12/btclib/bip32/key_origin.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """BIP32 key origin."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Mapping, MutableMapping, Sequence
 
 from btclib.alias import Octets
```

### Comparing `btclib-2023.5.30/btclib/bip32/slip132.py` & `btclib-2023.7.12/btclib/bip32/slip132.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """SLIP132 address.
 
 https://github.com/satoshilabs/slips/blob/master/slip-0132.md
 """
 from __future__ import annotations
 
 import contextlib
```

### Comparing `btclib-2023.5.30/btclib/block/__init__.py` & `btclib-2023.7.12/btclib/block/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,13 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.ecc."""
 
 from btclib.block.block import Block
 from btclib.block.block_header import BlockHeader
 
 __all__ = ["Block", "BlockHeader"]
```

### Comparing `btclib-2023.5.30/btclib/block/block.py` & `btclib-2023.7.12/btclib/block/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Block dataclass.
 
 Dataclass encapsulating BlockHeader and list[Tx].
 """
 from __future__ import annotations
 
 from dataclasses import dataclass
@@ -50,15 +49,16 @@
     def height(self) -> int | None:
         """Return the height committed into a BIP34 coinbase script_sig.
 
         Version 2 blocks commit block height into the coinbase
         script_sig.
 
         https://github.com/bitcoin/bips/blob/master/bip-0034.mediawiki
-        Block 227,835 (2013-03-24 15:49:13 GMT) was the last version 1 block.
+        Block 227,835 (2013-03-24 15
+        :49: 13 GMT) was the last version 1 block.
         """
         if not self.transactions[0].is_coinbase():
             raise BTClibValueError("first transaction is not a coinbase")
 
         if self.header.version == 1:
             return None
```

### Comparing `btclib-2023.5.30/btclib/block/block_header.py` & `btclib-2023.7.12/btclib/block/block_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """BlockHeader dataclass.
 
 Dataclass encapsulating version, previous block hash, merkle root, time,
 bits, and nonce.
 """
 from __future__ import annotations
 
@@ -57,24 +56,23 @@
         power_term = pow(256, (self.bits[0] - 3))
         return int(significand * power_term).to_bytes(_HF_LEN, "big", signed=False)
 
     @property
     def difficulty(self) -> float:
         """Return the BlockHeader difficulty.
 
-        Difficulty is the ratio of the genesis block target
-        over the BlockHeader target.
+        Difficulty is the ratio of the genesis block target over the
+        BlockHeader target.
 
         It represents the average number of hash function evaluations
-        required to satisfy the BlockHeader target,
-        expressed as multiple of the genesis block difficulty used as
-        unit.
+        required to satisfy the BlockHeader target, expressed as
+        multiple of the genesis block difficulty used as unit.
 
-        The difficulty of the genesis block is 2^32 (4*2^30),
-        i.e. 4 GigaHash function evaluations.
+        The difficulty of the genesis block is 2^32 (4*2^30), i.e. 4
+        GigaHash function evaluations.
         """
         # genesis block target
         genesis_significand = 0x00FFFF
         genesis_exponent = 0x1D
         # significand ratio
         significand = genesis_significand / int.from_bytes(
             self.bits[1:], byteorder="big", signed=False
```

### Comparing `btclib-2023.5.30/btclib/ec/__init__.py` & `btclib-2023.7.12/btclib/ec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.ec."""
 
 from btclib.ec.curve import Curve, double_mult, mult, multi_mult, secp256k1
 from btclib.ec.curve_group import (
     CurveGroup,
     cached_multiples,
     jac_from_aff,
```

### Comparing `btclib-2023.5.30/btclib/ec/_data/ec_Brainpool.json` & `btclib-2023.7.12/btclib/ec/_data/ec_Brainpool.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/ec/_data/ec_NIST.json` & `btclib-2023.7.12/btclib/ec/_data/ec_NIST.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/ec/_data/ec_SEC2v1_insecure.json` & `btclib-2023.7.12/btclib/ec/_data/ec_SEC2v1_insecure.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/ec/_data/ec_SEC2v2.json` & `btclib-2023.7.12/btclib/ec/_data/ec_SEC2v2.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/ec/curve.py` & `btclib-2023.7.12/btclib/ec/curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Elliptic curve classes and functions."""
 from __future__ import annotations
 
 import json
 from math import sqrt
 from os import path
 from typing import Sequence
```

### Comparing `btclib-2023.5.30/btclib/ec/curve_group.py` & `btclib-2023.7.12/btclib/ec/curve_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Elliptic CurveGroup class and functions.
 
 Note that CurveGroup does not have to be a cyclic subgroup. For the
 cyclic subgroup class CurveSubGroup and the cyclic subgroup class of
 prime order Curve, see the btclib.ec.curve module.
 """
 from __future__ import annotations
@@ -36,20 +35,18 @@
     """
     return Q[0], Q[1], 1 if Q[1] else 0
 
 
 class CurveGroup:
     """Finite group of the points of an elliptic curve over Fp.
 
-    The elliptic curve is the set of points (x, y)
-    that are solutions to a Weierstrass equation y^2 = x^3 + a*x + b,
-    with x, y, a, and b in Fp (p being a prime),
-    together with a point at infinity INF.
-    The constants a, b must satisfy the relationship
-    4 a^3 + 27 b^2 ≠ 0.
+    The elliptic curve is the set of points (x, y) that are solutions to
+    a Weierstrass equation y^2 = x^3 + a*x + b, with x, y, a, and b in
+    Fp (p being a prime), together with a point at infinity INF. The
+    constants a, b must satisfy the relationship 4 a^3 + 27 b^2 ≠ 0.
 
     The group is defined by the point addition group law.
     """
 
     def __init__(self, p: Integer, a: Integer, b: Integer) -> None:
         # Parameters are checked according to SEC 1 v.2 3.1.1.2.1
         p = int_from_integer(p)
@@ -351,21 +348,20 @@
         legendre = legendre_symbol(root, self.p)
         return root if legendre else self.p - root
 
 
 def mult_recursive_aff(m: int, Q: Point, ec: CurveGroup) -> Point:
     """Scalar multiplication of a curve point in affine coordinates.
 
-    This implementation uses
-    a recursive version of 'double & add',
+    This implementation uses a recursive version of 'double & add',
     affine coordinates.
 
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     if m == 0:
         return INF
 
@@ -374,21 +370,20 @@
 
     return mult_recursive_aff((m // 2), ec.double_aff(Q), ec)
 
 
 def mult_recursive_jac(m: int, Q: JacPoint, ec: CurveGroup) -> JacPoint:
     """Scalar multiplication of a curve point in affine coordinates.
 
-    This implementation uses
-    a recursive version of 'double & add',
+    This implementation uses a recursive version of 'double & add',
     jacobian coordinates.
 
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     if m == 0:
         return INFJ
 
@@ -397,22 +392,20 @@
 
     return mult_recursive_jac((m // 2), ec.double_jac(Q), ec)
 
 
 def mult_aff(m: int, Q: Point, ec: CurveGroup) -> Point:
     """Scalar multiplication of a curve point in affine coordinates.
 
-    This implementation uses
-    'double & add' algorithm,
-    'right-to-left' binary decomposition of the m coefficient,
-    affine coordinates.
+    This implementation uses 'double & add' algorithm, 'right-to-left'
+    binary decomposition of the m coefficient, affine coordinates.
 
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     # R[0] is the running result, R[1] = R[0] + Q is an ancillary variable
     R = [INF, Q]
     # if least significant bit of m is 1, then add Q to R[0]
@@ -429,22 +422,20 @@
         m >>= 1
     return R[0]
 
 
 def mult_jac(m: int, Q: JacPoint, ec: CurveGroup) -> JacPoint:
     """Scalar multiplication of a curve point in Jacobian coordinates.
 
-    This implementation uses
-    'double & add' algorithm,
-    'right-to-left' binary decomposition of the m coefficient,
-    Jacobian coordinates.
+    This implementation uses 'double & add' algorithm, 'right-to-left'
+    binary decomposition of the m coefficient, Jacobian coordinates.
 
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     # R[0] is the running result, R[1] = R[0] + Q is an ancillary variable
     R = [INFJ, Q]
     # if least significant bit of m is 1, then add Q to R[0]
@@ -548,22 +539,20 @@
         R[i] = ec.double_jac(R[i])
     return R[0]
 
 
 def mult_base_3(m: int, Q: JacPoint, ec: CurveGroup) -> JacPoint:
     """Scalar multiplication using ternary decomposition of the scalar.
 
-    This implementation uses
-    'triple & add' algorithm,
-    'left-to-right' ternary decomposition of the m coefficient,
-    Jacobian coordinates.
+    This implementation uses 'triple & add' algorithm, 'left-to-right'
+    ternary decomposition of the m coefficient, Jacobian coordinates.
 
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     # at each step one of the points in T will be added
     T = [INFJ, Q, ec.double_jac(Q)]
     # T = multiples(Q, 3, ec)
@@ -582,24 +571,23 @@
 
 
 def mult_fixed_window(
     m: int, Q: JacPoint, ec: CurveGroup, w: int = 4, cached: bool = False
 ) -> JacPoint:
     """Scalar multiplication using "fixed window".
 
-    This implementation uses
-    'multiple-double & add' algorithm,
-    'left-to-right' window decomposition of the m coefficient,
-    Jacobian coordinates.
+    This implementation uses 'multiple-double & add' algorithm, 'left-
+    to-right' window decomposition of the m coefficient, Jacobian
+    coordinates.
 
     For 256-bit scalars it is suggested to choose w=4 or w=5.
 
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     # a number cannot be written in basis 1 (ie w=0)
     if w <= 0:
         raise BTClibValueError(f"non positive w: {w}")
@@ -623,25 +611,24 @@
 
 
 def mult_fixed_window_cached(
     m: int, Q: JacPoint, ec: CurveGroup, w: int = 4
 ) -> JacPoint:
     """Scalar multiplication using "fixed window" & cached values.
 
-    This implementation uses
-    'multiple-double & add' algorithm,
-    'left-to-right' window decomposition of the m coefficient,
-    Jacobian coordinates.
-
-    For 256-bit scalars it is suggested to choose w=4.
-    Thanks to the pre-computed values, it just needs addictions.
-
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    This implementation uses 'multiple-double & add' algorithm, 'left-
+    to-right' window decomposition of the m coefficient, Jacobian
+    coordinates.
+
+    For 256-bit scalars it is suggested to choose w=4. Thanks to the
+    pre-computed values, it just needs addictions.
+
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     # a number cannot be written in basis 1 (ie w=0)
     if w <= 0:
         raise BTClibValueError(f"non positive w: {w}")
@@ -665,21 +652,21 @@
 
 
 def _double_mult(
     u: int, HJ: JacPoint, v: int, QJ: JacPoint, ec: CurveGroup
 ) -> JacPoint:
     """Double scalar multiplication (u*H + v*Q).
 
-    This implementation uses the Shamir-Strauss algorithm,
-    'left-to-right' binary decomposition of the u and v coefficients,
-    Jacobian coordinates.
-
-    Strauss algorithm consists of a single 'double & add' loop
-    for the parallel calculation of u*H and v*Q, efficiently
-    using a single 'doubling' for both scalar multiplications (see
+    This implementation uses the Shamir-Strauss algorithm, 'left-to-
+    right' binary decomposition of the u and v coefficients, Jacobian
+    coordinates.
+
+    Strauss algorithm consists of a single 'double & add' loop for the
+    parallel calculation of u*H and v*Q, efficiently using a single
+    'doubling' for both scalar multiplications (see
 
     https://stackoverflow.com/questions/50993471/ec-scalar-multiplication-with-strauss-shamir-method).
     The Shamir trick adds the precomputation of H+Q,
     which is to be added in the loop when the binary digits
     of u and v are both equal to 1 (on average 1/4 of the cases).
 
     The input points are assumed to be on curve,
@@ -712,17 +699,17 @@
 def _multi_mult(
     scalars: Sequence[int], jac_points: Sequence[JacPoint], ec: CurveGroup
 ) -> JacPoint:
     """Return the multi scalar multiplication u1*Q1 + ... + un*Qn.
 
     Use Bos-Coster's algorithm for efficient computation.
 
-    The input points are assumed to be on curve,
-    the scalar coefficients are assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    The input points are assumed to be on curve, the scalar coefficients
+    are assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     # source: https://cr.yp.to/badbatch/boscoster2.py
     if len(scalars) != len(jac_points):
         err_msg = "mismatch between number of scalars and points: "
         err_msg += f"{len(scalars)} vs {len(jac_points)}"
         raise BTClibValueError(err_msg)
```

### Comparing `btclib-2023.5.30/btclib/ec/curve_group_2.py` & `btclib-2023.7.12/btclib/ec/curve_group_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Elliptic curve point multiplication functions.
 
 The implemented algorithms are:
     - Montgomery Ladder
     - Scalar multiplication on basis 3
     - Fixed window
     - Sliding window
@@ -90,22 +89,21 @@
 
     return M
 
 
 def mult_sliding_window(m: int, Q: JacPoint, ec: CurveGroup, w: int = 4) -> JacPoint:
     """Scalar multiplication using "sliding window".
 
-    It has the benefit that the pre-computation stage
-    is roughly half as complex as the normal windowed method.
-    It is not constant time.
-    For 256-bit scalars choose w=4 or w=5.
-
-    The input point is assumed to be on curve and
-    the m coefficient is assumed to have been reduced mod n
-    if appropriate (e.g. cyclic groups of order n).
+    It has the benefit that the pre-computation stage is roughly half as
+    complex as the normal windowed method. It is not constant time. For
+    256-bit scalars choose w=4 or w=5.
+
+    The input point is assumed to be on curve and the m coefficient is
+    assumed to have been reduced mod n if appropriate (e.g. cyclic
+    groups of order n).
     """
     if m < 0:
         raise BTClibValueError(f"negative m: {hex(m)}")
 
     # a number cannot be written in basis 1 (ie w=0)
     if w <= 0:
         raise BTClibValueError(f"non positive w: {w}")
@@ -197,19 +195,19 @@
                 R = ec.add_jac(R, T[(b // 4) - ((M[j] + 1) // 2)])
     return R
 
 
 def multiplier_decomposer(m: int, ec: CurveGroup) -> tuple[int, int]:
     """Decompose m in two integers m1 e m2 so that mP = m1*P + m2*lambda*P.
 
-    Used for point multiplication with efficiently computable endomorphisms.
+    Used for point multiplication with efficiently computable
+    endomorphisms.
 
-    Based on alghoritm 3.74 of
-    D. Hankerson, 'Guide to Elliptic Curve Cryptography'.
-    Values computed for secp256k1.
+    Based on alghoritm 3.74 of D. Hankerson, 'Guide to Elliptic Curve
+    Cryptography'. Values computed for secp256k1.
     """
     if m < 0:
         raise ValueError(f"negative m: {hex(m)}")
 
     m %= ec.p
 
     # balanced length-two representation of a multiplier m.
```

### Comparing `btclib-2023.5.30/btclib/ec/curve_group_f.py` & `btclib-2023.7.12/btclib/ec/curve_group_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """CurveGroup explorer functions.
 
 These functions are meant to explore low-cardinality CurveGroup, for
 didactical (and fun) reason only.
 """
 from __future__ import annotations
```

### Comparing `btclib-2023.5.30/btclib/ec/libsecp256k1.py` & `btclib-2023.7.12/btclib/ec/libsecp256k1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Helper functions to use the libsecp256k1 python bindings."""
 
 
 from __future__ import annotations
 
 import contextlib
```

### Comparing `btclib-2023.5.30/btclib/ec/sec_point.py` & `btclib-2023.7.12/btclib/ec/sec_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """SEC compressed/uncompressed point representation."""
 
 from btclib.alias import Octets, Point
 from btclib.ec.curve import Curve, secp256k1
 from btclib.exceptions import BTClibValueError
 from btclib.utils import bytes_from_octets, hex_string
```

### Comparing `btclib-2023.5.30/btclib/ecc/__init__.py` & `btclib-2023.7.12/btclib/ecc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.ecc."""
 
 from btclib.ecc.bip340_nonce import bip340_nonce_
 from btclib.ecc.dh import ansi_x9_63_kdf, diffie_hellman
 from btclib.ecc.pedersen import second_generator
 
 __all__ = ["bip340_nonce_", "second_generator", "ansi_x9_63_kdf", "diffie_hellman"]
```

### Comparing `btclib-2023.5.30/btclib/ecc/bip340_nonce.py` & `btclib-2023.7.12/btclib/ecc/bip340_nonce.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Deterministic generation of the ephemeral key following BIP340.
 
 https://github.com/bitcoin/bips/blob/master/bip-0340.mediawiki
 
 The BIP340-Schnorr scheme advocates a custom deterministic algorithm
 for the ephemeral key (nonce) used for signing,
 instead of the RFC6979 standard:
```

### Comparing `btclib-2023.5.30/btclib/ecc/bms.py` & `btclib-2023.7.12/btclib/ecc/bms.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Bitcoin message signing (BMS).
 
 Bitcoin uses a P2PKH address-based scheme for message signature: such
 a signature does prove the control of the private key corresponding to
 the address and, consequently, of the associated bitcoins (if any).
 Message signature adopts a custom compact 65-bytes (fixed size)
 serialization format (i.e. not the ASN.1 DER format used for
```

### Comparing `btclib-2023.5.30/btclib/ecc/borromean.py` & `btclib-2023.7.12/btclib/ecc/borromean.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Borromean signature functions."""
+
 from __future__ import annotations
 
 import secrets
 from hashlib import sha256 as hf  # FIXME any hf
 from typing import List, Sequence
 
 from btclib.alias import Octets, Point
```

### Comparing `btclib-2023.5.30/btclib/ecc/dh.py` & `btclib-2023.7.12/btclib/ecc/dh.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Diffie-Hellman elliptic curve key agreement scheme.
 
-Implementation of the Diffie-Hellman key agreement scheme using
-elliptic curve cryptography. A key agreement scheme is used
-by two entities to establish shared keying data, which will be
-later utilized e.g. in symmetric cryptographic scheme.
+Implementation of the Diffie-Hellman key agreement scheme using elliptic
+curve cryptography. A key agreement scheme is used by two entities to
+establish shared keying data, which will be later utilized e.g. in
+symmetric cryptographic scheme.
 
 The two entities must agree on the elliptic curve and key derivation
 function to use.
 """
 from __future__ import annotations
 
 from hashlib import sha256
```

### Comparing `btclib-2023.5.30/btclib/ecc/dsa.py` & `btclib-2023.7.12/btclib/ecc/dsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Elliptic Curve Digital Signature Algorithm (ECDSA).
 
 Implementation according to SEC 1 v.2:
 
 http://www.secg.org/sec1-v2.pdf
 
 specialized with bitcoin canonical 'lower-s' form
@@ -46,28 +45,31 @@
 def _serialize_scalar(scalar: int) -> bytes:
     # 'highest bit set' padding included here
     scalar_size = scalar.bit_length() // 8 + 1
     scalar_bytes = scalar.to_bytes(scalar_size, byteorder="big", signed=False)
     return _DER_SCALAR_MARKER + var_bytes.serialize(scalar_bytes)
 
 
-def _deserialize_scalar(sig_data_stream: BytesIO) -> int:
+def _deserialize_scalar(sig_data_stream: BytesIO, strict: bool = True) -> int:
     marker = sig_data_stream.read(1)
     if marker != _DER_SCALAR_MARKER:
         err_msg = f"invalid value header: {marker.hex()}"
         err_msg += f", instead of integer element {_DER_SCALAR_MARKER.hex()}"
         raise BTClibValueError(err_msg)
 
     r_bytes = var_bytes.parse(sig_data_stream, forbid_zero_size=True)
-    if r_bytes[0] == 0 and r_bytes[1] < 0x80:
+    if r_bytes[0] == 0 and r_bytes[1] < 0x80 and strict:
         raise BTClibValueError("invalid 'highest bit set' padding")
-    if r_bytes[0] >= 0x80:
+
+    scalar = int.from_bytes(r_bytes, byteorder="big", signed=False)
+
+    if r_bytes[0] >= 0x80 and strict:
         raise BTClibValueError("invalid negative scalar")
 
-    return int.from_bytes(r_bytes, byteorder="big", signed=False)
+    return abs(scalar)
 
 
 @dataclass(frozen=True)
 class Sig:
     """ECDSA signature with strict ASN.1 DER serialization.
 
     The original Bitcoin implementation used OpenSSL to verify
@@ -158,15 +160,20 @@
             self.assert_valid()
 
         out = _serialize_scalar(self.r)
         out += _serialize_scalar(self.s)
         return _DER_SIG_MARKER + var_bytes.serialize(out)
 
     @classmethod
-    def parse(cls: type[Sig], data: BinaryData, check_validity: bool = True) -> Sig:
+    def parse(
+        cls: type[Sig],
+        data: BinaryData,
+        check_validity: bool = True,
+        strict: bool = True,
+    ) -> Sig:
         """Return a Sig by parsing binary data.
 
         Deserialize a strict ASN.1 DER representation of an ECDSA
         signature.
         """
         stream = bytesio_from_binarydata(data)
         ec = secp256k1
@@ -179,16 +186,16 @@
             raise BTClibValueError(err_msg)
 
         # [data-size][0x02][r-size][r][0x02][s-size][s]
         sig_data = var_bytes.parse(stream, forbid_zero_size=True)
 
         # [0x02][r-size][r][0x02][s-size][s]
         sig_data_substream = bytesio_from_binarydata(sig_data)
-        r = _deserialize_scalar(sig_data_substream)
-        s = _deserialize_scalar(sig_data_substream)
+        r = _deserialize_scalar(sig_data_substream, strict)
+        s = _deserialize_scalar(sig_data_substream, strict)
 
         # to prevent malleability
         # the sig_data_substream must have been consumed entirely
         if sig_data_substream.read(1) != b"":
             err_msg = "invalid DER sequence length"
             raise BTClibValueError(err_msg)
 
@@ -284,30 +291,31 @@
     nonce: PrvKey | None = None,
     lower_s: bool = True,
     ec: Curve = secp256k1,
     hf: HashF = sha256,
 ) -> Sig:
     """ECDSA signature with canonical low-s preference.
 
-    Implemented according to SEC 1 v.2
-    The message msg is first processed by hf, yielding the value
+    Implemented according to SEC 1 v.2 The message msg is first
+    processed by hf, yielding the value
 
-        msg_hash = hf(msg),
+    msg_hash = hf(msg),
 
     a sequence of bits of length *hf_len*.
 
     Normally, hf is chosen such that its output length *hf_len* is
     roughly equal to *nlen*, the bit-length of the group order *n*,
     since the overall security of the signature scheme will depend on
     the smallest of *hf_len* and *nlen*; however, the ECDSA standard
     supports all combinations of *hf_len* and *nlen*.
 
     RFC6979 is used for deterministic nonce.
 
-    See https://tools.ietf.org/html/rfc6979#section-3.2
+    See
+    https://tools.ietf.org/html/rfc6979#section-3.2
     """
     msg_hash = reduce_to_hlen(msg, hf)
     return sign_(msg_hash, prv_key, nonce, lower_s, ec, hf)
 
 
 def _assert_as_valid_(
     c: int, QJ: JacPoint, r: int, s: int, lower_s: bool, ec: Curve
```

### Comparing `btclib-2023.5.30/btclib/ecc/libsecp256k1.py` & `btclib-2023.7.12/btclib/ecc/libsecp256k1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Helper functions to use the libsecp256k1 python bindings."""
 
 from __future__ import annotations
 
 import contextlib
 import secrets
```

### Comparing `btclib-2023.5.30/btclib/ecc/pedersen.py` & `btclib-2023.7.12/btclib/ecc/pedersen.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Pedersen commitment functions.
 
 In a commitment scheme the committer:
 
 * decides (or is given) a secret message v
 * decides a random secret r
 * *commits* to v by applying the public commitment
```

### Comparing `btclib-2023.5.30/btclib/ecc/rfc6979_nonce.py` & `btclib-2023.7.12/btclib/ecc/rfc6979_nonce.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Deterministic generation of the ephemeral key following RFC6979.
 
 https://tools.ietf.org/html/rfc6979
 
 ECDSA and ECSSA need to produce, for each signature generation,
 a fresh random value (ephemeral key, hereafter designated as nonce).
 For effective security, nonce must be chosen randomly and uniformly
```

### Comparing `btclib-2023.5.30/btclib/ecc/sign_to_contract.py` & `btclib-2023.7.12/btclib/ecc/sign_to_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Include a commitment inside an elliptic curve DSA/SSA signature.
 
 Let commit_hash be the commitment value and R a curve point, then
 
-    e = hash(R||commit_hash)
+e = hash(R||commit_hash)
 
 is a commitment operation.
 
 When signing, an ephemeral secret key k is generated and its
-corresponding curve point R = kG is used. Here, instead of
-using (k, R), compute the commitment to commit_hash
+corresponding curve point R = kG is used. Here, instead of using (k, R),
+compute the commitment to commit_hash
 
-    e = hash(R||commit_hash),
+e = hash(R||commit_hash),
 
-tweak k with e and consequently substitute R with W = (k+e)G = R+eG,
-the proceed signing in the standard way, using (k+e, W).
+tweak k with e and consequently substitute R with W = (k+e)G = R+eG, the
+proceed signing in the standard way, using (k+e, W).
 
-When the committer/signer will reveal R and commit_hash,
-the verifier will check that
+When the committer/signer will reveal R and commit_hash, the verifier
+will check that
 
-    W.x = (R+eG).x
+W.x = (R+eG).x
 
 with e = hash(R||commit_hash)) and W.x being known from the signature.
 """
 from __future__ import annotations
 
 from hashlib import sha256
```

### Comparing `btclib-2023.5.30/btclib/ecc/ssa.py` & `btclib-2023.7.12/btclib/ecc/ssa.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Elliptic Curve Schnorr Signature Algorithm (ECSSA).
 
 This implementation is according to BIP340-Schnorr:
 
 https://github.com/bitcoin/bips/blob/master/bip-0340.mediawiki
 
 The BIP340-Schnorr scheme uses as public key the x-coordinate (field element)
@@ -241,23 +240,23 @@
     ec: Curve = secp256k1,
     hf: HashF = sha256,
 ) -> Sig:
     """Sign message according to BIP340 signature algorithm.
 
     The message msg is first processed by hf, yielding the value
 
-        msg_hash = hf(msg),
+    msg_hash = hf(msg),
 
     a sequence of bits of length *hf_len*.
 
     Normally, hf is chosen such that its output length *hf_len* is
     roughly equal to *nlen*, the bit-length of the group order *n*,
     since the overall security of the signature scheme will depend on
-    the smallest of *hf_len* and *nlen*; however, ECSSA
-    supports all combinations of *hf_len* and *nlen*.
+    the smallest of *hf_len* and *nlen*; however, ECSSA supports all
+    combinations of *hf_len* and *nlen*.
 
     The BIP340 deterministic nonce (not RFC6979) is used.
     """
     msg_hash = reduce_to_hlen(msg, hf)
     return sign_(msg_hash, prv_key, aux, ec, hf)
```

### Comparing `btclib-2023.5.30/btclib/exceptions.py` & `btclib-2023.7.12/btclib/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Expception classes.
 
-This are only meant to dicriminate between Exceptions being raised
-by btclib from those raised by other codebase.
+This are only meant to dicriminate between Exceptions being raised by
+btclib from those raised by other codebase.
 
-Users are usually better off just dealing with the regular
-ValueError, TypeError, and RuntimeError
-from which the btclib versions are derived.
+Users are usually better off just dealing with the regular ValueError,
+TypeError, and RuntimeError from which the btclib versions are derived.
 """
 
 
 class BTClibValueError(ValueError):
     pass
```

### Comparing `btclib-2023.5.30/btclib/hashes.py` & `btclib-2023.7.12/btclib/hashes.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Hash based helper functions."""
 from __future__ import annotations
 
 import hashlib
 from typing import Callable, Sequence
 
 from btclib.alias import HashF, Octets
@@ -31,14 +30,20 @@
 
 def ripemd160(octets: Octets) -> bytes:
     """Return the RIPEMD160(*) of the input octet sequence."""
     octets = bytes_from_octets(octets)
     return hashlib.new("ripemd160", octets).digest()
 
 
+def sha1(octets: Octets) -> bytes:
+    """Return the SHA1(*) of the input octet sequence."""
+    octets = bytes_from_octets(octets)
+    return hashlib.sha1(octets).digest()  # nosec
+
+
 def sha256(octets: Octets) -> bytes:
     """Return the SHA256(*) of the input octet sequence."""
     octets = bytes_from_octets(octets)
     return hashlib.sha256(octets).digest()
 
 
 def hash160(octets: Octets) -> bytes:
```

### Comparing `btclib-2023.5.30/btclib/mnemonic/__init__.py` & `btclib-2023.7.12/btclib/mnemonic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.mnemonic."""
 
 from btclib.mnemonic.entropy import (
     BinStr,
     Entropy,
     bin_str_entropy_from_bytes,
     bin_str_entropy_from_entropy,
```

### Comparing `btclib-2023.5.30/btclib/mnemonic/_data/english.txt` & `btclib-2023.7.12/btclib/mnemonic/_data/english.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/mnemonic/_data/italian.txt` & `btclib-2023.7.12/btclib/mnemonic/_data/italian.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/btclib/mnemonic/bip39.py` & `btclib-2023.7.12/btclib/mnemonic/bip39.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """BIP39 entropy / mnemonic / seed functions.
 
 https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki.
 
 Checksummed entropy (**ENT+CS**) is converted from/to mnemonic.
 
 * bits per word = bpw = 11
@@ -79,26 +78,25 @@
     checksum_bits = len(bytes_entropy) // 4
     return bin_str_entropy, checksum[:checksum_bits]
 
 
 def mnemonic_from_entropy(entropy: Entropy | None = None, lang: str = "en") -> Mnemonic:
     """Convert input entropy to BIP39 checksummed mnemonic sentence.
 
-    Input entropy can be expressed as
-    binary 0/1 string, bytes-like, or integer;
-    it must be 128, 160, 192, 224, or 256 bits.
+    Input entropy can be expressed as binary 0/1 string, bytes-like, or
+    integer; it must be 128, 160, 192, 224, or 256 bits.
 
-    In the case of binary 0/1 string and bytes-like,
-    leading zeros are not considered redundant padding.
+    In the case of binary 0/1 string and bytes-like, leading zeros are
+    not considered redundant padding.
 
     In the case of integer, where leading zeros cannot be represented,
     if the bit length is not an allowed value, then the binary 0/1
     string is padded with leading zeros up to the next allowed bit
-    length; if the integer bit length is longer than the maximum
-    length, then only the leftmost bits are retained.
+    length; if the integer bit length is longer than the maximum length,
+    then only the leftmost bits are retained.
     """
     if entropy is None or entropy == "":
         entropy = secrets.randbits(128)
     bin_str_entropy, checksum = _entropy_checksum(entropy)
     base = WORDLISTS.language_length(lang)
     indexes = wordlist_indexes_from_bin_str_entropy(bin_str_entropy + checksum, base)
     return mnemonic_from_indexes(indexes, lang)
```

### Comparing `btclib-2023.5.30/btclib/mnemonic/electrum.py` & `btclib-2023.7.12/btclib/mnemonic/electrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Electrum entropy / mnemonic / seed functions.
 
 Electrum mnemonic is versioned, conveying BIP32 derivation rule too.
 """
 from __future__ import annotations
 
 import hmac
@@ -68,19 +67,19 @@
 
 
 def mnemonic_from_entropy(
     mnemonic_type: str = "standard", entropy: Entropy | None = None, lang: str = "en"
 ) -> Mnemonic:
     """Convert input entropy to Electrum versioned mnemonic sentence.
 
-    Input entropy can be expressed as
-    binary 0/1 string, bytes-like, or integer.
+    Input entropy can be expressed as binary 0/1 string, bytes-like, or
+    integer.
 
-    In the case of binary 0/1 string and bytes-like,
-    leading zeros are considered redundant padding.
+    In the case of binary 0/1 string and bytes-like, leading zeros are
+    considered redundant padding.
     """
     if mnemonic_type not in _MNEMONIC_VERSIONS:
         err_msg = f"unknown electrum mnemonic version: '{mnemonic_type}'; "
         err_msg += f"not in {list(_MNEMONIC_VERSIONS.keys())}"
         raise BTClibValueError(err_msg)
     version = _MNEMONIC_VERSIONS[mnemonic_type]
```

### Comparing `btclib-2023.5.30/btclib/mnemonic/entropy.py` & `btclib-2023.7.12/btclib/mnemonic/entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Entropy conversion functions.
 
-Depending on the function, input entropy can be expressed
-as raw (i.e. binary 0/1 string), bytes, or integer
-and their equivalent representations.
+Depending on the function, input entropy can be expressed as raw (i.e.
+binary 0/1 string), bytes, or integer and their equivalent
+representations.
 
-Leading zeros in raw or bytes entropy
-are never considered redundant padding.
+Leading zeros in raw or bytes entropy are never considered redundant
+padding.
 
 Output entropy is always raw.
 """
 from __future__ import annotations
 
 import math
 import secrets
@@ -112,19 +111,19 @@
 
 
 def bin_str_entropy_from_bytes(
     bytes_entropy: Octets, bits: OneOrMoreInt = _bits
 ) -> BinStr:
     """Return raw entropy from the input Octets entropy.
 
-    Input entropy can be expressed as hex-string or bytes;
-    it is never padded to satisfy the bit-size requirement.
+    Input entropy can be expressed as hex-string or bytes; it is never
+    padded to satisfy the bit-size requirement.
 
-    If more bits than required are provided,
-    the leftmost ones are retained.
+    If more bits than required are provided, the leftmost ones are
+    retained.
 
     Default bit-sizes are 128, 160, 192, 224, 256, or 512 bits.
     """
     bytes_entropy = bytes_from_octets(bytes_entropy)
 
     # if a single int, make it a tuple
     if isinstance(bits, int):
@@ -155,21 +154,20 @@
 
 
 def bin_str_entropy_from_int(
     int_entropy: int | str, bits: OneOrMoreInt = _bits
 ) -> BinStr:
     """Return raw entropy from the input integer entropy.
 
-    Input entropy can be expressed as int
-    or string starting with "0x"/"0b";
-    it is front-padded with zeros digits
-    as much as necessary to satisfy the bit-size requirement.
+    Input entropy can be expressed as int or string starting with
+    "0x"/"0b"; it is front-padded with zeros digits as much as necessary
+    to satisfy the bit-size requirement.
 
-    If more bits than required are provided,
-    the leftmost ones are retained.
+    If more bits than required are provided, the leftmost ones are
+    retained.
 
     Default bit-sizes are 128, 160, 192, 224, 256, or 512 bits.
     """
     if isinstance(int_entropy, str):
         int_entropy = int_entropy.strip().lower()
         if int_entropy[:2] == "0b":
             int_entropy = int(int_entropy, 2)
@@ -198,19 +196,19 @@
     n_bits = next(v for v in bits if v >= n_bits)
     return bin_str.zfill(n_bits)
 
 
 def bin_str_entropy_from_str(str_entropy: str, bits: OneOrMoreInt = _bits) -> BinStr:
     """Return raw entropy from the input raw entropy.
 
-    Input entropy must be expressed as raw entropy;
-    it is never padded to satisfy the bit-size requirement.
+    Input entropy must be expressed as raw entropy; it is never padded
+    to satisfy the bit-size requirement.
 
-    If more bits than required are provided,
-    the leftmost ones are retained.
+    If more bits than required are provided, the leftmost ones are
+    retained.
 
     Default bit-sizes are 128, 160, 192, 224, 256, or 512 bits.
     """
     int(str_entropy, 2)
 
     # if a single int, make it a tuple
     if isinstance(bits, int):
@@ -278,22 +276,22 @@
     bits: int, dice_sides: int, rolls: list[int], shuffle: bool = True
 ) -> BinStr:
     """Return raw entropy from the input dice rolls.
 
     Dice rolls are represented by integers in the [1-dice_sides] range;
     there must be enough rolls to satisfy the bit-size requirement.
 
-    Only rolls having value in the [1-base] range are used,
-    with base being the highest power of 2 that is lower than the
-    dice_sides (e.g. for a traditional D6 dice, only rolls having value
-    in [1-4] are used; for a D20 dice, only rolls having value in
-    [1-16] are used; etc.). Rolls can also be shuffled.
+    Only rolls having value in the [1-base] range are used, with base
+    being the highest power of 2 that is lower than the dice_sides (e.g.
+    for a traditional D6 dice, only rolls having value in [1-4] are
+    used; for a D20 dice, only rolls having value in [1-16] are used;
+    etc.). Rolls can also be shuffled.
 
-    If more bits than required are provided,
-    the leftmost ones are retained.
+    If more bits than required are provided, the leftmost ones are
+    retained.
     """
     if dice_sides < 2:
         raise BTClibValueError(f"invalid dice base: {dice_sides}, must be >= 2")
     bits_per_roll = math.floor(math.log2(dice_sides))
     # used base
     base = 2**bits_per_roll
```

### Comparing `btclib-2023.5.30/btclib/mnemonic/mnemonic.py` & `btclib-2023.7.12/btclib/mnemonic/mnemonic.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Mnemonic sentence conversion from/to sequence of integer indexes."""
 from __future__ import annotations
 
 from os import path
 from typing import Sequence
 
 from btclib.exceptions import BTClibValueError
```

### Comparing `btclib-2023.5.30/btclib/network.py` & `btclib-2023.7.12/btclib/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Network constants and associated functions."""
 
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
 from os import path
```

### Comparing `btclib-2023.5.30/btclib/number_theory.py` & `btclib-2023.7.12/btclib/number_theory.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Number theory and modular arithmetic functions.
 
 Implementations originally from
 https://en.wikibooks.org/wiki/Algorithm_Implementation/Mathematics/Extended_Euclidean_algorithm
 and
 https://codereview.stackexchange.com/questions/43210/tonelli-shanks-algorithm-implementation-of-prime-modular-square-root/43267
 with the following modifications:
@@ -58,17 +57,16 @@
     err_msg += f"{hex_string(m)}" if m > 0xFFFFFFFF else f"{m}"
     raise BTClibValueError(err_msg)
 
 
 def legendre_symbol(a: int, p: int) -> int:
     """Compute the Legendre symbol a|p using Euler's criterion.
 
-    p is a prime, a is relatively prime to p (if p divides a,
-    then a|p = 0).
-    It returns 1 if a has a square root modulo p, -1 otherwise.
+    p is a prime, a is relatively prime to p (if p divides a, then a|p =
+    0). It returns 1 if a has a square root modulo p, -1 otherwise.
 
     https://codereview.stackexchange.com/questions/43210/tonelli-shanks-algorithm-implementation-of-prime-modular-square-root/43267
     """
     ls = pow(a, p >> 1, p)
     return -1 if ls == p - 1 else ls
```

### Comparing `btclib-2023.5.30/btclib/psbt/__init__.py` & `btclib-2023.7.12/btclib/psbt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.psbt."""
 
 from btclib.psbt.psbt import Psbt, combine_psbts, extract_tx, finalize_psbt, join_psbts
 from btclib.psbt.psbt_in import PsbtIn
 from btclib.psbt.psbt_out import PsbtOut
 from btclib.psbt.psbt_utils import (
     assert_valid_unknown,
```

### Comparing `btclib-2023.5.30/btclib/psbt/psbt.py` & `btclib-2023.7.12/btclib/psbt/psbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Partially Signed Bitcoin Transaction (Psbt) dataclass and functions.
 
 https://github.com/bitcoin/bips/blob/master/bip-0174.mediawiki
 """
 from __future__ import annotations
 
 import base64
 import random
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Callable, Mapping, Sequence, TypeVar
+from typing import Any, Callable, Mapping, Sequence, TypeVar, cast
 
-from btclib.alias import Octets, String
+from btclib.alias import Octets, ScriptList, String
 from btclib.bip32 import (
     BIP32KeyOrigin,
     HdKeyPaths,
     assert_valid_hd_key_paths,
     decode_from_bip32_derivs,
     decode_hd_key_paths,
     encode_to_bip32_derivs,
@@ -186,21 +185,24 @@
             "unknown": dict(sorted(encode_dict_bytes_bytes(self.unknown).items())),
         }
 
     @classmethod
     def from_dict(
         cls: type[Psbt], dict_: Mapping[str, Any], check_validity: bool = True
     ) -> Psbt:
+        hd_key_paths = cast(
+            Mapping[Octets, BIP32KeyOrigin],
+            decode_from_bip32_derivs(dict_["bip32_derivs"]),
+        )
         return cls(
             Tx.from_dict(dict_["tx"]),
             [PsbtIn.from_dict(psbt_in, False) for psbt_in in dict_["inputs"]],
             [PsbtOut.from_dict(psbt_out, False) for psbt_out in dict_["outputs"]],
             dict_["version"],
-            # FIXME
-            decode_from_bip32_derivs(dict_["bip32_derivs"]),  # type: ignore[arg-type]
+            hd_key_paths,
             dict_["unknown"],
             check_validity,
         )
 
     def serialize(self, check_validity: bool = True) -> bytes:
         if check_validity:
             self.assert_valid()
@@ -389,25 +391,23 @@
 
 
 def finalize_psbt(psbt: Psbt) -> Psbt:
     """Finalize the Psbt.
 
     The Input Finalizer must only accept a PSBT.
 
-    For each input, the Input Finalizer determines
-    if the input has enough data to pass validation.
-    If it does, it must construct the
-    0x07 Finalized scriptSig and
-    0x08 Finalized scriptWitness
-    and place them into the input key-value map.
-
-    All other data except the UTXO and unknown fields
-    in the input key-value map should be cleared from the PSBT.
-    The UTXO should be kept to allow Transaction Extractors
-    to verify the final network serialized transaction.
+    For each input, the Input Finalizer determines if the input has
+    enough data to pass validation. If it does, it must construct the
+    0x07 Finalized scriptSig and 0x08 Finalized scriptWitness and place
+    them into the input key-value map.
+
+    All other data except the UTXO and unknown fields in the input key-
+    value map should be cleared from the PSBT. The UTXO should be kept
+    to allow Transaction Extractors to verify the final network
+    serialized transaction.
     """
     psbt = deepcopy(psbt)
     psbt.assert_valid()
     # TODO finalizers must fail to finalize inputs
     # which have signatures that do not match the specified sign_ type
     for psbt_in in psbt.inputs:
         if not psbt_in.partial_sigs:
@@ -416,45 +416,45 @@
         # https://github.com/bitcoin/bips/blob/master/bip-0147.mediawiki#motivation
         cmds: list[bytes] = [b""] if len(sigs) > 1 else []
         cmds += sigs
         if psbt_in.witness_script:
             psbt_in.final_script_sig = serialize([psbt_in.redeem_script])
             psbt_in.final_script_witness = Witness(cmds + [psbt_in.witness_script])
         else:
-            psbt_in.final_script_sig = serialize(cmds + [psbt_in.redeem_script])
+            psbt_in.final_script_sig = serialize(
+                cast(ScriptList, cmds + [psbt_in.redeem_script])
+            )
         psbt_in.partial_sigs = {}
         psbt_in.sig_hash_type = None
         psbt_in.redeem_script = b""
         psbt_in.witness_script = b""
         psbt_in.hd_key_paths = {}
     return psbt
 
 
 def extract_tx(psbt: Psbt, check_validity: bool = True) -> Tx:
     """Extract the Tx fro the Psbt.
 
-    The Transaction Extractor must only accept a PSBT.
-    It checks whether all inputs have complete scriptSigs
-    and scriptWitnesses by checking for the presence of
-    0x07 Finalized scriptSig and 0x08 Finalized scriptWitness typed
-    records.
-
-    If they do, the Transaction Extractor should construct
-    complete scriptSigs and scriptWitnesses and encode them
-    into network serialized transactions.
-    Otherwise the Extractor must not modify the PSBT.
-
-    The Extractor should produce a fully valid,
-    network serialized transaction if all inputs are complete.
-
-    The Transaction Extractor does not need to know
-    how to interpret scripts in order to extract
-    the network serialized transaction.
-    However it may be able to in order to validate
-    the network serialized transaction at the same time.
+    The Transaction Extractor must only accept a PSBT. It checks whether
+    all inputs have complete scriptSigs and scriptWitnesses by checking
+    for the presence of 0x07 Finalized scriptSig and 0x08 Finalized
+    scriptWitness typed records.
+
+    If they do, the Transaction Extractor should construct complete
+    scriptSigs and scriptWitnesses and encode them into network
+    serialized transactions. Otherwise the Extractor must not modify the
+    PSBT.
+
+    The Extractor should produce a fully valid, network serialized
+    transaction if all inputs are complete.
+
+    The Transaction Extractor does not need to know how to interpret
+    scripts in order to extract the network serialized transaction.
+    However it may be able to in order to validate the network
+    serialized transaction at the same time.
     """
     if check_validity:
         psbt.assert_valid()
 
     tx = psbt.tx
     for tx_in, psbt_input in zip(tx.vin, psbt.inputs):
         tx_in.script_sig = psbt_input.final_script_sig
@@ -482,15 +482,15 @@
     if len(sequence_a) != len(sequence_b):
         raise BTClibValueError("sequences must have same length")
 
     tmp = list(zip(sequence_a, sequence_b))
     if ordering_func is None:
         random.shuffle(tmp)
     else:
-        tmp.sort(key=lambda t: ordering_func(t[0]))  # type: ignore
+        tmp.sort(key=lambda t: ordering_func(t[0]))  # type: ignore[misc]
     tuple_a, tuple_b = zip(*tmp)
     return list(tuple_a), list(tuple_b)
 
 
 def _ensure_consistency(psbts: Sequence[Psbt]) -> None:
     """Check validity of each psbt and conflicts in key_paths or unknown."""
     key_paths: dict[bytes, BIP32KeyOrigin] = {}
```

### Comparing `btclib-2023.5.30/btclib/script/__init__.py` & `btclib-2023.7.12/btclib/script/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.script."""
 
 from btclib.script.script import Command, Script, op_int, parse, serialize
 from btclib.script.script_pub_key import (
     ScriptPubKey,
     address,
     assert_nulldata,
```

### Comparing `btclib-2023.5.30/btclib/script/script.py` & `btclib-2023.7.12/btclib/script/script.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Bitcoin Script.
 
 https://en.bitcoin.it/wiki/Script
 
-Scripts are represented by list[Command], where Command = Union[int, str, bytes]
+Scripts are represented by List[Command], where Command = Union[int, str, bytes]
 
 * ascii string are for opcodes (e.g. 'OP_HASH160', 'OP_1', 'OP_1NEGATE', etc.)
 * hex-string or bytes (i.e., Octets) are for data
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Sequence, Union
+from typing import Sequence
 from warnings import warn
 
-from btclib.alias import BinaryData, Octets
+from btclib.alias import BinaryData, Command, Octets, ScriptList
 from btclib.exceptions import BTClibValueError
 from btclib.utils import bytes_from_octets, bytesio_from_binarydata, encode_num
 
 BYTE_FROM_OP_CODE_NAME = {
     # Constants
     "OP_0": b"\x00",
     "OP_FALSE": b"\x00",
     "OP_PUSHDATA1": b"\x4c",
     "OP_PUSHDATA2": b"\x4d",
     "OP_PUSHDATA4": b"\x4e",
     "OP_1NEGATE": b"\x4f",
+    "OP_RESERVED": b"\x50",
     "OP_1": b"\x51",
     "OP_TRUE": b"\x51",
     "OP_2": b"\x52",
     "OP_3": b"\x53",
     "OP_4": b"\x54",
     "OP_5": b"\x55",
     "OP_6": b"\x56",
@@ -137,20 +137,22 @@
     "OP_NOP8": b"\xb7",
     "OP_NOP9": b"\xb8",
     "OP_NOP10": b"\xb9",
     # Taproot
     "OP_CHECKSIGADD": b"\xba",
 }
 
+
 OP_CODE_NAME_FROM_INT = {
     0: "OP_0",
     76: "OP_PUSHDATA1",
     77: "OP_PUSHDATA2",
     78: "OP_PUSHDATA4",
     79: "OP_1NEGATE",
+    80: "OP_RESERVED",
     81: "OP_1",
     82: "OP_2",
     83: "OP_3",
     84: "OP_4",
     85: "OP_5",
     86: "OP_6",
     87: "OP_7",
@@ -247,32 +249,24 @@
     if i == -1:
         return "OP_1NEGATE"
     if 0 <= i <= 16:
         return f"OP_{i}"
     raise BTClibValueError(f"invalid OP_INT: {i}")
 
 
-Command = Union[int, str, bytes]
-
-
 def _serialize_int_command(command: int) -> bytes:
     if -1 <= command <= 16:
         warn(f"consider using OP_{command} instead")
     return _serialize_bytes_command(encode_num(command))
 
 
 def _serialize_str_command(command: str) -> bytes:
     command = command.strip().upper()
     if command in BYTE_FROM_OP_CODE_NAME:
         return BYTE_FROM_OP_CODE_NAME[command]
-    if command.startswith("OP_SUCCESS"):
-        x = int(command[10:])
-        if x in OP_CODE_NAME_FROM_INT or 0 < x < 76:
-            raise BTClibValueError(f"invalid OP_SUCCESS number: {x}")
-        return x.to_bytes(1, "little")
     try:
         data = bytes.fromhex(command)
     except ValueError as e:
         raise BTClibValueError(f"invalid string command: {command}") from e
     return _serialize_bytes_command(data)
 
 
@@ -307,23 +301,26 @@
 
 def serialize(script: Sequence[Command]) -> bytes:
     r: list[bytes] = []
     for command in script:
         if isinstance(command, int):
             r.append(_serialize_int_command(command))
         elif isinstance(command, str):
-            r.append(_serialize_str_command(command))
+            if "UNKNOWN_OP_CODE_" in command:
+                r.append(int(command[16:]).to_bytes(1, "big"))
+            else:
+                r.append(_serialize_str_command(command))
         else:  # must be bytes
             r.append(_serialize_bytes_command(command))
     return b"".join(r)
 
 
-def parse(stream: BinaryData, exit_on_op_success: bool = False) -> list[Command]:
+def parse(stream: BinaryData, accept_unknown: bool = False) -> ScriptList:
     s = bytesio_from_binarydata(stream)
-    r: list[Command] = []  # initialize the result list
+    r: ScriptList = []  # initialize the result list
 
     while True:
         t = s.read(1)  # get one byte
         if not t:
             break
         i = t[0]  # convert the first byte to an integer
         if 0 < i <= 78:  # push
@@ -332,50 +329,51 @@
                 # i == 76 -> OP_PUSHDATA1 | 1-byte-data-length | data
                 # i == 77 -> OP_PUSHDATA2 | 2-byte-data-length | data
                 x = i - 75
                 if i == 78:  # OP_PUSHDATA4 | 4-byte-data-length | data
                     x = 4
                 y = s.read(x)
                 if len(y) != x:
-                    raise BTClibValueError("not enough data for pushdata length")
+                    raise BTClibValueError("Not enough data for pushdata length")
                 data_length = int.from_bytes(y, byteorder="little")
-                if data_length > 520:
-                    raise BTClibValueError(f"invalid pushdata length: {data_length}")
+            if data_length > 520:
+                raise BTClibValueError(f"Invalid pushdata length: {data_length}")
             data = s.read(data_length)
             if len(data) != data_length:
-                raise BTClibValueError("not enough data for pushdata")
+                raise BTClibValueError("Not enough data for pushdata")
             command = data.hex().upper()
         elif i in OP_CODE_NAME_FROM_INT:  # OP_CODE
             command = OP_CODE_NAME_FROM_INT[i]
             # Opcodes which take integers and bools off the stack require
             # that they be no more than 4 bytes long.
             # If this is the case, parse that command as int
             # t = r[-1]
             # if isinstance(t, bytes) and len(t) <= 4:
             #    r[-1] = decode_num(t)
-        else:  # OP_SUCCESSx
-            command = f"OP_SUCCESS{i}"
-            if exit_on_op_success:
-                return ["OP_SUCCESS"]
+        elif accept_unknown:
+            # https://bitcoin.stackexchange.com/a/98652/111488
+            command = f"UNKNOWN_OP_CODE_{i}"
 
+        else:
+            raise BTClibValueError("Unknown op code")
         r.append(command)
 
     return r
 
 
 @dataclass
 class Script:
-    # Bitcoin script expressed as list[Command]
+    # Bitcoin script expressed as ScriptList
     # e.g. [OP_HASH160, script_h160, OP_EQUAL]
     # or Octets of its byte-encoded representation
     script: bytes
 
     @property
-    def asm(self) -> list[Command]:
-        return parse(self.script)
+    def asm(self) -> ScriptList:
+        return parse(self.script, accept_unknown=True)
 
     def __add__(self, other: Script) -> Script:
         return (
             Script(self.script + other.script)
             if isinstance(other, Script)
             else NotImplemented
         )
```

### Comparing `btclib-2023.5.30/btclib/script/script_pub_key.py` & `btclib-2023.7.12/btclib/script/script_pub_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """ScriptPubKey class and functions."""
 
 from __future__ import annotations
 
 from typing import Callable, Sequence
 
 from btclib import b32, b58, var_bytes
-from btclib.alias import Octets, String
+from btclib.alias import Octets, ScriptList, String
 from btclib.ec import point_from_octets
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash160, sha256
 from btclib.network import NETWORKS
-from btclib.script.script import Command, Script, op_int, serialize
+from btclib.script.script import Script, op_int, serialize
 from btclib.script.taproot import TaprootScriptTree, output_pubkey
 from btclib.to_pub_key import Key, pub_keyinfo_from_key
 from btclib.utils import bytes_from_octets, bytesio_from_binarydata
 
 
 def address(script_pub_key: Octets, network: str = "mainnet") -> str:
     """Return the bech32/base58 address from a script_pub_key."""
@@ -176,14 +175,29 @@
         raise BTClibValueError(err_msg)
 
 
 def is_nulldata(script_pub_key: Octets) -> bool:
     return _is_funct(assert_nulldata, script_pub_key)
 
 
+def assert_segwit(script_pub_key: Octets) -> None:
+    # doesn't check if script_pub_key is a valid script
+    script_pub_key = bytes_from_octets(script_pub_key)
+    if not (script_pub_key[0] == 0 or 0x51 <= script_pub_key[0] <= 0x60):
+        raise BTClibValueError()
+    if len(script_pub_key) == 1 or not 2 <= script_pub_key[1] <= 40:
+        raise BTClibValueError()
+    if len(script_pub_key) != script_pub_key[1] + 2:
+        raise BTClibValueError()
+
+
+def is_segwit(script_pub_key: Octets) -> bool:
+    return _is_funct(assert_segwit, script_pub_key)
+
+
 def assert_p2wpkh(script_pub_key: Octets) -> None:
     script_pub_key = bytes_from_octets(script_pub_key, 22)
     # p2wpkh [OP_0, pub_key hash]
     # 0x0014{20-byte pub_key hash}
     if script_pub_key[0] != 0:
         err_msg = f"invalid witness version: {script_pub_key[0]}"
         err_msg += " instead of 0"
@@ -346,15 +360,15 @@
         """Return the ScriptPubKey of the input bech32/base58 address."""
         if b32.has_segwit_prefix(addr):
             wit_ver, wit_prg, network = b32.witness_from_address(addr)
             return cls(serialize([op_int(wit_ver), wit_prg]), network, check_validity)
 
         script_type, h160, network = b58.h160_from_address(addr)
         if script_type == "p2sh":
-            commands: list[Command] = ["OP_HASH160", h160, "OP_EQUAL"]
+            commands: ScriptList = ["OP_HASH160", h160, "OP_EQUAL"]
         else:  # it must be "p2pkh"
             commands = [
                 "OP_DUP",
                 "OP_HASH160",
                 h160,
                 "OP_EQUALVERIFY",
                 "OP_CHECKSIG",
```

### Comparing `btclib-2023.5.30/btclib/script/sig_hash.py` & `btclib-2023.7.12/btclib/script/sig_hash.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,41 +3,37 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Transaction hashes to be signed and their hash types.
 
 - https://medium.com/@bitaps.com/exploring-bitcoin-signature-hash-types-15427766f0a9
 - https://raghavsood.com/blog/2018/06/10/bitcoin-signature-types-sighash
 - https://wiki.bitcoinsv.io/index.php/SIGHASH_flags
 """
 
 from __future__ import annotations
 
-from copy import deepcopy
-from typing import Sequence
-
 from btclib import var_bytes
-from btclib.alias import Octets
+from btclib.alias import Octets, ScriptList
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash256, sha256, tagged_hash
-from btclib.script.script import Command, parse, serialize
+from btclib.script.script import parse, serialize
 from btclib.script.script_pub_key import (
     ScriptPubKey,
     is_p2sh,
     is_p2tr,
     is_p2wpkh,
     is_p2wsh,
     type_and_payload,
 )
-from btclib.tx import Tx, TxOut
+from btclib.tx import Tx, TxIn, TxOut
 from btclib.utils import bytes_from_octets
 
 DEFAULT = 0
 ALL = 1
 NONE = 2
 SINGLE = 3
 ANYONECANPAY = 0b10000000
@@ -54,54 +50,100 @@
 
 
 def assert_valid_hash_type(hash_type: int) -> None:
     if hash_type not in SIG_HASH_TYPES:
         raise BTClibValueError(f"invalid sig_hash type: {hex(hash_type)}")
 
 
+# TODO: should remove signature even if not standard
 def legacy_script(script_pub_key: Octets) -> list[bytes]:
     script_s: list[bytes] = []
-    current_script: list[Command] = []
-    for cmd in parse(script_pub_key)[::-1]:
-        if cmd == "OP_CODESEPARATOR":
+    current_script: ScriptList = []
+    for token in parse(script_pub_key)[::-1]:
+        if token == "OP_CODESEPARATOR":  # nosec required for python < 3.8
             script_s.append(serialize(current_script[::-1]))
         else:
-            current_script.append(cmd)
+            current_script.append(token)
     script_s.append(serialize(current_script[::-1]))
     return script_s[::-1]
 
 
-# FIXME remove OP_CODESEPARATOR only if executed
+# FIXME: remove OP_CODESEPARATOR only if executed
 def witness_v0_script(script_pub_key: Octets) -> list[bytes]:
     script_type, payload = type_and_payload(script_pub_key)
 
     if script_type == "p2wpkh":
         script = serialize(
             ["OP_DUP", "OP_HASH160", payload, "OP_EQUALVERIFY", "OP_CHECKSIG"]
         )
         return [script]
 
     script_s: list[bytes] = []
-    current_script: list[Command] = []
-    for cmd in parse(script_pub_key)[::-1]:
-        if cmd == "OP_CODESEPARATOR":
+    current_script: ScriptList = []
+    for token in parse(script_pub_key)[::-1]:
+        if token == "OP_CODESEPARATOR":  # nosec required for python < 3.8
             script_s.append(serialize(current_script[::-1]))
-        current_script.append(cmd)
+        current_script.append(token)
     script_s.append(serialize(current_script[::-1]))
     return script_s[::-1]
 
 
-def legacy(script_: Octets, tx: Tx, vin_i: int, hash_type: int) -> bytes:
-    script_ = bytes_from_octets(script_)
+def taproot_annex_and_ext(
+    tx: Tx, prevouts: list[TxOut], vin_i: int
+) -> tuple[bytes, bytes]:
+    witness = tx.vin[vin_i].script_witness
+    if len(witness.stack) == 0:
+        raise BTClibValueError("Empty stack")
+
+    annex = b""
+    if len(witness.stack) >= 2 and witness.stack[-1][0] == 0x50:
+        annex = witness.stack[-1]
+        witness.stack = witness.stack[:-1]
+
+    ext = b""
+    if len(witness.stack) > 1:
+        leaf_version = witness.stack[-1][0] & 0xFE
+        preimage = leaf_version.to_bytes(1, "big")
+        preimage += var_bytes.serialize(witness.stack[-2])
+        tapleaf_hash = tagged_hash(b"TapLeaf", preimage)
+        ext = tapleaf_hash + b"\x00\xff\xff\xff\xff"
+
+    return annex, ext
+
+
+def legacy(script_code: Octets, tx: Tx, vin_i: int, hash_type: int) -> bytes:
+    script_code = bytes_from_octets(script_code)
+
+    new_tx = Tx(
+        version=tx.version,
+        lock_time=tx.lock_time,
+        vin=[],
+        vout=[],
+        check_validity=False,
+    )
+
+    for txin in tx.vin:
+        new_tx.vin.append(
+            TxIn(
+                prev_out=txin.prev_out,
+                script_sig=b"",
+                sequence=txin.sequence,
+                check_validity=False,
+            )
+        )
+    for txout in tx.vout:
+        new_tx.vout.append(
+            TxOut(
+                value=txout.value,
+                script_pub_key=txout.script_pub_key,
+                check_validity=False,
+            )
+        )
+    new_tx.vin[vin_i].script_sig = script_code
 
-    new_tx = deepcopy(tx)
-    for txin in new_tx.vin:
-        txin.script_sig = b""
-    # TODO delete sig from script_ (even if non standard)
-    new_tx.vin[vin_i].script_sig = script_
     if hash_type & 0x1F is NONE:
         new_tx.vout = []
         for i, txin in enumerate(new_tx.vin):
             if i != vin_i:
                 txin.sequence = 0
 
     if hash_type & 0x1F == SINGLE:
@@ -123,21 +165,27 @@
     preimage += hash_type.to_bytes(4, byteorder="little", signed=False)
 
     return hash256(preimage)
 
 
 # https://github.com/bitcoin/bitcoin/blob/4b30c41b4ebf2eb70d8a3cd99cf4d05d405eec81/test/functional/test_framework/script.py#L673
 def segwit_v0(
-    script_: Octets, tx: Tx, vin_i: int, hash_type: int, amount: int
+    script_code: Octets,
+    tx: Tx,
+    vin_i: int,
+    hash_type: int,
+    amount: int,
 ) -> bytes:
-    script_ = bytes_from_octets(script_)
+    script_code = bytes_from_octets(script_code)
 
     hash_prev_outs = b"\x00" * 32
     if not hash_type & ANYONECANPAY:
-        hash_prev_outs = b"".join([vin.prev_out.serialize() for vin in tx.vin])
+        hash_prev_outs = b"".join(
+            [vin.prev_out.serialize(check_validity=False) for vin in tx.vin]
+        )
         hash_prev_outs = hash256(hash_prev_outs)
 
     hash_seqs = b"\x00" * 32
     if (
         not (hash_type & ANYONECANPAY)
         and (hash_type & 0x1F) != SINGLE
         and (hash_type & 0x1F) != NONE
@@ -148,46 +196,50 @@
                 for vin in tx.vin
             ]
         )
         hash_seqs = hash256(hash_seqs)
 
     hash_outputs = b"\x00" * 32
     if hash_type & 0x1F not in (SINGLE, NONE):
-        hash_outputs = b"".join([vout.serialize() for vout in tx.vout])
+        hash_outputs = b"".join(
+            [vout.serialize(check_validity=False) for vout in tx.vout]
+        )
         hash_outputs = hash256(hash_outputs)
     elif (hash_type & 0x1F) == SINGLE and vin_i < len(tx.vout):
-        hash_outputs = hash256(tx.vout[vin_i].serialize())
+        hash_outputs = hash256(tx.vout[vin_i].serialize(check_validity=False))
 
     preimage = b"".join(
         [
             tx.version.to_bytes(4, byteorder="little", signed=False),
             hash_prev_outs,
             hash_seqs,
-            tx.vin[vin_i].prev_out.serialize(),
-            var_bytes.serialize(script_),
+            tx.vin[vin_i].prev_out.serialize(check_validity=False),
+            var_bytes.serialize(script_code),
             amount.to_bytes(8, byteorder="little", signed=False),  # value
             tx.vin[vin_i].sequence.to_bytes(4, byteorder="little", signed=False),
             hash_outputs,
             tx.lock_time.to_bytes(4, byteorder="little", signed=False),
             hash_type.to_bytes(4, byteorder="little", signed=False),
         ]
     )
     return hash256(preimage)
 
 
 def taproot(
     transaction: Tx,
     input_index: int,
-    amounts: Sequence[int],
-    scriptpubkeys: Sequence[ScriptPubKey],
+    prevouts: list[TxOut],
     hashtype: int,
     ext_flag: int,
     annex: bytes,
     message_extension: bytes,
 ) -> bytes:
+    amounts = [x.value for x in prevouts]
+    scriptpubkeys = [x.script_pub_key for x in prevouts]
+
     if hashtype not in SIG_HASH_TYPES:
         raise BTClibValueError(f"Unknown hash type: {hashtype}")
     if hashtype & 0x03 == SINGLE and input_index >= len(transaction.vout):
         raise BTClibValueError("Sighash single wihout a corresponding output")
 
     preimage = b"\x00"
     preimage += hashtype.to_bytes(1, "little")
@@ -238,57 +290,28 @@
     return tagged_hash(b"TapSighash", preimage)
 
 
 def from_tx(prevouts: list[TxOut], tx: Tx, vin_i: int, hash_type: int) -> bytes:
     script = prevouts[vin_i].script_pub_key.script
 
     if is_p2tr(script):
-        return _script_from_p2tr(prevouts, tx, vin_i, hash_type)
+        annex, ext = taproot_annex_and_ext(tx, prevouts, vin_i)
+        return taproot(tx, vin_i, prevouts, hash_type, int(bool(ext)), annex, ext)
 
+    # handle all p2sh-wrapped scripts
     if is_p2sh(script):
         script = tx.vin[vin_i].script_sig
-        if is_p2tr(script):
-            raise BTClibValueError("taproot scripts cannot be wrapped in p2sh")
 
     if is_p2wpkh(script):
-        script_ = witness_v0_script(script)[0]
-        return segwit_v0(script_, tx, vin_i, hash_type, prevouts[vin_i].value)
+        script_code = witness_v0_script(script)[0]
+        return segwit_v0(script_code, tx, vin_i, hash_type, prevouts[vin_i].value)
 
     if is_p2wsh(script):
         # the real script is contained in the witness
-        script_ = witness_v0_script(tx.vin[vin_i].script_witness.stack[-1])[0]
-        return segwit_v0(script_, tx, vin_i, hash_type, prevouts[vin_i].value)
-
-    script_ = legacy_script(script)[0]
-    return legacy(script_, tx, vin_i, hash_type)
-
-
-def _script_from_p2tr(
-    prevouts: Sequence[TxOut], tx: Tx, vin_i: int, hash_type: int
-) -> bytes:
-    witness = tx.vin[vin_i].script_witness
-    if len(witness.stack) == 0:
-        raise BTClibValueError("empty stack")
-
-    annex = b""
-    if len(witness.stack) >= 2 and witness.stack[-1][0] == 0x50:
-        annex = witness.stack[-1]
-        witness.stack = witness.stack[:-1]
+        script_code = witness_v0_script(tx.vin[vin_i].script_witness.stack[-1])[0]
+        return segwit_v0(script_code, tx, vin_i, hash_type, prevouts[vin_i].value)
 
-    ext = b""
-    if len(witness.stack) > 1:
-        leaf_version = witness.stack[-1][0] & 0xFE
-        preimage = leaf_version.to_bytes(1, "big")
-        preimage += var_bytes.serialize(witness.stack[-2])
-        tapleaf_hash = tagged_hash(b"TapLeaf", preimage)
-        ext = tapleaf_hash + b"\x00\xff\xff\xff\xff"
+    if is_p2tr(script):
+        raise BTClibValueError("Taproot scripts cannot be wrapped in p2sh")
 
-    return taproot(
-        tx,
-        vin_i,
-        [x.value for x in prevouts],
-        [x.script_pub_key for x in prevouts],
-        hash_type,
-        int(bool(ext)),
-        annex,
-        ext,
-    )
+    script_code = legacy_script(script)[0]
+    return legacy(script_code, tx, vin_i, hash_type)
```

### Comparing `btclib-2023.5.30/btclib/script/witness.py` & `btclib-2023.7.12/btclib/script/witness.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Witness (list[bytes]) class."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Mapping, Sequence
```

### Comparing `btclib-2023.5.30/btclib/to_prv_key.py` & `btclib-2023.7.12/btclib/to_prv_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Functions for conversions between different private key formats."""
 from __future__ import annotations
 
 import contextlib
 from typing import Tuple, Union
 
 from btclib.alias import String
```

### Comparing `btclib-2023.5.30/btclib/to_pub_key.py` & `btclib-2023.7.12/btclib/to_pub_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Functions for conversions between different public key formats."""
 from __future__ import annotations
 
 import contextlib
 from typing import Tuple, Union
 
 from btclib.alias import Point
```

### Comparing `btclib-2023.5.30/btclib/tx/__init__.py` & `btclib-2023.7.12/btclib/tx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Module btclib.tx."""
 
 from btclib.tx.out_point import OutPoint
 from btclib.tx.tx import Tx, join_txs
 from btclib.tx.tx_in import TxIn
 from btclib.tx.tx_out import TxOut
```

### Comparing `btclib-2023.5.30/btclib/tx/out_point.py` & `btclib-2023.7.12/btclib/tx/out_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """OutPoint dataclass.
 
 Dataclass encapsulating tx_id and vout.
 """
 
 
 from __future__ import annotations
```

### Comparing `btclib-2023.5.30/btclib/tx/tx.py` & `btclib-2023.7.12/btclib/tx/tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Transaction (Tx) class.
 
 Dataclass encapsulating version, lock_time,
 vin (list[TxIn]), and vout (list[TxOut]).
 
 - https://en.bitcoin.it/wiki/Transaction
 - https://learnmeabitcoin.com/guide/coinbase-transaction
@@ -181,14 +180,22 @@
         self.assert_valid()
 
         # should be a 4-bytes __signed__ integer
         if not 0 < self.version <= 0x7FFFFFFF:
             raise BTClibValueError(f"invalid version: {self.version}")
 
     def assert_valid(self) -> None:
+        if self.is_coinbase():
+            if not 2 <= len(self.vin[0].script_sig) <= 100:
+                raise BTClibValueError("Invalid coinbase script size")
+        else:
+            for tx_in in self.vin:
+                if tx_in.is_coinbase():
+                    raise BTClibValueError()
+
         # must be a 4-bytes integer
         if not 0 <= self.version <= 0xFFFFFFFF:
             raise BTClibValueError(f"invalid version: {self.version}")
 
         # must be a 4-bytes int
         if not 0 <= self.lock_time <= 0xFFFFFFFF:
             raise BTClibValueError(f"invalid lock time: {self.lock_time}")
```

### Comparing `btclib-2023.5.30/btclib/tx/tx_in.py` & `btclib-2023.7.12/btclib/tx/tx_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Transaction Input (TxIn) dataclass.
 
 Dataclass encapsulating prev_out, script_sig, sequence, and
 script_witness.
 """
 
 from __future__ import annotations
```

### Comparing `btclib-2023.5.30/btclib/tx/tx_out.py` & `btclib-2023.7.12/btclib/tx/tx_out.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Transaction Output (TxOut) dataclass.
 
 Dataclass encapsulating value and script_pub_key (and network to convert
 script_pub_key to and from address).
 """
 
 from __future__ import annotations
```

### Comparing `btclib-2023.5.30/btclib/utils.py` & `btclib-2023.7.12/btclib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Assorted conversion utilities.
 
 Most conversions from SEC 1 v.2 2.3 are included.
 
 https://www.secg.org/sec1-v2.pdf
 """
 from __future__ import annotations
```

### Comparing `btclib-2023.5.30/btclib/var_bytes.py` & `btclib-2023.7.12/btclib/var_bytes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Varbytes encoding and decoding functions."""
 
 from btclib import var_int
 from btclib.alias import BinaryData, Octets
 from btclib.exceptions import BTClibRuntimeError
 from btclib.utils import bytes_from_octets, bytesio_from_binarydata
```

### Comparing `btclib-2023.5.30/btclib/var_int.py` & `btclib-2023.7.12/btclib/var_int.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Varint encoding and decoding functions.
 
 A var_int (variable integer) is variable-length quantity that uses an
 arbitrary number of binary octets (eight-bit bytes) to represent an
 arbitrarily large integer.
 It is usually a base-128 (7 bits) representation of an unsigned integer
 with the addition of the eighth bit to mark continuation of bytes;
```

### Comparing `btclib-2023.5.30/btclib.egg-info/PKG-INFO` & `btclib-2023.7.12/btclib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btclib
-Version: 2023.5.30
+Version: 2023.7.12
 Summary: A library for 'bitcoin cryptography'
 Home-page: https://btclib.org
 Author: The btclib developers
 Author-email: devs@btclib.org
 License: MIT License
 Project-URL: Download, https://github.com/btclib-org/btclib/releases
 Project-URL: Documentation, https://btclib.readthedocs.io/
```

### Comparing `btclib-2023.5.30/btclib.egg-info/SOURCES.txt` & `btclib-2023.7.12/btclib.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 btclib/__init__.py
 btclib/alias.py
 btclib/amount.py
 btclib/b32.py
 btclib/b58.py
 btclib/base58.py
 btclib/bech32.py
+btclib/descriptors.py
 btclib/exceptions.py
 btclib/hashes.py
 btclib/network.py
 btclib/number_theory.py
 btclib/py.typed
 btclib/to_prv_key.py
 btclib/to_pub_key.py
@@ -83,35 +84,50 @@
 btclib/mnemonic/_data/italian.txt
 btclib/psbt/__init__.py
 btclib/psbt/psbt.py
 btclib/psbt/psbt_in.py
 btclib/psbt/psbt_out.py
 btclib/psbt/psbt_utils.py
 btclib/script/__init__.py
+btclib/script/op_codes_tapscript.py
 btclib/script/script.py
 btclib/script/script_pub_key.py
 btclib/script/sig_hash.py
 btclib/script/taproot.py
 btclib/script/witness.py
+btclib/script/engine/__init__.py
+btclib/script/engine/script.py
+btclib/script/engine/script_op_codes.py
+btclib/script/engine/tapscript.py
 btclib/tx/__init__.py
 btclib/tx/out_point.py
 btclib/tx/tx.py
 btclib/tx/tx_in.py
 btclib/tx/tx_out.py
 docs/Makefile
 docs/README.rst
 docs/make.bat
 docs/requirements.txt
+docs/build/html/_sources/btclib.bip32.rst.txt
+docs/build/html/_sources/btclib.ecc.rst.txt
+docs/build/html/_sources/btclib.mnemonic.rst.txt
+docs/build/html/_sources/btclib.psbt.rst.txt
+docs/build/html/_sources/btclib.rst.txt
+docs/build/html/_sources/btclib.script.rst.txt
+docs/build/html/_sources/btclib.tx.rst.txt
+docs/build/html/_sources/index.rst.txt
+docs/build/html/_sources/modules.rst.txt
 docs/source/btclib.bip32.rst
 docs/source/btclib.block.rst
 docs/source/btclib.ec.rst
 docs/source/btclib.ecc.rst
 docs/source/btclib.mnemonic.rst
 docs/source/btclib.psbt.rst
 docs/source/btclib.rst
+docs/source/btclib.script.engine.rst
 docs/source/btclib.script.rst
 docs/source/btclib.tx.rst
 docs/source/conf.py
 docs/source/contributing_link.md
 docs/source/history_link.md
 docs/source/index.rst
 docs/source/modules.rst
@@ -121,22 +137,24 @@
 tests/__init__.py
 tests/py.typed
 tests/test_amount.py
 tests/test_b32.py
 tests/test_b58.py
 tests/test_base58.py
 tests/test_bech32.py
+tests/test_descriptors.py
 tests/test_hashes.py
 tests/test_network.py
 tests/test_number_theory.py
 tests/test_to_key.py
 tests/test_to_prv_key.py
 tests/test_to_pub_key.py
 tests/test_utils.py
 tests/test_var_int.py
+tests/_data/descriptor_checksums.json
 tests/_generated_files/mainnet.json
 tests/_generated_files/regtest.json
 tests/_generated_files/testnet.json
 tests/bip32/__init__.py
 tests/bip32/test_bip32.py
 tests/bip32/test_der_path.py
 tests/bip32/test_key_origin.py
@@ -187,30 +205,38 @@
 tests/mnemonic/_data/fakeenglish.txt
 tests/psbt/__init__.py
 tests/psbt/test_psbt.py
 tests/psbt/test_psbt_in.py
 tests/psbt/test_psbt_out.py
 tests/psbt/test_psbt_utils.py
 tests/psbt/_data/bip174_test_vectors.json
+tests/psbt/_data/bip371_test_vectors.json
 tests/psbt/_generated_files/psbt.json
 tests/psbt/_generated_files/psbt_in.json
 tests/psbt/_generated_files/psbt_out.json
 tests/script/__init__.py
+tests/script/test_op_codes_taproot.py
 tests/script/test_script.py
 tests/script/test_script_pub_key.py
 tests/script/test_sig_hash_legacy.py
 tests/script/test_sig_hash_segwitv0.py
 tests/script/test_sig_hash_taproot.py
 tests/script/test_taproot.py
 tests/script/test_witness.py
 tests/script/_data/bip67_test_vectors.json
 tests/script/_data/sig_hash_legacy_test_vectors.json
 tests/script/_data/taproot_test_vector.json
 tests/script/_data/tapscript_test_vector.json
 tests/script/_generated_files/witness.json
+tests/script_engine/__init__.py
+tests/script_engine/test_script.py
+tests/script_engine/test_transactions.py
+tests/script_engine/_data/script_tests.json
+tests/script_engine/_data/tx_invalid_legacy.json
+tests/script_engine/_data/tx_valid_legacy.json
 tests/tx/__init__.py
 tests/tx/test_out_point.py
 tests/tx/test_tx.py
 tests/tx/test_tx_in.py
 tests/tx/test_tx_out.py
 tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin
 tests/tx/_generated_files/out_point.json
```

### Comparing `btclib-2023.5.30/docs/Makefile` & `btclib-2023.7.12/docs/Makefile`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/README.rst` & `btclib-2023.7.12/docs/README.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/make.bat` & `btclib-2023.7.12/docs/make.bat`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.bip32.rst` & `btclib-2023.7.12/docs/build/html/_sources/btclib.bip32.rst.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.ec.rst` & `btclib-2023.7.12/docs/source/btclib.ec.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.ecc.rst` & `btclib-2023.7.12/docs/source/btclib.ecc.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.mnemonic.rst` & `btclib-2023.7.12/docs/build/html/_sources/btclib.mnemonic.rst.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.psbt.rst` & `btclib-2023.7.12/docs/build/html/_sources/btclib.psbt.rst.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.rst` & `btclib-2023.7.12/docs/source/btclib.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.script.rst` & `btclib-2023.7.12/docs/build/html/_sources/btclib.script.rst.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/btclib.tx.rst` & `btclib-2023.7.12/docs/source/btclib.tx.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/docs/source/conf.py` & `btclib-2023.7.12/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Configuration file for the Sphinx documentation builder.
 
 For the full list of built-in configuration values, see the
 documentation: https://www.sphinx-
 doc.org/en/master/usage/configuration.html
 """
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "btclib"
 project_copyright = "2017-2023 The btclib developers"
 author = "The btclib developers"
-release = "2023.5.30"
+release = "2023.7.12"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     # "m2r2",
     "myst_parser",
```

### Comparing `btclib-2023.5.30/pyproject.toml` & `btclib-2023.7.12/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 [tool.pytest.ini_options]
 addopts = "--durations=8 -n auto"
 
+[tool.coverage.run]
+omit = ["*/site-packages/*"]
+
+[tool.coverage.report]
+show_missing = true
+skip_covered = true
+precision = 2
+
 [tool.mypy]
 strict = false
 show_column_numbers = true
 show_error_codes = true
 exclude = [
     "build",
 ]
@@ -34,14 +42,16 @@
     "too-many-instance-attributes",  # R0902
     "too-many-return-statements",  # R0911
     "too-many-branches",  # R0912
     "too-many-arguments",   # R0913
     "too-many-locals",   # R0914
     "too-many-statements",  # R0915
     "fixme",  # W0511
+    "unsubscriptable-object",  # E1136 python3.9-only pylint bug
+    "unused-argument", # W0613
 ]
 
 [tool.pylint.logging]
 logging-format-style = "new"
 logging-modules = "logging"
 
 [tool.pylint.spelling]
```

### Comparing `btclib-2023.5.30/setup.py` & `btclib-2023.7.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Build script for setuptools."""
 
-from setuptools import find_packages, setup  # type: ignore
+from setuptools import find_namespace_packages, setup  # type: ignore[import]
 
 import btclib
 
 with open("README.md", encoding="ascii") as file_:
     longdescription = file_.read()
 
 
@@ -31,15 +30,15 @@
     },
     license=btclib.__license__,
     author=btclib.__author__,
     author_email=btclib.__author_email__,
     description="A library for 'bitcoin cryptography'",
     long_description=longdescription,
     long_description_content_type="text/markdown",
-    packages=find_packages(exclude=["tests", "tests.*"]),
+    packages=find_namespace_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     # test_suite="btclib.tests",
     install_requires=["btclib_libsecp256k1"],
     # extras_require={"secp256k1": ["btclib_libsecp256k1"]},
     keywords=(
         "bitcoin cryptography elliptic-curves ecdsa schnorr RFC-6979 "
         "bip32 bip39 electrum base58 bech32 segwit message-signing "
```

### Comparing `btclib-2023.5.30/tests/README.md` & `btclib-2023.7.12/tests/README.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/_generated_files/mainnet.json` & `btclib-2023.7.12/tests/_generated_files/mainnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/_generated_files/regtest.json` & `btclib-2023.7.12/tests/_generated_files/regtest.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/_generated_files/testnet.json` & `btclib-2023.7.12/tests/_generated_files/testnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/bip32/_data/bip32_invalid_keys.json` & `btclib-2023.7.12/tests/bip32/_data/bip32_invalid_keys.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/bip32/_data/bip32_test_vectors.json` & `btclib-2023.7.12/tests/bip32/_data/bip32_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/bip32/_generated_files/key_paths.json` & `btclib-2023.7.12/tests/bip32/_generated_files/key_paths.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/bip32/test_bip32.py` & `btclib-2023.7.12/tests/bip32/test_bip32.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.bip32` module."""
 
 import json
 import re
 from os import path
 
 import pytest
 
-from btclib import base58, hashes
+from btclib import base58
 from btclib.b58 import p2pkh  # FIXME why it is needed here
 from btclib.bip32 import (
     BIP32KeyData,
     crack_prv_key,
     derive,
     derive_from_account,
     rootxprv_from_seed,
     xpub_from_xprv,
 )
 from btclib.bip32.bip32 import _derive
 from btclib.bip32.der_path import _indexes_from_bip32_path_str
 from btclib.exceptions import BTClibValueError
+from btclib.hashes import hash160
 from btclib.to_pub_key import pub_keyinfo_from_key
 
 
 def test_exceptions() -> None:
     with pytest.raises(BTClibValueError, match="not a private or public key: "):
         # invalid checksum
         xprv = "xppp9s21ZrQH143K2oxHiQ5f7D7WYgXD9h6HAXDBuMoozDGGiYHWsq7TLBj2yvGuHTLSPCaFmUyN1v3fJRiY2A4YuNSrqQMPVLZKt76goL6LP7L"
@@ -74,15 +74,15 @@
 
     xkey_data = BIP32KeyData.b58decode(xkey)
     xkey_data.depth = 256
     with pytest.raises(BTClibValueError, match="invalid depth: "):
         xkey_data.assert_valid()
 
     xkey_data = BIP32KeyData.b58decode(xkey)
-    xkey_data.depth = tuple()  # type: ignore[assignment]
+    xkey_data.depth = ()  # type: ignore[assignment]
     with pytest.raises(TypeError):
         xkey_data.assert_valid()
 
     xkey_data = BIP32KeyData.b58decode(xkey)
     xkey_data.parent_fingerprint = (xkey_data.parent_fingerprint)[:-1]
     with pytest.raises(BTClibValueError, match="invalid parent_fingerprint length: "):
         xkey_data.assert_valid()
@@ -99,15 +99,15 @@
 
     xkey_data = BIP32KeyData.b58decode(xkey)
     xkey_data.index = 0xFFFFFFFF + 1
     with pytest.raises(BTClibValueError, match="invalid index: "):
         xkey_data.assert_valid()
 
     xkey_data = BIP32KeyData.b58decode(xkey)
-    xkey_data.index = tuple()  # type: ignore[assignment]
+    xkey_data.index = ()  # type: ignore[assignment]
     with pytest.raises(TypeError):
         xkey_data.assert_valid()
 
     xkey_data = BIP32KeyData.b58decode(xkey)
     xkey_data.chain_code = (xkey_data.chain_code)[:-1]
     with pytest.raises(BTClibValueError, match="invalid chain_code length: "):
         xkey_data.assert_valid()
@@ -220,15 +220,15 @@
     rootmxprv = "xprv9s21ZrQH143K3QTDL4LXw2F7HEK3wJUD2nW2nRk4stbPy6cq3jPPqjiChkVvvNKmPGJxWUtg6LnF5kejMRNNU3TGtRBeJgk33yuGBxrMPHi"
     xprv = BIP32KeyData.b58decode(rootmxprv)
     # FIXME
     # assert xprv == _derive(xprv, "m")
     assert rootmxprv == derive(xprv, "m")
     assert rootmxprv == derive(xprv, "")
 
-    fingerprint = hashes.hash160(pub_keyinfo_from_key(xprv)[0])[:4]
+    fingerprint = hash160(pub_keyinfo_from_key(xprv)[0])[:4]
     assert fingerprint == _derive(xprv, bytes.fromhex("80000000")).parent_fingerprint
 
     for der_path in ("/1", "800000", "80000000"):
         xkey = _derive(xprv, der_path)
         assert fingerprint == xkey.parent_fingerprint
 
     err_msg = "invalid literal for int"
@@ -358,7 +358,21 @@
     seed = "57fb1e450b8afb95c62afbcd49e4100d6790e0822b8905608679180ac34ca0bd45bf7ccc6c5f5218236d0eb93afc78bd117b9f02a6b7df258ea182dfaef5aad7"
     xroot = rootxprv_from_seed(seed)
     der_path = "m/44H/60H/0H"
     xprv = "xprv9yqXG1Cns3YEQi6fsCJ7NGV5sHPiyZcbgLVst61dbLYyn7qy1G9aFtRmaYp481ounqnVf9Go2ymQ4gmxZLEwYSRhU868aDk4ZxzGvqHJVhe"
     assert derive(xroot, der_path) == xprv
     xpub = "xpub6CpsfWjghR6XdCB8yDq7jQRpRKEDP2LT3ZRUgURF9g5xevB7YoTpogkFRqq5nQtVSN8YCMZo2CD8u4zCaxRv85ctCWmzEi9gQ5DBhBFaTNo"
     assert xpub_from_xprv(xprv) == xpub
+
+
+def test_pub_key_derivation() -> None:
+    parent_xpub = "xpub6CpsfWjghR6XdCB8yDq7jQRpRKEDP2LT3ZRUgURF9g5xevB7YoTpogkFRqq5nQtVSN8YCMZo2CD8u4zCaxRv85ctCWmzEi9gQ5DBhBFaTNo"
+    proper_child = "xpub6FCCuDg6j52SWRVZ1TugkjrnGkqPcDuNNKDzohU2mmd4dxiGJypZa535iqYT8KcN2oouRF7A6tXEGAX6HCSjQe7HVSDR4LQ4yUT3HwF1Tqi"
+    assert derive(parent_xpub, "m/0") == proper_child
+    parent_key = BIP32KeyData.b58decode(parent_xpub).key
+    parent_fingerprint = hash160(parent_key)[:4]
+    assert BIP32KeyData.b58decode(proper_child).parent_fingerprint == parent_fingerprint
+
+    orphan_child_key = BIP32KeyData.b58decode(proper_child)
+    orphan_child_key.parent_fingerprint = b"\x00" * 4
+    orphan_child = "xpub6DXuQW1FgeHbhsSchbuDWE9Bj8mPiPUpiroAmAvRdRqYbGHXHTyEkttkxSvtCac64QzpasL1Tvd5Znvn5GQMswQUrpRBsPRz7npvyZ8ExWi"
+    assert orphan_child_key.b58encode() == orphan_child
```

### Comparing `btclib-2023.5.30/tests/bip32/test_der_path.py` & `btclib-2023.7.12/tests/bip32/test_der_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.bip32_path` module."""
 
 
 import pytest
 
 from btclib.bip32 import (
     bytes_from_bip32_path,
```

### Comparing `btclib-2023.5.30/tests/bip32/test_key_origin.py` & `btclib-2023.7.12/tests/bip32/test_key_origin.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.bip32_path` module."""
 
 import json
 from os import path
 
 import pytest
```

### Comparing `btclib-2023.5.30/tests/bip32/test_slip132.py` & `btclib-2023.7.12/tests/bip32/test_slip132.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.slip132` module."""
 
 from __future__ import annotations
 
 import pytest
 
 from btclib import b32, b58
```

### Comparing `btclib-2023.5.30/tests/block/_data/block_200000.bin` & `btclib-2023.7.12/tests/block/_data/block_200000.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/block/_data/block_481824.bin` & `btclib-2023.7.12/tests/block/_data/block_481824.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/block/_data/block_481824_complete.bin` & `btclib-2023.7.12/tests/block/_data/block_481824_complete.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/block/_generated_files/block_481824.json` & `btclib-2023.7.12/tests/block/_generated_files/block_481824.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/block/test_block.py` & `btclib-2023.7.12/tests/block/test_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.block` module."""
 
 import json
 from datetime import datetime, timezone
 from os import path
 
 import pytest
@@ -196,37 +195,37 @@
         block.assert_valid()
     with pytest.raises(BTClibValueError, match=err_msg):
         _ = block.height
 
 
 def test_block_481824() -> None:
     """Test first block with segwit transaction as seen from legacy nodes."""
+    prev_block = "000000000000000000cbeff0b533f8e1189cf09dfbebf57a8ebe349362811b80"
+    merkle_root = "6438250cad442b982801ae6994edb8a9ec63c0a0ba117779fbe7ef7f07cad140"
+    hash_ = "0000000000000000001c8018d9cb3b742ef25114f27563e3fc4a1902167f9893"
     for i, fname in enumerate(["block_481824.bin", "block_481824_complete.bin"]):
         filename = path.join(path.dirname(__file__), "_data", fname)
         with open(filename, "rb") as file_:
             block_bytes = file_.read()
 
         block = Block.parse(block_bytes)
         assert len(block.transactions) == 1866
         assert block.height == 481_824
         assert block == Block.parse(block.serialize())
         assert block == Block.from_dict(block.to_dict())
 
         header = block.header
         assert header.version == 0x20000002
-        prev_block = "000000000000000000cbeff0b533f8e1189cf09dfbebf57a8ebe349362811b80"
         assert header.previous_block_hash.hex() == prev_block
-        merkle_root = "6438250cad442b982801ae6994edb8a9ec63c0a0ba117779fbe7ef7f07cad140"
         assert header.merkle_root.hex() == merkle_root
         timestamp = datetime(2017, 8, 24, 1, 57, 37, tzinfo=timezone.utc)
         assert header.time == timestamp
         assert header.bits.hex() == "18013ce9"
         assert header.nonce == 0x2254FF22
 
-        hash_ = "0000000000000000001c8018d9cb3b742ef25114f27563e3fc4a1902167f9893"
         assert header.hash.hex() == hash_
         assert 0 <= header.difficulty - 888_171_856_257 < 1
         assert header == BlockHeader.parse(header.serialize())
         assert header == BlockHeader.from_dict(header.to_dict())
 
         if i:  # segwit nodes see the witness data
             assert block.has_segwit_tx()
```

### Comparing `btclib-2023.5.30/tests/ec/_data/pubkey.json` & `btclib-2023.7.12/tests/ec/_data/pubkey.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/ec/test_curve.py` & `btclib-2023.7.12/tests/ec/test_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.curve` module."""
 
 
 import itertools
 import json
 from os import path
```

### Comparing `btclib-2023.5.30/tests/ec/test_curve_group.py` & `btclib-2023.7.12/tests/ec/test_curve_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.curve_group` module."""
 
 import pytest
 
 from btclib.alias import INF, INFJ
 from btclib.ec import (
     cached_multiples,
```

### Comparing `btclib-2023.5.30/tests/ec/test_curve_group_2.py` & `btclib-2023.7.12/tests/ec/test_curve_group_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.curve_group_2` module."""
 
 import pytest
 
 from btclib.alias import INFJ
 from btclib.ec import (
     mult_endomorphism_secp256k1,
```

### Comparing `btclib-2023.5.30/tests/ec/test_curve_group_f.py` & `btclib-2023.7.12/tests/ec/test_curve_group_f.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.curve_group_f` module."""
 
 import pytest
 
 from btclib.ec import CurveGroup, find_all_points, find_subgroup_points, mult_aff
 from btclib.exceptions import BTClibValueError
```

### Comparing `btclib-2023.5.30/tests/ec/test_sec_point.py` & `btclib-2023.7.12/tests/ec/test_sec_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.sec_point` module."""
 
 import pytest
 
 from btclib.alias import INF
 from btclib.ec import Curve, bytes_from_point, point_from_octets
 from btclib.ec.curve import CURVES
```

### Comparing `btclib-2023.5.30/tests/ecc/_data/bip340_test_vectors.csv` & `btclib-2023.7.12/tests/ecc/_data/bip340_test_vectors.csv`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/ecc/_data/bms.json` & `btclib-2023.7.12/tests/ecc/_data/bms.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/ecc/_data/ecdsa_custom_nonce_sig.json` & `btclib-2023.7.12/tests/ecc/_data/ecdsa_custom_nonce_sig.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/ecc/_data/ecdsa_sig.json` & `btclib-2023.7.12/tests/ecc/_data/ecdsa_sig.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/ecc/_data/rfc6979.json` & `btclib-2023.7.12/tests/ecc/_data/rfc6979.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/ecc/test_bms.py` & `btclib-2023.7.12/tests/ecc/test_bms.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.bms` module."""
 
 import json
 from hashlib import sha256
 from os import path
 
 import pytest
```

### Comparing `btclib-2023.5.30/tests/ecc/test_borromean.py` & `btclib-2023.7.12/tests/ecc/test_borromean.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.borromean` module."""
 
 from btclib.ecc import borromean, dsa
 
 
 def test_borromean() -> None:
     nring = 4  # FIXME minimum number of rings?
```

### Comparing `btclib-2023.5.30/tests/ecc/test_der.py` & `btclib-2023.7.12/tests/ecc/test_der.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.der` module."""
 
 import pytest
 
 from btclib.ec import secp256k1
 from btclib.ecc.dsa import Sig
 from btclib.exceptions import BTClibRuntimeError, BTClibValueError
```

### Comparing `btclib-2023.5.30/tests/ecc/test_dh.py` & `btclib-2023.7.12/tests/ecc/test_dh.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.dh` module."""
 
 from hashlib import sha1, sha224, sha256, sha384, sha512
 
 import pytest
 
 from btclib.ec import bytes_from_point, mult
```

### Comparing `btclib-2023.5.30/tests/ecc/test_dsa.py` & `btclib-2023.7.12/tests/ecc/test_dsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.dsa` module."""
 
 import json
 import secrets
 from hashlib import sha1
 from os import path
```

### Comparing `btclib-2023.5.30/tests/ecc/test_pedersen.py` & `btclib-2023.7.12/tests/ecc/test_pedersen.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.pedersen` module."""
 
 from hashlib import sha256, sha384
 
 import pytest
 
 from btclib.ec import secp256k1
```

### Comparing `btclib-2023.5.30/tests/ecc/test_rfc6979.py` & `btclib-2023.7.12/tests/ecc/test_rfc6979.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.rfc6979` module."""
 
 import hashlib
 import json
 from os import path
 
 from btclib.ec import mult
-from btclib.ec.curve import CURVES
+from btclib.ec.curve import CURVES, Curve
 from btclib.ecc import dsa
 from btclib.ecc.rfc6979_nonce import rfc6979_nonce_
 from btclib.hashes import reduce_to_hlen
 
 
 def test_rfc6979() -> None:
     # source: https://bitcointalk.org/index.php?topic=285142.40
@@ -28,27 +27,29 @@
     x = 0x1
     k = 0x8F8A276C19F4149656B280621E358CCE24F5F52542772691EE69063B74F15D15
     k2 = rfc6979_nonce_(msg_hash, x, hf=hashlib.sha256)
     assert k == k2
 
 
 def test_rfc6979_nonce_example() -> None:
-    class _helper:  # pylint: disable=too-few-public-methods
+    class _helper(
+        Curve
+    ):  # pylint: disable=too-few-public-methods, super-init-not-called
         def __init__(self, n: int) -> None:
             self.n = n
             self.nlen = n.bit_length()
             self.n_size = (self.nlen + 7) // 8
 
     # source: https://tools.ietf.org/html/rfc6979 section A.1
     fake_ec = _helper(0x4000000000000000000020108A2E0CC0D99F8A5EF)
     x = 0x09A4D6792295A7F730FC3F2B49CBC0F62E862272F
     msg = b"sample"
     msg_hash = hashlib.sha256(msg).digest()
     k = 0x23AF4074C90A02B3FE61D286D5C87F425E6BDD81B
-    assert k == rfc6979_nonce_(msg_hash, x, fake_ec)  # type: ignore[arg-type]
+    assert k == rfc6979_nonce_(msg_hash, x, fake_ec)
 
 
 def test_rfc6979_nonce_tv() -> None:
     fname = "rfc6979.json"
     filename = path.join(path.dirname(__file__), "_data", fname)
     with open(filename, encoding="ascii") as file_:
         test_dict = json.load(file_)
```

### Comparing `btclib-2023.5.30/tests/ecc/test_sign_to_contract.py` & `btclib-2023.7.12/tests/ecc/test_sign_to_contract.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.sign_to_contract` module."""
 
 import random
 from hashlib import sha1, sha256
 
 from btclib.ec import secp256k1
 from btclib.ec.curve import CURVES
```

### Comparing `btclib-2023.5.30/tests/ecc/test_ssa.py` & `btclib-2023.7.12/tests/ecc/test_ssa.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.ssa` module."""
 
 from __future__ import annotations
 
 import csv
 from hashlib import sha256 as hf
 from os import path
```

### Comparing `btclib-2023.5.30/tests/mnemonic/_data/bip39_test_vectors.json` & `btclib-2023.7.12/tests/mnemonic/_data/bip39_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/mnemonic/_data/electrum_test_vectors.json` & `btclib-2023.7.12/tests/mnemonic/_data/electrum_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/mnemonic/_data/english.txt` & `btclib-2023.7.12/tests/mnemonic/_data/english.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/mnemonic/_data/fakeenglish.txt` & `btclib-2023.7.12/tests/mnemonic/_data/fakeenglish.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/mnemonic/test_bip39.py` & `btclib-2023.7.12/tests/mnemonic/test_bip39.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.bip39` module."""
 
 import json
 import secrets
 from math import ceil
 from os import path
```

### Comparing `btclib-2023.5.30/tests/mnemonic/test_electrum.py` & `btclib-2023.7.12/tests/mnemonic/test_electrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.electrum` module."""
 
 import json
 import secrets
 from os import path
 
 import pytest
```

### Comparing `btclib-2023.5.30/tests/mnemonic/test_entropy.py` & `btclib-2023.7.12/tests/mnemonic/test_entropy.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.entropy` module."""
 
 import math
 import secrets
 from io import StringIO
 
 import pytest
@@ -154,15 +153,15 @@
     assert entropy != bin_str_entropy216
 
     err_msg = "invalid number of bits: "
     with pytest.raises(BTClibValueError, match=err_msg):
         bin_str_entropy_from_entropy(bytes_entropy216, 224)
 
     with pytest.raises(BTClibValueError, match=err_msg):
-        bin_str_entropy_from_entropy(tuple())  # type: ignore[arg-type]
+        bin_str_entropy_from_entropy(())  # type: ignore[arg-type]
 
     with pytest.raises(ValueError):
         bin_str_entropy_from_int("not an int")
 
     with pytest.raises(TypeError):
         bin_str_entropy_from_str(3)  # type: ignore[arg-type]
```

### Comparing `btclib-2023.5.30/tests/mnemonic/test_mnemonic.py` & `btclib-2023.7.12/tests/mnemonic/test_mnemonic.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.mnemonic` module."""
 
 from os import path
 
 import pytest
 
 from btclib.exceptions import BTClibValueError
```

### Comparing `btclib-2023.5.30/tests/psbt/_data/bip174_test_vectors.json` & `btclib-2023.7.12/tests/psbt/_data/bip174_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/psbt/_generated_files/psbt.json` & `btclib-2023.7.12/tests/psbt/_generated_files/psbt.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9392857142857144%*

 * *Differences: {"'inputs'": "{0: {'taproot_key_spend_signature': '', 'taproot_script_spend_signatures': "*

 * *             "OrderedDict(), 'taproot_leaf_scripts': OrderedDict(), 'taproot_hd_key_paths': [], "*

 * *             "'taproot_internal_key': '', 'taproot_merkle_root': ''}, 1: "*

 * *             "{'taproot_key_spend_signature': '', 'taproot_script_spend_signatures': "*

 * *             "OrderedDict(), 'taproot_leaf_scripts': OrderedDict(), 'taproot_hd_key_paths': [], "*

 * *             "'taproot_internal_key': '', 'taproot_merkle_root' […]*

```diff
@@ -68,14 +68,20 @@
                 "029583bf39ae0a609747ad199addd634fa6108559d6c5cd39b4c2183f1ab96e07f": "3044022074018ad4180097b873323c0015720b3684cc8123891048e7dbcd9b55ad679c99022073d369b740e3eb53dcefa33823c8070514ca55a7dd9544f157c167913261118c01",
                 "02dab61ff49a14db6a7d02b0cd1fbb78fc4b18312b5b4e54dae4dba2fbfef536d7": "3045022100f61038b308dc1da865a34852746f015772934208c6d24454393cd99bdf2217770220056e675a675a6d0a02b85b14e5e29074d8a25a9b5760bea2816f661910a006ea01"
             },
             "redeem_script": "5221029583bf39ae0a609747ad199addd634fa6108559d6c5cd39b4c2183f1ab96e07f2102dab61ff49a14db6a7d02b0cd1fbb78fc4b18312b5b4e54dae4dba2fbfef536d752ae",
             "ripemd160_preimages": {},
             "sha256_preimages": {},
             "sig_hash": 1,
+            "taproot_hd_key_paths": [],
+            "taproot_internal_key": "",
+            "taproot_key_spend_signature": "",
+            "taproot_leaf_scripts": {},
+            "taproot_merkle_root": "",
+            "taproot_script_spend_signatures": {},
             "unknown": {},
             "witness_script": "",
             "witness_utxo": null
         },
         {
             "bip32_derivs": [
                 {
@@ -100,14 +106,20 @@
                 "023add904f3d6dcf59ddb906b0dee23529b7ffb9ed50e5e86151926860221f0e73": "3044022065f45ba5998b59a27ffe1a7bed016af1f1f90d54b3aa8f7450aa5f56a25103bd02207f724703ad1edb96680b284b56d4ffcb88f7fb759eabbe08aa30f29b851383d201",
                 "03089dc10c7ac6db54f91329af617333db388cead0c231f723379d1b99030b02dc": "3044022062eb7a556107a7c73f45ac4ab5a1dddf6f7075fb1275969a7f383efff784bcb202200c05dbb7470dbf2f08557dd356c7325c1ed30913e996cd3840945db12228da5f01"
             },
             "redeem_script": "00208c2353173743b595dfb4a07b72ba8e42e3797da74e87fe7d9d7497e3b2028903",
             "ripemd160_preimages": {},
             "sha256_preimages": {},
             "sig_hash": 1,
+            "taproot_hd_key_paths": [],
+            "taproot_internal_key": "",
+            "taproot_key_spend_signature": "",
+            "taproot_leaf_scripts": {},
+            "taproot_merkle_root": "",
+            "taproot_script_spend_signatures": {},
             "unknown": {},
             "witness_script": "522103089dc10c7ac6db54f91329af617333db388cead0c231f723379d1b99030b02dc21023add904f3d6dcf59ddb906b0dee23529b7ffb9ed50e5e86151926860221f0e7352ae",
             "witness_utxo": {
                 "addresses": [
                     "3JTiFf9xWFqryQ7CXK3hMX8oh4GxYxUyAr"
                 ],
                 "network": "mainnet",
@@ -124,26 +136,32 @@
                 {
                     "master_fingerprint": "d90c6a4f",
                     "path": "m/0h/0h/4h",
                     "pub_key": "03a9a4c37f5996d3aa25dbac6b570af0650394492942460b354753ed9eeca58771"
                 }
             ],
             "redeem_script": "",
+            "taproot_hd_key_paths": [],
+            "taproot_internal_key": "",
+            "taproot_tree": [],
             "unknown": {},
             "witness_script": ""
         },
         {
             "bip32_derivs": [
                 {
                     "master_fingerprint": "d90c6a4f",
                     "path": "m/0h/0h/5h",
                     "pub_key": "027f6399757d2eff55a136ad02c684b1838b6556e5f1b6b34282a94b6b50051096"
                 }
             ],
             "redeem_script": "",
+            "taproot_hd_key_paths": [],
+            "taproot_internal_key": "",
+            "taproot_tree": [],
             "unknown": {},
             "witness_script": ""
         }
     ],
     "tx": {
         "hash": "82efd652d7ab1197f01a5f4d9a30cb4c68bb79ab6fec58dfa1bf112291d1617b",
         "locktime": 0,
```

### Comparing `btclib-2023.5.30/tests/psbt/_generated_files/psbt_in.json` & `btclib-2023.7.12/tests/psbt/_generated_files/psbt_in.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {"'taproot_hd_key_paths'": '[]',*

 * * "'taproot_internal_key'": "''",*

 * * "'taproot_key_spend_signature'": "''",*

 * * "'taproot_leaf_scripts'": 'OrderedDict()',*

 * * "'taproot_merkle_root'": "''",*

 * * "'taproot_script_spend_signatures'": 'OrderedDict()'}*

```diff
@@ -65,11 +65,17 @@
         "029583bf39ae0a609747ad199addd634fa6108559d6c5cd39b4c2183f1ab96e07f": "3044022074018ad4180097b873323c0015720b3684cc8123891048e7dbcd9b55ad679c99022073d369b740e3eb53dcefa33823c8070514ca55a7dd9544f157c167913261118c01",
         "02dab61ff49a14db6a7d02b0cd1fbb78fc4b18312b5b4e54dae4dba2fbfef536d7": "3045022100f61038b308dc1da865a34852746f015772934208c6d24454393cd99bdf2217770220056e675a675a6d0a02b85b14e5e29074d8a25a9b5760bea2816f661910a006ea01"
     },
     "redeem_script": "5221029583bf39ae0a609747ad199addd634fa6108559d6c5cd39b4c2183f1ab96e07f2102dab61ff49a14db6a7d02b0cd1fbb78fc4b18312b5b4e54dae4dba2fbfef536d752ae",
     "ripemd160_preimages": {},
     "sha256_preimages": {},
     "sig_hash": 1,
+    "taproot_hd_key_paths": [],
+    "taproot_internal_key": "",
+    "taproot_key_spend_signature": "",
+    "taproot_leaf_scripts": {},
+    "taproot_merkle_root": "",
+    "taproot_script_spend_signatures": {},
     "unknown": {},
     "witness_script": "",
     "witness_utxo": null
 }
```

### Comparing `btclib-2023.5.30/tests/psbt/test_psbt.py` & `btclib-2023.7.12/tests/psbt/test_psbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.psbt.psbt` module."""
 
 import json
 from os import path
 
 import pytest
 
@@ -57,14 +56,39 @@
             psbt_decoded.assert_signable()
         assert test_vector["error message"] in str(
             excinfo.value
         ), f"signer check failure {i+1}: {test_vector['description']}\n{excinfo.value}"
         assert test_vector["encoded psbt"] == Psbt.b64encode(psbt_decoded)
 
 
+def test_vectors_bip371() -> None:
+    """Test https://github.com/bitcoin/bips/blob/master/bip-0371.mediawiki."""
+
+    data_folder = path.join(path.dirname(__file__), "_data")
+    filename = path.join(data_folder, "bip371_test_vectors.json")
+    with open(filename, encoding="ascii") as file_:
+        # json.dump(test_vectors, f, indent=4)
+        test_vectors = json.load(file_)
+
+    for i, test_vector in enumerate(test_vectors["valid psbts"]):
+        try:
+            psbt_decoded = Psbt.b64decode(test_vector["encoded psbt"])
+        except Exception as e:  # pragma: no cover # pylint: disable=broad-except
+            print(f"valid case {i+1}: {test_vector['description']}")  # pragma: no cover
+            raise e  # pragma: no cover
+        assert test_vector["encoded psbt"] == Psbt.b64encode(psbt_decoded)
+
+    for i, test_vector in enumerate(test_vectors["invalid psbts"]):
+        with pytest.raises(BTClibValueError) as excinfo:
+            Psbt.b64decode(test_vector["encoded psbt"])
+        assert test_vector["error message"] in str(
+            excinfo.value
+        ), f"invalid case {i+1}: {test_vector['description']}\n{excinfo.value}"
+
+
 def test_creation() -> None:
     psbt_str = "cHNidP8BAJoCAAAAAljoeiG1ba8MI76OcHBFbDNvfLqlyHV5JPVFiHuyq911AAAAAAD/////g40EJ9DsZQpoqka7CwmK6kQiwHGyyng1Kgd5WdB86h0BAAAAAP////8CcKrwCAAAAAAWABTYXCtx0AYLCcmIauuBXlCZHdoSTQDh9QUAAAAAFgAUAK6pouXw+HaliN9VRuh0LR2HAI8AAAAAAAAAAAA="
     psbt = Psbt.b64decode(psbt_str)
     assert psbt.b64encode() == psbt_str
 
     output_1 = TxOut(
         149990000, ScriptPubKey("0014d85c2b71d0060b09c9886aeb815e50991dda124d")
@@ -396,40 +420,40 @@
 
 
 def test_exceptions() -> None:
     # from creator example
     psbt_str = "cHNidP8BAJoCAAAAAljoeiG1ba8MI76OcHBFbDNvfLqlyHV5JPVFiHuyq911AAAAAAD/////g40EJ9DsZQpoqka7CwmK6kQiwHGyyng1Kgd5WdB86h0BAAAAAP////8CcKrwCAAAAAAWABTYXCtx0AYLCcmIauuBXlCZHdoSTQDh9QUAAAAAFgAUAK6pouXw+HaliN9VRuh0LR2HAI8AAAAAAAAAAAA="
 
     psbt = Psbt.b64decode(psbt_str)
-    psbt.outputs[0].redeem_script = "bad script"  # type: ignore
+    psbt.outputs[0].redeem_script = "bad script"  # type: ignore[assignment]
     with pytest.raises(TypeError):
         psbt.serialize()
 
     psbt = Psbt.b64decode(psbt_str)
-    psbt.inputs[0].witness_script = "bad script"  # type: ignore
+    psbt.inputs[0].witness_script = "bad script"  # type: ignore[assignment]
     with pytest.raises(TypeError):
         psbt.serialize()
 
     psbt = Psbt.b64decode(psbt_str)
-    psbt.outputs[0].unknown = {"bad key": b""}  # type: ignore
+    psbt.outputs[0].unknown = {"bad key": b""}  # type: ignore[dict-item]
     with pytest.raises(TypeError):
         psbt.serialize()
 
     psbt = Psbt.b64decode(psbt_str)
-    psbt.outputs[0].unknown = {b"deadbeef": "bad value"}  # type: ignore
+    psbt.outputs[0].unknown = {b"deadbeef": "bad value"}  # type: ignore[dict-item]
     with pytest.raises(TypeError):
         psbt.serialize()
 
     psbt = Psbt.b64decode(psbt_str)
     psbt.inputs[0].sig_hash_type = 101
     with pytest.raises(BTClibValueError, match="invalid sig_hash type: "):
         psbt.serialize()
 
     psbt = Psbt.b64decode(psbt_str)
-    psbt.inputs[0].final_script_sig = "bad script"  # type: ignore
+    psbt.inputs[0].final_script_sig = "bad script"  # type: ignore[assignment]
     with pytest.raises(TypeError):
         psbt.serialize()
 
     psbt = Psbt.b64decode(psbt_str)
     _, Q = dsa.gen_keys()
     pub_key = sec_point.bytes_from_point(Q)
     r = s = int.from_bytes(bytes.fromhex("FF" * 32), byteorder="big", signed=False)
```

### Comparing `btclib-2023.5.30/tests/psbt/test_psbt_in.py` & `btclib-2023.7.12/tests/psbt/test_psbt_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.psbt.psbt_in` module."""
 
 import json
 from os import path
 
 from btclib.psbt import Psbt, PsbtIn
```

### Comparing `btclib-2023.5.30/tests/psbt/test_psbt_out.py` & `btclib-2023.7.12/tests/psbt/test_psbt_out.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.psbt.psbt_out` module."""
 from __future__ import annotations
 
 import json
 from os import path
 
 from btclib.alias import Octets
```

### Comparing `btclib-2023.5.30/tests/psbt/test_psbt_utils.py` & `btclib-2023.7.12/tests/psbt/test_psbt_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.psbt.psbt_utils` module."""
 
 import pytest
 
 from btclib.exceptions import BTClibValueError
 from btclib.psbt import serialize_hd_key_paths
```

### Comparing `btclib-2023.5.30/tests/script/_data/bip67_test_vectors.json` & `btclib-2023.7.12/tests/script/_data/bip67_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/script/_data/sig_hash_legacy_test_vectors.json` & `btclib-2023.7.12/tests/script/_data/sig_hash_legacy_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/script/_data/taproot_test_vector.json` & `btclib-2023.7.12/tests/script/_data/taproot_test_vector.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/script/_data/tapscript_test_vector.json` & `btclib-2023.7.12/tests/script/_data/tapscript_test_vector.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/script/_generated_files/witness.json` & `btclib-2023.7.12/tests/script/_generated_files/witness.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/script/test_script.py` & `btclib-2023.7.12/tests/script/test_script.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.script.script` module."""
 
 from __future__ import annotations
 
 import warnings
 
 import pytest
 
+from btclib.alias import ScriptList
 from btclib.exceptions import BTClibValueError
-from btclib.script import Command, Script, op_int, parse, serialize
-from btclib.script.script import (
-    BYTE_FROM_OP_CODE_NAME,
-    OP_CODE_NAME_FROM_INT,
-    _serialize_str_command,
-)
+from btclib.script import Script, op_int, parse, serialize
+from btclib.script.script import BYTE_FROM_OP_CODE_NAME, OP_CODE_NAME_FROM_INT
 from btclib.utils import hex_string
 
 
 def test_operators() -> None:
     for i, name in OP_CODE_NAME_FROM_INT.items():
         b = BYTE_FROM_OP_CODE_NAME[name]
         assert i == b[0]
@@ -72,36 +68,25 @@
     length = 255
     b = b"\x0A" * length
     assert len(serialize([b])) == length + 2
     b = b"\x0A" * (length + 1)
     assert len(serialize([b])) == (length + 1) + 3
 
 
-def test_invalid_op_success() -> None:
-    err_msg = "invalid OP_SUCCESS number: "
-    with pytest.raises(BTClibValueError, match=err_msg):
-        _serialize_str_command("OP_SUCCESS1")
-    err_msg = "invalid OP_SUCCESS number: "
-    with pytest.raises(BTClibValueError, match=err_msg):
-        _serialize_str_command("OP_SUCCESS173")
-
-    assert _serialize_str_command("OP_SUCCESS80") == b"\x50"
-
-
 def test_add_and_eq() -> None:
     script_1 = serialize(["OP_2", "OP_3", "OP_ADD", "OP_5"])
     script_2 = serialize(["OP_EQUAL"])
     assert Script(script_1) + Script(script_2) == Script(script_1 + script_2)
 
     with pytest.raises(TypeError):
-        _ = Script(script_1) + script_2  # type: ignore
+        _ = Script(script_1) + script_2  # type: ignore[operator]
 
 
 def test_simple_scripts() -> None:
-    script_list: list[list[Command]] = [
+    script_list: list[ScriptList] = [
         ["OP_2", "OP_3", "OP_ADD", "OP_5", "OP_EQUAL"],
         [0x1ADD, "OP_1ADD", 0x1ADE, "OP_EQUAL"],
         [26, "OP_1NEGATE", "OP_ADD", 26, "OP_EQUAL"],
         [0x7FFFFFFF, "OP_1NEGATE", "OP_ADD", 0x7FFFFFFF, "OP_EQUAL"],
         [0x80000000, "OP_1NEGATE", "OP_ADD", 0x7FFFFFFF, "OP_EQUAL"],
         [0xFFFFFFFF - 1, "OP_1NEGATE", "OP_ADD", 0x7FFFFFFF, "OP_EQUAL"],
         [0xFFFFFFFF, "OP_1NEGATE", "OP_ADD", 0x7FFFFFFF, "OP_EQUAL"],
@@ -111,66 +96,67 @@
     for script_pub_key in script_list:
         serialized_script = serialize(script_pub_key)
         assert serialized_script == serialize(parse(serialized_script))
         assert serialized_script == serialize(parse(serialized_script.hex()))
 
 
 def test_exceptions() -> None:
-    script_pub_key: list[Command] = ["OP_2", "OP_3", "OP_ADD", "OP_5", "OP_RETURN_244"]
+    script_pub_key: ScriptList = ["OP_2", "OP_3", "OP_ADD", "OP_5", "OP_RETURN_244"]
     err_msg = "invalid string command: OP_RETURN_244"
     with pytest.raises(BTClibValueError, match=err_msg):
         serialize(script_pub_key)
 
     with pytest.raises(TypeError):
         serialize(["OP_2", "OP_3", "OP_ADD", "OP_5", serialize])  # type: ignore
 
     err_msg = "too many bytes for OP_PUSHDATA: "
     with pytest.raises(BTClibValueError, match=err_msg):
         script_pub_key = ["1f" * 521, "OP_DROP"]
         serialize(script_pub_key)
 
     # A script_pub_key with OP_PUSHDATA4 can't be decoded
     script_bytes = "4e09020000" + "0A" * 521 + "75"  # ['0A'*521, 'OP_DROP']
-    err_msg = "invalid pushdata length: "
+    err_msg = "Invalid pushdata length: "
     with pytest.raises(BTClibValueError, match=err_msg):
         parse(script_bytes)
 
     # and can't be encoded
-    script_pub_key_ = ["0A" * 521, "OP_DROP"]
+    script_pub_key_: ScriptList = ["00" * 521, "OP_DROP"]
     err_msg = "too many bytes for OP_PUSHDATA: "
     with pytest.raises(BTClibValueError, match=err_msg):
         serialize(script_pub_key_)
 
 
 def test_nulldata() -> None:
-    scripts: list[list[Command]] = [["OP_RETURN", "1A" * 79], ["OP_RETURN", "0A" * 79]]
+    scripts: list[ScriptList] = [["OP_RETURN", "1A" * 79], ["OP_RETURN", "0A" * 79]]
     for script_pub_key in scripts:
         assert script_pub_key == parse(serialize(script_pub_key))
         assert script_pub_key == parse(serialize(script_pub_key).hex())
 
 
 def test_encoding() -> None:
     script_bytes = b"jKBIP141 \\o/ Hello SegWit :-) keep it strong! LLAP Bitcoin twitter.com/khs9ne"
     assert serialize(parse(script_bytes)) == script_bytes
 
 
 def test_opcode_length() -> None:
-    err_msg = "not enough data for pushdata length"
+    err_msg = "Not enough data for pushdata length"
     with pytest.raises(BTClibValueError, match=err_msg):
         parse(b"\x4e\x00")
-    err_msg = "not enough data for pushdata"
+    err_msg = "Not enough data for pushdata"
     with pytest.raises(BTClibValueError, match=err_msg):
         parse(b"\x40\x00")
 
-    assert parse(b"\x01\x00\x50")[1] == "OP_SUCCESS80"
-    assert parse(b"\x01\x00\x50", exit_on_op_success=True) == ["OP_SUCCESS"]
+    err_msg = "Unknown op code"
+    with pytest.raises(BTClibValueError, match=err_msg):
+        assert parse(b"\x01\x00\x7e")
 
 
 def test_regressions() -> None:
-    script_list: list[list[Command]] = [
+    script_list: list[ScriptList] = [
         [1],
         ["OP_1"],
         [51],
         [b"\x01"],
         ["01"],
         ["AA"],
         ["aa"],
@@ -189,15 +175,15 @@
 
         for s in script_list:
             serialized = serialize(s)
             assert serialize(parse(serialized)) == serialized
 
 
 def test_null_serialization() -> None:
-    empty_script: list[Command] = []
+    empty_script: ScriptList = []
     assert empty_script == parse(b"")
     assert serialize(empty_script) == b""
 
     assert parse(serialize([""])) == ["OP_0"]
     assert parse(serialize([" "])) == ["OP_0"]
     assert parse(serialize([b""])) == ["OP_0"]
     assert parse(serialize([b" "])) == ["20"]
```

### Comparing `btclib-2023.5.30/tests/script/test_script_pub_key.py` & `btclib-2023.7.12/tests/script/test_script_pub_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.script.script_pub_key` module."""
 
 from __future__ import annotations
 
 import json
 from os import path
 
 import pytest
 
 from btclib import b32, b58, var_bytes
+from btclib.alias import ScriptList
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash160, sha256
 from btclib.script import (
-    Command,
     Script,
     ScriptPubKey,
     address,
     assert_p2ms,
     assert_p2pk,
     assert_p2pkh,
     assert_p2sh,
@@ -142,15 +141,15 @@
     assert len(serialize(["OP_RETURN", b"\x00" * 75])) == 77
     assert len(serialize(["OP_RETURN", b"\x00" * 76])) == 79
     script_pub_key = serialize(["OP_RETURN", b"\x00" * 76])[:-1]
     assert not is_nulldata(script_pub_key)
 
 
 def test_nulldata4() -> None:
-    script_: list[Command] = [
+    script_: ScriptList = [
         "OP_RETURN",
         "OP_RETURN",
         "OP_3",
         "OP_1",
         "OP_VERIF",
         "OP_0",
         "OP_3",
@@ -404,15 +403,15 @@
     with pytest.raises(BTClibValueError, match=err_msg):
         ScriptPubKey.p2ms(17, pub_keys)
 
     err_msg = "not a private or public key: "
     with pytest.raises(BTClibValueError, match=err_msg):
         ScriptPubKey.p2ms(1, [f"{pub_key0}00", pub_key1])
 
-    script_: list[Command] = [
+    script_: ScriptList = [
         "OP_1",
         f"{pub_key0}00",
         pub_key1,
         "OP_2",
         "OP_CHECKMULTISIG",
     ]
 
@@ -482,34 +481,34 @@
             assert script_type == "p2ms"
             assert payload == script_pub_key[:-1]
 
 
 def test_p2ms_3() -> None:
     # tx_id 33ac2af1a6f894276713b59ed09ce1a20fed5b36d169f20a3fe831dc45564d57
     # output n 0
-    keys: list[Command] = [
+    keys: ScriptList = [
         "036D568125A969DC78B963B494FA7ED5F20EE9C2F2FC2C57F86C5DF63089F2ED3A",
         "03FE4E6231D614D159741DF8371FA3B31AB93B3D28A7495CDAA0CD63A2097015C7",
     ]
-    cmds: list[Command] = ["OP_1", *keys, "OP_2", "OP_CHECKMULTISIG"]
+    cmds: ScriptList = ["OP_1", *keys, "OP_2", "OP_CHECKMULTISIG"]
     script_pub_key = ScriptPubKey(serialize(cmds))
     assert script_pub_key == ScriptPubKey.p2ms(1, keys)
 
     pub_keys = script_pub_key.addresses
     exp_pub_keys = [
         "1Ng4YU2e2H3E86syX2qrsmD9opBHZ42vCF",
         "14XufxyGiY6ZBJsFYHJm6awdzpJdtsP1i3",
     ]
     for pub_key, key, exp_pub_key in zip(pub_keys, keys, exp_pub_keys):
         assert pub_key == b58.p2pkh(key)
         assert pub_key == exp_pub_key
 
     # tx 56214420a7c4dcc4832944298d169a75e93acf9721f00656b2ee0e4d194f9970
     # input n 1
-    cmds_sig: list[Command] = [
+    cmds_sig: ScriptList = [
         "OP_0",
         "3045022100dba1e9b1c8477fd364edcc1f81845928202daf465a1e2d92904c13c88761cbd002200add6af863dfdb7efb95f334baec041e90811ae9d81624f9f87f33a56761f29401",
     ]
     script_sig = Script(serialize(cmds_sig))
     script = script_sig + script_pub_key
     # parse(serialize(*)) is to enforce same string case convention
     assert script.asm == parse(serialize(cmds_sig + cmds))
@@ -542,31 +541,31 @@
 def test_non_standard_script_in_p2wsh() -> None:
     network = "mainnet"
 
     addr = "bc1qqst9un5sz8576fy2nnqkpm4rpfh0weveqwtt8zxgjp02g2mx5q7s2vresu"
     script_pub_key = ScriptPubKey.from_address(addr)
     assert addr == address(script_pub_key.script, network)
 
-    fed_pub_keys: list[Command] = [
+    fed_pub_keys: ScriptList = [
         "03356aeda9c56586fe1e4a63d5118ffa3bf29bd91c6323e31de113a500a1ffe441".upper(),
         "0339f970e066a3efe1787722bd9cd59f69f1cf5cd29cb39fdec845415d8dbcb7a6".upper(),
         "0346f1233885981cc50b4064b6ed27174a149ac0842a25941f280302ddd7d2153d".upper(),
         "035d237b0807dd736cf4f3ab9c093bae2ccd128596dca883d3470f6327e6551688".upper(),
         "037b5acce33944ae02454c65011ffb04e604f36f685c474134e8874ddac45ff7c8".upper(),
         "03a88488e5ab6ae35c7d22d76efb9578e4a71b59c2ff0bd3cc3277e3a60717f3d6".upper(),
     ]
 
-    rec_pub_keys: list[Command] = [
+    rec_pub_keys: ScriptList = [
         "02219c3f199942fdd37a88065a8a8333189aadb5667a7c27681f66952fddf0eea4".upper(),
         "034c52cdf0125e50a53556c3f7586245f3f556bf26a80a4dae0ea6d0c81c11ebef".upper(),
         "03e8abfc4e3dcd5be461e79c9fa68a4d657b344391d7fd65ed40aaa56f584c7711".upper(),
     ]
 
     # fmt: off
-    redeem_script_cmds: list[Command] = [
+    redeem_script_cmds: ScriptList = [
         "OP_IF",
             "OP_3", *fed_pub_keys, "OP_6", "OP_CHECKMULTISIG",  # noqa E131
         "OP_ELSE",
             5184, "OP_CHECKSEQUENCEVERIFY", "OP_DROP",  # E131
             "OP_2", *rec_pub_keys, "OP_3", "OP_CHECKMULTISIG",  # E131
         "OP_ENDIF",
     ]
```

### Comparing `btclib-2023.5.30/tests/script/test_sig_hash_legacy.py` & `btclib-2023.7.12/tests/script/test_sig_hash_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.sig_hash` module.
 
 - https://github.com/bitcoin/bitcoin/blob/master/src/test/data/sighash.json
 """
 
 import json
 from os import path
```

### Comparing `btclib-2023.5.30/tests/script/test_sig_hash_segwitv0.py` & `btclib-2023.7.12/tests/script/test_sig_hash_segwitv0.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.sig_hash` module.
 
 test vector at
 https://github.com/bitcoin/bips/blob/master/bip-0143.mediawiki
 """
 
 from btclib.script import Witness, sig_hash
```

### Comparing `btclib-2023.5.30/tests/script/test_sig_hash_taproot.py` & `btclib-2023.7.12/tests/script/test_sig_hash_taproot.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.sig_hash` module.
 
 - test vector https://github.com/bitcoin/bips/blob/master/bip-0341.mediawiki
 """
 
 import json
 from os import path
 
 import pytest
 
+from btclib.alias import ScriptList
 from btclib.ecc import ssa
 from btclib.exceptions import BTClibRuntimeError, BTClibValueError
 from btclib.hashes import hash160
 from btclib.script import Witness, is_p2tr, parse, serialize, sig_hash, type_and_payload
 from btclib.tx import OutPoint, Tx, TxIn, TxOut
 
 
@@ -151,34 +151,34 @@
 def test_empty_stack() -> None:
     utxo = TxOut(
         100000000,
         serialize(
             ["OP_1", "cc71eb30d653c0c3163990c47b976f3fb3f37cccdcbedb169a1dfef58bbfbfaf"]
         ),
     )
-    tx_in = TxIn(OutPoint(), "", 1, Witness([]))
+    tx_in = TxIn(OutPoint(), "5151", 1, Witness([]))
     tx = Tx(vin=[tx_in], vout=[TxOut(100000000, "")])
 
-    err_msg = "empty stack"
+    err_msg = "Empty stack"
     with pytest.raises(BTClibValueError, match=err_msg):
         sig_hash.from_tx([utxo], tx, 0, 0)
 
 
 def test_wrapped_p2tr() -> None:
-    script = [
+    script: ScriptList = [
         "OP_1",
         "cc71eb30d653c0c3163990c47b976f3fb3f37cccdcbedb169a1dfef58bbfbfaf",
     ]
     utxo = TxOut(
         100000000, serialize(["OP_HASH160", hash160(serialize(script)), "OP_EQUAL"])
     )
     tx_in = TxIn(OutPoint(), serialize(script), 1, Witness(["0A" * 32]))
     tx = Tx(vin=[tx_in], vout=[TxOut(100000000, "")])
 
-    err_msg = "taproot scripts cannot be wrapped in p2sh"
+    err_msg = "Taproot scripts cannot be wrapped in p2sh"
     with pytest.raises(BTClibValueError, match=err_msg):
         sig_hash.from_tx([utxo], tx, 0, 0)
 
 
 def test_bip_test_vector() -> None:
     fname = "taproot_test_vector.json"
     filename = path.join(path.dirname(__file__), "_data", fname)
```

### Comparing `btclib-2023.5.30/tests/script/test_taproot.py` & `btclib-2023.7.12/tests/script_engine/test_transactions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,148 @@
 #!/usr/bin/env python3
 
-# Copyright (C) The btclib developers
+# Copyright (C) 2017-2021 The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
-"""Tests for the `btclib.script.taproot` module."""
+"""Tests for the `btclib.script.engine` module."""
 
 import json
+import warnings
 from os import path
 
 import pytest
 
-from btclib import b32
-from btclib.ec import mult
 from btclib.exceptions import BTClibValueError
-from btclib.script import (
-    TaprootScriptTree,
-    Witness,
-    check_output_pubkey,
-    input_script_sig,
-    is_p2tr,
-    output_prvkey,
-    output_pubkey,
-    parse,
-    serialize,
-    type_and_payload,
-)
-from btclib.tx import TxOut
+from btclib.script.engine import verify_input, verify_transaction
+from btclib.script.witness import Witness
+from btclib.tx.tx import Tx
+from btclib.tx.tx_out import ScriptPubKey, TxOut
+from tests.script_engine import parse_script
 
 
-def test_valid_script_path() -> None:
+def test_valid_taproot() -> None:
     fname = "tapscript_test_vector.json"
-    filename = path.join(path.dirname(__file__), "_data", fname)
+    filename = path.join(path.dirname(path.dirname(__file__)), "script", "_data", fname)
+
     with open(filename, encoding="ascii") as file_:
         data = json.load(file_)
 
-    for x in data:
+    for x in filter(lambda x: "TAPROOT" in x["flags"], data):
+        tx = Tx.parse(x["tx"])
+
         prevouts = [TxOut.parse(prevout) for prevout in x["prevouts"]]
         index = x["index"]
 
-        if not is_p2tr(prevouts[index].script_pub_key.script):
-            continue
-
-        script_sig = x["success"]["scriptSig"]
-        assert not script_sig
-
         witness = Witness(x["success"]["witness"])
-        if len(witness.stack) >= 2 and witness.stack[-1][0] == 0x50:
-            witness.stack = witness.stack[:-1]
-
-        # check script paths
-        if len(witness.stack) < 2:
-            continue
-
-        Q = type_and_payload(prevouts[index].script_pub_key.script)[1]
-
-        script = witness.stack[-2]
-        control = witness.stack[-1]
-
-        assert check_output_pubkey(Q, script, control)
-
+        tx.vin[index].script_witness = witness
+        tx.vin[index].script_sig = bytes.fromhex(x["success"]["scriptSig"])
 
-def test_taproot_key_tweaking() -> None:
-    prv_key = 123456
-    pub_key = mult(prv_key)
+        flags = x["flags"].split(",")
 
-    script_trees = [
-        None,
-        [(0xC0, ["OP_1"])],
-        [[(0xC0, ["OP_2"])], [(0xC0, ["OP_3"])]],
-    ]
+        verify_input(prevouts, tx, index, flags)
 
-    for script_tree in script_trees:
-        tweaked_prvkey = output_prvkey(prv_key, script_tree)
-        tweaked_pubkey = output_pubkey(pub_key, script_tree)[0]
-
-        assert tweaked_pubkey == mult(tweaked_prvkey)[0].to_bytes(32, "big")
 
+def test_invalid_taproot() -> None:
+    fname = "tapscript_test_vector.json"
+    filename = path.join(path.dirname(path.dirname(__file__)), "script", "_data", fname)
+    with open(filename, encoding="ascii") as file_:
+        data = json.load(file_)
 
-def test_invalid_control_block() -> None:
-    err_msg = "control block too long"
-    with pytest.raises(BTClibValueError, match=err_msg):
-        check_output_pubkey(b"\x00" * 32, b"\x00", b"\x00" * 4130)
+    for x in filter(lambda x: "TAPROOT" in x["flags"] and "failure" in x.keys(), data):
+        tx = Tx.parse(x["tx"])
 
-    err_msg = "invalid control block length"
-    with pytest.raises(BTClibValueError, match=err_msg):
-        check_output_pubkey(b"\x00" * 32, b"\x00", b"\x00" * 100)
+        prevouts = [TxOut.parse(prevout) for prevout in x["prevouts"]]
+        index = x["index"]
 
+        witness = Witness(x["failure"]["witness"])
+        tx.vin[index].script_witness = witness
+        tx.vin[index].script_sig = bytes.fromhex(x["failure"]["scriptSig"])
 
-def test_unspendable_script() -> None:
-    err_msg = "missing data"
-    with pytest.raises(BTClibValueError, match=err_msg):
-        output_pubkey()
+        flags = x["flags"].split(",")
+        with pytest.raises((BTClibValueError, IndexError, KeyError)):
+            verify_input(prevouts, tx, index, flags)
 
 
-def test_control_block() -> None:
-    script_tree = [[(0xC0, ["OP_2"])], [(0xC0, ["OP_3"])]]
-    pub_key = output_pubkey(None, script_tree)[0]
-    script, control = input_script_sig(None, script_tree, 0)
-    assert check_output_pubkey(pub_key, serialize(script), control)
+def test_valid_legacy() -> None:
+    fname = "tx_valid_legacy.json"
+    filename = path.join(path.dirname(__file__), "_data", fname)
+    with open(filename, encoding="ascii") as file_:
+        data = json.load(file_)
 
-    prv_key = 123456
-    internal_pubkey = mult(prv_key)
-    script_tree = [[(0xC0, ["OP_2"])], [(0xC0, ["OP_3"])]]
-    pub_key = output_pubkey(internal_pubkey, script_tree)[0]
-    script, control = input_script_sig(internal_pubkey, script_tree, 0)
-    assert check_output_pubkey(pub_key, serialize(script), control)
+    for x in data:
+        if isinstance(x[0], str):
+            continue
 
+        try:
+            tx = Tx.parse(x[1])
+        except BTClibValueError as e:
+            if "invalid satoshi amount:" in str(e):
+                continue
+
+        flags = [
+            "P2SH",
+            "SIGPUSHONLY",
+            "LOW_S",
+            "STRICTENC",
+            "DERSIG",
+            "CONST_SCRIPTCODE",
+            "NULLDUMMY",
+            "CLEANSTACK",
+            "MINIMALDATA",
+            # only standard, not consensus
+            # "NULLFAIL",
+            # "MINMALIF",
+            # "DISCOURAGE_UPGRADABLE_NOPS",
+            # "DISCOURAGE_UPGRADABLE_WITNESS_PROGRAM",
+            "CHECKLOCKTIMEVERIFY",
+            "CHECKSEQUENCEVERIFY",
+            "WITNESS",
+            "WITNESS_PUBKEYTYPE",
+            "TAPROOT",
+        ]
+        for f in x[2].split(","):
+            if f in flags:
+                flags.remove(f)
+
+        prevouts = []
+        for i in x[0]:
+            amount = 0 if len(i) == 3 else i[3]
+            script_pub_key = parse_script(i[2])
+            prevouts.append(TxOut(amount, ScriptPubKey(script_pub_key)))
 
-def convert_script_tree(script_tree: TaprootScriptTree) -> TaprootScriptTree:
-    if isinstance(script_tree, list):
-        return [convert_script_tree(x) for x in script_tree]
-    if isinstance(script_tree, dict):
-        return [[script_tree["leafVersion"], parse(script_tree["script"])]]
-    return []
+        verify_transaction(prevouts, tx, flags if flags != ["NONE"] else None)
 
 
-def test_bip_test_vector() -> None:
-    fname = "taproot_test_vector.json"
+def test_invalid_legacy() -> None:
+    fname = "tx_invalid_legacy.json"
     filename = path.join(path.dirname(__file__), "_data", fname)
     with open(filename, encoding="ascii") as file_:
-        data = json.load(file_)["scriptPubKey"]
+        data = json.load(file_)
 
-    for test in data:
-        pub_key = test["given"]["internalPubkey"]
-        script_tree = convert_script_tree(test["given"]["scriptTree"])
+    for x in data:
+        if isinstance(x[0], str):
+            continue
 
-        tweaked_pubkey = output_pubkey(f"02{pub_key}", script_tree)[0]
-        address = b32.p2tr(tweaked_pubkey)
+        try:
+            tx = Tx.parse(x[1])
+        except BTClibValueError as e:
+            if "invalid satoshi amount:" not in str(e):
+                continue
+            if "missing outputs" not in str(e):
+                continue
+
+        flags = x[2].split(",")  # different flags handling
+
+        prevouts = []
+        for i in x[0]:
+            amount = 0 if len(i) == 3 else i[3]
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                script_pub_key = parse_script(i[2])
+            prevouts.append(TxOut(amount, ScriptPubKey(script_pub_key)))
 
-        assert tweaked_pubkey.hex() == test["intermediary"]["tweakedPubkey"]
-        assert address == test["expected"]["bip350Address"]
+        with pytest.raises((BTClibValueError, IndexError, KeyError)):
+            verify_transaction(prevouts, tx, flags if flags != ["NONE"] else None)
```

### Comparing `btclib-2023.5.30/tests/script/test_witness.py` & `btclib-2023.7.12/tests/script/test_witness.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.script.witness` module."""
 
 import json
 from os import path
 
 from btclib.script import Witness
```

### Comparing `btclib-2023.5.30/tests/test_amount.py` & `btclib-2023.7.12/tests/test_amount.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.amount` module."""
 
 from __future__ import annotations
 
 from decimal import Decimal, FloatOperation, localcontext
 
 import pytest
```

### Comparing `btclib-2023.5.30/tests/test_b32.py` & `btclib-2023.7.12/tests/test_b32.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-
 """Tests for the `btclib.b32` module.
 
 Some of these tests are originally from
 https://github.com/sipa/bech32/tree/master/ref/python,
 with the following modifications:
 
 - splitted the original tests.py file in test_bech32.py
@@ -40,18 +39,19 @@
 """
 
 from __future__ import annotations
 
 import pytest
 
 from btclib import b32, b58
+from btclib.alias import ScriptList
 from btclib.ec import bytes_from_point, point_from_octets
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash160, sha256
-from btclib.script import Command, op_int, output_pubkey, serialize
+from btclib.script import op_int, output_pubkey, serialize
 
 
 def test_has_segwit_prefix() -> None:
     addr = b"bc1q0hy024867ednvuhy9en4dggflt5w9unw4ztl5a"
     assert b32.has_segwit_prefix(addr)
     assert b32.has_segwit_prefix(addr.decode("ascii"))
     addr = b"1PMycacnJaSqwwJqjawXBErnLsZ7RkXUAs"
@@ -100,15 +100,15 @@
         assert address.lower().strip() == addr
 
         wit_ver, wit_prg, network = b32.witness_from_address(
             address.strip().encode("ascii")
         )
         assert addr == b32.address_from_witness(wit_ver, wit_prg, network)
 
-        script_pub_key: list[Command] = [op_int(wit_ver), wit_prg]
+        script_pub_key: ScriptList = [op_int(wit_ver), wit_prg]
         assert serialize(script_pub_key).hex() == hexscript
 
 
 def test_invalid_address() -> None:
     """Test whether invalid addresses fail to decode."""
     invalid_addresses = [
         ("tc1qw508d6qejxtdg4y5r3zarvary0c5xw7kg3g4ty", "invalid hrp: "),
@@ -280,24 +280,24 @@
     with pytest.raises(BTClibValueError, match=err_msg):
         b32.address_from_witness(0, hash160(pub) + b"\x00")
 
 
 def test_p2wsh_p2sh() -> None:
     # leading/trailing spaces should be tolerated
     pub = " 02 79BE667EF9DCBBAC55A06295CE870B07029BFCDB2DCE28D959F2815B16F81798"
-    script_pub_key: list[Command] = [pub, "OP_CHECKSIG"]
+    script_pub_key: ScriptList = [pub, "OP_CHECKSIG"]
     witness_script_bytes = serialize(script_pub_key)
     b58.p2wsh_p2sh(witness_script_bytes)
     b58.p2wsh_p2sh(witness_script_bytes, "testnet")
 
 
 def test_p2wsh() -> None:
     # https://github.com/bitcoin/bips/blob/master/bip-0173.mediawiki
     pub = "02 79BE667EF9DCBBAC55A06295CE870B07029BFCDB2DCE28D959F2815B16F81798"
-    script_pub_key: list[Command] = [pub, "OP_CHECKSIG"]
+    script_pub_key: ScriptList = [pub, "OP_CHECKSIG"]
     witness_script_bytes = serialize(script_pub_key)
 
     addr = "tb1qrp33g0q5c5txsp9arysrx4k6zdkfs4nce4xj0gdcccefvpysxf3q0sl5k7"
     assert addr == b32.p2wsh(witness_script_bytes, "testnet")
     _, wit_prg, _ = b32.witness_from_address(addr)
     assert wit_prg == sha256(witness_script_bytes)
```

### Comparing `btclib-2023.5.30/tests/test_b58.py` & `btclib-2023.7.12/tests/test_b58.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.b58` module."""
 
 from __future__ import annotations
 
 import pytest
 
 from btclib import b32, b58
+from btclib.alias import ScriptList
 from btclib.base58 import b58encode
 from btclib.bip32 import bip32, slip132
 from btclib.ec import bytes_from_point, point_from_octets, secp256k1
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash160
-from btclib.script import Command, serialize
+from btclib.script.script import serialize
 from btclib.to_prv_key import prv_keyinfo_from_prv_key
 from btclib.to_pub_key import pub_keyinfo_from_key, pub_keyinfo_from_prv_key
 
 ec = secp256k1
 
 
 def test_wif_from_prv_key() -> None:
@@ -177,15 +177,15 @@
     assert address == b58.p2sh(script_pub_key, network)
 
     script_hash = hash160(script_pub_key)
     assert ("p2sh", script_hash, network) == b58.h160_from_address(address)
     assert ("p2sh", script_hash, network) == b58.h160_from_address(f" {address} ")
 
     assert script_hash.hex() == "4266fc6f2c2861d7fe229b279a79803afca7ba34"
-    script_sig: list[Command] = ["OP_HASH160", script_hash.hex(), "OP_EQUAL"]
+    script_sig: ScriptList = ["OP_HASH160", script_hash.hex(), "OP_EQUAL"]
     serialize(script_sig)
 
 
 def test_p2w_p2sh() -> None:
     pub_key_str = "03 a1af804ac108a8a51782198c2d034b28bf90c8803f5a53f76276fa69a4eae77f"
     pub_key, network = pub_keyinfo_from_key(pub_key_str, compressed=True)
     witness_program = hash160(pub_key)
```

### Comparing `btclib-2023.5.30/tests/test_base58.py` & `btclib-2023.7.12/tests/test_base58.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.base58` module."""
 
 import pytest
 
 from btclib.base58 import (
     _b58decode,
     _b58decode_to_int,
```

### Comparing `btclib-2023.5.30/tests/test_bech32.py` & `btclib-2023.7.12/tests/test_bech32.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-
 """Tests for the `btclib.bech32` module.
 
 These tests are originally from
 https://github.com/sipa/bech32/tree/master/ref/python,
 with the following modifications:
 
 - splitted the original tests.py file in test_bech32.py
```

### Comparing `btclib-2023.5.30/tests/test_hashes.py` & `btclib-2023.7.12/tests/test_hashes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.hashes` module."""
 
 from btclib.hashes import hash160, hash256
 from tests.test_to_key import (
     net_unaware_compressed_pub_keys,
     net_unaware_uncompressed_pub_keys,
     plain_prv_keys,
```

### Comparing `btclib-2023.5.30/tests/test_network.py` & `btclib-2023.7.12/tests/test_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.network` module."""
 
 import json
 from os import path
 
 import pytest
```

### Comparing `btclib-2023.5.30/tests/test_number_theory.py` & `btclib-2023.7.12/tests/test_number_theory.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.number_theory` module."""
 
 import pytest
 
 from btclib.exceptions import BTClibValueError
 from btclib.number_theory import mod_inv, mod_sqrt, tonelli
```

### Comparing `btclib-2023.5.30/tests/test_to_key.py` & `btclib-2023.7.12/tests/test_to_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Test vectors of valid and invalid keys.
 
 Used by `btclib.tests.to_pub_key` and `btclib.tests.to_pub_key` modules.
 Test vectors do include str only: no int, point tuble, or BIP32KeyData.
 """
 
 from __future__ import annotations
```

### Comparing `btclib-2023.5.30/tests/test_to_prv_key.py` & `btclib-2023.7.12/tests/test_to_prv_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.to_prv_key` module."""
 
 # Third party imports
 import pytest
 
 # Library imports
 from btclib.alias import INF
```

### Comparing `btclib-2023.5.30/tests/test_to_pub_key.py` & `btclib-2023.7.12/tests/test_to_pub_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.to_pub_key` module."""
 
 import pytest
 
 from btclib.alias import INF
 from btclib.bip32 import BIP32KeyData, derive, rootxprv_from_seed
 from btclib.ec import bytes_from_point
@@ -115,17 +114,17 @@
             point_from_pub_key(prv_key5, secp256r1)
         assert pub_keyinfo_from_pub_key(prv_key5) in (m_c, m_unc)
         assert pub_keyinfo_from_pub_key(prv_key5, "mainnet") in (m_c, m_unc)
         assert pub_keyinfo_from_pub_key(prv_key5, "testnet") in (t_c, t_unc)
 
     for invalid_pub_key in [INF, INF_xpub_data, *invalid_pub_keys]:
         with pytest.raises(BTClibValueError):
-            point_from_pub_key(invalid_pub_key)  # type: ignore
+            point_from_pub_key(invalid_pub_key)  # type: ignore[arg-type]
         with pytest.raises(BTClibValueError):
-            pub_keyinfo_from_pub_key(invalid_pub_key)  # type: ignore
+            pub_keyinfo_from_pub_key(invalid_pub_key)  # type: ignore[arg-type]
 
     for not_a_pub_key in [
         INF,
         INF_xpub_data,
         *not_a_pub_keys,
         q,
         q0,
@@ -134,17 +133,17 @@
         xprv_data,
         xprv0_data,
         xprvn_data,
         *compressed_prv_keys,
         *uncompressed_prv_keys,
     ]:
         with pytest.raises(BTClibValueError):
-            point_from_pub_key(not_a_pub_key)  # type: ignore
+            point_from_pub_key(not_a_pub_key)  # type: ignore[arg-type]
         with pytest.raises(BTClibValueError):
-            pub_keyinfo_from_pub_key(not_a_pub_key)  # type: ignore
+            pub_keyinfo_from_pub_key(not_a_pub_key)  # type: ignore[arg-type]
 
     for key in [Q, *plain_pub_keys, q, *plain_prv_keys]:
         assert Q == point_from_key(key)
         assert m_c == pub_keyinfo_from_key(key)
         assert m_c == pub_keyinfo_from_key(key, "mainnet")
         assert m_c == pub_keyinfo_from_key(key, "mainnet", compressed=True)
         assert m_c == pub_keyinfo_from_key(key, compressed=True)
@@ -202,17 +201,17 @@
         q0,
         qn,
         xprv0_data,
         xprvn_data,
         *invalid_prv_keys,
     ]:
         with pytest.raises(BTClibValueError):
-            point_from_key(invalid_key)  # type: ignore
+            point_from_key(invalid_key)  # type: ignore[arg-type]
         with pytest.raises(BTClibValueError):
-            pub_keyinfo_from_key(invalid_key)  # type: ignore
+            pub_keyinfo_from_key(invalid_key)  # type: ignore[arg-type]
 
     for not_a_key in [
         q0,
         qn,
         xprv0_data,
         xprvn_data,
         INF,
```

### Comparing `btclib-2023.5.30/tests/test_utils.py` & `btclib-2023.7.12/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.utils` module."""
 
 import random
 
 import pytest
 
 from btclib.exceptions import BTClibValueError
```

### Comparing `btclib-2023.5.30/tests/test_var_int.py` & `btclib-2023.7.12/tests/test_var_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.var_int` module."""
 
 import pytest
 
 from btclib import var_int
 from btclib.exceptions import BTClibValueError
```

### Comparing `btclib-2023.5.30/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin` & `btclib-2023.7.12/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/tx/_generated_files/tx.json` & `btclib-2023.7.12/tests/tx/_generated_files/tx.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/tx/_generated_files/tx_in.json` & `btclib-2023.7.12/tests/tx/_generated_files/tx_in.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.5.30/tests/tx/test_out_point.py` & `btclib-2023.7.12/tests/tx/test_out_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.tx_in` module."""
 
 import json
 from os import path
 
 import pytest
```

### Comparing `btclib-2023.5.30/tests/tx/test_tx.py` & `btclib-2023.7.12/tests/tx/test_tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.tx` module."""
 
 import json
 from os import path
 
 import pytest
 
 from btclib.exceptions import BTClibValueError
-from btclib.script import Witness
+from btclib.script import ScriptPubKey, Witness
 from btclib.tx import OutPoint, Tx, TxIn, TxOut, join_txs
 
 
 def test_tx() -> None:
     # default constructor
     tx = Tx(check_validity=False)
     assert not tx.is_segwit()
@@ -37,15 +36,17 @@
     assert tx.id.hex() == tx_id
     assert tx.hash == tx.id
     assert tx.size == 10
     assert tx.vsize == tx.size
     assert tx.weight == tx.size * 4
 
     with pytest.raises(BTClibValueError, match="Missing inputs"):
-        tx.assert_valid()
+        Tx(vout=[TxOut(0, ScriptPubKey(""))])
+    with pytest.raises(BTClibValueError, match="Missing outputs"):
+        Tx(vin=[TxIn(script_sig="0000")])
 
     tx_2 = Tx.from_dict(tx.to_dict(check_validity=False), check_validity=False)
     assert tx_2.is_segwit() == tx.is_segwit()
     assert tx_2 == tx
 
     tx_2 = Tx.parse(
         tx.serialize(include_witness=True, check_validity=False), check_validity=False
@@ -334,15 +335,15 @@
     assert any(bool(tx_in.script_witness) for tx_in in tx.vin)
     assert tx.vin[0].script_witness
     assert tx.vin[0].script_witness.stack
 
     # Tx dataclass to dict
     tx_dict = tx.to_dict()
     assert isinstance(tx_dict, dict)
-    assert tx_dict["vin"][0]["txinwitness"]["stack"]  # type: ignore
+    assert tx_dict["vin"][0]["txinwitness"]["stack"]  # type: ignore[index]
 
     # Tx dataclass dict to file
     datadir = path.join(path.dirname(__file__), "_generated_files")
     filename = path.join(datadir, "tx.json")
     with open(filename, "w", encoding="ascii") as file_:
         json.dump(tx_dict, file_, indent=4)
         file_.write("\n")  # end-of-file-fixer
```

### Comparing `btclib-2023.5.30/tests/tx/test_tx_in.py` & `btclib-2023.7.12/tests/tx/test_tx_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.tx_in` module."""
 
 import json
 from os import path
 
 import pytest
```

### Comparing `btclib-2023.5.30/tests/tx/test_tx_out.py` & `btclib-2023.7.12/tests/tx/test_tx_out.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) The btclib developers
 #
 # This file is part of btclib. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution.
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
-
 """Tests for the `btclib.tx_out` module."""
 
 import json
 from os import path
 
 import pytest
```

