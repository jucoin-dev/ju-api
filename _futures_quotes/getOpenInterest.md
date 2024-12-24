---
title: Get the open position of a trading pair
position_number: 21
type: get
description: /v1/future-u/market/public/contract/open-interest
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: Trading pair
        ranges:
content_markdown: >-

  #### **Limit Flow Rules**

  1/s/ip
  <br>
  Note：This method does not require a signature.
  
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
            "symbol": "", //Trading pair
            "openInterest": "", //open position
            "openInterestUsd": 0, //open value
            "time": "", //time
          },
          "code": 200
        }
      title: Response
      language: json
---