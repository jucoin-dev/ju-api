---
title: Get Ask Bid Market Information for Specific Trading Pair
position_number: 18
type: get
description: /v1/future-u/market/public/q/ticker/book
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: Trading pair
        ranges:
content_markdown: Note：This method does not require a signature.
left_code_blocks:
    -
        code_block: "public void getTickerBokk() {\r\n\tString text = HttpUtil.get(URL + \"/data/api//v1/future-u/market/public/q/ticker/book?symbol=btc_usdt\");\r\n\tSystem.out.println(text);\r\n}"
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
        "data": {
          "ap": "", //ask price
          "aq": "", //ask amount
          "bp": "", //bid price
          "bq": "", //bid amount
          "s": "", //Trading pair
          "t": 0 //Time
        },
        "code": 200
      }
    title: Response
    language: json
---
