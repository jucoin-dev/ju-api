---
title: 获取币种资产列表
position_number: 3
type: get
split: -------------------------------------
description: /v1/spot/balances
parameters:
    -
        name: currencies
        type: string
        mandatory: false
        default:
        description: '币种列表,逗号分隔，eg:  usdt,btc'
        ranges:
    -
        name: queryAccountId
        type: long
        mandatory: false
        default:
        description: '查询账户id不传递的话默认使用当前账户id'
        ranges:
    -
        name: filterIsDisplayFalse
        type: boolean
        mandatory: false
        default: true
        description: 
        ranges:
content_markdown: >-
    #### **限流规则**

    10/s/apikey
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
                    "totalBtcAmount": 0,
                    "totalUsdtAmount": 0,
                    "assets": [    //参数内容参考获取单个币种资产接口
                      {        
                        "currency": "string",
                        "currencyId": 0,
                        "frozenAmount": 0,      //不可用(全部冻结=冻结+锁仓+跟单+委托+提现)
                        "freeze": 0,            //冻结
                        "lock": 0,              //锁仓
                        "copyTrade": 0,         //跟单
                        "trade": 0,             //委托
                        "withdraw": 0,          //提现
                        "availableAmount": 0,
                        "totalAmount": 0,
                        "convertBtcAmount": 0,
                        "convertUsdtAmount": 0   //折算USDT数量
                      }
                    ]
                  }
                }
        title: Response
        language: json
---

