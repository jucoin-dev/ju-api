---
title: Get leader future profit total
position_number: 4
type: get
description: /ct/copy-trade/my-profit-history
parameters:
    -
        name: direction
        type: string
        mandatory: false
        default:
        description: direction
        ranges: NEXT,PREV
    -
        name: limit
        type: number
        mandatory: false
        default:
        description: page size
        ranges: 10
    -
       name: id
       type: number
       mandatory: false
       default:
       description: id
       ranges:
content_markdown: >-
    #### **Limit Flow Rules**

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
                        "data": {
                            "hasPrev": false,
                            "hasNext": false,
                             "items": [
                                       {
                                        "avatar": "string", // avatar
                                        "name": "string", // leader name
                                        "profit": 5, // amount
                                        "profitTime": "time", // time
                                        "coin": 0, // currency
                                        "id":  // id
                                        }
                               ]
                        }
                        }
        title: Response
        language: json
---
