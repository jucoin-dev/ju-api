---
title: Get Trading Pair Risk Fund Balance
position_number: 20
type: get
description: /market/public/contract/risk-balance
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: 
        description: Trading pair
        ranges:
    -
        name: direction
        type: string
        mandatory: false
        default: NEXT
        description: "Direction（PREV:Previous page；NEXT:Next page）\t"
        ranges: PREV;NEXT
    -
        name: id
        type: integer
        mandatory: false
        default: N/A
        description: id
        ranges:
    -
        name: limit
        type: integer
        mandatory: false
        default: 10
        description: "Limit\t"
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
            "hasNext": false, //Is there a next page
            "hasPrev": false, //Is there a previous page
            "items": [ //Datasheets
              {
                "amount": 0, //Balance
                "coin": "", //Currency
                "createdTime": 0, //Time
                "id": 0 //id
              }
            ]
          },
          "code": 200
        }
      title: Response
      language: json
---