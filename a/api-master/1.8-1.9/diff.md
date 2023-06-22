# Comparing `tmp/api_master-1.8.tar.gz` & `tmp/api_master-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_master-1.8.tar", last modified: Tue Jun 20 19:28:05 2023, max compression
+gzip compressed data, was "api_master-1.9.tar", last modified: Tue Jun 20 19:39:12 2023, max compression
```

## Comparing `api_master-1.8.tar` & `api_master-1.9.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.456256 api_master-1.8/
--rw-rw-rw-   0        0        0     2484 2023-06-20 19:28:05.454993 api_master-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-12 00:29:12.000000 api_master-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.268426 api_master-1.8/api_master/
--rw-rw-rw-   0        0        0        0 2023-06-20 17:56:44.000000 api_master-1.8/api_master/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.289899 api_master-1.8/api_master/_discord/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/__init__.py
--rw-rw-rw-   0        0        0     7983 2023-06-18 18:41:08.000000 api_master-1.8/api_master/_discord/discord_stock_example.py
--rw-rw-rw-   0        0        0    44936 2023-06-18 18:41:08.000000 api_master-1.8/api_master/_discord/discord_stock_market.py
--rw-rw-rw-   0        0        0    16306 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/embeddings.py
--rw-rw-rw-   0        0        0      581 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/emojis.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.291898 api_master-1.8/api_master/_discord/hooks/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/hooks/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/hooks/channel_webhooks.py
--rw-rw-rw-   0        0        0    10521 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/hooks/hook_dicts.py
--rw-rw-rw-   0        0        0     5462 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/hooks/send_webhook.py
--rw-rw-rw-   0        0        0    33594 2023-06-18 18:41:08.000000 api_master-1.8/api_master/_discord/live_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.293897 api_master-1.8/api_master/_discord/selectmenus/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/selectmenus/__init__.py
--rw-rw-rw-   0        0        0    33209 2023-06-18 18:41:08.000000 api_master-1.8/api_master/_discord/selectmenus/mainselect.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.294900 api_master-1.8/api_master/_discord/views/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/views/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-18 18:41:08.000000 api_master-1.8/api_master/_discord/views/mainview.py
--rw-rw-rw-   0        0        0     3792 2023-06-11 21:54:23.000000 api_master-1.8/api_master/_discord/views/menus.py
--rw-rw-rw-   0        0        0     7502 2023-06-18 18:41:08.000000 api_master-1.8/api_master/_discord/webhook_creation.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.297898 api_master-1.8/api_master/bot/
--rw-rw-rw-   0        0        0       72 2023-06-16 22:29:19.000000 api_master-1.8/api_master/bot/__init__.py
--rw-rw-rw-   0        0        0    13401 2023-06-18 18:55:44.000000 api_master-1.8/api_master/bot/autocomp.py
--rw-rw-rw-   0        0        0     6919 2023-06-11 22:19:59.000000 api_master-1.8/api_master/bot/discord_emojis.py
--rw-rw-rw-   0        0        0     3838 2023-06-20 14:10:53.000000 api_master-1.8/api_master/bot/main.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.301896 api_master-1.8/api_master/bot/utils/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.8/api_master/bot/utils/__init__.py
--rw-rw-rw-   0        0        0     1368 2023-06-16 02:40:26.000000 api_master-1.8/api_master/bot/utils/crypto_coins.py
--rw-rw-rw-   0        0        0      998 2023-06-16 02:35:33.000000 api_master-1.8/api_master/bot/utils/date_times.py
--rw-rw-rw-   0        0        0   224003 2023-06-16 03:10:59.000000 api_master-1.8/api_master/bot/utils/lists_and_dicts.py
--rw-rw-rw-   0        0        0   199781 2023-06-16 02:46:46.000000 api_master-1.8/api_master/bot/utils/webull_tickers.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.303897 api_master-1.8/api_master/bot/views/
--rw-rw-rw-   0        0        0       49 2023-06-16 22:29:34.000000 api_master-1.8/api_master/bot/views/__init__.py
--rw-rw-rw-   0        0        0  1503926 2023-06-18 18:41:09.000000 api_master-1.8/api_master/bot/views/learnviews.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.321490 api_master-1.8/api_master/bot/views/uiviews/
--rw-rw-rw-   0        0        0   320159 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/MarketAnalysis.py
--rw-rw-rw-   0        0        0     5109 2023-06-16 03:43:55.000000 api_master-1.8/api_master/bot/views/uiviews/TickerAnalysis.py
--rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.8/api_master/bot/views/uiviews/__init__ copy.py
--rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.8/api_master/bot/views/uiviews/__init__.py
--rw-rw-rw-   0        0        0     5169 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/capitalflow.py
--rw-rw-rw-   0        0        0   110984 2022-11-14 02:53:40.000000 api_master-1.8/api_master/bot/views/uiviews/cmslist.py
--rw-rw-rw-   0        0        0   107414 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/cmslist2.py
--rw-rw-rw-   0        0        0    18026 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/directiondrop.py
--rw-rw-rw-   0        0        0     9311 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/financialselects.py
--rw-rw-rw-   0        0        0    12480 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/ftds.py
--rw-rw-rw-   0        0        0     4675 2023-06-16 03:04:58.000000 api_master-1.8/api_master/bot/views/uiviews/leveragedropdown.py
--rw-rw-rw-   0        0        0     7693 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/lowfloat.py
--rw-rw-rw-   0        0        0     4487 2023-06-16 03:51:49.000000 api_master-1.8/api_master/bot/views/uiviews/masterview.py
--rw-rw-rw-   0        0        0     5619 2022-11-05 23:34:22.000000 api_master-1.8/api_master/bot/views/uiviews/mostactive.py
--rw-rw-rw-   0        0        0     6579 2022-11-05 23:04:27.000000 api_master-1.8/api_master/bot/views/uiviews/pressrelease.py
--rw-rw-rw-   0        0        0     3355 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/quote.py
--rw-rw-rw-   0        0        0    13749 2023-06-18 18:41:08.000000 api_master-1.8/api_master/bot/views/uiviews/shortinterest.py
--rw-rw-rw-   0        0        0     3714 2023-06-20 00:08:12.000000 api_master-1.8/api_master/cfg.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.400553 api_master-1.8/api_master/examples/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.8/api_master/examples/__init__.py
--rw-rw-rw-   0        0        0      703 2023-06-14 15:26:12.000000 api_master-1.8/api_master/examples/helpers.py
--rw-rw-rw-   0        0        0      333 2023-06-20 17:45:26.000000 api_master-1.8/api_master/examples/nasdaq_bigmac.py
--rw-rw-rw-   0        0        0      294 2023-06-19 16:25:15.000000 api_master-1.8/api_master/examples/nasdaq_economic_indicators.py
--rw-rw-rw-   0        0        0      204 2023-06-19 16:36:33.000000 api_master-1.8/api_master/examples/nasdaq_gdp.py
--rw-rw-rw-   0        0        0      293 2023-06-19 16:19:39.000000 api_master-1.8/api_master/examples/nasdaq_income_expenditures.py
--rw-rw-rw-   0        0        0      254 2023-06-19 16:05:10.000000 api_master-1.8/api_master/examples/nasdaq_inflation.py
--rw-rw-rw-   0        0        0      278 2023-06-19 16:31:10.000000 api_master-1.8/api_master/examples/nasdaq_interest_rates.py
--rw-rw-rw-   0        0        0      249 2023-06-19 16:10:55.000000 api_master-1.8/api_master/examples/nasdaq_repos.py
--rw-rw-rw-   0        0        0      252 2023-06-19 16:14:00.000000 api_master-1.8/api_master/examples/nasdaq_sp500.py
--rw-rw-rw-   0        0        0      231 2023-06-19 16:30:11.000000 api_master-1.8/api_master/examples/nasdaq_unemployment.py
--rw-rw-rw-   0        0        0      661 2023-06-19 21:19:24.000000 api_master-1.8/api_master/examples/occ_stock_loans.py
--rw-rw-rw-   0        0        0      456 2023-06-19 21:44:19.000000 api_master-1.8/api_master/examples/occ_volume_totals.py
--rw-rw-rw-   0        0        0     5940 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_attributes.py
--rw-rw-rw-   0        0        0      533 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_bollinger_bands.py
--rw-rw-rw-   0        0        0     4375 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_candle_patterns.py
--rw-rw-rw-   0        0        0      706 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_create_option_symbol.py
--rw-rw-rw-   0        0        0     2479 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_crypto_market.py
--rw-rw-rw-   0        0        0    44945 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_discord_market.py
--rw-rw-rw-   0        0        0     1376 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_ema.py
--rw-rw-rw-   0        0        0      910 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_fetch_entire_chain.py
--rw-rw-rw-   0        0        0      693 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_find_gaps.py
--rw-rw-rw-   0        0        0      922 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_forex_market.py
--rw-rw-rw-   0        0        0      823 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_all_options_data.py
--rw-rw-rw-   0        0        0    36288 2023-06-17 02:25:07.000000 api_master-1.8/api_master/examples/polygon_get_data.py
--rw-rw-rw-   0        0        0     2399 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_ema.py
--rw-rw-rw-   0        0        0      619 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      585 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_latest_forex_data.py
--rw-rw-rw-   0        0        0      446 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_latest_indices_data.py
--rw-rw-rw-   0        0        0      762 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_latest_options_data.py
--rw-rw-rw-   0        0        0      598 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_latest_ticker_data.py
--rw-rw-rw-   0        0        0      644 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_logo.py
--rw-rw-rw-   0        0        0     3195 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_macd.py
--rw-rw-rw-   0        0        0      665 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_pivot_points.py
--rw-rw-rw-   0        0        0     1192 2023-06-19 15:17:22.000000 api_master-1.8/api_master/examples/polygon_get_price_data.py
--rw-rw-rw-   0        0        0     2051 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_rsi.py
--rw-rw-rw-   0        0        0     1935 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_get_sma.py
--rw-rw-rw-   0        0        0      776 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_indices_market.py
--rw-rw-rw-   0        0        0     1796 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_latest_news.py
--rw-rw-rw-   0        0        0      930 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_macd_sma_rsi.py
--rw-rw-rw-   0        0        0     1625 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_option_quote.py
--rw-rw-rw-   0        0        0     2408 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_option_trades.py
--rw-rw-rw-   0        0        0      989 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_options_market.py
--rw-rw-rw-   0        0        0     1509 2023-06-19 15:17:30.000000 api_master-1.8/api_master/examples/polygon_plot_aggs.py
--rw-rw-rw-   0        0        0      796 2023-06-19 16:18:45.000000 api_master-1.8/api_master/examples/polygon_plot_macd.py
--rw-rw-rw-   0        0        0     1797 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_plot_option_aggs.py
--rw-rw-rw-   0        0        0      487 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_rate_of_change.py
--rw-rw-rw-   0        0        0      628 2023-06-20 19:26:38.000000 api_master-1.8/api_master/examples/polygon_rsi.py
--rw-rw-rw-   0        0        0     8185 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_scan_candles.py
--rw-rw-rw-   0        0        0     5590 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_scanner_example.py
--rw-rw-rw-   0        0        0     2116 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_stock_aggregates.py
--rw-rw-rw-   0        0        0     1189 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/polygon_support_resistance.py
--rw-rw-rw-   0        0        0     1052 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/sec_sec_filings.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.403553 api_master-1.8/api_master/examples/simulated_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.8/api_master/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-11 21:54:23.000000 api_master-1.8/api_master/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     5115 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/simulated_markets/mock_discord.py
--rw-rw-rw-   0        0        0     1951 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1551 2023-06-18 18:41:08.000000 api_master-1.8/api_master/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0        0 2023-06-19 02:12:58.000000 api_master-1.8/api_master/examples/stocksera-web_mentions.py
--rw-rw-rw-   0        0        0      804 2023-06-19 01:10:14.000000 api_master-1.8/api_master/examples/stocksera_IPO_calendar.py
--rw-rw-rw-   0        0        0     1209 2023-06-19 01:01:37.000000 api_master-1.8/api_master/examples/stocksera_earnings_calendar.py
--rw-rw-rw-   0        0        0      651 2023-06-19 02:55:19.000000 api_master-1.8/api_master/examples/stocksera_fails_to_deliver.py
--rw-rw-rw-   0        0        0      286 2023-06-19 00:56:26.000000 api_master-1.8/api_master/examples/stocksera_inflation.py
--rw-rw-rw-   0        0        0      458 2023-06-19 01:05:25.000000 api_master-1.8/api_master/examples/stocksera_jim_cramer.py
--rw-rw-rw-   0        0        0      537 2023-06-19 00:40:17.000000 api_master-1.8/api_master/examples/stocksera_jobless_claims.py
--rw-rw-rw-   0        0        0      579 2023-06-19 00:55:25.000000 api_master-1.8/api_master/examples/stocksera_latest_insider_summary.py
--rw-rw-rw-   0        0        0     1147 2023-06-19 00:44:35.000000 api_master-1.8/api_master/examples/stocksera_low_floats.py
--rw-rw-rw-   0        0        0      400 2023-06-19 00:37:38.000000 api_master-1.8/api_master/examples/stocksera_market_news.py
--rw-rw-rw-   0        0        0      501 2023-06-19 00:42:29.000000 api_master-1.8/api_master/examples/stocksera_news_sentiment.py
--rw-rw-rw-   0        0        0      544 2023-06-19 01:12:25.000000 api_master-1.8/api_master/examples/stocksera_retail_sales.py
--rw-rw-rw-   0        0        0      522 2023-06-19 00:41:01.000000 api_master-1.8/api_master/examples/stocksera_reverse_repo.py
--rw-rw-rw-   0        0        0      561 2023-06-19 00:53:52.000000 api_master-1.8/api_master/examples/stocksera_sec_filings.py
--rw-rw-rw-   0        0        0      772 2023-06-19 00:48:53.000000 api_master-1.8/api_master/examples/stocksera_short_interest.py
--rw-rw-rw-   0        0        0      593 2023-06-19 00:46:32.000000 api_master-1.8/api_master/examples/stocksera_short_volume.py
--rw-rw-rw-   0        0        0      496 2023-06-19 00:50:13.000000 api_master-1.8/api_master/examples/stocksera_stocktwits.py
--rw-rw-rw-   0        0        0      603 2023-06-19 00:51:40.000000 api_master-1.8/api_master/examples/stocksera_subreddits.py
--rw-rw-rw-   0        0        0      643 2023-06-19 00:40:51.000000 api_master-1.8/api_master/examples/stocksera_treasury_balance.py
--rw-rw-rw-   0        0        0      534 2023-06-19 02:28:28.000000 api_master-1.8/api_master/examples/stocksera_wsb_options.py
--rw-rw-rw-   0        0        0      988 2023-06-20 19:19:22.000000 api_master-1.8/api_master/examples/webull_analyst_ratings.py
--rw-rw-rw-   0        0        0     5595 2023-06-20 19:19:50.000000 api_master-1.8/api_master/examples/webull_balance_sheet.py
--rw-rw-rw-   0        0        0     3288 2023-06-20 19:20:32.000000 api_master-1.8/api_master/examples/webull_cash_flow.py
--rw-rw-rw-   0        0        0     1549 2023-06-20 19:20:53.000000 api_master-1.8/api_master/examples/webull_cost_distribution.py
--rw-rw-rw-   0        0        0     4558 2023-06-20 19:21:34.000000 api_master-1.8/api_master/examples/webull_earnings_calendar.py
--rw-rw-rw-   0        0        0     2286 2023-06-20 19:21:53.000000 api_master-1.8/api_master/examples/webull_examples.py
--rw-rw-rw-   0        0        0     4335 2023-06-20 19:22:12.000000 api_master-1.8/api_master/examples/webull_financial_statement.py
--rw-rw-rw-   0        0        0      377 2023-06-20 18:14:28.000000 api_master-1.8/api_master/examples/webull_get_webull_data.py
--rw-rw-rw-   0        0        0     2128 2023-06-20 19:22:38.000000 api_master-1.8/api_master/examples/webull_institutions.py
--rw-rw-rw-   0        0        0     1241 2023-06-20 19:22:55.000000 api_master-1.8/api_master/examples/webull_short_interest.py
--rw-rw-rw-   0        0        0     1537 2023-06-20 19:25:22.000000 api_master-1.8/api_master/examples/webull_stock_data.py
--rw-rw-rw-   0        0        0      809 2023-06-20 19:25:47.000000 api_master-1.8/api_master/examples/webull_volume_analysis.py
--rw-rw-rw-   0        0        0    14776 2023-06-16 14:39:01.000000 api_master-1.8/api_master/examples/webull_webull_data.py
--rw-rw-rw-   0        0        0     1383 2023-06-17 17:45:02.000000 api_master-1.8/api_master/myconfig.py
--rw-rw-rw-   0        0        0     4167 2023-06-17 02:16:41.000000 api_master-1.8/api_master/oldapp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.404554 api_master-1.8/api_master/sdks/
--rw-rw-rw-   0        0        0      275 2023-06-16 23:26:41.000000 api_master-1.8/api_master/sdks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.407553 api_master-1.8/api_master/sdks/discord_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/discord_sdk/__init__.py
--rw-rw-rw-   0        0        0       53 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/discord_sdk/channel_ids.py
--rw-rw-rw-   0        0        0     4497 2023-06-18 18:41:08.000000 api_master-1.8/api_master/sdks/discord_sdk/discord_sdk.py
--rw-rw-rw-   0        0        0     2157 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/discord_sdk/searching.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.410553 api_master-1.8/api_master/sdks/fudstop_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-12 00:06:40.000000 api_master-1.8/api_master/sdks/fudstop_sdk/__init__.py
--rw-rw-rw-   0        0        0     3095 2023-06-18 18:41:08.000000 api_master-1.8/api_master/sdks/fudstop_sdk/fudstop_sdk.py
--rw-rw-rw-   0        0        0     1847 2023-06-16 23:24:08.000000 api_master-1.8/api_master/sdks/fudstop_sdk/gaps.py
--rw-rw-rw-   0        0        0      613 2023-06-16 23:24:13.000000 api_master-1.8/api_master/sdks/fudstop_sdk/option_vol_totals.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.412552 api_master-1.8/api_master/sdks/helpers/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/helpers/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/helpers/conditions.py
--rw-rw-rw-   0        0        0     5442 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.414553 api_master-1.8/api_master/sdks/models/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/models/__init__.py
--rw-rw-rw-   0        0        0      488 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/models/common.py
--rw-rw-rw-   0        0        0     5097 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/models/maps.py
--rw-rw-rw-   0        0        0    13078 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/models/test_events.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.433004 api_master-1.8/api_master/sdks/polygon_sdk/
--rw-rw-rw-   0        0        0      543 2023-06-16 22:28:47.000000 api_master-1.8/api_master/sdks/polygon_sdk/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/polygon_sdk/aggregates.py
--rw-rw-rw-   0        0        0    29379 2023-06-18 18:40:00.000000 api_master-1.8/api_master/sdks/polygon_sdk/async_options_sdk.py
--rw-rw-rw-   0        0        0    52759 2023-06-18 18:40:39.000000 api_master-1.8/api_master/sdks/polygon_sdk/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     1135 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/polygon_sdk/company_info.py
--rw-rw-rw-   0        0        0      703 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/polygon_sdk/daily_open_close.py
--rw-rw-rw-   0        0        0    15043 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/polygon_sdk/financials.py
--rw-rw-rw-   0        0        0     6644 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/polygon_sdk/forex_crypto.py
--rw-rw-rw-   0        0        0     8957 2023-06-18 18:40:47.000000 api_master-1.8/api_master/sdks/polygon_sdk/get_all_options.py
--rw-rw-rw-   0        0        0     1131 2023-06-11 21:54:24.000000 api_master-1.8/api_master/sdks/polygon_sdk/indices_snapshot.py
--rw-rw-rw-   0        0        0      823 2023-06-18 18:40:55.000000 api_master-1.8/api_master/sdks/polygon_sdk/logo.py
--rw-rw-rw-   0        0        0    27900 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/mapping_dicts.py
--rw-rw-rw-   0        0        0      782 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/models.py
--rw-rw-rw-   0        0        0      819 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/news.py
--rw-rw-rw-   0        0        0      820 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/option_aggs.py
--rw-rw-rw-   0        0        0     1493 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/option_quote.py
--rw-rw-rw-   0        0        0     3079 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/option_snapshot.py
--rw-rw-rw-   0        0        0      873 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/option_trades.py
--rw-rw-rw-   0        0        0      538 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/pivot_points.py
--rw-rw-rw-   0        0        0      690 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/quote.py
--rw-rw-rw-   0        0        0      151 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/sec.py
--rw-rw-rw-   0        0        0     4192 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/snapshot.py
--rw-rw-rw-   0        0        0     1313 2023-06-18 18:41:08.000000 api_master-1.8/api_master/sdks/polygon_sdk/technical_conditions.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.439483 api_master-1.8/api_master/sdks/polygon_sdk/technicals/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/technicals/__init__.py
--rw-rw-rw-   0        0        0      248 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/technicals/ema.py
--rw-rw-rw-   0        0        0      229 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/technicals/macd.py
--rw-rw-rw-   0        0        0      233 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/technicals/rsi.py
--rw-rw-rw-   0        0        0      244 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/polygon_sdk/technicals/sma.py
--rw-rw-rw-   0        0        0     3361 2023-06-18 18:41:08.000000 api_master-1.8/api_master/sdks/polygon_sdk/tickernews.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.439483 api_master-1.8/api_master/sdks/terminals/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/terminals/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.439483 api_master-1.8/api_master/sdks/terminals/crypto/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/terminals/crypto/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/terminals/crypto/menu.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.448487 api_master-1.8/api_master/sdks/webull_sdk/
--rw-rw-rw-   0        0        0      440 2023-06-16 22:31:19.000000 api_master-1.8/api_master/sdks/webull_sdk/__init__.py
--rw-rw-rw-   0        0        0      882 2023-06-11 22:15:21.000000 api_master-1.8/api_master/sdks/webull_sdk/calendar.py
--rw-rw-rw-   0        0        0     9220 2023-06-17 03:02:45.000000 api_master-1.8/api_master/sdks/webull_sdk/capitalflow.py
--rw-rw-rw-   0        0        0     1152 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/webull_sdk/cost_distribution.py
--rw-rw-rw-   0        0        0     2282 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/webull_sdk/derivative_query.py
--rw-rw-rw-   0        0        0     2426 2023-06-11 22:15:21.000000 api_master-1.8/api_master/sdks/webull_sdk/etf_finder.py
--rw-rw-rw-   0        0        0      486 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/webull_sdk/etf_holdings.py
--rw-rw-rw-   0        0        0     1100 2023-06-16 14:24:58.000000 api_master-1.8/api_master/sdks/webull_sdk/events.py
--rw-rw-rw-   0        0        0    14035 2023-06-20 18:27:35.000000 api_master-1.8/api_master/sdks/webull_sdk/financial_statement.py
--rw-rw-rw-   0        0        0     3780 2023-06-11 21:54:25.000000 api_master-1.8/api_master/sdks/webull_sdk/forecast.py
--rw-rw-rw-   0        0        0     1033 2023-06-17 17:59:48.000000 api_master-1.8/api_master/sdks/webull_sdk/institutional_holdings.py
--rw-rw-rw-   0        0        0     1235 2023-06-16 22:35:10.000000 api_master-1.8/api_master/sdks/webull_sdk/manage.py
--rw-rw-rw-   0        0        0      617 2023-06-11 22:15:21.000000 api_master-1.8/api_master/sdks/webull_sdk/news.py
--rw-rw-rw-   0        0        0      307 2023-06-11 22:15:21.000000 api_master-1.8/api_master/sdks/webull_sdk/shortinterest.py
--rw-rw-rw-   0        0        0     5986 2023-06-17 21:36:17.000000 api_master-1.8/api_master/sdks/webull_sdk/top_gainers.py
--rw-rw-rw-   0        0        0    16238 2023-06-17 21:46:04.000000 api_master-1.8/api_master/sdks/webull_sdk/top_options.py
--rw-rw-rw-   0        0        0     5556 2023-06-11 22:15:21.000000 api_master-1.8/api_master/sdks/webull_sdk/webull_data.py
--rw-rw-rw-   0        0        0    44347 2023-06-18 18:30:58.000000 api_master-1.8/api_master/sdks/webull_sdk/webull_sdk.py
--rw-rw-rw-   0        0        0      674 2023-06-17 21:48:36.000000 api_master-1.8/api_master/test.py
--rw-rw-rw-   0        0        0    11892 2023-06-20 12:47:22.000000 api_master-1.8/api_master/trial.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.284897 api_master-1.8/api_master.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-06-20 19:28:05.000000 api_master-1.8/api_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8942 2023-06-20 19:28:05.000000 api_master-1.8/api_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 19:28:05.000000 api_master-1.8/api_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-20 19:28:05.000000 api_master-1.8/api_master.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.448487 api_master-1.8/files/
--rw-rw-rw-   0        0        0        0 2023-06-20 17:56:55.000000 api_master-1.8/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.448487 api_master-1.8/read-me/
--rw-rw-rw-   0        0        0        0 2023-06-20 17:57:02.000000 api_master-1.8/read-me/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-20 19:28:05.456256 api_master-1.8/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-06-20 19:27:51.000000 api_master-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:28:05.448487 api_master-1.8/templates/
--rw-rw-rw-   0        0        0        0 2023-06-16 22:25:34.000000 api_master-1.8/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.737717 api_master-1.9/
+-rw-rw-rw-   0        0        0     2484 2023-06-20 19:39:12.737717 api_master-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-12 00:29:12.000000 api_master-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.581114 api_master-1.9/api_master/
+-rw-rw-rw-   0        0        0        0 2023-06-20 17:56:44.000000 api_master-1.9/api_master/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.605617 api_master-1.9/api_master/_discord/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/__init__.py
+-rw-rw-rw-   0        0        0     7983 2023-06-18 18:41:08.000000 api_master-1.9/api_master/_discord/discord_stock_example.py
+-rw-rw-rw-   0        0        0    44936 2023-06-18 18:41:08.000000 api_master-1.9/api_master/_discord/discord_stock_market.py
+-rw-rw-rw-   0        0        0    16306 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/embeddings.py
+-rw-rw-rw-   0        0        0      581 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/emojis.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.607617 api_master-1.9/api_master/_discord/hooks/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1594 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/hooks/channel_webhooks.py
+-rw-rw-rw-   0        0        0    10521 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/hooks/hook_dicts.py
+-rw-rw-rw-   0        0        0     5462 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/hooks/send_webhook.py
+-rw-rw-rw-   0        0        0    33594 2023-06-18 18:41:08.000000 api_master-1.9/api_master/_discord/live_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.608617 api_master-1.9/api_master/_discord/selectmenus/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/selectmenus/__init__.py
+-rw-rw-rw-   0        0        0    33209 2023-06-18 18:41:08.000000 api_master-1.9/api_master/_discord/selectmenus/mainselect.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.610616 api_master-1.9/api_master/_discord/views/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/views/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-18 18:41:08.000000 api_master-1.9/api_master/_discord/views/mainview.py
+-rw-rw-rw-   0        0        0     3792 2023-06-11 21:54:23.000000 api_master-1.9/api_master/_discord/views/menus.py
+-rw-rw-rw-   0        0        0     7502 2023-06-18 18:41:08.000000 api_master-1.9/api_master/_discord/webhook_creation.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.614125 api_master-1.9/api_master/bot/
+-rw-rw-rw-   0        0        0       72 2023-06-16 22:29:19.000000 api_master-1.9/api_master/bot/__init__.py
+-rw-rw-rw-   0        0        0    13401 2023-06-18 18:55:44.000000 api_master-1.9/api_master/bot/autocomp.py
+-rw-rw-rw-   0        0        0     6919 2023-06-11 22:19:59.000000 api_master-1.9/api_master/bot/discord_emojis.py
+-rw-rw-rw-   0        0        0     3838 2023-06-20 14:10:53.000000 api_master-1.9/api_master/bot/main.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.618125 api_master-1.9/api_master/bot/utils/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.9/api_master/bot/utils/__init__.py
+-rw-rw-rw-   0        0        0     1368 2023-06-16 02:40:26.000000 api_master-1.9/api_master/bot/utils/crypto_coins.py
+-rw-rw-rw-   0        0        0      998 2023-06-16 02:35:33.000000 api_master-1.9/api_master/bot/utils/date_times.py
+-rw-rw-rw-   0        0        0   224003 2023-06-16 03:10:59.000000 api_master-1.9/api_master/bot/utils/lists_and_dicts.py
+-rw-rw-rw-   0        0        0   199781 2023-06-16 02:46:46.000000 api_master-1.9/api_master/bot/utils/webull_tickers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.619125 api_master-1.9/api_master/bot/views/
+-rw-rw-rw-   0        0        0       49 2023-06-16 22:29:34.000000 api_master-1.9/api_master/bot/views/__init__.py
+-rw-rw-rw-   0        0        0  1503926 2023-06-18 18:41:09.000000 api_master-1.9/api_master/bot/views/learnviews.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.633319 api_master-1.9/api_master/bot/views/uiviews/
+-rw-rw-rw-   0        0        0   320159 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/MarketAnalysis.py
+-rw-rw-rw-   0        0        0     5109 2023-06-16 03:43:55.000000 api_master-1.9/api_master/bot/views/uiviews/TickerAnalysis.py
+-rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.9/api_master/bot/views/uiviews/__init__ copy.py
+-rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.9/api_master/bot/views/uiviews/__init__.py
+-rw-rw-rw-   0        0        0     5169 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/capitalflow.py
+-rw-rw-rw-   0        0        0   110984 2022-11-14 02:53:40.000000 api_master-1.9/api_master/bot/views/uiviews/cmslist.py
+-rw-rw-rw-   0        0        0   107414 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/cmslist2.py
+-rw-rw-rw-   0        0        0    18026 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/directiondrop.py
+-rw-rw-rw-   0        0        0     9311 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/financialselects.py
+-rw-rw-rw-   0        0        0    12480 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/ftds.py
+-rw-rw-rw-   0        0        0     4675 2023-06-16 03:04:58.000000 api_master-1.9/api_master/bot/views/uiviews/leveragedropdown.py
+-rw-rw-rw-   0        0        0     7693 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/lowfloat.py
+-rw-rw-rw-   0        0        0     4487 2023-06-16 03:51:49.000000 api_master-1.9/api_master/bot/views/uiviews/masterview.py
+-rw-rw-rw-   0        0        0     5619 2022-11-05 23:34:22.000000 api_master-1.9/api_master/bot/views/uiviews/mostactive.py
+-rw-rw-rw-   0        0        0     6579 2022-11-05 23:04:27.000000 api_master-1.9/api_master/bot/views/uiviews/pressrelease.py
+-rw-rw-rw-   0        0        0     3355 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/quote.py
+-rw-rw-rw-   0        0        0    13749 2023-06-18 18:41:08.000000 api_master-1.9/api_master/bot/views/uiviews/shortinterest.py
+-rw-rw-rw-   0        0        0     3714 2023-06-20 00:08:12.000000 api_master-1.9/api_master/cfg.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.688055 api_master-1.9/api_master/examples/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.9/api_master/examples/__init__.py
+-rw-rw-rw-   0        0        0      703 2023-06-14 15:26:12.000000 api_master-1.9/api_master/examples/helpers.py
+-rw-rw-rw-   0        0        0      333 2023-06-20 17:45:26.000000 api_master-1.9/api_master/examples/nasdaq_bigmac.py
+-rw-rw-rw-   0        0        0      294 2023-06-19 16:25:15.000000 api_master-1.9/api_master/examples/nasdaq_economic_indicators.py
+-rw-rw-rw-   0        0        0      204 2023-06-19 16:36:33.000000 api_master-1.9/api_master/examples/nasdaq_gdp.py
+-rw-rw-rw-   0        0        0      293 2023-06-19 16:19:39.000000 api_master-1.9/api_master/examples/nasdaq_income_expenditures.py
+-rw-rw-rw-   0        0        0      254 2023-06-19 16:05:10.000000 api_master-1.9/api_master/examples/nasdaq_inflation.py
+-rw-rw-rw-   0        0        0      278 2023-06-19 16:31:10.000000 api_master-1.9/api_master/examples/nasdaq_interest_rates.py
+-rw-rw-rw-   0        0        0      249 2023-06-19 16:10:55.000000 api_master-1.9/api_master/examples/nasdaq_repos.py
+-rw-rw-rw-   0        0        0      252 2023-06-19 16:14:00.000000 api_master-1.9/api_master/examples/nasdaq_sp500.py
+-rw-rw-rw-   0        0        0      231 2023-06-19 16:30:11.000000 api_master-1.9/api_master/examples/nasdaq_unemployment.py
+-rw-rw-rw-   0        0        0      661 2023-06-19 21:19:24.000000 api_master-1.9/api_master/examples/occ_stock_loans.py
+-rw-rw-rw-   0        0        0      456 2023-06-19 21:44:19.000000 api_master-1.9/api_master/examples/occ_volume_totals.py
+-rw-rw-rw-   0        0        0     5940 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_attributes.py
+-rw-rw-rw-   0        0        0      533 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_bollinger_bands.py
+-rw-rw-rw-   0        0        0     4375 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_candle_patterns.py
+-rw-rw-rw-   0        0        0      706 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_create_option_symbol.py
+-rw-rw-rw-   0        0        0     2479 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_crypto_market.py
+-rw-rw-rw-   0        0        0    44945 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_discord_market.py
+-rw-rw-rw-   0        0        0     1376 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_ema.py
+-rw-rw-rw-   0        0        0      910 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_fetch_entire_chain.py
+-rw-rw-rw-   0        0        0      693 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_find_gaps.py
+-rw-rw-rw-   0        0        0      922 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_forex_market.py
+-rw-rw-rw-   0        0        0      823 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_all_options_data.py
+-rw-rw-rw-   0        0        0    36288 2023-06-17 02:25:07.000000 api_master-1.9/api_master/examples/polygon_get_data.py
+-rw-rw-rw-   0        0        0     2399 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_ema.py
+-rw-rw-rw-   0        0        0      619 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      585 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      446 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      762 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_latest_options_data.py
+-rw-rw-rw-   0        0        0      598 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0      644 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_logo.py
+-rw-rw-rw-   0        0        0     3195 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_macd.py
+-rw-rw-rw-   0        0        0      665 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_pivot_points.py
+-rw-rw-rw-   0        0        0     1192 2023-06-19 15:17:22.000000 api_master-1.9/api_master/examples/polygon_get_price_data.py
+-rw-rw-rw-   0        0        0     2051 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_rsi.py
+-rw-rw-rw-   0        0        0     1935 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_get_sma.py
+-rw-rw-rw-   0        0        0      776 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_indices_market.py
+-rw-rw-rw-   0        0        0     1796 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_latest_news.py
+-rw-rw-rw-   0        0        0      930 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_macd_sma_rsi.py
+-rw-rw-rw-   0        0        0     1625 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_option_quote.py
+-rw-rw-rw-   0        0        0     2408 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_option_trades.py
+-rw-rw-rw-   0        0        0      989 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_options_market.py
+-rw-rw-rw-   0        0        0     1509 2023-06-19 15:17:30.000000 api_master-1.9/api_master/examples/polygon_plot_aggs.py
+-rw-rw-rw-   0        0        0      796 2023-06-19 16:18:45.000000 api_master-1.9/api_master/examples/polygon_plot_macd.py
+-rw-rw-rw-   0        0        0     1797 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_plot_option_aggs.py
+-rw-rw-rw-   0        0        0      487 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_rate_of_change.py
+-rw-rw-rw-   0        0        0      628 2023-06-20 19:26:38.000000 api_master-1.9/api_master/examples/polygon_rsi.py
+-rw-rw-rw-   0        0        0     8185 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_scan_candles.py
+-rw-rw-rw-   0        0        0     5590 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_scanner_example.py
+-rw-rw-rw-   0        0        0     2116 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_stock_aggregates.py
+-rw-rw-rw-   0        0        0     1189 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/polygon_support_resistance.py
+-rw-rw-rw-   0        0        0     1052 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/sec_sec_filings.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.691052 api_master-1.9/api_master/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.9/api_master/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-06-11 21:54:23.000000 api_master-1.9/api_master/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     5115 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/simulated_markets/mock_discord.py
+-rw-rw-rw-   0        0        0     1951 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1551 2023-06-18 18:41:08.000000 api_master-1.9/api_master/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 02:12:58.000000 api_master-1.9/api_master/examples/stocksera-web_mentions.py
+-rw-rw-rw-   0        0        0      804 2023-06-19 01:10:14.000000 api_master-1.9/api_master/examples/stocksera_IPO_calendar.py
+-rw-rw-rw-   0        0        0     1209 2023-06-19 01:01:37.000000 api_master-1.9/api_master/examples/stocksera_earnings_calendar.py
+-rw-rw-rw-   0        0        0      651 2023-06-19 02:55:19.000000 api_master-1.9/api_master/examples/stocksera_fails_to_deliver.py
+-rw-rw-rw-   0        0        0      286 2023-06-19 00:56:26.000000 api_master-1.9/api_master/examples/stocksera_inflation.py
+-rw-rw-rw-   0        0        0      458 2023-06-19 01:05:25.000000 api_master-1.9/api_master/examples/stocksera_jim_cramer.py
+-rw-rw-rw-   0        0        0      537 2023-06-19 00:40:17.000000 api_master-1.9/api_master/examples/stocksera_jobless_claims.py
+-rw-rw-rw-   0        0        0      579 2023-06-19 00:55:25.000000 api_master-1.9/api_master/examples/stocksera_latest_insider_summary.py
+-rw-rw-rw-   0        0        0     1147 2023-06-19 00:44:35.000000 api_master-1.9/api_master/examples/stocksera_low_floats.py
+-rw-rw-rw-   0        0        0      400 2023-06-19 00:37:38.000000 api_master-1.9/api_master/examples/stocksera_market_news.py
+-rw-rw-rw-   0        0        0      501 2023-06-19 00:42:29.000000 api_master-1.9/api_master/examples/stocksera_news_sentiment.py
+-rw-rw-rw-   0        0        0      544 2023-06-19 01:12:25.000000 api_master-1.9/api_master/examples/stocksera_retail_sales.py
+-rw-rw-rw-   0        0        0      522 2023-06-19 00:41:01.000000 api_master-1.9/api_master/examples/stocksera_reverse_repo.py
+-rw-rw-rw-   0        0        0      561 2023-06-19 00:53:52.000000 api_master-1.9/api_master/examples/stocksera_sec_filings.py
+-rw-rw-rw-   0        0        0      772 2023-06-19 00:48:53.000000 api_master-1.9/api_master/examples/stocksera_short_interest.py
+-rw-rw-rw-   0        0        0      593 2023-06-19 00:46:32.000000 api_master-1.9/api_master/examples/stocksera_short_volume.py
+-rw-rw-rw-   0        0        0      496 2023-06-19 00:50:13.000000 api_master-1.9/api_master/examples/stocksera_stocktwits.py
+-rw-rw-rw-   0        0        0      603 2023-06-19 00:51:40.000000 api_master-1.9/api_master/examples/stocksera_subreddits.py
+-rw-rw-rw-   0        0        0      643 2023-06-19 00:40:51.000000 api_master-1.9/api_master/examples/stocksera_treasury_balance.py
+-rw-rw-rw-   0        0        0      534 2023-06-19 02:28:28.000000 api_master-1.9/api_master/examples/stocksera_wsb_options.py
+-rw-rw-rw-   0        0        0      988 2023-06-20 19:38:06.000000 api_master-1.9/api_master/examples/webull_analyst_ratings.py
+-rw-rw-rw-   0        0        0     5776 2023-06-20 19:36:41.000000 api_master-1.9/api_master/examples/webull_balance_sheet.py
+-rw-rw-rw-   0        0        0     3479 2023-06-20 19:35:55.000000 api_master-1.9/api_master/examples/webull_cash_flow.py
+-rw-rw-rw-   0        0        0     1549 2023-06-20 19:20:53.000000 api_master-1.9/api_master/examples/webull_cost_distribution.py
+-rw-rw-rw-   0        0        0     4799 2023-06-20 19:37:22.000000 api_master-1.9/api_master/examples/webull_earnings_calendar.py
+-rw-rw-rw-   0        0        0     2286 2023-06-20 19:21:53.000000 api_master-1.9/api_master/examples/webull_examples.py
+-rw-rw-rw-   0        0        0     4523 2023-06-20 19:35:04.000000 api_master-1.9/api_master/examples/webull_financial_statement.py
+-rw-rw-rw-   0        0        0      377 2023-06-20 18:14:28.000000 api_master-1.9/api_master/examples/webull_get_webull_data.py
+-rw-rw-rw-   0        0        0     2128 2023-06-20 19:22:38.000000 api_master-1.9/api_master/examples/webull_institutions.py
+-rw-rw-rw-   0        0        0     1456 2023-06-20 19:37:50.000000 api_master-1.9/api_master/examples/webull_short_interest.py
+-rw-rw-rw-   0        0        0     1537 2023-06-20 19:25:22.000000 api_master-1.9/api_master/examples/webull_stock_data.py
+-rw-rw-rw-   0        0        0      809 2023-06-20 19:25:47.000000 api_master-1.9/api_master/examples/webull_volume_analysis.py
+-rw-rw-rw-   0        0        0    14776 2023-06-16 14:39:01.000000 api_master-1.9/api_master/examples/webull_webull_data.py
+-rw-rw-rw-   0        0        0     1383 2023-06-17 17:45:02.000000 api_master-1.9/api_master/myconfig.py
+-rw-rw-rw-   0        0        0     4167 2023-06-17 02:16:41.000000 api_master-1.9/api_master/oldapp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.691052 api_master-1.9/api_master/sdks/
+-rw-rw-rw-   0        0        0      275 2023-06-16 23:26:41.000000 api_master-1.9/api_master/sdks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.693052 api_master-1.9/api_master/sdks/discord_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/discord_sdk/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/discord_sdk/channel_ids.py
+-rw-rw-rw-   0        0        0     4497 2023-06-18 18:41:08.000000 api_master-1.9/api_master/sdks/discord_sdk/discord_sdk.py
+-rw-rw-rw-   0        0        0     2157 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/discord_sdk/searching.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.697562 api_master-1.9/api_master/sdks/fudstop_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-12 00:06:40.000000 api_master-1.9/api_master/sdks/fudstop_sdk/__init__.py
+-rw-rw-rw-   0        0        0     3095 2023-06-18 18:41:08.000000 api_master-1.9/api_master/sdks/fudstop_sdk/fudstop_sdk.py
+-rw-rw-rw-   0        0        0     1847 2023-06-16 23:24:08.000000 api_master-1.9/api_master/sdks/fudstop_sdk/gaps.py
+-rw-rw-rw-   0        0        0      613 2023-06-16 23:24:13.000000 api_master-1.9/api_master/sdks/fudstop_sdk/option_vol_totals.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.701560 api_master-1.9/api_master/sdks/helpers/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/helpers/conditions.py
+-rw-rw-rw-   0        0        0     5442 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.704561 api_master-1.9/api_master/sdks/models/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/models/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/models/common.py
+-rw-rw-rw-   0        0        0     5097 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/models/maps.py
+-rw-rw-rw-   0        0        0    13078 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/models/test_events.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.720544 api_master-1.9/api_master/sdks/polygon_sdk/
+-rw-rw-rw-   0        0        0      543 2023-06-16 22:28:47.000000 api_master-1.9/api_master/sdks/polygon_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/polygon_sdk/aggregates.py
+-rw-rw-rw-   0        0        0    29379 2023-06-18 18:40:00.000000 api_master-1.9/api_master/sdks/polygon_sdk/async_options_sdk.py
+-rw-rw-rw-   0        0        0    52759 2023-06-18 18:40:39.000000 api_master-1.9/api_master/sdks/polygon_sdk/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0     1135 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/polygon_sdk/company_info.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/polygon_sdk/daily_open_close.py
+-rw-rw-rw-   0        0        0    15043 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/polygon_sdk/financials.py
+-rw-rw-rw-   0        0        0     6644 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/polygon_sdk/forex_crypto.py
+-rw-rw-rw-   0        0        0     8957 2023-06-18 18:40:47.000000 api_master-1.9/api_master/sdks/polygon_sdk/get_all_options.py
+-rw-rw-rw-   0        0        0     1131 2023-06-11 21:54:24.000000 api_master-1.9/api_master/sdks/polygon_sdk/indices_snapshot.py
+-rw-rw-rw-   0        0        0      823 2023-06-18 18:40:55.000000 api_master-1.9/api_master/sdks/polygon_sdk/logo.py
+-rw-rw-rw-   0        0        0    27900 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/mapping_dicts.py
+-rw-rw-rw-   0        0        0      782 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/models.py
+-rw-rw-rw-   0        0        0      819 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/news.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/option_aggs.py
+-rw-rw-rw-   0        0        0     1493 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/option_quote.py
+-rw-rw-rw-   0        0        0     3079 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/option_snapshot.py
+-rw-rw-rw-   0        0        0      873 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/option_trades.py
+-rw-rw-rw-   0        0        0      538 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/pivot_points.py
+-rw-rw-rw-   0        0        0      690 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/quote.py
+-rw-rw-rw-   0        0        0      151 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/sec.py
+-rw-rw-rw-   0        0        0     4192 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/snapshot.py
+-rw-rw-rw-   0        0        0     1313 2023-06-18 18:41:08.000000 api_master-1.9/api_master/sdks/polygon_sdk/technical_conditions.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.722543 api_master-1.9/api_master/sdks/polygon_sdk/technicals/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/technicals/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/technicals/ema.py
+-rw-rw-rw-   0        0        0      229 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/technicals/macd.py
+-rw-rw-rw-   0        0        0      233 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/technicals/rsi.py
+-rw-rw-rw-   0        0        0      244 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/polygon_sdk/technicals/sma.py
+-rw-rw-rw-   0        0        0     3361 2023-06-18 18:41:08.000000 api_master-1.9/api_master/sdks/polygon_sdk/tickernews.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.723544 api_master-1.9/api_master/sdks/terminals/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/terminals/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.724545 api_master-1.9/api_master/sdks/terminals/crypto/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/terminals/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1672 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/terminals/crypto/menu.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.731056 api_master-1.9/api_master/sdks/webull_sdk/
+-rw-rw-rw-   0        0        0      440 2023-06-16 22:31:19.000000 api_master-1.9/api_master/sdks/webull_sdk/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-06-11 22:15:21.000000 api_master-1.9/api_master/sdks/webull_sdk/calendar.py
+-rw-rw-rw-   0        0        0     9220 2023-06-17 03:02:45.000000 api_master-1.9/api_master/sdks/webull_sdk/capitalflow.py
+-rw-rw-rw-   0        0        0     1152 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/webull_sdk/cost_distribution.py
+-rw-rw-rw-   0        0        0     2282 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/webull_sdk/derivative_query.py
+-rw-rw-rw-   0        0        0     2426 2023-06-11 22:15:21.000000 api_master-1.9/api_master/sdks/webull_sdk/etf_finder.py
+-rw-rw-rw-   0        0        0      486 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/webull_sdk/etf_holdings.py
+-rw-rw-rw-   0        0        0     1100 2023-06-16 14:24:58.000000 api_master-1.9/api_master/sdks/webull_sdk/events.py
+-rw-rw-rw-   0        0        0    14035 2023-06-20 18:27:35.000000 api_master-1.9/api_master/sdks/webull_sdk/financial_statement.py
+-rw-rw-rw-   0        0        0     3780 2023-06-11 21:54:25.000000 api_master-1.9/api_master/sdks/webull_sdk/forecast.py
+-rw-rw-rw-   0        0        0     1033 2023-06-17 17:59:48.000000 api_master-1.9/api_master/sdks/webull_sdk/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1235 2023-06-16 22:35:10.000000 api_master-1.9/api_master/sdks/webull_sdk/manage.py
+-rw-rw-rw-   0        0        0      617 2023-06-11 22:15:21.000000 api_master-1.9/api_master/sdks/webull_sdk/news.py
+-rw-rw-rw-   0        0        0      307 2023-06-11 22:15:21.000000 api_master-1.9/api_master/sdks/webull_sdk/shortinterest.py
+-rw-rw-rw-   0        0        0     5986 2023-06-17 21:36:17.000000 api_master-1.9/api_master/sdks/webull_sdk/top_gainers.py
+-rw-rw-rw-   0        0        0    16238 2023-06-17 21:46:04.000000 api_master-1.9/api_master/sdks/webull_sdk/top_options.py
+-rw-rw-rw-   0        0        0     5556 2023-06-11 22:15:21.000000 api_master-1.9/api_master/sdks/webull_sdk/webull_data.py
+-rw-rw-rw-   0        0        0    44347 2023-06-18 18:30:58.000000 api_master-1.9/api_master/sdks/webull_sdk/webull_sdk.py
+-rw-rw-rw-   0        0        0      674 2023-06-17 21:48:36.000000 api_master-1.9/api_master/test.py
+-rw-rw-rw-   0        0        0    11892 2023-06-20 12:47:22.000000 api_master-1.9/api_master/trial.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.600108 api_master-1.9/api_master.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-06-20 19:39:12.000000 api_master-1.9/api_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8942 2023-06-20 19:39:12.000000 api_master-1.9/api_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:39:12.000000 api_master-1.9/api_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-20 19:39:12.000000 api_master-1.9/api_master.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.737717 api_master-1.9/files/
+-rw-rw-rw-   0        0        0        0 2023-06-20 17:56:55.000000 api_master-1.9/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.737717 api_master-1.9/read-me/
+-rw-rw-rw-   0        0        0        0 2023-06-20 17:57:02.000000 api_master-1.9/read-me/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 19:39:12.737717 api_master-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-06-20 19:39:02.000000 api_master-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:39:12.737717 api_master-1.9/templates/
+-rw-rw-rw-   0        0        0        0 2023-06-16 22:25:34.000000 api_master-1.9/templates/__init__.py
```

### Comparing `api_master-1.8/PKG-INFO` & `api_master-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_master
-Version: 1.8
+Version: 1.9
 Summary: Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.
 Home-page: https://github.com/your-username/your-package-repo
 Author: Chuck Dustin
 Author-email: chuckdustin12@gmail.com
 Keywords: trading,stocks,options,crypto,forex,indices,discord
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `api_master-1.8/README.md` & `api_master-1.9/README.md`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/discord_stock_example.py` & `api_master-1.9/api_master/_discord/discord_stock_example.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/discord_stock_market.py` & `api_master-1.9/api_master/_discord/discord_stock_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/embeddings.py` & `api_master-1.9/api_master/_discord/embeddings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/emojis.py` & `api_master-1.9/api_master/_discord/emojis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/hooks/channel_webhooks.py` & `api_master-1.9/api_master/_discord/hooks/channel_webhooks.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/hooks/hook_dicts.py` & `api_master-1.9/api_master/_discord/hooks/hook_dicts.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/hooks/send_webhook.py` & `api_master-1.9/api_master/_discord/hooks/send_webhook.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/live_discord.py` & `api_master-1.9/api_master/_discord/live_discord.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/selectmenus/mainselect.py` & `api_master-1.9/api_master/_discord/selectmenus/mainselect.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/views/mainview.py` & `api_master-1.9/api_master/_discord/views/mainview.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/views/menus.py` & `api_master-1.9/api_master/_discord/views/menus.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/_discord/webhook_creation.py` & `api_master-1.9/api_master/_discord/webhook_creation.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/autocomp.py` & `api_master-1.9/api_master/bot/autocomp.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/discord_emojis.py` & `api_master-1.9/api_master/bot/discord_emojis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/main.py` & `api_master-1.9/api_master/bot/main.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/utils/crypto_coins.py` & `api_master-1.9/api_master/bot/utils/crypto_coins.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/utils/date_times.py` & `api_master-1.9/api_master/bot/utils/date_times.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/utils/lists_and_dicts.py` & `api_master-1.9/api_master/bot/utils/lists_and_dicts.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/utils/webull_tickers.py` & `api_master-1.9/api_master/bot/utils/webull_tickers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/learnviews.py` & `api_master-1.9/api_master/bot/views/learnviews.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/MarketAnalysis.py` & `api_master-1.9/api_master/bot/views/uiviews/MarketAnalysis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/TickerAnalysis.py` & `api_master-1.9/api_master/bot/views/uiviews/TickerAnalysis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/capitalflow.py` & `api_master-1.9/api_master/bot/views/uiviews/capitalflow.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/cmslist.py` & `api_master-1.9/api_master/bot/views/uiviews/cmslist.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/cmslist2.py` & `api_master-1.9/api_master/bot/views/uiviews/cmslist2.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/directiondrop.py` & `api_master-1.9/api_master/bot/views/uiviews/directiondrop.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/financialselects.py` & `api_master-1.9/api_master/bot/views/uiviews/financialselects.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/ftds.py` & `api_master-1.9/api_master/bot/views/uiviews/ftds.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/leveragedropdown.py` & `api_master-1.9/api_master/bot/views/uiviews/leveragedropdown.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/lowfloat.py` & `api_master-1.9/api_master/bot/views/uiviews/lowfloat.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/masterview.py` & `api_master-1.9/api_master/bot/views/uiviews/masterview.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/mostactive.py` & `api_master-1.9/api_master/bot/views/uiviews/mostactive.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/pressrelease.py` & `api_master-1.9/api_master/bot/views/uiviews/pressrelease.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/quote.py` & `api_master-1.9/api_master/bot/views/uiviews/quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/bot/views/uiviews/shortinterest.py` & `api_master-1.9/api_master/bot/views/uiviews/shortinterest.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/cfg.py` & `api_master-1.9/api_master/cfg.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/helpers.py` & `api_master-1.9/api_master/examples/helpers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/occ_stock_loans.py` & `api_master-1.9/api_master/examples/occ_stock_loans.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_attributes.py` & `api_master-1.9/api_master/examples/polygon_attributes.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_bollinger_bands.py` & `api_master-1.9/api_master/examples/polygon_bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_candle_patterns.py` & `api_master-1.9/api_master/examples/polygon_candle_patterns.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_create_option_symbol.py` & `api_master-1.9/api_master/examples/polygon_create_option_symbol.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_crypto_market.py` & `api_master-1.9/api_master/examples/polygon_crypto_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_discord_market.py` & `api_master-1.9/api_master/examples/polygon_discord_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_ema.py` & `api_master-1.9/api_master/examples/polygon_ema.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_fetch_entire_chain.py` & `api_master-1.9/api_master/examples/polygon_fetch_entire_chain.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_find_gaps.py` & `api_master-1.9/api_master/examples/polygon_find_gaps.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_forex_market.py` & `api_master-1.9/api_master/examples/polygon_forex_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_all_options_data.py` & `api_master-1.9/api_master/examples/polygon_get_all_options_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_data.py` & `api_master-1.9/api_master/examples/polygon_get_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_ema.py` & `api_master-1.9/api_master/examples/polygon_get_ema.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_latest_crypto_data.py` & `api_master-1.9/api_master/examples/polygon_get_latest_crypto_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_latest_forex_data.py` & `api_master-1.9/api_master/examples/polygon_get_latest_forex_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_latest_options_data.py` & `api_master-1.9/api_master/examples/polygon_get_latest_options_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_latest_ticker_data.py` & `api_master-1.9/api_master/examples/polygon_get_latest_ticker_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_logo.py` & `api_master-1.9/api_master/examples/polygon_get_logo.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_macd.py` & `api_master-1.9/api_master/examples/polygon_get_macd.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_pivot_points.py` & `api_master-1.9/api_master/examples/polygon_get_pivot_points.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_price_data.py` & `api_master-1.9/api_master/examples/polygon_get_price_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_rsi.py` & `api_master-1.9/api_master/examples/polygon_get_rsi.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_get_sma.py` & `api_master-1.9/api_master/examples/polygon_get_sma.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_indices_market.py` & `api_master-1.9/api_master/examples/polygon_indices_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_latest_news.py` & `api_master-1.9/api_master/examples/polygon_latest_news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_macd_sma_rsi.py` & `api_master-1.9/api_master/examples/polygon_macd_sma_rsi.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_option_quote.py` & `api_master-1.9/api_master/examples/polygon_option_quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_option_trades.py` & `api_master-1.9/api_master/examples/polygon_option_trades.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_options_market.py` & `api_master-1.9/api_master/examples/polygon_options_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_plot_aggs.py` & `api_master-1.9/api_master/examples/polygon_plot_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_plot_macd.py` & `api_master-1.9/api_master/examples/polygon_plot_macd.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_plot_option_aggs.py` & `api_master-1.9/api_master/examples/polygon_plot_option_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_rsi.py` & `api_master-1.9/api_master/examples/polygon_rsi.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_scan_candles.py` & `api_master-1.9/api_master/examples/polygon_scan_candles.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_scanner_example.py` & `api_master-1.9/api_master/examples/polygon_scanner_example.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_stock_aggregates.py` & `api_master-1.9/api_master/examples/polygon_stock_aggregates.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/polygon_support_resistance.py` & `api_master-1.9/api_master/examples/polygon_support_resistance.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/sec_sec_filings.py` & `api_master-1.9/api_master/examples/sec_sec_filings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/simulated_markets/helpers.py` & `api_master-1.9/api_master/examples/simulated_markets/helpers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/simulated_markets/mock_discord.py` & `api_master-1.9/api_master/examples/simulated_markets/mock_discord.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/simulated_markets/mock_market.py` & `api_master-1.9/api_master/examples/simulated_markets/mock_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/simulated_markets/mock_options_market.py` & `api_master-1.9/api_master/examples/simulated_markets/mock_options_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_IPO_calendar.py` & `api_master-1.9/api_master/examples/stocksera_IPO_calendar.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_earnings_calendar.py` & `api_master-1.9/api_master/examples/stocksera_earnings_calendar.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_fails_to_deliver.py` & `api_master-1.9/api_master/examples/stocksera_fails_to_deliver.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_jobless_claims.py` & `api_master-1.9/api_master/examples/stocksera_jobless_claims.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_latest_insider_summary.py` & `api_master-1.9/api_master/examples/stocksera_latest_insider_summary.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_low_floats.py` & `api_master-1.9/api_master/examples/stocksera_low_floats.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_retail_sales.py` & `api_master-1.9/api_master/examples/stocksera_retail_sales.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_reverse_repo.py` & `api_master-1.9/api_master/examples/stocksera_reverse_repo.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_sec_filings.py` & `api_master-1.9/api_master/examples/stocksera_sec_filings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_short_interest.py` & `api_master-1.9/api_master/examples/stocksera_short_interest.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_short_volume.py` & `api_master-1.9/api_master/examples/stocksera_short_volume.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_subreddits.py` & `api_master-1.9/api_master/examples/stocksera_subreddits.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_treasury_balance.py` & `api_master-1.9/api_master/examples/stocksera_treasury_balance.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/stocksera_wsb_options.py` & `api_master-1.9/api_master/examples/stocksera_wsb_options.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/webull_analyst_ratings.py` & `api_master-1.9/api_master/examples/webull_analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/webull_balance_sheet.py` & `api_master-1.9/api_master/examples/webull_balance_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,15 +103,21 @@
 
     # Iterate over the balance_sheet objects and extract attribute values
     for sheet in balance_sheet:
         data.append(sheet.to_dict())
 
     # Convert the list of dictionaries to a DataFrame
     df = pd.DataFrame(data)
