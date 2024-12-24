---
title: Public get leader day income
position_number: 23
type: get
description: /v1/future-u/ct/public/user/v1/public/copy-trade/leader-day-income
parameters:
   -
        name: accountId
        type: number
        mandatory: true
        default:
        description: leader accountId
        ranges:
   -
        name: days
        type: number
        mandatory: false
        default:
        description: days
        ranges:

content_markdown: >-
    #### **Limit Flow Rules**

    2/s/ip
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
                        "msg": "success",
                        "msgInfo": null,
                        "data": [
                                {
                                "amount": 0, // amount
                                "time": 0 // time
                                }
                        ]
                        }
        title: Response
        language: json
---
