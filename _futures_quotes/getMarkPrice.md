---
title: Get Mark Price for Single Trading Pair
position_number: 13
type: get
description: /market/public/q/symbol-mark-price
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
          "data": {
            "p": 0, //Price
            "s": "", //Trading pair
            "t": 0 //Time
          },
          "code": 200
        }
      title: Response
      language: json
---