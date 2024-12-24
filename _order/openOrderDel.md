---
title: Cancel the current pending order
position_number: 9
type: delete
split: -------------------------------------
description: /v1/spot/open-order
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default:
        description: Trading pair, if not filled in, represents all
        ranges:
    -
        name: bizType
        type: enum
        mandatory: true
        default:
        description: "SPOT, LEVER"
        ranges:
    -
        name: side
        type: enum
        mandatory: false
        default:
        description: BUY,SELL
        ranges:
    -
        name: mode
        type: enum
        mandatory: false
        default:
        description: CMD, ITERATOR
        ranges:
content_markdown: >-
    #### **Limit Flow Rules**

    10/s/apikey
    <br>
    Note: The parameters should be placed in the request body in the form of json
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
                  "data": {}
                }
        title: Response
        language: json
---
