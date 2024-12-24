---
title: Cancell order by query param
position_number: 3
type: delete
split: -------------------------------------
description: /v1/spot/order
parameters:
    -
        name: orderId
        type: number
        mandatory: true
        default:
        description: 
        ranges:
content_markdown:
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
        code_block:  |-
                 {
                    "code": 200,
                    "msg": "string",
                    "msgInfo": [
                      {}
                    ],
                    "data": {
                        "orderId": "123",
                        "cancelId": "0",
                        "clientCancelId": "123"
                    }
                 }
        title: Response
        language: json
---