+    # Define the directory path
+    directory = 'files/financials/balance_sheet/'
+
+    # Create the directory if it doesn't exist
+    if not os.path.exists(directory):
+        os.makedirs(directory)
 
     # Define the file path
-    filename = f'files/financials/balance_sheet/{ticker}_balance_sheet.csv'
+    filename = f'{directory}{ticker}_cash_flow.csv'
 
     # Save the DataFrame to a CSV file
     df.to_csv(filename, index=False)
 
 asyncio.run(balance_sheet(ticker="AAPL"))
```

### Comparing `api_master-1.8/api_master/examples/webull_cash_flow.py` & `api_master-1.9/api_master/examples/webull_cash_flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,17 +64,26 @@
     # Iterate over the balance_sheet objects and extract attribute values
     for sheet in cash_flow:
         data.append(sheet.to_dict())
 
     # Convert the list of dictionaries to a DataFrame
     df = pd.DataFrame(data)
 
+    # Define the directory path
+    directory = 'files/financials/cash_flow/'
+
+    # Create the directory if it doesn't exist
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
     # Define the file path
-    filename = f'files/financials/cash_flow/{ticker}_cash_flow.csv'
+    filename = f'{directory}{ticker}_cash_flow.csv'
 
     # Save the DataFrame to a CSV file
     df.to_csv(filename, index=False)
 
 
 
 
