---
title: Get a list of currency assets
position_number: 3
type: get
split: -------------------------------------
description: /v1/spot/balances
parameters:
    -
        name: currencies
        type: string
        mandatory: false
        default:
        description: 'List of currencies, comma separated,eg:  usdt,btc'
        ranges:
    -
        name: queryAccountId
        type: long
        mandatory: false
        default:
        description: 
        ranges:
    -
        name: filterIsDisplayFalse
        type: boolean
        mandatory: false
        default: true
        description:
        ranges:
content_markdown: >-
    #### **Limit Flow Rules**

    10/s/apikey
left_code_blocks:
    -
        code_block:
        title: Java
        language: java
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: |-
                {
                  "code": 200,
                  "msg": "string",
                  "msgInfo": [
                    {}
                  ],
                  "data": {
                    "totalBtcAmount": 0,
                    "totalUsdtAmount": 0,
                    "assets": [    
                      {        
                        "currency": "string",
                        "currencyId": 0,
                        "frozenAmount": 0,      
                        "freeze": 0,            
                        "lock": 0,              
                        "copyTrade": 0,         
                        "trade": 0,            
                        "withdraw": 0,         
                        "availableAmount": 0,
                        "totalAmount": 0,
                        "convertBtcAmount": 0,
                        "convertUsdtAmount": 0   
                      }
                    ]
                  }
                }
        title: Response
        language: json
---

