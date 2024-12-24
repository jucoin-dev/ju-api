---
title: Get depth data
position_number: 4
type: get
split: -------------------------------------
description: /v1/spot/public/depth
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default:
        description: trading pair  eg:btc_usdt
        ranges:
    -
        name: limit
        type: number
        mandatory: false
        default: '50'
        description: 
        ranges: 1~1000
content_markdown: >-
    #### **Limit Flow Rules**
    
    1/s/ip


left_code_blocks:
    -
        code_block: |-
            public String depth(){


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
                  "msg": "SUCCESS",
                  "msgInfo": [],
                  "data": {
                    "timestamp": 1662445330524,  
                    "lastUpdateId": 137333589606963580,     //Last updated record
                    "bids": [                               //buy order([?][0]=price;[?][1]=pending order volume)
                      [
                        "200.0000",                         //price
                        "0.996000"                          //pending order volume
                      ],
                      [
                        "100.0000",
                        "0.001000"
                      ],
                      [
                        "20.0000",
                        "10.000000"
                      ]
                    ],
                    "asks": []                              //sell order([?][0]=price;[?][1]=pending order volume)
                  }
                }
        title: Response
        language: json
---
