---
title: Create Stop Limit
position_number: 7
type: post
description: /trade/entrust/create-profit
remark: Content-Type = application/x-www-form-urlencoded && application/json
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: Trading pair
        ranges:
    -
        name: origQty
        type: integer
        mandatory: true
        default:
        description: Quantity (Cont)
        ranges:
    -
        name: triggerProfitPrice
        type: integer
        mandatory: true
        default:
        description: TP trigger price
        ranges:
    -
        name: triggerStopPrice
        type: integer
        mandatory: true
        default:
        description: SL trigger price
        ranges:
    -
        name: expireTime
        type: integer
        mandatory: true
        default:
        description: Expiration time
        ranges:
    -
        name: positionSide
        type: string
        mandatory: true
        default:
        description: Position side:LONG;SHORT
        ranges: LONG;SHORT
        
content_markdown: |-

                  #### **Limit Flow Rules**

                  200/s/apikey
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/future-u/trade/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
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
            "data": {},
            "code": 200
        }
        title: Response
        language: json
---