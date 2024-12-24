---
title: Get Depth Data of Trading Pairs
position_number: 10
type: get
description: /v1/future-u/market/public/q/depth
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: Trading pair
        ranges:
    -
        name: level
        type: integer
        mandatory: true
        default: N/A
        description: "Level(min:1,max:50)\t"
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
            "a": [], //Buy
            "b": [], //Sell
            "s": "", //Trading pair
            "t": 0, //Time
            "u": 0 //updateId
          },
          "code": 200
        }
      title: Response
      language: json
---