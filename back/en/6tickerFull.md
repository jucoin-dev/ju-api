---
title: Get complete ticker
position_number: 6
type: get
description: /v1/spot/public/ticker
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default:
        description: trading pair  eg:btc_usdt
        ranges:
    -
        name: symbols
        type: array
        mandatory: false
        default:
        description: 'Collection of trading pairs. Priority is higher than symbol. eg: btc_usdt,eth_usdt'
        ranges:
    -
        name: tags
        type: array
        mandatory: false
        default:
        description: '标签集合'
        ranges:
content_markdown:
left_code_blocks:
    -
        code_block: |-
            public String full(){


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
            "data": [
              {
                "s": "btc_usdt",        //symbol
                "t": 1662444879425,     //time
                "cv": "0.00",           //change value
                "cr": "0.0000",         //change rate
                "o": "200.00",          //open
                "l": "200.00",          //low
                "h": "200.00",          //high
                "c": "200.00",          //close
                "q": "0.002",           //quantity
                "v": "0.40",            //volume
                "ap": null,             //asks price
                "aq": null,             //asks qty
                "bp": null,             //bids price
                "bq": null              //bids qty
              }
            ]
          }
        title: Response
        language: json
---
