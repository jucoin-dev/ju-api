---
title: Get available symbol list
position_number: 19
type: get
description: /v1/future-u/ct/public/user/v1/public/copy-trade/symbol-list
parameters:
    
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
                        "data": [string,string] // symbols
                        }
        title: Response
        language: json
---
