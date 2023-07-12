# Comparing `tmp/moneyonchain_prices_source-0.6.6b1.tar.gz` & `tmp/moneyonchain_prices_source-0.6.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.6.6b1.tar", last modified: Tue Jul 11 17:57:21 2023, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.6.6b2.tar", last modified: Wed Jul 12 20:12:19 2023, max compression
```

## Comparing `moneyonchain_prices_source-0.6.6b1.tar` & `moneyonchain_prices_source-0.6.6b2.tar`

### file list

```diff
@@ -1,112 +1,115 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.858010 moneyonchain_prices_source-0.6.6b1/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:57:21.854010 moneyonchain_prices_source-0.6.6b1/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.830008 moneyonchain_prices_source-0.6.6b1/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4577 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2213 2023-07-11 14:14:12.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.834009 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2219 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.854010 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-10 19:48:43.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4635 2023-07-11 14:12:57.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-10 19:46:36.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-07-11 17:52:42.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bithumbpro.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 14:34:01.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_emdx.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_clarin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-07-11 17:54:55.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4710 2022-12-28 13:47:46.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.854010 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4527 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-11 17:57:21.858010 moneyonchain_prices_source-0.6.6b1/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-12 20:12:19.052638 moneyonchain_prices_source-0.6.6b2/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-12 20:12:19.052638 moneyonchain_prices_source-0.6.6b2/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-12 20:12:19.028649 moneyonchain_prices_source-0.6.6b2/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4577 2023-07-12 17:16:52.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2437 2023-07-12 15:17:54.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-12 20:12:19.028649 moneyonchain_prices_source-0.6.6b2/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2312 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-12 20:12:19.048640 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 20:25:45.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4783 2023-07-12 15:17:54.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-12 15:36:26.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-10 19:46:36.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_bithumbpro.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 14:34:01.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccb_emdx.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccb_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_clarin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-12 20:08:15.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 21:09:00.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usdt_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 20:50:33.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usdt_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-11 21:05:01.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usdt_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-07-12 20:11:08.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4710 2022-12-28 13:47:46.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-12 20:12:19.052638 moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-12 20:12:18.000000 moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4666 2023-07-12 20:12:18.000000 moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-12 20:12:18.000000 moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-12 20:12:18.000000 moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-12 20:12:18.000000 moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-12 20:12:19.052638 moneyonchain_prices_source-0.6.6b2/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b2/setup.py
```

### Comparing `moneyonchain_prices_source-0.6.6b1/PKG-INFO` & `moneyonchain_prices_source-0.6.6b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain_prices_source
-Version: 0.6.6b1
+Version: 0.6.6b2
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # MoC prices source
```

### Comparing `moneyonchain_prices_source-0.6.6b1/README.md` & `moneyonchain_prices_source-0.6.6b2/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/cli_check.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/computed_pairs.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,42 +4,46 @@
 from types   import LambdaType
 
 base_dir = dirname(abspath(__file__))
 
 bkpath   = sys.path[:]
 sys.path.append(dirname(base_dir))
 
