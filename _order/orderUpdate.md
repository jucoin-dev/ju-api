---
title: Update Order(Limit)
position_number: 5
type: put
description: /v1/spot/order/{orderId}
parameters:
    -
        name: orderId
        type: number
        mandatory: true
        default:
        description: order ID
        ranges:
    -
        name: price
        type: number
        mandatory: true
        default:
        description: Price
        ranges:
    -
        name: quantity
        type: number
        mandatory: true
        default:
        description: Quantity
        ranges:
    -
        name: clientOrderId
        type: string
        mandatory: false
        default:
        description: client Order Id
        ranges: 
               
content_markdown: >-
  
    #### **Limit Flow Rules**

    50/s/apikey

left_code_blocks:
    -
        code_block: |-
            public String orderPost(){


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
                  "data": {
                    "orderId": "6216559590087220004",   //order id
                    "modifyId": "407329711723834560",    //modify id
                    "clientModifyId": "string"
                  }
                }
        title: Response
        language: json
---
