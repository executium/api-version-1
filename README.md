![Executium API Version 2](https://i.imgur.com/nn0w8Eo.jpg)

# Executium API Version 2 Documentation
Executium version 2 is currently in private beta mode as we look to launch our new version of executium which has hundreds of new options and an extensive API which can connect with your business. 

## All Official Documentation for Executium
* Announcements regarding changes, upgrades, important exchange information, fixes, etc. to the API and Trading System will be reported here: **UPDATING-URL**
* Endpoints, parameters, payloads, etc. outlined in the documents in this repo are considered **official releases** and **supported by executium**.
* The use of any other endpoints, parameters, or payloads, etc. not outlined in this repo and the documents within are **not supported** and you **use them at your own risk and with no guarantees of functionality**.


Name | Description
------------ | ------------
[rest-api.md](./rest-api.md) | Detailed information on the Executium V2 Rest API (/api/v2)
[errors.md](./errors.md) | Details and descriptions of error messages from the Rest API
[symbols-supported.md](./symbols-supported.md) | Information related to the current supported symbols by executium.
[exchanges-supported.md](./exchanges-supported.md) | Information related to the current supported exchanges by executium.

## Supported Exchanges in Version 2
A table of supported exchanges in executium for version 2. The following table is the status as of 26th July 2020.

Exchange | Executium Code |Active | Symbols Count
------------ | ------------ | ------------ | ------------
Binance|binance|Yes|638
Bitfinex|bitfinex|Yes|305
Bitflyer|bitflyer|Yes|10
Bithumb|bithumb|Yes|104
Bitmart|bitmart|Yes|5
Bitmex|bitmex|Yes|15
Bitstamp|bitstamp|Yes|32
Bittrex|bittrex|Yes|484
Bybit|bybit|Yes|5
Coinbase|coinbase|Yes|169
Coinbasepro|coinbasepro|Yes|74
Coincheck|coincheck|Yes|1
Deribit|deribit|Yes|8
Ftx|ftx|Yes|366
Gateio|gateio|Yes|473
Hbdm|hbdm|Yes|44
Huobipro|huobipro|Yes|573
Indodax|indodax|Yes|68
Itbit|itbit|Yes|6
Kraken|kraken|Yes|155
Kucoin|kucoin|Yes|451
Liquid|liquid|Yes|157
Okex|okex|Yes|386
Poloniex|poloniex|Yes|199
Upbit|upbit|Yes|263



## Supported Symbols in Version 2
We have increased our symbols and exchange support with version 2, as of the 22nd June 2020 (https://executium.com/symbols-exchanges-marketspreads/). 

Version | Exchanges | Markets | Market Spreads | Permutation 
------------ | ------------ | ------------  | ------------   | ------------
Version 2|24|4,924|12,120,426 | 24,240,852
Version 1|12|140|869 | 869

### Quote to Quote Permutation

Quote | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
BTC|1481|2,193,361|Binance, Bitfinex, Bitflyer, Bitmart, Bitmax, Bittrex, Coinbasepro, Ftx, Kucoin, Liquid, Okex, Poloniex, Upbit
ETH|747|558,009|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Kucoin, Liquid, Okex, Poloniex
USDT|1007|1,014,049|Binance, Bitmart, Bitmax, Bittrex, Ftx, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
BNB|80|6,400|Binance, Kucoin
TUSD|22|484|Binance, Kucoin
PAX|25|625|Binance, Bitmart, Bitmax, Kucoin, Poloniex
USDC|69|4,761|Binance, Bitmart, Bitmax, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
TRX|19|361|Binance, Kucoin, Poloniex
BUSD|38|1,444|Binance
NGN|4|16|Binance, Coinbase
RUB|7|49|Binance, Coinbase
TRY|7|49|Binance, Coinbase
EUR|47|2,209|Binance, Bitfinex, Bitflyer, Bittrex, Coinbase, Coinbasepro, Itbit, Liquid
ZAR|6|36|Binance, Coinbase
BKRW|3|9|Binance
IDRT|5|25|Binance, Liquid
USD|529|279,841|Bitfinex, Bitflyer, Bittrex, Coinbase, Coinbasepro, Deribit, Ftx, Itbit, Liquid
JPY|20|400|Bitfinex, Bitflyer, Coinbase, Liquid
GBP|21|441|Bitfinex, Coinbase, Coinbasepro
EOS|3|9|Bitfinex
DAI|14|196|Bitfinex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
UST|19|361|Bitfinex
CNHT|3|9|Bitfinex
USTF0|4|16|Bitfinex
KRW|199|39,601|Bithumb, Coinbase, Upbit
XBT|7|49|Bitmex
CUSTOM1|6|36|Bitmex
AUD|4|16|Coinbase, Liquid
BRL|2|4|Coinbase, Ftx
CHF|6|36|Coinbase, Kraken
HKD|3|9|Coinbase, Liquid
IDR|58|3,364|Coinbase
PHP|2|4|Coinbase, Liquid
SGD|8|64|Coinbase, Itbit, Liquid
XETH|23|529|Kraken
ZEUR|33|1,089|Kraken
ZUSD|35|1,225|Kraken
XXBT|29|841|Kraken
ZGBP|7|49|Kraken
ZCAD|6|36|Kraken
ZJPY|6|36|Kraken
NEO|7|49|Kucoin
KCS|7|49|Kucoin
QASH|18|324|Liquid
USDK|30|900|Okex
OKB|13|169|Okex
USDJ|3|9|Poloniex

We are adding and updating symbols supported by executium daily, the list for [Symbols Supported](./symbols-supported.md) can be monitored. We intend to update this support list weekly with version 2, and for a real-time look at support you can access via the api endpoint `system/symbols` for a full list of support symbols, or keep up to date in real-time via the executium website.


### Pairing Permutation (Exact symbol match)

Base | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
ETHBTC|18|324|Binance, Bitfinex, Bitflyer, Bitmart, Bitmax, Bitstamp, Bittrex, Coinbasepro, Ftx, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
LTCBTC|15|225|Binance, Bitfinex, Bitmax, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
BNBBTC|3|9|Binance, Bitmax, Kucoin
NEOBTC|10|100|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Liquid, Okex, Poloniex
QTUMETH|6|36|Binance, Bittrex, Gateio, Huobipro, Kraken, Okex
EOSETH|10|100|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex
SNTETH|5|25|Binance, Bitfinex, Bittrex, Gateio, Kucoin
BNTETH|3|9|Binance, Bittrex, Gateio
GASBTC|6|36|Binance, Gateio, Huobipro, Kucoin, Okex, Poloniex
BNBETH|2|4|Binance, Bitmax
BTCUSDT|14|196|Binance, Bitfinex, Bitmart, Bitmax, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
ETHUSDT|14|196|Binance, Bitfinex, Bitmart, Bitmax, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
MCOETH|5|25|Binance, Bittrex, Gateio, Huobipro, Okex
MCOBTC|5|25|Binance, Bittrex, Huobipro, Okex, Upbit
WTCBTC|4|16|Binance, Huobipro, Kucoin, Okex
WTCETH|3|9|Binance, Huobipro, Okex
LRCBTC|6|36|Binance, Bitfinex, Bittrex, Gateio, Okex, Upbit
LRCETH|3|9|Binance, Gateio, Okex
QTUMBTC|12|144|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
YOYOWBTC|2|4|Binance, Okex
OMGBTC|12|144|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
OMGETH|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex
ZRXBTC|11|121|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ZRXETH|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
STRATBTC|4|16|Binance, Bittrex, Poloniex, Upbit
STRATETH|2|4|Binance, Bittrex
KNCBTC|7|49|Binance, Bitfinex, Coinbasepro, Huobipro, Kucoin, Okex, Poloniex
KNCETH|4|16|Binance, Gateio, Huobipro, Kucoin
FUNBTC|2|4|Binance, Okex
FUNETH|3|9|Binance, Bitfinex, Gateio
NEOETH|6|36|Binance, Bitfinex, Bitmax, Bittrex, Kucoin, Okex
IOTABTC|6|36|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Okex
IOTAETH|4|16|Binance, Bitfinex, Huobipro, Okex
LINKBTC|7|49|Binance, Bitmax, Bittrex, Huobipro, Kraken, Okex, Poloniex
LINKETH|8|64|Binance, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Okex
XVGBTC|5|25|Binance, Bitfinex, Bittrex, Gateio, Huobipro
XVGETH|2|4|Binance, Huobipro
MDAETH|2|4|Binance, Gateio
MTLBTC|4|16|Binance, Bittrex, Huobipro, Upbit
EOSBTC|12|144|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
SNTBTC|9|81|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ETCETH|7|49|Binance, Bittrex, Gateio, Kraken, Kucoin, Okex, Poloniex
ETCBTC|12|144|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
ENGBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ENGETH|3|9|Binance, Bittrex, Huobipro
DNTBTC|3|9|Binance, Bittrex, Upbit
ZECBTC|12|144|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex
ZECETH|4|16|Binance, Bittrex, Okex, Poloniex
BNTBTC|5|25|Binance, Bittrex, Okex, Poloniex, Upbit
ASTBTC|2|4|Binance, Huobipro
DASHBTC|13|169|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex
DASHETH|4|16|Binance, Bittrex, Kucoin, Okex
OAXBTC|3|9|Binance, Gateio, Liquid
BTGBTC|5|25|Binance, Bitfinex, Gateio, Huobipro, Okex
EVXBTC|2|4|Binance, Huobipro
EVXETH|2|4|Binance, Huobipro
REQBTC|3|9|Binance, Huobipro, Kucoin
VIBBTC|4|16|Binance, Bittrex, Okex, Upbit
VIBETH|2|4|Binance, Bittrex
TRXBTC|11|121|Binance, Bitfinex, Bitmax, Bittrex, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
TRXETH|9|81|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex
POWRBTC|6|36|Binance, Bittrex, Gateio, Huobipro, Kucoin, Upbit
POWRETH|5|25|Binance, Bittrex, Gateio, Huobipro, Kucoin
ARKBTC|4|16|Binance, Bittrex, Okex, Upbit
XRPBTC|15|225|Binance, Bitfinex, Bitmax, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
XRPETH|6|36|Binance, Bitmax, Bittrex, Kraken, Kucoin, Okex
ENJBTC|5|25|Binance, Bittrex, Kucoin, Liquid, Upbit
ENJETH|3|9|Binance, Bittrex, Kucoin
STORJBTC|7|49|Binance, Bittrex, Gateio, Huobipro, Liquid, Poloniex, Upbit
STORJETH|3|9|Binance, Gateio, Okex
BNBUSDT|5|25|Binance, Bitmax, Ftx, Gateio, Kucoin
KMDBTC|5|25|Binance, Bittrex, Huobipro, Liquid, Upbit
KMDETH|2|4|Binance, Huobipro
RCNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
NULSBTC|4|16|Binance, Huobipro, Kucoin, Okex
NULSETH|4|16|Binance, Huobipro, Kucoin, Okex
RDNBTC|2|4|Binance, Huobipro
RDNETH|2|4|Binance, Gateio
XMRBTC|10|100|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex
XMRETH|5|25|Binance, Bittrex, Huobipro, Kucoin, Okex
AMBBTC|2|4|Binance, Kucoin
BATBTC|10|100|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kraken, Okex, Poloniex, Upbit
BATETH|8|64|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Poloniex
BCPTBTC|2|4|Binance, Upbit
ARNETH|2|4|Binance, Gateio
GVTBTC|2|4|Binance, Kucoin
GVTETH|2|4|Binance, Kucoin
CDTETH|2|4|Binance, Gateio
GXSBTC|2|4|Binance, Gateio
NEOUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
QSPBTC|2|4|Binance, Huobipro
QSPETH|2|4|Binance, Gateio
BTSBTC|7|49|Binance, Bittrex, Gateio, Huobipro, Indodax, Poloniex, Upbit
XZCBTC|3|9|Binance, Bittrex, Huobipro
XZCETH|2|4|Binance, Huobipro
LSKBTC|9|81|Binance, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
LSKETH|4|16|Binance, Huobipro, Kraken, Kucoin
TNTBTC|2|4|Binance, Huobipro
TNTETH|2|4|Binance, Gateio
MANABTC|8|64|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Poloniex, Upbit
MANAETH|6|36|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex
BCDBTC|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
BCDETH|2|4|Binance, Kucoin
ADXBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ADXETH|2|4|Binance, Bittrex
ADABTC|9|81|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Upbit
ADAETH|6|36|Binance, Bitmax, Bittrex, Huobipro, Kraken, Okex
PPTBTC|2|4|Binance, Kucoin
PPTETH|2|4|Binance, Kucoin
CMTBTC|3|9|Binance, Huobipro, Okex
CMTETH|3|9|Binance, Huobipro, Okex
XLMBTC|15|225|Binance, Bitfinex, Bitmax, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
XLMETH|8|64|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex
CNDBTC|2|4|Binance, Bittrex
LENDETH|2|4|Binance, Gateio
WABIBTC|2|4|Binance, Liquid
LTCETH|6|36|Binance, Bitmax, Bittrex, Kraken, Kucoin, Okex
LTCUSDT|12|144|Binance, Bitfinex, Bitmax, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
TNBBTC|3|9|Binance, Bitfinex, Huobipro
WAVESBTC|7|49|Binance, Bittrex, Gateio, Huobipro, Kraken, Okex, Upbit
WAVESETH|5|25|Binance, Bittrex, Huobipro, Kraken, Okex
GTOBTC|4|16|Binance, Bittrex, Okex, Upbit
GTOETH|2|4|Binance, Okex
ICXBTC|5|25|Binance, Bittrex, Huobipro, Kraken, Okex
ICXETH|4|16|Binance, Gateio, Huobipro, Kraken
OSTBTC|4|16|Binance, Bittrex, Huobipro, Upbit
OSTETH|2|4|Binance, Gateio
ELFBTC|7|49|Binance, Bitmax, Bittrex, Huobipro, Kucoin, Okex, Upbit
ELFETH|6|36|Binance, Bitmax, Gateio, Huobipro, Kucoin, Okex
AIONBTC|3|9|Binance, Bitfinex, Kucoin
AIONETH|2|4|Binance, Kucoin
NEBLBTC|2|4|Binance, Kucoin
EDOBTC|3|9|Binance, Bitfinex, Okex
EDOETH|2|4|Binance, Bitfinex
NAVBTC|2|4|Binance, Bittrex
LUNBTC|2|4|Binance, Huobipro
APPCBTC|2|4|Binance, Huobipro
RLCBTC|4|16|Binance, Bitfinex, Bittrex, Upbit
RLCETH|2|4|Binance, Gateio
PIVXBTC|3|9|Binance, Bittrex, Kucoin
PIVXETH|2|4|Binance, Kucoin
IOSTBTC|8|64|Binance, Bitfinex, Bitmax, Bittrex, Huobipro, Kucoin, Okex, Upbit
IOSTETH|6|36|Binance, Bitfinex, Bitmax, Huobipro, Kucoin, Okex
STEEMBTC|5|25|Binance, Bittrex, Huobipro, Poloniex, Upbit
STEEMETH|2|4|Binance, Huobipro
NANOBTC|6|36|Binance, Gateio, Huobipro, Kraken, Kucoin, Okex
NANOETH|5|25|Binance, Huobipro, Kraken, Kucoin, Okex
VIABTC|2|4|Binance, Bittrex
BLZBTC|2|4|Binance, Huobipro
BLZETH|3|9|Binance, Gateio, Huobipro
AEBTC|3|9|Binance, Gateio, Huobipro
AEETH|3|9|Binance, Gateio, Huobipro
NCASHETH|2|4|Binance, Huobipro
ZILBTC|7|49|Binance, Bitmax, Bittrex, Huobipro, Kucoin, Okex, Upbit
ZILETH|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
ONTBTC|6|36|Binance, Bitmax, Bittrex, Huobipro, Kucoin, Okex
ONTETH|6|36|Binance, Bitmax, Gateio, Huobipro, Kucoin, Okex
STORMBTC|3|9|Binance, Bittrex, Upbit
STORMETH|2|4|Binance, Bittrex
QTUMUSDT|6|36|Binance, Bitmax, Gateio, Huobipro, Okex, Poloniex
XEMBTC|11|121|Binance, Bitmax, Bittrex, Gateio, Huobipro, Indodax, Kucoin, Liquid, Okex, Poloniex, Upbit
XEMETH|4|16|Binance, Bittrex, Gateio, Okex
WANBTC|4|16|Binance, Bitmax, Huobipro, Kucoin
WANETH|3|9|Binance, Huobipro, Kucoin
WPRBTC|2|4|Binance, Huobipro
QLCBTC|2|4|Binance, Gateio
QLCETH|2|4|Binance, Gateio
SYSBTC|3|9|Binance, Bittrex, Upbit
GRSBTC|4|16|Binance, Bittrex, Huobipro, Upbit
GRSETH|2|4|Binance, Huobipro
ADAUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Upbit
GNTBTC|7|49|Binance, Bitfinex, Bittrex, Huobipro, Okex, Poloniex, Upbit
GNTETH|5|25|Binance, Bitfinex, Bittrex, Gateio, Huobipro
LOOMBTC|6|36|Binance, Bittrex, Huobipro, Kucoin, Poloniex, Upbit
LOOMETH|3|9|Binance, Huobipro, Kucoin
XRPUSDT|10|100|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
REPBTC|7|49|Binance, Bitfinex, Bittrex, Coinbasepro, Kraken, Poloniex, Upbit
REPETH|6|36|Binance, Bitfinex, Bittrex, Gateio, Kraken, Poloniex
BTCTUSD|2|4|Binance, Kucoin
ETHTUSD|2|4|Binance, Kucoin
ZENBTC|4|16|Binance, Bittrex, Huobipro, Okex
ZENETH|3|9|Binance, Huobipro, Okex
EOSUSDT|9|81|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
CVCBTC|7|49|Binance, Bittrex, Huobipro, Kucoin, Okex, Poloniex, Upbit
CVCETH|5|25|Binance, Bittrex, Gateio, Huobipro, Okex
THETABTC|3|9|Binance, Huobipro, Okex
THETAETH|3|9|Binance, Gateio, Huobipro
TUSDUSDT|6|36|Binance, Bitfinex, Bittrex, Gateio, Okex, Upbit
IOTAUSDT|4|16|Binance, Gateio, Huobipro, Okex
XLMUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
IOTXBTC|4|16|Binance, Bittrex, Kucoin, Upbit
IOTXETH|3|9|Binance, Gateio, Kucoin
QKCBTC|3|9|Binance, Gateio, Kucoin
QKCETH|3|9|Binance, Gateio, Kucoin
AGIBTC|2|4|Binance, Kucoin
AGIETH|2|4|Binance, Kucoin
NXSBTC|3|9|Binance, Bittrex, Upbit
DATABTC|2|4|Binance, Bitfinex
DATAETH|3|9|Binance, Bitfinex, Gateio
ONTUSDT|7|49|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex
TRXUSDT|10|100|Binance, Bitmax, Bittrex, Ftx, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ETCUSDT|9|81|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ICXUSDT|3|9|Binance, Gateio, Okex
SCBTC|7|49|Binance, Bittrex, Huobipro, Kraken, Okex, Poloniex, Upbit
SCETH|5|25|Binance, Bittrex, Huobipro, Kraken, Okex
NPXSETH|4|16|Binance, Bittrex, Huobipro, Kucoin
KEYETH|2|4|Binance, Kucoin
NASBTC|4|16|Binance, Gateio, Huobipro, Okex
NASETH|4|16|Binance, Gateio, Huobipro, Okex
DENTETH|2|4|Binance, Kucoin
ARDRBTC|6|36|Binance, Bittrex, Huobipro, Okex, Poloniex, Upbit
NULSUSDT|3|9|Binance, Huobipro, Okex
VETBTC|7|49|Binance, Bitfinex, Bitmax, Bittrex, Huobipro, Kucoin, Upbit
VETETH|4|16|Binance, Gateio, Huobipro, Kucoin
VETUSDT|6|36|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin
DOCKBTC|3|9|Binance, Huobipro, Kucoin
DOCKETH|4|16|Binance, Gateio, Huobipro, Kucoin
POLYBTC|4|16|Binance, Huobipro, Poloniex, Upbit
HCBTC|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
HCETH|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
GOBTC|4|16|Binance, Bittrex, Kucoin, Upbit
PAXUSDT|6|36|Binance, Bitfinex, Bitmax, Gateio, Okex, Poloniex
RVNBTC|5|25|Binance, Bitmax, Bittrex, Okex, Upbit
DCRBTC|8|64|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
MITHBTC|3|9|Binance, Liquid, Okex
BCHBTC|15|225|Binance, Bitfinex, Bitflyer, Bitmax, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
BCHUSDT|12|144|Binance, Bitfinex, Bitmax, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
BTCPAX|7|49|Binance, Bitmart, Bitmax, Bitstamp, Gateio, Kucoin, Poloniex
ETHPAX|4|16|Binance, Bitstamp, Kucoin, Poloniex
XRPPAX|3|9|Binance, Bitstamp, Kucoin
RENBTC|2|4|Binance, Huobipro
XRPTUSD|2|4|Binance, Kucoin
BTCUSDC|10|100|Binance, Bitmart, Bitmax, Coinbasepro, Gateio, Kraken, Kucoin, Liquid, Okex, Poloniex
ETHUSDC|6|36|Binance, Coinbasepro, Kraken, Kucoin, Okex, Poloniex
XRPUSDC|3|9|Binance, Okex, Poloniex
EOSUSDC|3|9|Binance, Okex, Poloniex
USDCUSDT|7|49|Binance, Bitfinex, Bitmax, Bittrex, Gateio, Kraken, Okex
LINKUSDT|8|64|Binance, Bitmax, Bittrex, Ftx, Gateio, Huobipro, Okex, Poloniex
WAVESUSDT|4|16|Binance, Gateio, Huobipro, Okex
BCHUSDC|4|16|Binance, Liquid, Okex, Poloniex
LTCUSDC|3|9|Binance, Okex, Poloniex
TRXUSDC|3|9|Binance, Okex, Poloniex
BTTUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
ONGBTC|2|4|Binance, Bittrex
ONGUSDT|3|9|Binance, Bitmax, Gateio
ZILUSDT|5|25|Binance, Bitmax, Gateio, Huobipro, Okex
ZRXUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Okex, Poloniex, Upbit
FETBTC|3|9|Binance, Bitmax, Kucoin
FETUSDT|2|4|Binance, Bitmax
BATUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Okex, Poloniex, Upbit
XMRUSDT|6|36|Binance, Bittrex, Gateio, Huobipro, Okex, Poloniex
ZECUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
ZECUSDC|3|9|Binance, Coinbasepro, Poloniex
IOSTUSDT|4|16|Binance, Bitmax, Huobipro, Okex
CELRBTC|2|4|Binance, Bitmax
CELRUSDT|3|9|Binance, Bitmax, Gateio
DASHUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
NANOUSDT|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
OMGUSDT|6|36|Binance, Bittrex, Gateio, Huobipro, Okex, Upbit
THETAUSDT|4|16|Binance, Gateio, Huobipro, Okex
ENJUSDT|2|4|Binance, Bittrex
MITHUSDT|3|9|Binance, Gateio, Okex
MATICBTC|3|9|Binance, Bitmax, Poloniex
MATICUSDT|3|9|Binance, Bitmax, Poloniex
ATOMBTC|12|144|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
ATOMUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
ATOMUSDC|2|4|Binance, Poloniex
BATUSDC|2|4|Binance, Coinbasepro
TFUELUSDT|2|4|Binance, Gateio
ONEBTC|4|16|Binance, Bitmax, Huobipro, Kucoin
ONEUSDT|5|25|Binance, Bitmax, Gateio, Huobipro, Kucoin
FTMBTC|3|9|Binance, Bitmax, Kucoin
FTMUSDT|4|16|Binance, Bitmax, Gateio, Okex
ALGOBTC|8|64|Binance, Bitfinex, Bitmax, Bittrex, Huobipro, Kraken, Kucoin, Okex
ALGOUSDT|7|49|Binance, Bitfinex, Bitmax, Gateio, Huobipro, Kucoin, Okex
GTOUSDT|2|4|Binance, Okex
ERDBTC|2|4|Binance, Bitmax
ERDUSDT|2|4|Binance, Bitmax
DOGEBTC|9|81|Binance, Bitmax, Bittrex, Gateio, Huobipro, Indodax, Kraken, Poloniex, Upbit
DOGEUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Okex, Poloniex, Upbit
DUSKBTC|3|9|Binance, Bitfinex, Bittrex
ANKRBTC|5|25|Binance, Bitmax, Bittrex, Kucoin, Upbit
ANKRUSDT|3|9|Binance, Bitmax, Gateio
WINUSDT|4|16|Binance, Gateio, Kucoin, Poloniex
COSUSDT|2|4|Binance, Gateio
NPXSUSDT|2|4|Binance, Bittrex
TOMOBTC|2|4|Binance, Kucoin
TOMOUSDT|3|9|Binance, Gateio, Kucoin
DOCKUSDT|3|9|Binance, Gateio, Huobipro
WANUSDT|2|4|Binance, Bitmax
FUNUSDT|2|4|Binance, Gateio
CVCUSDT|4|16|Binance, Gateio, Huobipro, Okex
BTTTRX|5|25|Binance, Gateio, Huobipro, Kucoin, Poloniex
WINTRX|3|9|Binance, Kucoin, Poloniex
CHZBTC|4|16|Binance, Bitmax, Kucoin, Upbit
CHZUSDT|3|9|Binance, Bitfinex, Bitmax
BANDUSDT|2|4|Binance, Bitmax
BEAMBTC|2|4|Binance, Gateio
BEAMUSDT|2|4|Binance, Gateio
XTZBTC|12|144|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
XTZUSDT|8|64|Binance, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
RENUSDT|2|4|Binance, Huobipro
RVNUSDT|6|36|Binance, Bitmax, Bittrex, Gateio, Okex, Upbit
HCUSDT|4|16|Binance, Gateio, Huobipro, Okex
HBARBTC|4|16|Binance, Bittrex, Liquid, Okex
HBARUSDT|4|16|Binance, Bittrex, Gateio, Okex
NKNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
NKNUSDT|3|9|Binance, Gateio, Huobipro
STXUSDT|2|4|Binance, Gateio
KAVABTC|2|4|Binance, Bitmax
KAVAUSDT|3|9|Binance, Bitmax, Gateio
BTCNGN|2|4|Binance, Coinbase
ARPABTC|2|4|Binance, Huobipro
ARPAUSDT|4|16|Binance, Gateio, Huobipro, Kucoin
IOTXUSDT|2|4|Binance, Gateio
RLCUSDT|2|4|Binance, Gateio
MCOUSDT|3|9|Binance, Gateio, Okex
CTXCBTC|5|25|Binance, Bittrex, Huobipro, Okex, Upbit
CTXCUSDT|3|9|Binance, Huobipro, Okex
BTCRUB|2|4|Binance, Coinbase
VITEBTC|4|16|Binance, Bittrex, Okex, Upbit
FTTBTC|4|16|Binance, Bitmax, Ftx, Huobipro
FTTUSDT|5|25|Binance, Bitfinex, Bitmax, Ftx, Huobipro
BTCTRY|2|4|Binance, Coinbase
BTCEUR|10|100|Binance, Bitfinex, Bitflyer, Bitstamp, Bittrex, Coinbase, Coinbasepro, Itbit, Kraken, Liquid
ETHEUR|8|64|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Itbit, Kraken, Liquid
XRPEUR|5|25|Binance, Bitstamp, Coinbasepro, Kraken, Liquid
OGNBTC|3|9|Binance, Bittrex, Upbit
DREPUSDT|3|9|Binance, Bitmax, Gateio
TCTBTC|2|4|Binance, Okex
TCTUSDT|3|9|Binance, Gateio, Okex
WRXUSDT|2|4|Binance, Ftx
BTSUSDT|3|9|Binance, Gateio, Huobipro
LSKUSDT|4|16|Binance, Gateio, Okex, Poloniex
BNTUSDT|2|4|Binance, Okex
LTOBTC|2|4|Binance, Bitmax
LTOUSDT|2|4|Binance, Bitmax
MBLUSDT|2|4|Binance, Gateio
COTIBTC|3|9|Binance, Bitmax, Kucoin
COTIUSDT|3|9|Binance, Bitmax, Kucoin
STPTBTC|4|16|Binance, Bitmax, Bittrex, Upbit
STPTUSDT|2|4|Binance, Bitmax
BTCZAR|2|4|Binance, Coinbase
WTCUSDT|3|9|Binance, Huobipro, Okex
DATAUSDT|2|4|Binance, Gateio
XZCUSDT|2|4|Binance, Huobipro
BTCIDRT|2|4|Binance, Liquid
HIVEBTC|3|9|Binance, Bittrex, Huobipro
HIVEUSDT|4|16|Binance, Bittrex, Gateio, Huobipro
CHRBTC|4|16|Binance, Bitmax, Bittrex, Kucoin
CHRUSDT|3|9|Binance, Bitmax, Kucoin
GXSUSDT|2|4|Binance, Gateio
BTCUSD|11|121|Bitfinex, Bitflyer, Bitmex, Bitstamp, Bittrex, Coinbase, Coinbasepro, Ftx, Itbit, Kraken, Liquid
LTCUSD|6|36|Bitfinex, Bitstamp, Bittrex, Coinbasepro, Ftx, Kraken
ETHUSD|9|81|Bitfinex, Bitmex, Bitstamp, Bittrex, Coinbasepro, Ftx, Itbit, Kraken, Liquid
ETCUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
ZECUSD|3|9|Bitfinex, Bittrex, Kraken
XMRUSD|2|4|Bitfinex, Kraken
DASHUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
BTCJPY|6|36|Bitfinex, Bitflyer, Coinbase, Coincheck, Kraken, Liquid
XRPUSD|7|49|Bitfinex, Bitmex, Bitstamp, Bittrex, Coinbasepro, Kraken, Liquid
EOSUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
OMGUSD|3|9|Bitfinex, Coinbasepro, Kraken
QTUMUSD|2|4|Bitfinex, Kraken
QASHUSD|2|4|Bitfinex, Liquid
BATUSD|3|9|Bitfinex, Bittrex, Kraken
ZRXUSD|3|9|Bitfinex, Bittrex, Coinbasepro
TNBETH|2|4|Bitfinex, Huobipro
TRXUSD|4|16|Bitfinex, Bittrex, Ftx, Kraken
REPUSD|3|9|Bitfinex, Coinbasepro, Kraken
BTCGBP|5|25|Bitfinex, Bitstamp, Coinbase, Coinbasepro, Kraken
ETHJPY|4|16|Bitfinex, Bitflyer, Kraken, Liquid
ETHGBP|4|16|Bitfinex, Bitstamp, Coinbasepro, Kraken
EOSEUR|3|9|Bitfinex, Coinbasepro, Kraken
WAXPUSD|2|4|Bitfinex, Bittrex
WAXPBTC|5|25|Bitfinex, Bittrex, Huobipro, Kucoin, Upbit
DAIUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
DAIBTC|3|9|Bitfinex, Bittrex, Upbit
DAIETH|2|4|Bitfinex, Bittrex
BFTBTC|4|16|Bitfinex, Bittrex, Huobipro, Upbit
ODEETH|2|4|Bitfinex, Kucoin
ANTBTC|3|9|Bitfinex, Bittrex, Upbit
ANTETH|2|4|Bitfinex, Bittrex
XLMUSD|4|16|Bitfinex, Bitstamp, Coinbasepro, Kraken
XLMEUR|4|16|Bitfinex, Bitstamp, Coinbasepro, Kraken
XLMGBP|2|4|Bitfinex, Bitstamp
MKRUSD|2|4|Bitfinex, Coinbasepro
MKRBTC|6|36|Bitfinex, Coinbasepro, Kucoin, Okex, Poloniex, Upbit
MKRETH|4|16|Bitfinex, Gateio, Kucoin, Okex
KNCUSD|3|9|Bitfinex, Coinbasepro, Ftx
XTZUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
TRXEUR|3|9|Bitfinex, Bittrex, Kraken
MLNUSD|2|4|Bitfinex, Kraken
DGBUSD|2|4|Bitfinex, Bittrex
DGBBTC|6|36|Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Upbit
BSVUSD|2|4|Bitfinex, Bittrex
BSVBTC|9|81|Bitfinex, Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
BCHUSD|7|49|Bitfinex, Bitstamp, Bittrex, Coinbasepro, Ftx, Kraken, Liquid
ENJUSD|2|4|Bitfinex, Bittrex
USDTUSD|4|16|Bitfinex, Bittrex, Ftx, Kraken
USDCUSD|3|9|Bitfinex, Bittrex, Kraken
TUSDUSD|2|4|Bitfinex, Bittrex
PAXUSD|3|9|Bitfinex, Bitstamp, Bittrex
RIFUSD|2|4|Bitfinex, Liquid
RIFBTC|3|9|Bitfinex, Kucoin, Liquid
VSYSBTC|4|16|Bitfinex, Huobipro, Kucoin, Okex
MKRDAI|2|4|Bitfinex, Kucoin
BTTBTC|8|64|Bitfinex, Bitmax, Bittrex, Huobipro, Kucoin, Okex, Poloniex, Upbit
GNOUSD|2|4|Bitfinex, Kraken
ATOMUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
ATOMETH|7|49|Bitfinex, Bitmax, Bittrex, Huobipro, Kraken, Kucoin, Okex
LEOBTC|3|9|Bitfinex, Gateio, Okex
LEOUSDT|3|9|Bitfinex, Gateio, Okex
LEOETH|2|4|Bitfinex, Okex
OKBUSDT|4|16|Bitfinex, Bitmax, Gateio, Okex
OKBBTC|3|9|Bitfinex, Bitmax, Okex
KANUSDT|3|9|Bitfinex, Huobipro, Okex
ALGOUSD|3|9|Bitfinex, Coinbasepro, Kraken
AMPLUSDT|2|4|Bitfinex, Kucoin
AMPLBTC|2|4|Bitfinex, Kucoin
FTTUSD|2|4|Bitfinex, Ftx
XAUTUSD|2|4|Bitfinex, Ftx
XAUTUSDT|2|4|Bitfinex, Ftx
BTCKRW|3|9|Bithumb, Coinbase, Upbit
ETHKRW|2|4|Bithumb, Upbit
LTCKRW|2|4|Bithumb, Upbit
ETCKRW|2|4|Bithumb, Upbit
XRPKRW|2|4|Bithumb, Upbit
BCHKRW|2|4|Bithumb, Upbit
QTUMKRW|2|4|Bithumb, Upbit
BTGKRW|2|4|Bithumb, Upbit
EOSKRW|2|4|Bithumb, Upbit
ICXKRW|2|4|Bithumb, Upbit
TRXKRW|2|4|Bithumb, Upbit
ELFKRW|2|4|Bithumb, Upbit
MCOKRW|2|4|Bithumb, Upbit
OMGKRW|2|4|Bithumb, Upbit
KNCKRW|2|4|Bithumb, Upbit
GNTKRW|2|4|Bithumb, Upbit
ZILKRW|2|4|Bithumb, Upbit
WAXPKRW|2|4|Bithumb, Upbit
POWRKRW|2|4|Bithumb, Upbit
STEEMKRW|2|4|Bithumb, Upbit
STRATKRW|2|4|Bithumb, Upbit
ZRXKRW|2|4|Bithumb, Upbit
REPKRW|2|4|Bithumb, Upbit
XEMKRW|2|4|Bithumb, Upbit
SNTKRW|2|4|Bithumb, Upbit
ADAKRW|2|4|Bithumb, Upbit
BATKRW|2|4|Bithumb, Upbit
THETAKRW|2|4|Bithumb, Upbit
LOOMKRW|2|4|Bithumb, Upbit
WAVESKRW|2|4|Bithumb, Upbit
ENJKRW|2|4|Bithumb, Upbit
VETKRW|2|4|Bithumb, Upbit
MTLKRW|2|4|Bithumb, Upbit
IOSTKRW|2|4|Bithumb, Upbit
QKCKRW|2|4|Bithumb, Upbit
NPXSKRW|2|4|Bithumb, Upbit
BSVKRW|2|4|Bithumb, Upbit
ORBSKRW|2|4|Bithumb, Upbit
ANKRKRW|2|4|Bithumb, Upbit
MBLKRW|2|4|Bithumb, Upbit
XLMKRW|2|4|Bithumb, Upbit
BTTKRW|2|4|Bithumb, Upbit
COSMKRW|2|4|Bithumb, Upbit
LBABTC|5|25|Bitmax, Bittrex, Huobipro, Okex, Upbit
BTMXUSDT|2|4|Bitmax, Gateio
BSVUSDT|7|49|Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
COVABTC|2|4|Bitmax, Huobipro
LAMBBTC|4|16|Bitmax, Bittrex, Huobipro, Upbit
LAMBUSDT|4|16|Bitmax, Gateio, Huobipro, Okex
CVNTBTC|2|4|Bitmax, Huobipro
RNTUSDT|2|4|Bitmax, Okex
AERGOETH|2|4|Bitmax, Kucoin
AERGOBTC|3|9|Bitmax, Kucoin, Upbit
HTETH|2|4|Bitmax, Huobipro
HTUSDT|3|9|Bitmax, Gateio, Huobipro
HTBTC|2|4|Bitmax, Huobipro
BOLTUSDT|2|4|Bitmax, Kucoin
BOLTBTC|2|4|Bitmax, Kucoin
LBAUSDT|4|16|Bitmax, Gateio, Huobipro, Okex
KCSUSDT|2|4|Bitmax, Kucoin
KCSBTC|2|4|Bitmax, Kucoin
MIXUSDT|2|4|Bitmax, Gateio
BHDUSDT|2|4|Bitmax, Huobipro
FSNUSDT|3|9|Bitmax, Huobipro, Okex
ABBCBTC|2|4|Bitmax, Bittrex
ELFUSDT|4|16|Bitmax, Gateio, Huobipro, Okex
GTUSDT|3|9|Bitmax, Gateio, Huobipro
GTBTC|3|9|Bitmax, Gateio, Huobipro
XEMUSDT|5|25|Bitmax, Gateio, Huobipro, Kucoin, Okex
OKBETH|2|4|Bitmax, Okex
HPBBTC|2|4|Bitmax, Kucoin
MHCUSDT|2|4|Bitmax, Kucoin
PROMBTC|2|4|Bitmax, Bittrex
XRPBEARUSDT|3|9|Bitmax, Ftx, Gateio
XRPBULLUSDT|3|9|Bitmax, Ftx, Gateio
BEARUSDT|4|16|Bitmax, Ftx, Gateio, Poloniex
BULLUSDT|4|16|Bitmax, Ftx, Gateio, Poloniex
BTMUSDT|4|16|Bitmax, Gateio, Huobipro, Okex
BTMBTC|7|49|Bitmax, Bittrex, Gateio, Huobipro, Kucoin, Okex, Upbit
CKBUSDT|4|16|Bitmax, Bittrex, Gateio, Huobipro
TOKOUSDT|2|4|Bitmax, Kucoin
XNSUSDT|2|4|Bitmax, Kucoin
XNSBTC|2|4|Bitmax, Kucoin
FLEXBTC|2|4|Bitmax, Liquid
ETHBULLUSDT|4|16|Bitmax, Ftx, Gateio, Poloniex
ETHBEARUSDT|4|16|Bitmax, Ftx, Gateio, Poloniex
LTCBULLUSDT|2|4|Bitmax, Ftx
LTCBEARUSDT|2|4|Bitmax, Ftx
EOSBULLUSDT|3|9|Bitmax, Ftx, Gateio
BNBBEARUSDT|2|4|Bitmax, Ftx
EOSBEARUSDT|3|9|Bitmax, Ftx, Gateio
BNBBULLUSDT|2|4|Bitmax, Ftx
VRAUSDT|2|4|Bitmax, Kucoin
BVOLUSDT|3|9|Bitmax, Ftx, Poloniex
IBVOLUSDT|3|9|Bitmax, Ftx, Poloniex
BEPROUSDT|2|4|Bitmax, Kucoin
GBPUSD|2|4|Bitstamp, Kraken
EURUSD|2|4|Bitstamp, Kraken
XRPGBP|2|4|Bitstamp, Kraken
LTCEUR|3|9|Bitstamp, Coinbasepro, Kraken
LTCGBP|3|9|Bitstamp, Coinbasepro, Kraken
BCHEUR|4|16|Bitstamp, Bittrex, Coinbasepro, Kraken
BCHGBP|3|9|Bitstamp, Coinbasepro, Kraken
ADAUSD|2|4|Bittrex, Kraken
AIDBTC|2|4|Bittrex, Upbit
AKROBTC|3|9|Bittrex, Huobipro, Kucoin
APMBTC|2|4|Bittrex, Okex
APMUSDT|2|4|Bittrex, Okex
BCHETH|3|9|Bittrex, Kraken, Kucoin
BLKBTC|2|4|Bittrex, Upbit
BLOCKBTC|2|4|Bittrex, Upbit
BORABTC|2|4|Bittrex, Upbit
BSVETH|2|4|Bittrex, Kucoin
BTUBTC|2|4|Bittrex, Upbit
BURSTBTC|2|4|Bittrex, Upbit
CKBBTC|3|9|Bittrex, Gateio, Huobipro
CMCTBTC|2|4|Bittrex, Upbit
COSMBTC|2|4|Bittrex, Upbit
CPCBTC|2|4|Bittrex, Kucoin
CROBTC|5|25|Bittrex, Huobipro, Kucoin, Okex, Upbit
CROUSDT|4|16|Bittrex, Gateio, Huobipro, Okex
CRWBTC|2|4|Bittrex, Upbit
CTCBTC|2|4|Bittrex, Okex
CVTBTC|2|4|Bittrex, Okex
DAIUSDT|5|25|Bittrex, Gateio, Kraken, Okex, Poloniex
DCRUSDT|5|25|Bittrex, Gateio, Huobipro, Okex, Upbit
DCTBTC|2|4|Bittrex, Upbit
DENTBTC|4|16|Bittrex, Kucoin, Liquid, Upbit
DGBETH|3|9|Bittrex, Huobipro, Kucoin
DGBUSDT|4|16|Bittrex, Kucoin, Okex, Upbit
DMTBTC|2|4|Bittrex, Upbit
DRGNBTC|2|4|Bittrex, Kucoin
DTABTC|3|9|Bittrex, Huobipro, Upbit
EDRBTC|2|4|Bittrex, Upbit
EMC2BTC|2|4|Bittrex, Upbit
EXPBTC|2|4|Bittrex, Upbit
FCTBTC|3|9|Bittrex, Liquid, Upbit
FSNBTC|4|16|Bittrex, Huobipro, Liquid, Upbit
FXBTC|3|9|Bittrex, Kucoin, Upbit
FXCBTC|2|4|Bittrex, Poloniex
FXETH|2|4|Bittrex, Kucoin
GBYTEBTC|2|4|Bittrex, Upbit
GNOBTC|2|4|Bittrex, Kraken
GNOETH|2|4|Bittrex, Kraken
GRINBTC|4|16|Bittrex, Gateio, Kucoin, Poloniex
GRINUSDT|4|16|Bittrex, Gateio, Kucoin, Poloniex
HBARETH|2|4|Bittrex, Liquid
HBARUSD|2|4|Bittrex, Liquid
HDAOUSDT|2|4|Bittrex, Okex
HYCBTC|2|4|Bittrex, Okex
HYDROBTC|3|9|Bittrex, Liquid, Upbit
IGNISBTC|2|4|Bittrex, Upbit
IONBTC|2|4|Bittrex, Upbit
IRISBTC|2|4|Bittrex, Huobipro
IRISUSDT|2|4|Bittrex, Huobipro
JNTBTC|3|9|Bittrex, Gateio, Upbit
LBCBTC|2|4|Bittrex, Upbit
LINKUSD|4|16|Bittrex, Coinbasepro, Ftx, Kraken
LUNABTC|3|9|Bittrex, Kucoin, Upbit
MDTBTC|3|9|Bittrex, Gateio, Okex
MDTUSDT|3|9|Bittrex, Gateio, Okex
MEDBTC|2|4|Bittrex, Upbit
METABTC|3|9|Bittrex, Kucoin, Upbit
METBTC|2|4|Bittrex, Upbit
MFTBTC|2|4|Bittrex, Upbit
MOCBTC|2|4|Bittrex, Upbit
MOFBTC|2|4|Bittrex, Okex
MOFUSDT|2|4|Bittrex, Okex
NMRBTC|3|9|Bittrex, Poloniex, Upbit
NPXSBTC|4|16|Bittrex, Huobipro, Kucoin, Upbit
NXTBTC|4|16|Bittrex, Indodax, Poloniex, Upbit
OCEANBTC|2|4|Bittrex, Kucoin
ORBSBTC|2|4|Bittrex, Upbit
OXTBTC|2|4|Bittrex, Okex
OXTUSDT|2|4|Bittrex, Okex
PALBTC|2|4|Bittrex, Upbit
PARTBTC|2|4|Bittrex, Upbit
PAXBTC|3|9|Bittrex, Okex, Upbit
PAYBTC|5|25|Bittrex, Gateio, Huobipro, Okex, Upbit
PAYETH|3|9|Bittrex, Gateio, Huobipro
PIBTC|2|4|Bittrex, Upbit
PMABTC|4|16|Bittrex, Liquid, Okex, Upbit
PXLBTC|2|4|Bittrex, Upbit
QNTBTC|2|4|Bittrex, Upbit
QRLBTC|2|4|Bittrex, Upbit
RADSBTC|2|4|Bittrex, Upbit
RDDBTC|2|4|Bittrex, Upbit
RFRBTC|2|4|Bittrex, Upbit
SBDBTC|2|4|Bittrex, Upbit
SCUSD|2|4|Bittrex, Kraken
SCUSDT|4|16|Bittrex, Okex, Poloniex, Upbit
SIXBTC|2|4|Bittrex, Liquid
SOLVEBTC|3|9|Bittrex, Kucoin, Upbit
SPCBTC|2|4|Bittrex, Upbit
SPNDBTC|4|16|Bittrex, Kucoin, Okex, Upbit
SRNBTC|3|9|Bittrex, Huobipro, Upbit
SRNETH|2|4|Bittrex, Huobipro
SXPBTC|2|4|Bittrex, Kucoin
TRACBTC|2|4|Bittrex, Kucoin
TSHPBTC|2|4|Bittrex, Upbit
TTCBTC|2|4|Bittrex, Upbit
TUSDBTC|3|9|Bittrex, Okex, Upbit
UBQBTC|2|4|Bittrex, Upbit
UKGBTC|2|4|Bittrex, Upbit
UPPBTC|2|4|Bittrex, Upbit
USDCBTC|2|4|Bittrex, Okex
USDTEUR|2|4|Bittrex, Kraken
UTKBTC|3|9|Bittrex, Huobipro, Kucoin
VBKBTC|2|4|Bittrex, Upbit
VDXBTC|2|4|Bittrex, Upbit
VEEBTC|2|4|Bittrex, Upbit
VRABTC|2|4|Bittrex, Kucoin
VTCBTC|2|4|Bittrex, Upbit
WAXPETH|3|9|Bittrex, Huobipro, Kucoin
WICCBTC|2|4|Bittrex, Huobipro
WICCUSDT|3|9|Bittrex, Gateio, Huobipro
XDNBTC|2|4|Bittrex, Upbit
XELBTC|2|4|Bittrex, Upbit
XTZETH|4|16|Bittrex, Gateio, Huobipro, Kraken
XUCUSDT|2|4|Bittrex, Okex
XVGUSDT|2|4|Bittrex, Gateio
YOUBTC|2|4|Bittrex, Okex
BTCAUD|2|4|Coinbase, Liquid
BTCBRL|2|4|Coinbase, Ftx
BTCCAD|2|4|Coinbase, Kraken
BTCCHF|2|4|Coinbase, Kraken
BTCHKD|2|4|Coinbase, Liquid
BTCIDR|2|4|Coinbase, Indodax
BTCSGD|3|9|Coinbase, Itbit, Liquid
ETCEUR|2|4|Coinbasepro, Kraken
ETHDAI|6|36|Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
COMPUSD|2|4|Coinbasepro, Ftx
OMGEUR|2|4|Coinbasepro, Kraken
KNCUSDT|3|9|Ftx, Gateio, Okex
PAXGUSD|2|4|Ftx, Kraken
BCHBEARUSDT|2|4|Ftx, Poloniex
BCHBULLUSDT|2|4|Ftx, Poloniex
BSVBEARUSDT|2|4|Ftx, Poloniex
BSVBULLUSDT|2|4|Ftx, Poloniex
SNTUSDT|3|9|Gateio, Huobipro, Okex
PAYUSDT|2|4|Gateio, Okex
PSTUSDT|2|4|Gateio, Okex
BTGUSDT|2|4|Gateio, Okex
LRCUSDT|2|4|Gateio, Okex
STORJUSDT|3|9|Gateio, Huobipro, Okex
AEUSDT|2|4|Gateio, Huobipro
REQETH|3|9|Gateio, Huobipro, Kucoin
MDAUSDT|2|4|Gateio, Okex
GNTUSDT|4|16|Gateio, Huobipro, Okex, Poloniex
ABTUSDT|2|4|Gateio, Okex
ABTETH|3|9|Gateio, Huobipro, Okex
OCNUSDT|2|4|Gateio, Huobipro
OCNETH|2|4|Gateio, Huobipro
OCNBTC|2|4|Gateio, Huobipro
COFIETH|2|4|Gateio, Kucoin
MTNETH|3|9|Gateio, Huobipro, Kucoin
RUFFUSDT|2|4|Gateio, Huobipro
RUFFETH|2|4|Gateio, Huobipro
RUFFBTC|2|4|Gateio, Huobipro
MKRUSDT|3|9|Gateio, Okex, Poloniex
SMTUSDT|2|4|Gateio, Huobipro
SMTETH|2|4|Gateio, Huobipro
MDTETH|2|4|Gateio, Okex
MANAUSDT|4|16|Gateio, Huobipro, Okex, Poloniex
LUNETH|2|4|Gateio, Huobipro
DRGNETH|2|4|Gateio, Kucoin
GTCETH|2|4|Gateio, Huobipro
GTCBTC|2|4|Gateio, Huobipro
DBCBTC|3|9|Gateio, Huobipro, Kucoin
DBCETH|3|9|Gateio, Huobipro, Kucoin
BIFIBTC|2|4|Gateio, Huobipro
MDSETH|2|4|Gateio, Huobipro
MDSUSDT|2|4|Gateio, Huobipro
DGDETH|2|4|Gateio, Huobipro
QASHETH|3|9|Gateio, Huobipro, Liquid
QASHBTC|3|9|Gateio, Huobipro, Liquid
BCDUSDT|2|4|Gateio, Okex
SBTCBTC|3|9|Gateio, Huobipro, Okex
BCXBTC|3|9|Gateio, Huobipro, Okex
GNXETH|3|9|Gateio, Huobipro, Okex
GASUSDT|2|4|Gateio, Okex
NASUSDT|3|9|Gateio, Huobipro, Okex
BTMETH|4|16|Gateio, Huobipro, Kucoin, Okex
RSRUSDT|2|4|Gateio, Huobipro
BUETH|2|4|Gateio, Kucoin
BUBTC|2|4|Gateio, Kucoin
BCNUSDT|2|4|Gateio, Poloniex
BCNBTC|2|4|Gateio, Poloniex
STEEMUSDT|3|9|Gateio, Huobipro, Poloniex
ATPUSDT|2|4|Gateio, Huobipro
KLAYUSDT|2|4|Gateio, Liquid
GRINETH|2|4|Gateio, Kucoin
BTTETH|4|16|Gateio, Huobipro, Kucoin, Okex
CSETH|2|4|Gateio, Kucoin
MANETH|3|9|Gateio, Huobipro, Kucoin
LYMETH|3|9|Gateio, Huobipro, Kucoin
LYMBTC|3|9|Gateio, Huobipro, Kucoin
LYMUSDT|2|4|Gateio, Kucoin
BFTETH|2|4|Gateio, Huobipro
TOMOETH|2|4|Gateio, Kucoin
SOULETH|2|4|Gateio, Kucoin
HITUSDT|2|4|Gateio, Huobipro
HITETH|2|4|Gateio, Huobipro
DXETH|2|4|Gateio, Kucoin
CNNSUSDT|2|4|Gateio, Huobipro
LAMBETH|2|4|Gateio, Huobipro
WICCETH|2|4|Gateio, Huobipro
VIDYUSDT|2|4|Gateio, Huobipro
FTMETH|2|4|Gateio, Kucoin
MTVUSDT|2|4|Gateio, Kucoin
FTIETH|2|4|Gateio, Huobipro
LBAETH|2|4|Gateio, Huobipro
OPENETH|2|4|Gateio, Kucoin
MITHETH|2|4|Gateio, Okex
SKMUSDT|2|4|Gateio, Huobipro
MXCBTC|2|4|Gateio, Huobipro
AKROUSDT|2|4|Huobipro, Kucoin
KANBTC|2|4|Huobipro, Okex
AACBTC|2|4|Huobipro, Okex
KCASHBTC|2|4|Huobipro, Okex
GNXBTC|2|4|Huobipro, Okex
WXTUSDT|3|9|Huobipro, Kucoin, Okex
AACETH|2|4|Huobipro, Okex
DATXBTC|2|4|Huobipro, Kucoin
UTKETH|2|4|Huobipro, Kucoin
TRIOBTC|2|4|Huobipro, Okex
DATXETH|2|4|Huobipro, Kucoin
KANETH|2|4|Huobipro, Okex
WXTBTC|3|9|Huobipro, Kucoin, Okex
EMUSDT|2|4|Huobipro, Okex
TRIOETH|2|4|Huobipro, Okex
LETUSDT|2|4|Huobipro, Okex
OGOUSDT|2|4|Huobipro, Kucoin
ELAETH|2|4|Huobipro, Kucoin
ABTBTC|2|4|Huobipro, Okex
SNCBTC|2|4|Huobipro, Okex
FAIRETH|2|4|Huobipro, Okex
OGOBTC|2|4|Huobipro, Kucoin
SWFTCETH|2|4|Huobipro, Okex
CMTUSDT|2|4|Huobipro, Okex
CTXCETH|2|4|Huobipro, Okex
ETNBTC|3|9|Huobipro, Kucoin, Liquid
TOPCETH|2|4|Huobipro, Okex
VSYSUSDT|3|9|Huobipro, Kucoin, Okex
NCASHBTC|2|4|Huobipro, Upbit
ETNETH|3|9|Huobipro, Kucoin, Liquid
ACTBTC|3|9|Huobipro, Kucoin, Okex
ACTETH|2|4|Huobipro, Kucoin
ITCETH|2|4|Huobipro, Kucoin
ACTUSDT|2|4|Huobipro, Okex
DCRETH|3|9|Huobipro, Kucoin, Okex
ALGOETH|4|16|Huobipro, Kraken, Kucoin, Okex
ITCBTC|3|9|Huobipro, Kucoin, Okex
EGTUSDT|2|4|Huobipro, Okex
QUNBTC|2|4|Huobipro, Okex
MANBTC|2|4|Huobipro, Kucoin
CHATBTC|2|4|Huobipro, Okex
ITCUSDT|3|9|Huobipro, Kucoin, Okex
SOCUSDT|2|4|Huobipro, Okex
GASETH|2|4|Huobipro, Okex
ELABTC|2|4|Huobipro, Kucoin
MTNBTC|2|4|Huobipro, Kucoin
SOCBTC|2|4|Huobipro, Okex
SWFTCBTC|3|9|Huobipro, Okex, Poloniex
LETBTC|2|4|Huobipro, Okex
EGTBTC|3|9|Huobipro, Kucoin, Okex
KCASHETH|2|4|Huobipro, Okex
ETHSGD|2|4|Itbit, Liquid
BTCDAI|5|25|Kraken, Kucoin, Liquid, Okex, Poloniex
XRPJPY|2|4|Kraken, Liquid
SNXUSDT|2|4|Kucoin, Poloniex
SNXBTC|3|9|Kucoin, Liquid, Poloniex
EGTETH|2|4|Kucoin, Okex
CRPTETH|2|4|Kucoin, Liquid
MTCBTC|2|4|Kucoin, Liquid
CRPTBTC|2|4|Kucoin, Liquid
USDTUSDC|2|4|Kucoin, Poloniex
BLOCUSDT|2|4|Kucoin, Okex
ROOBEEBTC|2|4|Kucoin, Liquid
ROADUSDT|2|4|Kucoin, Okex
XNKBTC|2|4|Liquid, Upbit
SWFTCUSDT|2|4|Okex, Poloniex
ETCUSDC|2|4|Okex, Poloniex
BSVUSDC|2|4|Okex, Poloniex

This brings a total possible exact matching permutation count of `14,328`.