-from moc_prices_source.engines.coins import RIF_USDT, BTC_USD, MOC_BTC, RIF_BTC, ETH_BTC, MOC_USD, RIF_USD, RIF_USD_B, RIF_USD_T, ETH_USD, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, USD_ARS_CCB_MOC, BTC_ARS
+from moc_prices_source.engines.coins import RIF_USDT, BTC_USD, MOC_BTC, RIF_BTC, ETH_BTC, MOC_USD, RIF_USD, RIF_USD_B, RIF_USD_T, ETH_USD, USDT_USD_B, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, USD_ARS_CCB_MOC, BTC_ARS, RIF_USD_TB
 
 sys.path = bkpath
 
 
 
 computed_pairs = {
     MOC_USD: {
         'requirements': [MOC_BTC, BTC_USD],
         'formula': lambda moc_btc, btc_usd: moc_btc * btc_usd
     },
     RIF_USD_B: { # Passing through Bitcoin
         'requirements': [RIF_BTC, BTC_USD],
         'formula': lambda rif_btc, btc_usd: rif_btc * btc_usd
     },
-    RIF_USD_T: { # Passing through Tether
+    RIF_USD_TB: { # Passing through Tether & Bitcoin
         'requirements': [RIF_USDT, BTC_USD, BTC_USDT],
         'formula': lambda rif_usdt, btc_usd, btc_usdt: rif_usdt * btc_usd / btc_usdt
     },
+    RIF_USD_T: { # Passing through Tether
+        'requirements': [RIF_USDT, USDT_USD],
+        'formula': lambda rif_usdt, usdt_usd: rif_usdt * usdt_usd
+    },
     RIF_USD: { # Leave this as legacy
         'requirements': [RIF_BTC, BTC_USD],
         'formula': lambda rif_btc, btc_usd: rif_btc * btc_usd
     },
     ETH_USD: {
         'requirements': [ETH_BTC, BTC_USD],
         'formula': lambda eth_btc, btc_usd: eth_btc * btc_usd
     },
-    USDT_USD: {
+    USDT_USD_B: { # Passing through Bitcoin
         'requirements': [BTC_USD, BTC_USDT],
         'formula': lambda btc_usd, btc_usdt: btc_usd / btc_usdt
     },
     BNB_USD: {
         'requirements': [BNB_USDT, BTC_USD, BTC_USDT],
         'formula': lambda bnb_usdt, btc_usd, btc_usdt: bnb_usdt * btc_usd / btc_usdt
     },
```

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/data/weighing.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'btc_usdt_binance'": '0.8',*

 * * "'btc_usdt_bitfinex'": '0.05',*

 * * "'btc_usdt_coinbase'": '0.1',*

 * * "'btc_usdt_kraken'": '0.05',*

 * * "'usdt_usd_bitstamp'": '0.15',*

 * * "'usdt_usd_coinbase'": '0.45',*

 * * "'usdt_usd_kraken'": '0.4'}*

```diff
@@ -11,18 +11,18 @@
     "btc_ars_rofex": 0.1,
     "btc_ars_satoshitango": 0.1,
     "btc_usd_bitfinex": 0.18,
     "btc_usd_bitstamp": 0.22,
     "btc_usd_coinbase": 0.25,
     "btc_usd_gemini": 0.17,
     "btc_usd_kraken": 0.18,
-    "btc_usdt_binance": 0.25,
-    "btc_usdt_bitfinex": 0.25,
-    "btc_usdt_coinbase": 0.25,
-    "btc_usdt_kraken": 0.25,
+    "btc_usdt_binance": 0.8,
+    "btc_usdt_bitfinex": 0.05,
+    "btc_usdt_coinbase": 0.1,
+    "btc_usdt_kraken": 0.05,
     "eth_btc_binance": 0.25,
     "eth_btc_bitfinex": 0.25,
     "eth_btc_bitstamp": 0.25,
     "eth_btc_gemini": 0,
     "eth_btc_kraken": 0.25,
     "gas_btc_rsk": 1,
     "moc_btc_sovryn": 1,
@@ -61,9 +61,12 @@
     "usd_mxn_currencymeuk": 0.1,
     "usd_mxn_eldolar_info": 0.1,
     "usd_mxn_eleconomista": 0.1,
     "usd_mxn_infodolar": 0.1,
     "usd_mxn_intercam": 0.1,
     "usd_mxn_themoneyconverter": 0.1,
     "usd_mxn_wise": 0.1,
-    "usd_mxn_xrates": 0.1
+    "usd_mxn_xrates": 0.1,
+    "usdt_usd_bitstamp": 0.15,
+    "usdt_usd_coinbase": 0.45,
+    "usdt_usd_kraken": 0.4
 }
```

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/database.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/coins.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,23 +118,25 @@
         return hash(str(self))
 
 
 BTC_USD         = CoinPair(BTC,  USD)
 BTC_ARS         = CoinPair(BTC,  ARS)
 RIF_BTC         = CoinPair(RIF,  BTC)
 RIF_USD         = CoinPair(RIF,  USD) # Leave this as legacy
-RIF_USD_B       = CoinPair(RIF,  USD, "B") # Passing through Tether
-RIF_USD_T       = CoinPair(RIF,  USD, "T") # Passing through Bitcoin
+RIF_USD_B       = CoinPair(RIF,  USD, "B") # Passing through Bitcoin
+RIF_USD_T       = CoinPair(RIF,  USD, "T") # Passing through Tether
+RIF_USD_TB      = CoinPair(RIF,  USD, "TB") # Passing through Tether & Bitcoin
 RIF_USDT        = CoinPair(RIF,  USDT)
 MOC_BTC         = CoinPair(MOC,  BTC)
 MOC_USD         = CoinPair(MOC,  USD)
 ETH_BTC         = CoinPair(ETH,  BTC)
 ETH_USD         = CoinPair(ETH,  USD)
 BTC_USDT        = CoinPair(BTC,  USDT)
 USDT_USD        = CoinPair(USDT, USD)
+USDT_USD_B      = CoinPair(USDT, USD, "B") # Passing through Bitcoin
 BNB_USDT        = CoinPair(BNB,  USDT)
 BNB_USD         = CoinPair(BNB,  USD)
 USD_ARS         = CoinPair(USD,  ARS)
 USD_ARS_CCL     = CoinPair(USD,  ARS, "CCL")
 USD_ARS_CCB     = CoinPair(USD,  ARS, "CCB")
 USD_ARS_CCB_MOC = CoinPair(USD,  ARS, "CCB by MOC")
 USD_MXN         = CoinPair(USD,  MXN)
```

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/engine_base.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/gas_btc_rsk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bithumbpro.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_bithumbpro.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_emdx.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccb_emdx.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_rofex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccb_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarito.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_clarin.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_clarin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarito.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.6.6b2/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain-prices-source
-Version: 0.6.6b1
+Version: 0.6.6b2
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # MoC prices source
```

### Comparing `moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.6.6b2/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,12 +94,15 @@
 moc_prices_source/engines/usd_mxn_eldolar_info.py
 moc_prices_source/engines/usd_mxn_eleconomista.py
 moc_prices_source/engines/usd_mxn_infodolar.py
 moc_prices_source/engines/usd_mxn_intercam.py
 moc_prices_source/engines/usd_mxn_themoneyconverter.py
 moc_prices_source/engines/usd_mxn_wise.py
 moc_prices_source/engines/usd_mxn_xrates.py
+moc_prices_source/engines/usdt_usd_bitstamp.py
+moc_prices_source/engines/usdt_usd_coinbase.py
+moc_prices_source/engines/usdt_usd_kraken.py
 moneyonchain_prices_source.egg-info/PKG-INFO
 moneyonchain_prices_source.egg-info/SOURCES.txt
 moneyonchain_prices_source.egg-info/dependency_links.txt
 moneyonchain_prices_source.egg-info/requires.txt
 moneyonchain_prices_source.egg-info/top_level.txt
```

### Comparing `moneyonchain_prices_source-0.6.6b1/setup.py` & `moneyonchain_prices_source-0.6.6b2/setup.py`

 * *Files identical despite different names*

