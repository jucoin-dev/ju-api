---
title: Get a single currency asset
position_number: 2
type: get
description: /v1/spot/balance
parameters:
    -
        name: currency
        type: string
        mandatory: true
        default:
        description: eg:usdt
        ranges:
content_markdown:
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
                    "currency": "usdt",  
                    "currencyId": 0,   
                    "frozenAmount": 0,      
                    "freeze": 0,            
                    "lock": 0,              
                    "copyTrade": 0,         
                    "trade": 0,             
                    "withdraw": 0,          
                    "availableAmount": 0,  
                    "totalAmount": 0,    
                    "convertBtcAmount": 0,   //折算BTC数量
                    "convertUsdtAmount": 0   //折算USDT数量
                  }
                }
        title: Response
        language: json
---

