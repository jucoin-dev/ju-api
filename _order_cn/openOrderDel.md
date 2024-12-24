---
title: 撤销当前挂单
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
        description: 交易对，不传代表所有
        ranges:
    -
        name: bizType
        type: enum
        mandatory: true
        default:
        description: >-
            业务类型  SPOT-现货, LEVER-杠杆
        ranges:
    -
        name: side
        type: enum
        mandatory: false
        default:
        description: BUY-买,SELL-卖
        ranges:
    -
        name: mode
        type: enum
        mandatory: false
        default:
        description: CMD, ITERATOR
        ranges:
content_markdown: >-
    #### **限流规则**

    10/s/apikey
    <br>
    注意：参数以json形式放在body中
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
