---
title: Get loan list
position_number: 2
type: get
split: -------------------------------------
description: /v1/spot/lever/loan
parameters:
  -
    name: symbol
    type: string
    mandatory: false
    default:
    description:
    ranges:
  -
    name: startTime
    type: long
    mandatory: false
    default:
    description: start time
    ranges:
  -
    name: endTime
    type: long
    mandatory: false
    default:
    description: end time
    ranges:
  -
    name: fromId
    type: long
    mandatory: false
    default:
    description: page from id
    ranges:
  -
    name: direction
    type: enum
    mandatory: false
    default:
    description: page direction  NEXT/PREV
    ranges:
  -
    name: limit
    type: int
    mandatory: false
    default: 20
    description: page limit
    ranges: 1-100
  
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
                  "msg": "SUCCESS",
                  "msgInfo": [{}],
                  "data": {
                      "hasNext": true,               //whether has next page
                      "hasPrev": true,               //whether has previous page
                      "items":[{
                           "id": "string",           //id
                           "amount": 0,              //amount
                           "currency": "string",     //currency
                           "currencyId": 0,          //currency id
                           "symbol": "string",       //symbol
                           "symbolId": 0,            //symbol id
                           "createTime": 0           //create time
                      }]
                  }
                }
        title: Response
        language: json
---