+
+
 asyncio.run(cash_flow(ticker="AMD"))
```

### Comparing `api_master-1.8/api_master/examples/webull_cost_distribution.py` & `api_master-1.9/api_master/examples/webull_cost_distribution.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/webull_earnings_calendar.py` & `api_master-1.9/api_master/examples/webull_earnings_calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,12 +127,21 @@
         'low_price': low_price,
         'volume': volume,
         'vibrate_ratio': vibrate_ratio,
         'symbol': symbol,
         'pe_ttm': pe_ttm
     }
 
+    # Define the directory path
+    directory = 'files/earnings/'
+
+    # Create the directory if it doesn't exist
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
+    # Define the file path
+    filename = f'{directory}earnings_calendar.csv'
     # Creating a DataFrame
     df = pd.DataFrame(data)
-    df.to_csv('files/earnings/earnings_calendar.csv')
+    df.to_csv(filename)
 
 asyncio.run(earnings_calendar(date=today_str))
```

### Comparing `api_master-1.8/api_master/examples/webull_examples.py` & `api_master-1.9/api_master/examples/webull_examples.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/webull_financial_statement.py` & `api_master-1.9/api_master/examples/webull_financial_statement.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,15 +87,22 @@
     # Iterate over the balance_sheet objects and extract attribute values
     for sheet in fin_statement:
         data.append(sheet.to_dict())
 
     # Convert the list of dictionaries to a DataFrame
     df = pd.DataFrame(data)
 
