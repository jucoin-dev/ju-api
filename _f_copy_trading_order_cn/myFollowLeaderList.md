---
title: 我跟随的交易员列表(当前跟随)
position_number: 17
type: get
description: /v1/future-u/ct/copy-trade/my-follow-list
parameters:
    
content_markdown: >-
    #### **限流规则**

    2/s/apikey
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
                        "data": [number,number] //交易员accountId
                        }
        title: Response
        language: json
---
