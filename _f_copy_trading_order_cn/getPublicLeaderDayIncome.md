---
title: 获取交易员收益额图表
position_number: 23
type: get
description: /ct/public/user/v1/public/copy-trade/leader-day-income
parameters:
   -
        name: accountId
        type: number
        mandatory: true
        default:
        description: 交易员帐号
        ranges:
   -
        name: days
        type: number
        mandatory: false
        default:
        description: 天数
        ranges:

content_markdown: >-
    #### **限流规则**

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
                                "amount": 0, // 收益额
                                "time": 0 // 时间
                                }
                        ]
                        }
        title: Response
        language: json
---
