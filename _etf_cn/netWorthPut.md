---
title: 净值更新
position_number: 1
type: put
description: /v1/spot/etf/net-worth
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default:
        description: 交易对，例如：btc3l_usdt
        ranges:
    -
        name: netWorth
        type: number
        mandatory: true
        default:
        description: 更新的净值
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

