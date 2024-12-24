---
title: Update net asset 
position_number: 2
type: put
description: /v1/spot/etf/net-asset
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default:
        description: Trading pair, e.g. btc3l_usdt
        ranges:
    -
        name: netAsset
        type: number
        mandatory: true
        default:
        description: net asset
        ranges:
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
                  "msg": "string",
                  "msgInfo": [
                    {}
                  ],
                  "data": {
                  }
                }
        title: Response
        language: json
---

