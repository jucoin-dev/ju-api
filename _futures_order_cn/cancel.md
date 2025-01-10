---
title: 撤销订单
position_number: 6
type: post
description: /trade/order/cancel
remark: Content-Type = application/x-www-form-urlencoded && application/json
parameters:
  - name: orderId
    type: Integer
    mandatory: true
    default: N/A
    description: 订单id
    ranges:
content_markdown: |-

              #### **限流规则**

              200/s/apikey
right_code_blocks:
  - code_block: |-
      {
        "msgInfo": {
          "code": "",
          "msg": ""
        },
        "msg": "",
        "data": "", //订单id
        "code": 200
      }
    title: Response
    language: json
---