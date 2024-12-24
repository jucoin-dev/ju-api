---
title: Close all orders
position_number: 11
type: post
description: /v1/future-u/ct/copy-trade/close-all  	
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default:
        description: symbol
        ranges:
    -
        name: closeLongShortType
        type: string
        mandatory: false
        default:
        description: direction
        ranges: LONG,SHORT,BOTH
content_markdown: >-
    #### **Limit Flow Rules**

    5/s/apikey
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
                        "data": Boolean //true=success false=fail
                        }
        title: Response
        language: json
---