+    # Define the directory path
+    directory = 'files/financials/financial_statement/'
+
+    # Create the directory if it doesn't exist
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
     # Define the file path
-    filename = f'files/financials/financial_statement/{ticker}financial_statement.csv'
+    filename = f'{directory}{ticker}_financial_statement.csv'
 
     # Save the DataFrame to a CSV file
     df.to_csv(filename, index=False)
 
 
 asyncio.run(financial_statement(ticker="META"))
```

### Comparing `api_master-1.8/api_master/examples/webull_institutions.py` & `api_master-1.9/api_master/examples/webull_institutions.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/webull_short_interest.py` & `api_master-1.9/api_master/examples/webull_short_interest.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,11 +40,19 @@
         'Settlement Date': short_int_data.settlement,
         'Days to Cover': short_int_data.days_to_cover
     }
 
 
     df = pd.DataFrame(data_dict)
 
-    filename= f'files/short_interest/{ticker}_short_interest.csv'
+    # Define the directory path
+    directory = 'files/short_interest/'
+
+    # Create the directory if it doesn't exist
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
+    # Define the file path
+    filename = f'{directory}{ticker}_shortinterest.csv'
 
     df.to_csv(filename)
 asyncio.run(short_interest(ticker="AMC"))
```

### Comparing `api_master-1.8/api_master/examples/webull_stock_data.py` & `api_master-1.9/api_master/examples/webull_stock_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/webull_volume_analysis.py` & `api_master-1.9/api_master/examples/webull_volume_analysis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/examples/webull_webull_data.py` & `api_master-1.9/api_master/examples/webull_webull_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/myconfig.py` & `api_master-1.9/api_master/myconfig.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/oldapp.py` & `api_master-1.9/api_master/oldapp.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/discord_sdk/discord_sdk.py` & `api_master-1.9/api_master/sdks/discord_sdk/discord_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/discord_sdk/searching.py` & `api_master-1.9/api_master/sdks/discord_sdk/searching.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/fudstop_sdk/fudstop_sdk.py` & `api_master-1.9/api_master/sdks/fudstop_sdk/fudstop_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/fudstop_sdk/gaps.py` & `api_master-1.9/api_master/sdks/fudstop_sdk/gaps.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/fudstop_sdk/option_vol_totals.py` & `api_master-1.9/api_master/sdks/fudstop_sdk/option_vol_totals.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/helpers/conditions.py` & `api_master-1.9/api_master/sdks/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/helpers/helpers.py` & `api_master-1.9/api_master/sdks/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/models/maps.py` & `api_master-1.9/api_master/sdks/models/maps.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/models/test_events.py` & `api_master-1.9/api_master/sdks/models/test_events.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/__init__.py` & `api_master-1.9/api_master/sdks/polygon_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/aggregates.py` & `api_master-1.9/api_master/sdks/polygon_sdk/aggregates.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/async_options_sdk.py` & `api_master-1.9/api_master/sdks/polygon_sdk/async_options_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/async_polygon_sdk.py` & `api_master-1.9/api_master/sdks/polygon_sdk/async_polygon_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/company_info.py` & `api_master-1.9/api_master/sdks/polygon_sdk/company_info.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/daily_open_close.py` & `api_master-1.9/api_master/sdks/polygon_sdk/daily_open_close.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/financials.py` & `api_master-1.9/api_master/sdks/polygon_sdk/financials.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/forex_crypto.py` & `api_master-1.9/api_master/sdks/polygon_sdk/forex_crypto.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/get_all_options.py` & `api_master-1.9/api_master/sdks/polygon_sdk/get_all_options.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/indices_snapshot.py` & `api_master-1.9/api_master/sdks/polygon_sdk/indices_snapshot.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/logo.py` & `api_master-1.9/api_master/sdks/polygon_sdk/logo.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/mapping_dicts.py` & `api_master-1.9/api_master/sdks/polygon_sdk/mapping_dicts.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/models.py` & `api_master-1.9/api_master/sdks/polygon_sdk/models.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/news.py` & `api_master-1.9/api_master/sdks/polygon_sdk/news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/option_aggs.py` & `api_master-1.9/api_master/sdks/polygon_sdk/option_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/option_quote.py` & `api_master-1.9/api_master/sdks/polygon_sdk/option_quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/option_snapshot.py` & `api_master-1.9/api_master/sdks/polygon_sdk/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/option_trades.py` & `api_master-1.9/api_master/sdks/polygon_sdk/option_trades.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/pivot_points.py` & `api_master-1.9/api_master/sdks/polygon_sdk/pivot_points.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/quote.py` & `api_master-1.9/api_master/sdks/polygon_sdk/quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/snapshot.py` & `api_master-1.9/api_master/sdks/polygon_sdk/snapshot.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/technical_conditions.py` & `api_master-1.9/api_master/sdks/polygon_sdk/technical_conditions.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/polygon_sdk/tickernews.py` & `api_master-1.9/api_master/sdks/polygon_sdk/tickernews.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/terminals/crypto/menu.py` & `api_master-1.9/api_master/sdks/terminals/crypto/menu.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/calendar.py` & `api_master-1.9/api_master/sdks/webull_sdk/calendar.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/capitalflow.py` & `api_master-1.9/api_master/sdks/webull_sdk/capitalflow.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/cost_distribution.py` & `api_master-1.9/api_master/sdks/webull_sdk/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/derivative_query.py` & `api_master-1.9/api_master/sdks/webull_sdk/derivative_query.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/etf_finder.py` & `api_master-1.9/api_master/sdks/webull_sdk/etf_finder.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/events.py` & `api_master-1.9/api_master/sdks/webull_sdk/events.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/financial_statement.py` & `api_master-1.9/api_master/sdks/webull_sdk/financial_statement.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/forecast.py` & `api_master-1.9/api_master/sdks/webull_sdk/forecast.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/institutional_holdings.py` & `api_master-1.9/api_master/sdks/webull_sdk/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/manage.py` & `api_master-1.9/api_master/sdks/webull_sdk/manage.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/news.py` & `api_master-1.9/api_master/sdks/webull_sdk/news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/top_gainers.py` & `api_master-1.9/api_master/sdks/webull_sdk/top_gainers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/top_options.py` & `api_master-1.9/api_master/sdks/webull_sdk/top_options.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/webull_data.py` & `api_master-1.9/api_master/sdks/webull_sdk/webull_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/sdks/webull_sdk/webull_sdk.py` & `api_master-1.9/api_master/sdks/webull_sdk/webull_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/test.py` & `api_master-1.9/api_master/test.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master/trial.py` & `api_master-1.9/api_master/trial.py`

 * *Files identical despite different names*

### Comparing `api_master-1.8/api_master.egg-info/PKG-INFO` & `api_master-1.9/api_master.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-master
-Version: 1.8
+Version: 1.9
 Summary: Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.
 Home-page: https://github.com/your-username/your-package-repo
 Author: Chuck Dustin
 Author-email: chuckdustin12@gmail.com
 Keywords: trading,stocks,options,crypto,forex,indices,discord
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `api_master-1.8/api_master.egg-info/SOURCES.txt` & `api_master-1.9/api_master.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `api_master-1.8/setup.py` & `api_master-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='api_master',
-    version='1.8',
+    version='1.9',
     author='Chuck Dustin',
     author_email='chuckdustin12@gmail.com',
     description='Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your-username/your-package-repo',
     packages=find_packages(),
```

