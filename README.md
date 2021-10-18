# public Api

In This webservice you get AsBazar Exchange public data by open api 

# **Get All Tickers Method:**

The summary endpoint is to provide an overview of market data for all tickers and all market pairs on the exchange.

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

The assets endpoint is to provide a detailed summary for each currency available on the exchange.

* Request Url  : **https://api.asbazar.com/assets**
* Request Type : **GET**
* Signature required : **No**
* Filters : **YES**  ||  **https://api.asbazar.com/assets/btc**

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



# **Get Ticker Method:**

The ticker endpoint is to provide a 24-hour pricing and volume summary for each market pair available on the exchange.

* Request Url  : **https://api.asbazar.com/ticker**
* Request Type : **GET**
* Signature required : **No**
* Filters : **YES**  ||  **https://api.asbazar.com/ticker/btc**

Output 
<pre><code class="json">{"BTC_USDT":{
    "base_id": "1",
    "quote_id": "2",
    "last_price": "61389.34",
    "base_volume": "0",
    "quote_volume": "0",
    "isFrozen": "0"
  },"ASB_USDT":{
    "base_id": "4",
    "quote_id": "2",
    "last_price": "0.4739",
    "base_volume": "157.58514455",
    "quote_volume": "74.6796",
    "isFrozen": "0"
  }}</code></pre>
<br>



# **Get OrderBook Method:**

The order book endpoint is to provide a complete level 2 order book (arranged by best asks/bids) with full depth returned for a given market pair.

* Request Url  : **https://api.asbazar.com/orderbook/{Market_Pair}**
* Request Type : **GET**
* Signature required : **No**
* Filters : **YES**  ||  **https://api.asbazar.com/orderbook/btc_usdt**

Output 
<pre><code class="json">{  
   "timestamp":"1634592347000",
   "bids":[[  
         "0.0000321",
         "100365.76323988"
      ],[  
         "0.000049",
         "3633896.04"
      ],[  
         "0.000049",
         "243001.037464"
      ]],
   "asks":[[  
         "0.0000321",
         "100365.76323988"
      ],[  
         "0.000049",
         "3633896.04"
      ],[  
         "0.000049",
         "243001.037464"
      ]]}</code></pre>
<br>



# **Get Last Trade Method:**

The trades endpoint is to return data on all recently completed trades for a given market pair.

* Request Url  : **https://api.asbazar.com/trades/{Market_Pair}**
* Request Type : **GET**
* Signature required : **No**
* Filters : **YES**  ||  **https://api.asbazar.com/trades/btc_usdt**

Output 
<pre><code class="json">[   
   {         
      "trade_id":3523643,
      "price":"0.01",
      "base_volume":"569000",
      "quote_volume":"0.01000000",
      "timestamp":"‭1585177482652‬",
      "type":"sell"
   }
]</code></pre>
<br>
