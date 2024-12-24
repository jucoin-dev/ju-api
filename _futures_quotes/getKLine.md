---
title: Get Trading Pair Information of Kline
position_number: 15
type: get
description: /v1/future-u/market/public/q/kline
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: Trading pair
        ranges:
    -
        name: interval
        type: string
        mandatory: true
        default: N/A
        description: Time-interval
        ranges: 1m;5m;15m;30m;1h;4h;1d;1w
    -
        name: startTime
        type: integer
        mandatory: false
        default: N/A
        description: Start time
        ranges:
    -
        name: endTime
        type: integer
        mandatory: false
        default: N/A
        description: End time
        ranges:
    -
        name: limit
        type: integer
        mandatory: false
        default: N/A
        description: Limit
        ranges:
content_markdown: Note：This method does not require a signature.
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
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
              "a": 0, //Volume
              "c": 0, //Close price
              "h": 0, //Highest price
              "l": 0, //Lowest price
              "o": 0, //Open price
              "s": "", //Trading pair
              "t": 0, //Time
              "v": 0 //Turnover
            }
          ],
          "code": 200
        }
      title: Response
      language: json
---