---
title: Query the list of recent transactions
position_number: 6
type: get
description: /v1/spot/public/trade/recent
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default:
        description: trading pair
        ranges:
    -
        name: limit
        type: number
        mandatory: false
        default: '200'
        description: 
        ranges: 1，1000
content_markdown: >-
    #### **Limit Flow Rules**
    
    10/s/ip

left_code_blocks:
    -
        code_block: |-
            public String tradeRecent(){


            }
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
                  "data": [
                    {
                      "i": 0,           //ID
                      "t": 0,           //transaction time
                      "p": "string",    //transaction price
                      "q": "string",    //transaction quantity
                      "v": "string",    //transaction volume
                      "b": true         //whether is buyerMaker or not
                    }
                  ]
                }
        title: Response
        language: json
---
