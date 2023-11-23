# TAU Protocol MVP API Requirements

## Endpoints

### 1. Get Tickers

- **Endpoint**: `GET https://arbitrum-api.gmxinfra.io/prices/tickers`
- **Response**:

  ```json
  [
    {
      "tokenAddress": "0x82aF49447D8a07e3bd95BD0d56f35241523fBab1",
      "tokenSymbol": "ETH",
      "minPrice": "2054852954650000",
      "maxPrice": "2055006248570000",
      "updatedAt": 1700700106887
    }
    ...
  ]
  ```

### 2. Get Candles

- **Endpoint**: `GET https://arbitrum-api.gmxinfra2.io/prices/candles?limit=5000&period=5m&tokenSymbol=ARB`
- **Response**:

  ```json
  {
    "period": "5m",
    "candles": [
      [1700700000, 1.0160913900000001, 1.0167, 1.0152305, 1.015748465],
      ...
    ]
  }
  ```

### 3. Get 24 Hour Prices

- **Endpoint**: `GET https://arbitrum-api.gmxinfra2.io/prices/24h`
- **Response**:

  ```json
  [
    {
      "tokenSymbol": "ARB",
      "high": 1.03619934,
      "low": 0.96294081,
      "open": 0.964295575,
      "close": 1.015723855
    },
    {
      "tokenSymbol": "BTC",
      "high": 37860.87873864,
      "low": 35985.39393133,
      "open": 36028.13593401,
      "close": 37330.938518455005
    }
    ...
  ]
  ```
