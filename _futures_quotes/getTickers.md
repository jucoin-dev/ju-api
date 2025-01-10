---
title: Get Market Information for All Trading Pairs
position_number: 8
type: get
description: /market/public/q/tickers
parameters:
content_markdown: Note：This method does not require a signature.
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/future-u/market/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    - code_block: |-
        {
         "msgInfo": {
            "code": "",
            "msg": ""
          },
          "msg": "",
          "data": [
            {
              "a": "", //24h volume
              "c": "", //Latest price
              "h": "", //Highest price in 24 hours
              "l": "", //Lowest price in 24 hours
              "o": "", //The first transaction price 24 hours ago
              "r": "", //24h Price Fluctuation Limit
              "s": "", //Trading pair
              "t": 0, //Time
              "v": "" //24h turnover
            }
          ],
          "code": 200
        }
      title: Response
      language: json
---