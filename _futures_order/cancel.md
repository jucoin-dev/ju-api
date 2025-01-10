---
title: Cancel Orders
position_number: 6
type: post
description: /trade/order/cancel
remark: Content-Type = application/x-www-form-urlencoded && application/json
parameters:
  - name: orderId
    type: Integer
    mandatory: true
    default: N/A
    description: Order ID
    ranges:
content_markdown: |-

               #### **Limit Flow Rules**

               200/s/apikey
right_code_blocks:
  - code_block: |-
      {
        "msgInfo": {
          "code": "",
          "msg": ""
        },
        "msg": "",
        "data": "", //Order ID
        "code": 200
      }
    title: Response
    language: json
---