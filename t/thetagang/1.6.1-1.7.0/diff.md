# Comparing `tmp/thetagang-1.6.1.tar.gz` & `tmp/thetagang-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetagang-1.6.1.tar", max compression
+gzip compressed data, was "thetagang-1.7.0.tar", max compression
```

## Comparing `thetagang-1.6.1.tar` & `thetagang-1.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    34523 2023-06-07 22:18:40.144360 thetagang-1.6.1/LICENSE
--rw-r--r--   0        0        0    14673 2023-06-07 22:18:40.144360 thetagang-1.6.1/README.md
--rw-r--r--   0        0        0     1634 2023-06-07 22:18:40.144360 thetagang-1.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 22:18:40.148360 thetagang-1.6.1/thetagang/__init__.py
--rw-r--r--   0        0        0     8247 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/config.py
--rw-r--r--   0        0        0     1068 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/config_defaults.py
--rw-r--r--   0        0        0     1461 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/dict_merge.py
--rw-r--r--   0        0        0       59 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/entry.py
--rw-r--r--   0        0        0     1091 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/fmt.py
--rw-r--r--   0        0        0     1022 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/main.py
--rw-r--r--   0        0        0      376 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/options.py
--rw-r--r--   0        0        0    69028 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/portfolio_manager.py
--rw-r--r--   0        0        0     3951 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/test_util.py
--rwxr-xr-x   0        0        0     8433 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/thetagang.py
--rw-r--r--   0        0        0     5488 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/util.py
--rw-r--r--   0        0        0    15885 1970-01-01 00:00:00.000000 thetagang-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-19 14:10:31.881745 thetagang-1.7.0/LICENSE
+-rw-r--r--   0        0        0    14617 2023-07-19 14:10:31.881745 thetagang-1.7.0/README.md
+-rw-r--r--   0        0        0     1660 2023-07-19 14:10:31.881745 thetagang-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/__init__.py
+-rw-r--r--   0        0        0     9120 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/config.py
+-rw-r--r--   0        0        0     1396 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/config_defaults.py
+-rw-r--r--   0        0        0     1461 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/dict_merge.py
+-rw-r--r--   0        0        0       59 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/entry.py
+-rw-r--r--   0        0        0     1091 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/fmt.py
+-rw-r--r--   0        0        0     1022 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/main.py
+-rw-r--r--   0        0        0      377 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/options.py
+-rw-r--r--   0        0        0    79453 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/portfolio_manager.py
+-rw-r--r--   0        0        0     3951 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/test_util.py
+-rwxr-xr-x   0        0        0     8433 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/thetagang.py
+-rw-r--r--   0        0        0     5820 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/util.py
+-rw-r--r--   0        0        0    15877 1970-01-01 00:00:00.000000 thetagang-1.7.0/PKG-INFO
```

### Comparing `thetagang-1.6.1/LICENSE` & `thetagang-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.1/README.md` & `thetagang-1.7.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![Docker publish](https://github.com/brndnmtthws/thetagang/workflows/Docker%20publish/badge.svg)](https://hub.docker.com/r/brndnmtthws/thetagang) [![Python Publish](https://github.com/brndnmtthws/thetagang/workflows/Python%20Publish/badge.svg)](https://pypi.org/project/thetagang/) [![Docker Pulls](https://img.shields.io/docker/pulls/brndnmtthws/thetagang)](https://hub.docker.com/r/brndnmtthws/thetagang) [![PyPI download month](https://img.shields.io/pypi/dm/thetagang?label=PyPI%20downloads)](https://pypi.python.org/pypi/thetagang/)
 
 [💬 Join the Matrix chat, we can get money together](https://matrix.to/#/#thetagang:frens.io).
 
 # Θ ThetaGang Θ
 
-*Beat the capitalists at their own game with ThetaGang 📈*
+_Beat the capitalists at their own game with ThetaGang 📈_
 
 ![Decay my sweet babies](thetagang.jpg)
 
 ThetaGang is an [IBKR](https://www.interactivebrokers.com/) trading bot for
 collecting premium by selling options using "The Wheel" strategy. The Wheel
 is a strategy that [surfaced on
 Reddit](https://www.reddit.com/r/options/comments/a36k4j/the_wheel_aka_triple_income_strategy_explained/),
@@ -71,45 +71,94 @@
 
 In normal usage, you would run the script as a cronjob on a daily, weekly, or
 monthly basis according to your preferences. Running more frequently than
 daily is not recommended, but the choice is yours.
 
 ![Paper account sample output](sample.png)
 
+### VIX call hedging
+
+ThetaGang can optionally hedge your account by purchasing VIX calls for the
+next month based on specified parameters. The strategy is based on the [Cboe
+VIX Tail Hedge Index](https://www.cboe.com/us/indices/dashboard/vxth/), which
+you can read about on the internet. You can enable this feature in `thetagang.toml` with:
+
+```toml
+[vix_call_hedge]
+enabled = true
+```
+
+Default values are provided, based on the VXTH index, but you may configure
+them to your taste (refer to
+[`thetagang.toml`](https://github.com/brndnmtthws/thetagang/blob/6eab3823120c10c0563e02c5d7f30dfcc0e333fc/thetagang.toml#L294-L331)
+for details).
+
+Buying VIX calls is not free, and it _will_ create some drag on your portfolio,
+but in times of extreme volatility–such as the COVID-related 2020 market
+panic–VIX calls can provide outsized returns.
+
+### Cash management
+
+At the time of writing, interest rates have reached yields that make bonds look
+attractive. To squeeze a little more juice, thetagang can do some simple cash
+management by purchasing a fund when you have extra cash. Although you do earn
+a yield on your cash balance, it's not the juiciest yield you can get, so a
+little optimization might help you earn 1 or 2 extra pennies to take the edge
+off your rent payments.
+
+There are quite a few ETFs that might be a decent place to stash your cash, and
+you should do some internet searches to find the most appropriate one for you
+and your feelings. Here are some internet web searches that you can test out to
+get some information on cash funds (ETFs):
+
+- ["cash etf reddit"](https://www.google.com/search?q=cash+etf+reddit)
+- ["sgov reddit"](https://www.google.com/search?q=sgov+reddit)
+- ["shv reddit"](https://www.google.com/search?q=shv+reddit)
+- ["short term government bond etf reddit"](https://www.google.com/search?q=short+term+government+bond+etf+reddit)
+
+You can enable cash management with:
+
+```toml
+[cash_management]
+enabled = true
+```
+
+Refer to [`thetagang.toml`](https://github.com/brndnmtthws/thetagang/blob/4fc34653786ec17fe6ce6ec2406b2d861277f934/thetagang.toml#L330-L377) for all the options.
+
 ## Project status
 
 This project is, in its current state, considered to be complete. I'm open
 to contributions, but I am unlikely to accept PRs or feature requests that
 involve significant changes to the underlying algorithm.
 
 If you find something that you think is a bug, or some other issue, please
 [create a new issue](https://github.com/brndnmtthws/thetagang/issues/new).
 
 ## "Show me your gains bro" – i.e., what are the returns?
 
-As discussed elsewhere in this README, you must conduct your own research,
-and I suggest starting with resources such as CBOE's BXM and BXDM indices,
-and comparing those to SPX. I've had a lot of people complain because "that
-strategy isn't better than buy and hold BRUH"–let me assure you, that is not
-my goal with this.
+As discussed elsewhere in this README, you must conduct your own research, and
+I suggest starting with resources such as CBOE's BXM and BXDM indices and
+comparing those to SPX. I've had a lot of people complain because "that
+strategy isn't better than buy and hold BRUH"–let me assure you, that is not my
+goal with this.
 
 There are conflicting opinions about whether selling options is good or bad,
-more or less risky, yadda yadda, but generally the risk profile for covered
+more or less risky, yadda yadda, but generally, the risk profile for covered
 calls and naked puts is no worse than the worst case for simply holding an
-ETF or stock. In fact, I'd argue that selling a naked put is better than
+ETF or stock. I'd argue that selling a naked put is better than
 buying SPY with a limit order, because at least if SPY goes to zero you keep
 the premium from selling the option. The main downside is that returns are
 capped on the upside. Depending on your goals, this may not matter. If you're
 like me, then you'd rather have consistent returns and give up a little bit
 of potential upside.
 
 Generally speaking, the point of selling options is not to exceed the returns
 of the underlying, but rather to reduce risk. Reducing risk is an important
 feature because it, in turn, allows one to increase risk in other ways
-(i.e., allocate higher percentage to stocks or buy riskier assets).
+(i.e., allocate a higher percentage to stocks or buy riskier assets).
 
 Whether you use this or not is up to you. I have not one single fuck to give,
 whether you use it or not. I am not here to convince you to use it, I merely
 want to share knowledge and perhaps help create a little bit of wealth
 redistribution.
 
 💫
@@ -133,31 +182,31 @@
 generally avoid low volume ETFs/stocks. If you don't have that kind of
 capital, you'll need to keep renting out your time to the capitalists until
 you can become a capitalist yourself. That's the way the pyramid scheme we
 call capitalism works.
 
 ## Installation
 
-*Before running ThetaGang, you should set up an IBKR paper account to test the
-code.*
+_Before running ThetaGang, you should set up an IBKR paper account to test the
+code._
 
 ```console
-$ pip install thetagang
+pip install thetagang
 ```
 
 It's recommended you familiarize yourself with
 [IBC](https://github.com/IbcAlpha/IBC) so you know how it works. You'll need
 to know how to configure the various knows and settings, and make sure things
 like API ports are configured correctly. If you don't want to mess around too
 much, consider [running ThetaGang with Docker](#running-with-docker).
 
 ## Usage
 
 ```console
-$ thetagang -h
+thetagang -h
 ```
 
 ## Up and running with Docker
 
 My preferred way for running ThetaGang is to use a cronjob to execute Docker
 commands. I've built a Docker image as part of this project, which you can
 use with your installation. There's a [prebuilt Docker image
@@ -170,29 +219,29 @@
 
 The easiest way to get the config files into the container is by mounting a
 volume.
 
 To get started, grab a copy of `thetagang.toml` and `config.ini`:
 
 ```console
-$ mkdir ~/thetagang
-$ cd ~/thetagang
-$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/thetagang.toml -o ./thetagang.toml
-$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/ibc-config.ini -o ./config.ini
+mkdir ~/thetagang
+cd ~/thetagang
+curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/thetagang.toml -o ./thetagang.toml
+curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/ibc-config.ini -o ./config.ini
 ```
 
 Edit `~/thetagang/thetagang.toml` to suit your needs. Pay particular
 attention to the symbols and weights. At a minimum, you must change the
 username, password, and account number. You may also want to change the
 trading move from paper to live when needed.
 
 Now, to run ThetaGang with Docker:
 
 ```console
-$ docker run --rm -i --net host \
+docker run --rm -i --net host \
     -v ~/thetagang:/etc/thetagang \
     brndnmtthws/thetagang:main \
     --config /etc/thetagang/thetagang.toml
 ```
 
 Lastly, to run ThetaGang as a daily cronjob Monday to Friday at 9am, add
 something like this to your crontab (on systems with a cron installation, use
@@ -205,48 +254,46 @@
 ## Determining which ETFs or stocks to run ThetaGang with
 
 I leave this as an exercise to the reader, however I will provide a few
 recommendations and resources:
 
 ### Recommendations
 
-* Stick with high volume ETFs or stocks
-* Careful with margin usage, you'll want to calculate the worst case scenario
+- Stick with high volume ETFs or stocks
+- Careful with margin usage, you'll want to calculate the worst case scenario
   and provide plenty of cushion for yourself based on your portfolio
 
-
 ### Resources
 
-* For discussions about selling options, check out
+- For discussions about selling options, check out
   [r/thetagang](https://www.reddit.com/r/thetagang/)
-* For backtesting portfolios, you can use [this
+- For backtesting portfolios, you can use [this
   tool](https://www.portfoliovisualizer.com/backtest-portfolio) and [this
   tool](https://www.portfoliovisualizer.com/optimize-portfolio) to get an idea
   of drawdown and typical volatility
 
 ## Development
 
 Check out the code to your local machine and install the Python dependencies:
 
-```shell
-$ poetry install
-$ poetry run autohooks activate
-$ poetry run thetagang -h
-...
+```console
+poetry install
+poetry run autohooks activate
+poetry run thetagang -h
 ```
 
 You are now ready to make a splash! 🐳
 
 ## FAQ
 
-| Error                                                                                                      | Cause                                                                                                                            | Resolution                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| Requested market data is not subscribed.                                                                   | Requisite market data subscriptions have not been set up on IBKR.                                                                | [Configure](https://www.interactivebrokers.com/en/software/am3/am/settings/marketdatasubscriptions.htm) your market data subscriptions. The default config that ships with this script uses the `Cboe One Add-On Bundle` and the `US Equity and Options Add-On Streaming Bundle`. **Note**: You _must_ fund your account before IBKR will send data for subscriptions. Without funding you can still subscribe but you will get an error from ibc. |
-| No market data during competing live session                                                               | Your account is logged in somewhere else, such as the IBKR web portal, the desktop app, or even another instance of this script. | Log out of all sessions and then re-run the script.                                                                                                                                                                                                                                                                                                                                                                                                |
-| `ib_insync.wrapper ERROR Error 200, reqId 10: The contract description specified for SYMBOL is ambiguous.` | IBKR needs to know which exchange is the primary exchange for a given symbol.                                                    | You need to specify the primary exchange for the stock. This is normal for companies, typically. For ETFs it usually isn't required. Specify the `primary_exchange` parameter for the symbol, i.e., `primary_exchange = "NYSE"`.                                                                                                                                                                                                                   |
+| Error | Cause | Resolution |
+|---|---|---|
+| Requested market data is not subscribed. | Requisite market data subscriptions have not been set up on IBKR. | [Configure](https://www.interactivebrokers.com/en/software/am3/am/settings/marketdatasubscriptions.htm) your market data subscriptions. The default config that ships with this script uses the `Cboe One Add-On Bundle` and the `US Equity and Options Add-On Streaming Bundle`. **Note**: You _must_ fund your account before IBKR will send data for subscriptions. Without funding you can still subscribe but you will get an error from ibc. |
+| No market data during competing live session | Your account is logged in somewhere else, such as the IBKR web portal, the desktop app, or even another instance of this script. | Log out of all sessions and then re-run the script. |
+| `ib_insync.wrapper ERROR Error 200, reqId 10: The contract description specified for SYMBOL is ambiguous.` | IBKR needs to know which exchange is the primary exchange for a given symbol. | You need to specify the primary exchange for the stock. This is normal for companies, typically. For ETFs it usually isn't required. Specify the `primary_exchange` parameter for the symbol, i.e., `primary_exchange = "NYSE"`. |
 
 ## Support and sponsorship
 
 If you get some value out of this, please consider [sponsoring me](https://github.com/sponsors/brndnmtthws)
 to continue maintaining this project well into the future. Like
 everyone else in the world, I'm just trying to survive.
```

### Comparing `thetagang-1.6.1/pyproject.toml` & `thetagang-1.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 description = "ThetaGang is an IBKR bot for getting money"
 documentation = "https://github.com/brndnmtthws/thetagang/blob/master/README.md"
 homepage = "https://github.com/brndnmtthws/thetagang"
 license = "AGPL-3.0-only"
 name = "thetagang"
 readme = "README.md"
 repository = "https://github.com/brndnmtthws/thetagang.git"
-version = "1.6.1"
+version = "1.7.0"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 click-log = "^0.4.0"
-ib_insync = "^0.9.81"
+ib_insync = "^0.9.86"
 python = ">=3.9,<4.0"
 python-dateutil = "^2.8.1"
 pytimeparse = "^1.1.8"
 schema = "^0.7.5"
 toml = "^0.10.2"
 rich = "^13.3.5"
+more-itertools = "^9.1.0"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.0"
 autohooks = "^23.4.0"
 autohooks-plugin-black = ">=22.11,<24.0"
 autohooks-plugin-isort = ">=22.8,<24.0"
 autohooks-plugin-pylint = ">=22.8.1,<24.0.0"
```

### Comparing `thetagang-1.6.1/thetagang/config.py` & `thetagang-1.7.0/thetagang/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,31 @@
 
 def validate_config(config):
     if "minimum_cushion" in config["account"]:
         raise RuntimeError(
             "Config error: minimum_cushion is deprecated and replaced with margin_usage. See sample config for details."
         )
 
+    algo_settings = {
+        "strategy": And(str, len),
+        "params": [And([str], lambda p: len(p) == 2)],
+    }
+
     schema = Schema(
         {
             "account": {
                 "number": And(str, len),
                 "cancel_orders": bool,
                 "margin_usage": And(float, lambda n: 0 <= n),
                 "market_data_type": And(int, lambda n: 1 <= n <= 4),
             },
             "orders": {
-                "exchange": And(str, len),
-                "algo": {
-                    "strategy": And(str, len),
-                    "params": [And([str], lambda p: len(p) == 2)],
-                },
+                Optional("exchange"): And(str, len),
+                Optional("algo"): algo_settings,
+                Optional("price_update_delay"): And([int], lambda p: len(p) == 2),
             },
             "option_chains": {
                 "expirations": And(int, lambda n: 1 <= n),
                 "strikes": And(int, lambda n: 1 <= n),
             },
             Optional("write_when"): {
                 Optional("calls"): {
@@ -142,17 +145,21 @@
                         Optional("strike_limit"): And(float, lambda n: n > 0),
                     },
                     Optional("puts"): {
                         Optional("delta"): And(float, lambda n: 0 <= n <= 1),
                         Optional("write_threshold"): And(float, lambda n: 0 <= n <= 1),
                         Optional("strike_limit"): And(float, lambda n: n > 0),
                     },
+                    Optional("adjust_price_after_delay"): bool,
                 }
             },
-            Optional("ib_insync"): {Optional("logfile"): And(str, len)},
+            Optional("ib_insync"): {
+                Optional("logfile"): And(str, len),
+                Optional("api_response_wait_time"): int,
+            },
             "ibc": {
                 Optional("password"): And(str, len),
                 Optional("userid"): And(str, len),
                 Optional("gateway"): bool,
                 Optional("RaiseRequestErrors"): bool,
                 Optional("ibcPath"): And(str, len),
                 Optional("tradingMode"): And(
@@ -190,14 +197,27 @@
                     {
                         Optional("lower_bound"): float,
                         Optional("upper_bound"): float,
                         Optional("weight"): float,
                     },
                 ],
             },
+            Optional("cash_management"): {
+                Optional("enabled"): bool,
+                Optional("cash_fund"): And(str, len),
+                Optional("primary_exchange"): And(str, len),
+                Optional("target_cash_balance"): int,
+                Optional("buy_threshold"): And(int, lambda n: n > 0),
+                Optional("sell_threshold"): And(int, lambda n: n > 0),
+                Optional("primary_exchange"): And(str, len),
+                Optional("orders"): {
+                    "exchange": And(str, len),
+                    "algo": algo_settings,
+                },
+            },
         }
     )
     schema.validate(config)
 
     assert len(config["symbols"]) > 0
 
     assert math.isclose(
```

### Comparing `thetagang-1.6.1/thetagang/dict_merge.py` & `thetagang-1.7.0/thetagang/dict_merge.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.1/thetagang/fmt.py` & `thetagang-1.7.0/thetagang/fmt.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.1/thetagang/main.py` & `thetagang-1.7.0/thetagang/main.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.1/thetagang/portfolio_manager.py` & `thetagang-1.7.0/thetagang/portfolio_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
 import math
 import sys
 from functools import lru_cache
 from typing import Optional
 
-from ib_insync import Order, Ticker, util
+from ib_insync import Ticker, Trade, util
 from ib_insync.contract import ComboLeg, Contract, Index, Option, Stock, TagValue
 from ib_insync.order import LimitOrder
+from more_itertools import partition
 from rich import box
 from rich.console import Console, Group
 from rich.panel import Panel
 from rich.pretty import Pretty
 from rich.progress import track
 from rich.table import Table
 
 from thetagang.fmt import dfmt, ffmt, ifmt, pfmt
 from thetagang.util import (
     account_summary_to_dict,
+    algo_params_from,
     count_short_option_positions,
     get_call_cap,
     get_higher_price,
     get_lower_price,
     get_strike_limit,
     get_target_delta,
     get_write_threshold,
@@ -31,19 +33,14 @@
     wait_n_seconds,
 )
 
 from .options import option_dte
 
 console = Console()
 
-# Typically the amount of time needed when waiting on data from the IBKR API.
-# Sometimes it can take a while to retrieve data, and it's lazy-loaded by the
-# API, so getting this number right is largely a matter of guesswork.
-API_RESPONSE_WAIT_TIME = 60
-
 
 # Turn off some of the more annoying logging output from ib_insync
 logging.getLogger("ib_insync.ib").setLevel(logging.ERROR)
 logging.getLogger("ib_insync.wrapper").setLevel(logging.CRITICAL)
 
 
 class PortfolioManager:
@@ -51,16 +48,19 @@
         self.account_number = config["account"]["number"]
         self.config = config
         self.ib = ib
         self.completion_future = completion_future
         self.ib.orderStatusEvent += self.orderStatusEvent
         self.has_excess_calls = set()
         self.has_excess_puts = set()
-        self.orders = []
-        self.trades = []
+        self.orders: list[tuple[Contract, LimitOrder]] = []
+        self.trades: list[Trade] = []
+
+    def api_response_wait_time(self) -> int:
+        return self.config["ib_insync"]["api_response_wait_time"]
 
     def orderStatusEvent(self, trade):
         if "Filled" in trade.orderStatus.status:
             console.print(
                 f"[green]Order filled, symbol={trade.contract.symbol}",
             )
         if "Cancelled" in trade.orderStatus.status:
@@ -92,64 +92,60 @@
                     ),
                     portfolio_positions[symbol],
                 )
             )
 
         return ret
 
-    def wait_for_midpoint_price(self, ticker, wait_time=API_RESPONSE_WAIT_TIME):
+    def wait_for_midpoint_price(self, ticker, wait_time):
         try:
             wait_n_seconds(
                 lambda: util.isNan(ticker.midpoint()),
                 lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
                 wait_time,
             )
         except RuntimeError:
             return False
         return True
 
-    def wait_for_market_price(self, ticker, wait_time=API_RESPONSE_WAIT_TIME):
+    def wait_for_market_price(self, ticker, wait_time):
         try:
             wait_n_seconds(
                 lambda: util.isNan(ticker.marketPrice()),
                 lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
                 wait_time,
             )
         except RuntimeError:
             return False
         return True
 
-    def wait_for_greeks(self, ticker, wait_time=API_RESPONSE_WAIT_TIME):
+    def wait_for_greeks(self, ticker, wait_time):
         try:
             wait_n_seconds(
                 lambda: ticker.modelGreeks is None
                 or util.isNan(ticker.modelGreeks.delta),
                 lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
                 wait_time,
             )
         except RuntimeError:
             return False
         return True
 
-    def wait_for_market_price_for(
-        self, tickers: list[Ticker], wait_time=API_RESPONSE_WAIT_TIME
-    ):
+    def wait_for_market_price_for(self, tickers: list[Ticker], wait_time):
         try:
             wait_n_seconds(
                 lambda: any(util.isNan(ticker.marketPrice()) for ticker in tickers),
                 lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
                 wait_time,
             )
         except RuntimeError:
             return False
         return True
 
-    def wait_for_greeks_for(
-        self, tickers: list[Ticker], wait_time=API_RESPONSE_WAIT_TIME
-    ):
+    def wait_for_greeks_for(self, tickers: list[Ticker], wait_time):
         try:
             wait_n_seconds(
                 lambda: any(
                     ticker.modelGreeks is None
                     or ticker.modelGreeks.delta is None
                     or util.isNan(ticker.modelGreeks.delta)
                     for ticker in tickers
@@ -157,75 +153,78 @@
                 lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
                 wait_time,
             )
         except RuntimeError:
             return False
         return True
 
-    def wait_for_open_interest_for(
-        self, tickers: list[Ticker], wait_time=API_RESPONSE_WAIT_TIME
-    ):
+    def wait_for_open_interest_for(self, tickers: list[Ticker], wait_time):
         def open_interest_is_not_ready(ticker):
             if ticker.contract.right.startswith("P"):
                 return util.isNan(ticker.putOpenInterest)
             return util.isNan(ticker.callOpenInterest)
 
         try:
             wait_n_seconds(
                 lambda: any(open_interest_is_not_ready(ticker) for ticker in tickers),
                 lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
                 wait_time,
             )
         except RuntimeError:
             console.print(
-                f"Timeout waiting on market data for contracts={[ticker.contract for ticker in tickers if open_interest_is_not_ready(ticker)]}, continuing...",
+                f"Timeout waiting on market data for contracts="
+                f"{[ticker.contract for ticker in tickers if open_interest_is_not_ready(ticker)]}, continuing...",
             )
             return False
         finally:
             for ticker in tickers:
                 if open_interest_is_not_ready(ticker):
                     self.ib.cancelMktData(ticker.contract)
 
     @lru_cache(maxsize=32)
     def get_chains_for_contract(self, contract):
         return self.ib.reqSecDefOptParams(
             contract.symbol, "", contract.secType, contract.conId
         )
 
     @lru_cache(maxsize=32)
-    def get_ticker_for_stock(self, symbol, primary_exchange):
+    def get_ticker_for_stock(
+        self, symbol, primary_exchange, order_exchange=None
+    ) -> Ticker:
         stock = Stock(
             symbol,
-            self.get_order_exchange(),
+            order_exchange or self.get_order_exchange(),
             currency="USD",
             primaryExchange=primary_exchange,
         )
         self.ib.qualifyContracts(stock)
         return self.get_ticker_for(stock)
 
     @lru_cache(maxsize=32)
-    def get_ticker_for(self, contract, midpoint=False):
+    def get_ticker_for(self, contract, midpoint=False) -> Ticker:
         [ticker] = self.ib.reqTickers(contract)
 
         if midpoint:
-            self.wait_for_midpoint_price(ticker)
+            self.wait_for_midpoint_price(
+                ticker, wait_time=self.api_response_wait_time()
+            )
         else:
-            self.wait_for_market_price(ticker)
+            self.wait_for_market_price(ticker, wait_time=self.api_response_wait_time())
 
         return ticker
 
     @lru_cache(maxsize=32)
-    def get_ticker_list_for(self, contracts):
+    def get_ticker_list_for(self, contracts) -> list[Ticker]:
         ticker_list = self.ib.reqTickers(*contracts)
 
         try:
             wait_n_seconds(
                 lambda: any([util.isNan(t.midpoint()) for t in ticker_list]),
                 lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
-                API_RESPONSE_WAIT_TIME,
+                self.api_response_wait_time(),
             )
         except RuntimeError:
             pass
 
         return ticker_list
 
     def put_is_itm(self, contract):
@@ -393,15 +392,19 @@
 
     def filter_positions(self, portfolio_positions):
         symbols = self.get_symbols()
         return [
             item
             for item in portfolio_positions
             if item.account == self.account_number
-            and (item.contract.symbol in symbols or item.contract.symbol == "VIX")
+            and (
+                item.contract.symbol in symbols
+                or item.contract.symbol == "VIX"
+                or item.contract.symbol == self.config["cash_management"]["cash_fund"]
+            )
             and item.position != 0
             and item.averageCost != 0
         ]
 
     def get_portfolio_positions(self):
         portfolio_positions = self.ib.portfolio(account=self.account_number)
         return portfolio_positions_to_dict(self.filter_positions(portfolio_positions))
@@ -415,14 +418,19 @@
             for trade in open_trades:
                 if not trade.isDone() and (
                     trade.contract.symbol in self.get_symbols()
                     or (
                         self.config["vix_call_hedge"]["enabled"]
                         and trade.contract.symbol == "VIX"
                     )
+                    or (
+                        self.config["cash_management"]["enabled"]
+                        and trade.contract.symbol
+                        == self.config["cash_management"]["cash_fund"]
+                    )
                 ):
                     console.print(f"[red]Canceling order {trade.order}[/red]")
                     self.ib.cancelOrder(trade.order)
 
     def summarize_account(self):
         account_summary = self.ib.accountSummary(self.account_number)
         account_summary = account_summary_to_dict(account_summary)
@@ -584,61 +592,56 @@
             self.write_puts(puts_to_write)
             self.write_calls(calls_to_write)
 
             # Refresh positions, in case anything changed from the orders above
             portfolio_positions = self.get_portfolio_positions()
 
             (rollable_puts, closeable_puts, group1) = self.check_puts(
-                account_summary, portfolio_positions
+                portfolio_positions
             )
             (rollable_calls, closeable_calls, group2) = self.check_calls(
-                account_summary, portfolio_positions
+                portfolio_positions
             )
             console.print(Panel(Group(group1, group2)))
 
             self.roll_puts(rollable_puts, account_summary)
             self.close_puts(closeable_puts)
             self.roll_calls(rollable_calls, account_summary, portfolio_positions)
             self.close_calls(closeable_calls)
 
             # check if we should do VIX call hedging
             self.do_vix_hedging(account_summary, portfolio_positions)
 
+            # manage dat cash
+            self.do_cashman(account_summary, portfolio_positions)
+
             self.submit_orders()
 
-            with console.status(
-                f"[bold blue_violet]Waiting for {len(self.trades)} orders to submit..."
-            ) as _status:
-                # Wait for pending orders
-                wait_n_seconds(
-                    lambda: any(
-                        [
-                            trade.orderStatus.status
-                            in ["PendingSubmit", "PreSubmitted"]
-                            for trade in self.trades
-                            if trade
-                        ]
-                    ),
-                    lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
-                    API_RESPONSE_WAIT_TIME,
-                )
+            try:
+                self.wait_for_pending_orders()
+            except RuntimeError:
+                pass
+
+            self.adjust_prices()
+
+            self.wait_for_pending_orders()
 
             console.print(
                 "[bright_yellow]ThetaGang is done, shutting down! Cya next time. :sparkles:[/bright_yellow]"
             )
 
         except:
             console.print_exception()
             raise
 
         finally:
             # Shut it down
             self.completion_future.set_result(True)
 
-    def check_puts(self, account_summary, portfolio_positions):
+    def check_puts(self, portfolio_positions):
         # Check for puts which may be rolled to the next expiration or a better price
         puts = self.get_puts(portfolio_positions)
 
         # find puts eligible to be rolled or closed
         rollable_puts = []
         closeable_puts = []
 
@@ -664,15 +667,15 @@
         if total_closeable_puts + total_rollable_puts > 0:
             group = Group(text1, text2, table)
         else:
             group = Group(text1, text2)
 
         return (rollable_puts, closeable_puts, group)
 
-    def check_calls(self, account_summary, portfolio_positions):
+    def check_calls(self, portfolio_positions):
         # Check for calls which may be rolled to the next expiration or a better price
         calls = self.get_calls(portfolio_positions)
 
         # find calls eligible to be rolled
         rollable_calls = []
         closeable_calls = []
 
@@ -718,17 +721,18 @@
 
     def check_for_uncovered_positions(self, account_summary, portfolio_positions):
         call_actions_table = Table(title="Call writing summary")
         call_actions_table.add_column("Symbol")
         call_actions_table.add_column("Action")
         call_actions_table.add_column("Detail")
         to_write = []
+        symbols = set(self.get_symbols())
         for symbol in portfolio_positions:
-            if symbol == "VIX":
-                # skip VIX positions
+            if symbol not in symbols:
+                # skip positions we don't care about
                 continue
             call_count = max(
                 [0, count_short_option_positions(symbol, portfolio_positions, "C")]
             )
             stock_count = math.floor(
                 sum(
                     [
@@ -850,15 +854,17 @@
             except RuntimeError:
                 console.print_exception()
                 console.print(
                     f"[yellow]Finding eligible contracts for {symbol} failed. Continuing anyway...",
                 )
                 continue
 
-            if not self.wait_for_midpoint_price(sell_ticker):
+            if not self.wait_for_midpoint_price(
+                sell_ticker, wait_time=self.api_response_wait_time()
+            ):
                 console.print(
                     f"[red]Couldn't get midpoint price for contract={sell_ticker.contract}, skipping for now",
                 )
                 continue
 
             # Create order
             order = LimitOrder(
@@ -890,15 +896,17 @@
             except RuntimeError:
                 console.print_exception()
                 console.print(
                     f"[yellow]Finding eligible contracts for {symbol} failed. Continuing anyway...",
                 )
                 continue
 
-            if not self.wait_for_midpoint_price(sell_ticker):
+            if not self.wait_for_midpoint_price(
+                sell_ticker, wait_time=self.api_response_wait_time()
+            ):
                 console.print(
                     f"[red]Couldn't get midpoint price for contract={sell_ticker.contract}, skipping for now",
                 )
                 continue
 
             # Create order
             order = LimitOrder(
@@ -1134,35 +1142,40 @@
                 self.enqueue_order(ticker.contract, order)
             except RuntimeError:
                 console.print_exception()
                 console.print(
                     "[yellow]Error occurred when trying to close position. Continuing anyway...",
                 )
 
-    def roll_positions(self, positions, right, account_summary, portfolio_positions={}):
+    def roll_positions(
+        self, positions, right, account_summary, portfolio_positions=None
+    ):
         for position in positions:
             try:
                 symbol = position.contract.symbol
 
                 position.contract.exchange = self.get_order_exchange()
                 buy_ticker = self.get_ticker_for(position.contract, midpoint=True)
 
                 strike_limit = get_strike_limit(self.config, symbol, right)
                 if right.startswith("C"):
+                    average_cost = (
+                        [
+                            p.averageCost
+                            for p in portfolio_positions[symbol]
+                            if isinstance(p.contract, Stock)
+                        ]
+                        if portfolio_positions and symbol in portfolio_positions
+                        else [0]
+                    )
                     strike_limit = round(
-                        max(
-                            [strike_limit or 0]
-                            + [
-                                p.averageCost
-                                for p in portfolio_positions[symbol]
-                                if isinstance(p.contract, Stock)
-                            ]
-                        ),
+                        max([strike_limit or 0] + average_cost),
                         2,
                     )
+
                 elif right.startswith("P"):
                     strike_limit = round(
                         min(
                             [strike_limit or sys.float_info.max]
                             + [
                                 position.contract.strike
                                 + (
@@ -1415,59 +1428,84 @@
                     )
 
                 return midpoint_or_market_price(
                     ticker
                 ) > minimum_price and cost_doesnt_exceed_market_price(ticker)
 
             # Filter out tickers with invalid or unavailable prices
-            self.wait_for_market_price_for(tickers)
+            self.wait_for_market_price_for(
+                tickers, wait_time=self.api_response_wait_time()
+            )
             status.stop()
             tickers = [
                 ticker
                 for ticker in track(
                     tickers,
-                    description=f"[royal_blue1]Filtering invalid prices for {main_contract.symbol} from {len(tickers)} tickers...",
+                    description=f"[royal_blue1]Filtering invalid prices for "
+                    f"{main_contract.symbol} from {len(tickers)} tickers...",
                 )
                 if price_is_valid(ticker)
             ]
             status.start()
             # Filter by delta
-            self.wait_for_greeks_for(tickers)
-            tickers = [ticker for ticker in tickers if delta_is_valid(ticker)]
-            # Fetch market data for open interest
-            tickers = [
-                self.ib.reqMktData(ticker.contract, genericTickList="101")
-                for ticker in tickers
-            ]
-            # Filter by open interest
-            self.wait_for_open_interest_for(tickers)
-            status.stop()
-            tickers = [
-                ticker
-                for ticker in track(
-                    tickers,
-                    description=f"[royal_blue1]Filtering by open interest for "
-                    f"{main_contract.symbol} from {len(tickers)} tickers...",
-                )
-                if open_interest_is_valid(ticker)
-            ]
-            status.start()
-            # Sort by delta first, then expiry date
-            tickers = sorted(
-                sorted(tickers, key=lambda t: abs(t.modelGreeks.delta), reverse=True),
-                key=lambda t: option_dte(t.contract.lastTradeDateOrContractMonth),
-            )
+            self.wait_for_greeks_for(tickers, wait_time=self.api_response_wait_time())
+            delta_reject_tickers, tickers = partition(delta_is_valid, tickers)
 
-            if len(tickers) == 0:
-                raise RuntimeError(
-                    f"No valid contracts found for {main_contract.symbol}. Continuing anyway..."
+            def filter_remaining_tickers(tickers, delta_ord_desc):
+                # Fetch market data for open interest
+                tickers = [
+                    self.ib.reqMktData(ticker.contract, genericTickList="101")
+                    for ticker in tickers
+                ]
+                # Filter by open interest
+                self.wait_for_open_interest_for(
+                    tickers, wait_time=self.api_response_wait_time()
                 )
+                status.stop()
+                tickers = [
+                    ticker
+                    for ticker in track(
+                        tickers,
+                        description=f"[royal_blue1]Filtering by open interest for "
+                        f"{main_contract.symbol} from {len(tickers)} tickers...",
+                    )
+                    if open_interest_is_valid(ticker)
+                ]
+                status.start()
+                # Sort by delta first, then expiry date
+                tickers = sorted(
+                    sorted(
+                        tickers,
+                        key=lambda t: abs(t.modelGreeks.delta),
+                        reverse=delta_ord_desc,
+                    ),
+                    key=lambda t: option_dte(t.contract.lastTradeDateOrContractMonth),
+                )
+                return tickers
+
+            tickers = filter_remaining_tickers(tickers, True)
 
             the_chosen_ticker = None
-            if preferred_minimum_price is not None:
+            if len(tickers) == 0:
+                if not math.isclose(minimum_price, 0.0):
+                    # if we arrive here, it means that 1) we expect to roll for a
+                    # credit only, but 2) we didn't find any suitable contracts,
+                    # most likely because we can't roll out and up/down to the
+                    # target delta
+                    #
+                    # because of this, we'll allow rolling to a less-than-optimal
+                    # strike, provided it's still a credit
+                    tickers = filter_remaining_tickers(delta_reject_tickers, False)
+                if len(tickers) == 0:
+                    # if there are _still_ no tickers remaining, there's nothing
+                    # more we can do
+                    raise RuntimeError(
+                        f"No valid contracts found for {main_contract.symbol}. Continuing anyway..."
+                    )
+            elif preferred_minimum_price is not None:
                 # if there's a preferred minimum price specified, try to find
                 # contracts that are at least that price first
                 for ticker in tickers:
                     if midpoint_or_market_price(ticker) > preferred_minimum_price:
                         the_chosen_ticker = ticker
                         break
                 if the_chosen_ticker is None:
@@ -1491,26 +1529,26 @@
 
             return the_chosen_ticker
 
     def get_algo_strategy(self):
         return self.config["orders"]["algo"]["strategy"]
 
     def get_algo_params(self):
-        return [TagValue(p[0], p[1]) for p in self.config["orders"]["algo"]["params"]]
+        return algo_params_from(self.config["orders"]["algo"]["params"])
 
     def get_order_exchange(self):
         return self.config["orders"]["exchange"]
 
     def do_vix_hedging(self, account_summary, portfolio_positions):
         to_print = []
 
         def inner_handler():
             if not self.config["vix_call_hedge"]["enabled"]:
                 to_print.append(
-                    "🛑 VIX call hedging not enabled, skipping",
+                    "[red]🛑 VIX call hedging not enabled, skipping",
                 )
                 return
 
             def vix_calls_should_be_closed() -> (
                 tuple[bool, Optional[Ticker], Optional[float]]
             ):
                 if "close_hedges_when_vix_exceeds" in self.config["vix_call_hedge"]:
@@ -1526,19 +1564,19 @@
                     return (False, vix_ticker, close_hedges_when_vix_exceeds)
                 return (False, None, None)
 
             with console.status(
                 "[bold blue_violet]Checking on our VIX call hedge..."
             ) as status:
                 net_vix_call_count = net_option_positions(
-                    "VIX", portfolio_positions, "C"
+                    "VIX", portfolio_positions, "C", ignore_zero_dte=True
                 )
                 if net_vix_call_count > 0:
                     status.update(
-                        f"[bold blue_violet]net_vix_call_count={net_vix_call_count}, "
+                        f"[bold blue_violet]net_vix_call_count={net_vix_call_count} (0dte contracts ignored), "
                         "checking if we need to close positions...",
                     )
                     (
                         close_vix_calls,
                         vix_ticker,
                         close_hedges_when_vix_exceeds,
                     ) = vix_calls_should_be_closed()
@@ -1687,27 +1725,146 @@
                             "[yellow]Error occurred when VIX call hedging. Continuing anyway...",
                         )
 
         inner_handler()
 
         console.print(Panel(Group(*to_print), title="VIX call hedging"))
 
-    def enqueue_order(self, contract: Contract, order: Order):
+    def do_cashman(self, account_summary, portfolio_positions):
+        to_print = []
+
+        def inner_handler():
+            if not self.config["cash_management"]["enabled"]:
+                to_print.append(
+                    "[red]🛑 Cash managementnot enabled, skipping",
+                )
+                return
+
+            target_cash_balance = self.config["cash_management"]["target_cash_balance"]
+            buy_threshold = self.config["cash_management"]["buy_threshold"]
+            sell_threshold = self.config["cash_management"]["sell_threshold"]
+            cash_balance = math.floor(float(account_summary["TotalCashValue"].value))
+
+            try:
+
+                def make_order() -> tuple[Optional[Ticker], Optional[LimitOrder]]:
+                    symbol = self.config["cash_management"]["cash_fund"]
+                    primary_exchange = self.config["cash_management"].get(
+                        "primary_exchange", ""
+                    )
+                    order_exchange = (
+                        self.config["cash_management"]["orders"]["exchange"]
+                        if "orders" in self.config["cash_management"]
+                        else None
+                    )
+                    ticker = self.get_ticker_for_stock(
+                        symbol, primary_exchange, order_exchange
+                    )
+                    algo = (
+                        self.config["cash_management"]["orders"]["algo"]
+                        if "orders" in self.config["cash_management"]
+                        else self.config["orders"]["algo"]
+                    )
+
+                    amount = cash_balance - target_cash_balance
+                    price = ticker.ask
+                    qty = amount // price
+
+                    if qty > 0:
+                        to_print.append(
+                            f"[green]cash_balance={cash_balance} which exceeds "
+                            f"(target_cash_balance + buy_threshold)={(target_cash_balance + buy_threshold)}"
+                        )
+                        to_print.append(
+                            f"[green]Will buy {symbol} with qty={qty} shares at price={price}"
+                        )
+
+                    # make sure qty does not exceed balance if it's a negative value
+                    if qty < 0:
+                        # subtract 1 to keep cash balance above target
+                        qty -= 1
+                        to_print.append(
+                            f"[green]cash_balance={cash_balance} which is less than "
+                            f"(target_cash_balance - sell_threshold)={(target_cash_balance + sell_threshold)}"
+                        )
+                        if symbol not in portfolio_positions:
+                            # we don't have any positions to sell
+                            to_print.append(
+                                f"[red]Will sell {symbol} with qty={-qty} at"
+                                f" price={price}, but we have no position to sell"
+                            )
+                            return (None, None)
+                        positions = [
+                            p.position
+                            for p in portfolio_positions[symbol]
+                            if isinstance(p.contract, Stock)
+                        ]
+                        position = positions[0] if len(positions) > 0 else 0
+                        qty = min([max([-position, qty]), 0])
+                        # if for some reason the qty is zero, do nothing
+                        if qty == 0:
+                            to_print.append(
+                                f"[red]Will sell {symbol} with qty={-qty} at price={price}, but we don't have any shares to sell"
+                            )
+                            return (None, None)
+                        to_print.append(
+                            f"[green]Will sell {symbol} with qty={-qty} at price={price}"
+                        )
+
+                    order = LimitOrder(
+                        "BUY" if qty > 0 else "SELL",
+                        abs(qty),
+                        round(price, 2),
+                        algoStrategy=algo["strategy"],
+                        algoParams=algo_params_from(algo["params"]),
+                        tif="DAY",
+                        account=self.account_number,
+                        transmit=True,
+                    )
+                    return (ticker, order)
+
+                if (
+                    cash_balance > target_cash_balance + buy_threshold
+                    or cash_balance < target_cash_balance - sell_threshold
+                ):
+                    (ticker, order) = make_order()
+                    if ticker and ticker.contract and order:
+                        self.enqueue_order(ticker.contract, order)
+                else:
+                    to_print.append(
+                        "[green]All good, nothing to do here.",
+                    )
+
+            except RuntimeError:
+                console.print_exception()
+                console.print(
+                    "[yellow]Error occurred when VIX call hedging. Continuing anyway...",
+                )
+
+        inner_handler()
+
+        console.print(Panel(Group(*to_print), title="Cash management"))
+
+    def enqueue_order(self, contract: Contract, order: LimitOrder):
         self.orders.append((contract, order))
 
     def submit_orders(self):
-        def submit(contract, order):
+        def submit(contract, order) -> Optional[Trade]:
             try:
                 trade = self.ib.placeOrder(contract, order)
                 return trade
             except RuntimeError:
                 console.print_exception()
             return None
 
-        self.trades = [submit(order[0], order[1]) for order in self.orders]
+        self.trades = [
+            trade
+            for trade in [submit(order[0], order[1]) for order in self.orders]
+            if trade
+        ]
 
         if len(self.trades) > 0:
             table = Table(
                 title="Orders submitted", show_lines=True, box=box.MINIMAL_HEAVY_HEAD
             )
             table.add_column("Symbol")
             table.add_column("Exchange")
@@ -1727,7 +1884,95 @@
                         trade.order.action,
                         dfmt(trade.order.lmtPrice),
                         ifmt(trade.order.totalQuantity),
                         trade.orderStatus.status,
                         ffmt(trade.orderStatus.filled, 0),
                     )
             console.print(table)
+
+    def adjust_prices(self):
+        if (
+            any(
+                [
+                    not self.config["symbols"][symbol].get(
+                        "adjust_price_after_delay", False
+                    )
+                    for symbol in self.config["symbols"]
+                ]
+            )
+            or len(self.trades) == 0
+        ):
+            return
+
+        import random
+
+        delay = random.randrange(
+            self.config["orders"]["price_update_delay"][0],
+            self.config["orders"]["price_update_delay"][1],
+        )
+        for _ in track(
+            range(delay),
+            description=f"Waiting {delay}s before we update prices...",
+        ):
+            self.ib.sleep(1)
+
+        unfilled = [
+            (idx, trade)
+            for idx, trade in enumerate(self.trades)
+            if trade
+            and trade.contract.symbol in self.config["symbols"]
+            and self.config["symbols"][trade.contract.symbol].get(
+                "adjust_price_after_delay", False
+            )
+            and not trade.isDone()
+        ]
+        for idx, trade in unfilled:
+            try:
+                ticker = self.ib.reqMktData(trade.contract)
+
+                if self.wait_for_midpoint_price(
+                    ticker, wait_time=self.api_response_wait_time()
+                ):
+                    (contract, order) = (trade.contract, trade.order)
+                    updated_price = round(ticker.midpoint(), 2)
+                    if order.lmtPrice != updated_price:
+                        console.print(
+                            f"[green]Resubmitting order for {contract.symbol}"
+                            f" with old lmtPrice={dfmt(order.lmtPrice)} updated lmtPrice={dfmt(updated_price)}"
+                        )
+                        order.lmtPrice = updated_price
+
+                        if contract.secType == "BAG":
+                            # for some reason, these fields need to be cleared
+                            # when modifying an existing BAG (combo) order
+                            # in-place (janky)
+                            order.algoStrategy = ""
+                            order.algoParams = []
+                            order.tif = ""
+                            order.account = ""
+
+                        # put the trade back from whence it came
+                        self.trades[idx] = self.ib.placeOrder(contract, order)
+                        console.print(f"[blue]Order updated, trade={self.trades[idx]}")
+                else:
+                    console.print(
+                        f"[red]Couldn't get midpoint price for {trade.contract}, skipping"
+                    )
+            except RuntimeError:
+                console.print_exception()
+
+    def wait_for_pending_orders(self):
+        with console.status(
+            f"[bold blue_violet]Waiting for {len(self.trades)} orders to submit..."
+        ) as _status:
+            # Wait for pending orders
+            wait_n_seconds(
+                lambda: any(
+                    [
+                        trade.orderStatus.status in ["PendingSubmit", "PreSubmitted"]
+                        for trade in self.trades
+                        if trade
+                    ]
+                ),
+                lambda remaining: self.ib.waitOnUpdate(timeout=remaining),
+                self.api_response_wait_time(),
+            )
```

### Comparing `thetagang-1.6.1/thetagang/test_util.py` & `thetagang-1.7.0/thetagang/test_util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.1/thetagang/thetagang.py` & `thetagang-1.7.0/thetagang/thetagang.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.1/thetagang/util.py` & `thetagang-1.7.0/thetagang/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 from datetime import datetime
 
-from ib_insync import util
+from ib_insync import TagValue, util
 from ib_insync.contract import Option
 
+from thetagang.options import option_dte
+
 
 def account_summary_to_dict(account_summary):
     d = dict()
     for s in account_summary:
         d[s.tag] = s
     return d
 
@@ -56,23 +58,27 @@
                 ]
             )
         )
 
     return 0
 
 
-def net_option_positions(symbol, portfolio_positions, right):
+def net_option_positions(symbol, portfolio_positions, right, ignore_zero_dte=False):
     if symbol in portfolio_positions:
         return math.floor(
             sum(
                 [
                     p.position
                     for p in portfolio_positions[symbol]
                     if isinstance(p.contract, Option)
                     and p.contract.right.upper().startswith(right.upper())
+                    and (
+                        not ignore_zero_dte
+                        or option_dte(p.contract.lastTradeDateOrContractMonth) > 0
+                    )
                 ]
             )
         )
 
     return 0
 
 
@@ -163,7 +169,11 @@
         p_or_c in config["symbols"][symbol]
         and "write_threshold" in config["symbols"][symbol][p_or_c]
     ):
         return config["symbols"][symbol][p_or_c]["write_threshold"]
     if "write_threshold" in config["symbols"][symbol]:
         return config["symbols"][symbol]["write_threshold"]
     return 0.0
+
+
+def algo_params_from(params):
+    return [TagValue(p[0], p[1]) for p in params]
```

### Comparing `thetagang-1.6.1/PKG-INFO` & `thetagang-1.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: thetagang
-Version: 1.6.1
+Version: 1.7.0
 Summary: ThetaGang is an IBKR bot for getting money
 Home-page: https://github.com/brndnmtthws/thetagang
 License: AGPL-3.0-only
 Author: Brenden Matthews
 Author-email: brenden@brndn.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
-Requires-Dist: ib_insync (>=0.9.81,<0.10.0)
+Requires-Dist: ib_insync (>=0.9.86,<0.10.0)
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Bug Tracker, https://github.com/brndnmtthws/thetagang/issues
 Project-URL: Documentation, https://github.com/brndnmtthws/thetagang/blob/master/README.md
@@ -28,15 +29,15 @@
 
 [![Docker publish](https://github.com/brndnmtthws/thetagang/workflows/Docker%20publish/badge.svg)](https://hub.docker.com/r/brndnmtthws/thetagang) [![Python Publish](https://github.com/brndnmtthws/thetagang/workflows/Python%20Publish/badge.svg)](https://pypi.org/project/thetagang/) [![Docker Pulls](https://img.shields.io/docker/pulls/brndnmtthws/thetagang)](https://hub.docker.com/r/brndnmtthws/thetagang) [![PyPI download month](https://img.shields.io/pypi/dm/thetagang?label=PyPI%20downloads)](https://pypi.python.org/pypi/thetagang/)
 
 [💬 Join the Matrix chat, we can get money together](https://matrix.to/#/#thetagang:frens.io).
 
 # Θ ThetaGang Θ
 
-*Beat the capitalists at their own game with ThetaGang 📈*
+_Beat the capitalists at their own game with ThetaGang 📈_
 
 ![Decay my sweet babies](thetagang.jpg)
 
 ThetaGang is an [IBKR](https://www.interactivebrokers.com/) trading bot for
 collecting premium by selling options using "The Wheel" strategy. The Wheel
 is a strategy that [surfaced on
 Reddit](https://www.reddit.com/r/options/comments/a36k4j/the_wheel_aka_triple_income_strategy_explained/),
@@ -99,45 +100,94 @@
 
 In normal usage, you would run the script as a cronjob on a daily, weekly, or
 monthly basis according to your preferences. Running more frequently than
 daily is not recommended, but the choice is yours.
 
 ![Paper account sample output](sample.png)
 
+### VIX call hedging
+
+ThetaGang can optionally hedge your account by purchasing VIX calls for the
+next month based on specified parameters. The strategy is based on the [Cboe
+VIX Tail Hedge Index](https://www.cboe.com/us/indices/dashboard/vxth/), which
+you can read about on the internet. You can enable this feature in `thetagang.toml` with:
+
+```toml
+[vix_call_hedge]
+enabled = true
+```
+
+Default values are provided, based on the VXTH index, but you may configure
+them to your taste (refer to
+[`thetagang.toml`](https://github.com/brndnmtthws/thetagang/blob/6eab3823120c10c0563e02c5d7f30dfcc0e333fc/thetagang.toml#L294-L331)
+for details).
+
+Buying VIX calls is not free, and it _will_ create some drag on your portfolio,
+but in times of extreme volatility–such as the COVID-related 2020 market
+panic–VIX calls can provide outsized returns.
+
+### Cash management
+
+At the time of writing, interest rates have reached yields that make bonds look
+attractive. To squeeze a little more juice, thetagang can do some simple cash
+management by purchasing a fund when you have extra cash. Although you do earn
+a yield on your cash balance, it's not the juiciest yield you can get, so a
+little optimization might help you earn 1 or 2 extra pennies to take the edge
+off your rent payments.
+
+There are quite a few ETFs that might be a decent place to stash your cash, and
+you should do some internet searches to find the most appropriate one for you
+and your feelings. Here are some internet web searches that you can test out to
+get some information on cash funds (ETFs):
+
+- ["cash etf reddit"](https://www.google.com/search?q=cash+etf+reddit)
+- ["sgov reddit"](https://www.google.com/search?q=sgov+reddit)
+- ["shv reddit"](https://www.google.com/search?q=shv+reddit)
+- ["short term government bond etf reddit"](https://www.google.com/search?q=short+term+government+bond+etf+reddit)
+
+You can enable cash management with:
+
+```toml
+[cash_management]
+enabled = true
+```
+
+Refer to [`thetagang.toml`](https://github.com/brndnmtthws/thetagang/blob/4fc34653786ec17fe6ce6ec2406b2d861277f934/thetagang.toml#L330-L377) for all the options.
+
 ## Project status
 
 This project is, in its current state, considered to be complete. I'm open
 to contributions, but I am unlikely to accept PRs or feature requests that
 involve significant changes to the underlying algorithm.
 
 If you find something that you think is a bug, or some other issue, please
 [create a new issue](https://github.com/brndnmtthws/thetagang/issues/new).
 
 ## "Show me your gains bro" – i.e., what are the returns?
 
-As discussed elsewhere in this README, you must conduct your own research,
-and I suggest starting with resources such as CBOE's BXM and BXDM indices,
-and comparing those to SPX. I've had a lot of people complain because "that
-strategy isn't better than buy and hold BRUH"–let me assure you, that is not
-my goal with this.
+As discussed elsewhere in this README, you must conduct your own research, and
+I suggest starting with resources such as CBOE's BXM and BXDM indices and
+comparing those to SPX. I've had a lot of people complain because "that
+strategy isn't better than buy and hold BRUH"–let me assure you, that is not my
+goal with this.
 
 There are conflicting opinions about whether selling options is good or bad,
-more or less risky, yadda yadda, but generally the risk profile for covered
+more or less risky, yadda yadda, but generally, the risk profile for covered
 calls and naked puts is no worse than the worst case for simply holding an
-ETF or stock. In fact, I'd argue that selling a naked put is better than
+ETF or stock. I'd argue that selling a naked put is better than
 buying SPY with a limit order, because at least if SPY goes to zero you keep
 the premium from selling the option. The main downside is that returns are
 capped on the upside. Depending on your goals, this may not matter. If you're
 like me, then you'd rather have consistent returns and give up a little bit
 of potential upside.
 
 Generally speaking, the point of selling options is not to exceed the returns
 of the underlying, but rather to reduce risk. Reducing risk is an important
 feature because it, in turn, allows one to increase risk in other ways
-(i.e., allocate higher percentage to stocks or buy riskier assets).
+(i.e., allocate a higher percentage to stocks or buy riskier assets).
 
 Whether you use this or not is up to you. I have not one single fuck to give,
 whether you use it or not. I am not here to convince you to use it, I merely
 want to share knowledge and perhaps help create a little bit of wealth
 redistribution.
 
 💫
@@ -161,31 +211,31 @@
 generally avoid low volume ETFs/stocks. If you don't have that kind of
 capital, you'll need to keep renting out your time to the capitalists until
 you can become a capitalist yourself. That's the way the pyramid scheme we
 call capitalism works.
 
 ## Installation
 
-*Before running ThetaGang, you should set up an IBKR paper account to test the
-code.*
+_Before running ThetaGang, you should set up an IBKR paper account to test the
+code._
 
 ```console
-$ pip install thetagang
+pip install thetagang
 ```
 
 It's recommended you familiarize yourself with
 [IBC](https://github.com/IbcAlpha/IBC) so you know how it works. You'll need
 to know how to configure the various knows and settings, and make sure things
 like API ports are configured correctly. If you don't want to mess around too
 much, consider [running ThetaGang with Docker](#running-with-docker).
 
 ## Usage
 
 ```console
-$ thetagang -h
+thetagang -h
 ```
 
 ## Up and running with Docker
 
 My preferred way for running ThetaGang is to use a cronjob to execute Docker
 commands. I've built a Docker image as part of this project, which you can
 use with your installation. There's a [prebuilt Docker image
@@ -198,29 +248,29 @@
 
 The easiest way to get the config files into the container is by mounting a
 volume.
 
 To get started, grab a copy of `thetagang.toml` and `config.ini`:
 
 ```console
-$ mkdir ~/thetagang
-$ cd ~/thetagang
-$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/thetagang.toml -o ./thetagang.toml
-$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/ibc-config.ini -o ./config.ini
+mkdir ~/thetagang
+cd ~/thetagang
+curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/thetagang.toml -o ./thetagang.toml
+curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/ibc-config.ini -o ./config.ini
 ```
 
 Edit `~/thetagang/thetagang.toml` to suit your needs. Pay particular
 attention to the symbols and weights. At a minimum, you must change the
 username, password, and account number. You may also want to change the
 trading move from paper to live when needed.
 
 Now, to run ThetaGang with Docker:
 
 ```console
-$ docker run --rm -i --net host \
+docker run --rm -i --net host \
     -v ~/thetagang:/etc/thetagang \
     brndnmtthws/thetagang:main \
     --config /etc/thetagang/thetagang.toml
 ```
 
 Lastly, to run ThetaGang as a daily cronjob Monday to Friday at 9am, add
 something like this to your crontab (on systems with a cron installation, use
@@ -233,48 +283,46 @@
 ## Determining which ETFs or stocks to run ThetaGang with
 
 I leave this as an exercise to the reader, however I will provide a few
 recommendations and resources:
 
 ### Recommendations
 
-* Stick with high volume ETFs or stocks
-* Careful with margin usage, you'll want to calculate the worst case scenario
+- Stick with high volume ETFs or stocks
+- Careful with margin usage, you'll want to calculate the worst case scenario
   and provide plenty of cushion for yourself based on your portfolio
 
-
 ### Resources
 
-* For discussions about selling options, check out
+- For discussions about selling options, check out
   [r/thetagang](https://www.reddit.com/r/thetagang/)
-* For backtesting portfolios, you can use [this
+- For backtesting portfolios, you can use [this
   tool](https://www.portfoliovisualizer.com/backtest-portfolio) and [this
   tool](https://www.portfoliovisualizer.com/optimize-portfolio) to get an idea
   of drawdown and typical volatility
 
 ## Development
 
 Check out the code to your local machine and install the Python dependencies:
 
-```shell
-$ poetry install
-$ poetry run autohooks activate
-$ poetry run thetagang -h
-...
+```console
+poetry install
+poetry run autohooks activate
+poetry run thetagang -h
 ```
 
 You are now ready to make a splash! 🐳
 
 ## FAQ
 
-| Error                                                                                                      | Cause                                                                                                                            | Resolution                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| Requested market data is not subscribed.                                                                   | Requisite market data subscriptions have not been set up on IBKR.                                                                | [Configure](https://www.interactivebrokers.com/en/software/am3/am/settings/marketdatasubscriptions.htm) your market data subscriptions. The default config that ships with this script uses the `Cboe One Add-On Bundle` and the `US Equity and Options Add-On Streaming Bundle`. **Note**: You _must_ fund your account before IBKR will send data for subscriptions. Without funding you can still subscribe but you will get an error from ibc. |
-| No market data during competing live session                                                               | Your account is logged in somewhere else, such as the IBKR web portal, the desktop app, or even another instance of this script. | Log out of all sessions and then re-run the script.                                                                                                                                                                                                                                                                                                                                                                                                |
-| `ib_insync.wrapper ERROR Error 200, reqId 10: The contract description specified for SYMBOL is ambiguous.` | IBKR needs to know which exchange is the primary exchange for a given symbol.                                                    | You need to specify the primary exchange for the stock. This is normal for companies, typically. For ETFs it usually isn't required. Specify the `primary_exchange` parameter for the symbol, i.e., `primary_exchange = "NYSE"`.                                                                                                                                                                                                                   |
+| Error | Cause | Resolution |
+|---|---|---|
+| Requested market data is not subscribed. | Requisite market data subscriptions have not been set up on IBKR. | [Configure](https://www.interactivebrokers.com/en/software/am3/am/settings/marketdatasubscriptions.htm) your market data subscriptions. The default config that ships with this script uses the `Cboe One Add-On Bundle` and the `US Equity and Options Add-On Streaming Bundle`. **Note**: You _must_ fund your account before IBKR will send data for subscriptions. Without funding you can still subscribe but you will get an error from ibc. |
+| No market data during competing live session | Your account is logged in somewhere else, such as the IBKR web portal, the desktop app, or even another instance of this script. | Log out of all sessions and then re-run the script. |
+| `ib_insync.wrapper ERROR Error 200, reqId 10: The contract description specified for SYMBOL is ambiguous.` | IBKR needs to know which exchange is the primary exchange for a given symbol. | You need to specify the primary exchange for the stock. This is normal for companies, typically. For ETFs it usually isn't required. Specify the `primary_exchange` parameter for the symbol, i.e., `primary_exchange = "NYSE"`. |
 
 ## Support and sponsorship
 
 If you get some value out of this, please consider [sponsoring me](https://github.com/sponsors/brndnmtthws)
 to continue maintaining this project well into the future. Like
 everyone else in the world, I'm just trying to survive.
```

