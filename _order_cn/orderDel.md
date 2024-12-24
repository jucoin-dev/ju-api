---
title: 单笔撤单
position_number: 3
type: delete
split: -------------------------------------
description: /v1/spot/order/{orderId}
parameters:
    -
        name: orderId
        type: number
        mandatory: true
        default:
        description: 订单ID
        ranges:
content_markdown: >-

left_code_blocks:
    -
        code_block: |-
            public String orderDel(){


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
                    "cancelId": "6216559590087220004",
                    "orderId": "string",
                    "clientCancelId": "string"
                  }
                }
        title: Response
        language: json
---
