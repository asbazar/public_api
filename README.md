# public Api

In This webservice you get AsBazar Exchange public data by open api 

# **Get All Tickers Method:**

* Request Url  : **https://api.asbazar.com/tickers/all**
* Request Type : **GET**
* Signature required : **No**

Output 
<pre><code class="json">[{
    "trading_pairs": "BTC_USDT",
    "base_currency": "BTC",
    "quote_currency": "USDT",
    "last_price": 61988.48,
    "lowest_ask": 0,
    "highest_bid": 0,
    "base_volume": 0,
    "quote_volume": 0,
    "price_change_percent_24h": 1.68,
    "highest_price_24h": 58961.54,
    "lowest_price_24h": 62680.01
  },{
    "trading_pairs": "ASB_USDT",
    "base_currency": "ASB",
    "quote_currency": "USDT",
    "last_price": 0.4739,
    "lowest_ask": 0.4739,
    "highest_bid": 0.4739,
    "base_volume": 157.58514455,
    "quote_volume": 74.6796,
    "price_change_percent_24h": 0,
    "highest_price_24h": 0.4739,
    "lowest_price_24h": 0.4739
  }]</code></pre>
<br>



# **Get Assets Method:**

* Request Url  : **https://api.asbazar.com/assets**
* Request Type : **GET**
* Signature required : **No**
* Filters : **YES** **https://api.asbazar.com/assets/btc**

Output 
<pre><code class="json">{"BTC":{
    "name": "bitcoin",
    "unified_cryptoasset_id": "1",
    "can_withdraw": "true",
    "can_deposit": "true",
    "min_withdraw": "0.001",
    "max_withdraw": "3.23404858090756",
    "maker_fee": "0.04",
    "taker_fee": "0.04"
  },"USDT":{
    "name": "tether usdt",
    "unified_cryptoasset_id": "2",
    "can_withdraw": "true",
    "can_deposit": "true",
    "min_withdraw": "1",
    "max_withdraw": "200000",
    "maker_fee": "0.04",
    "taker_fee": "0.04"
  }}</code></pre>
<br>

