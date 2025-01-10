---
title: 撤销跟踪委托（单个）
position_number: 14
type: post
description: /trade/entrust/cancel-track
remark: Content-Type = application/x-www-form-urlencoded
parameters:
    -
        name: trackId
        type: integer
        mandatory: true
        default: N/A
        description: 跟踪委托id
        ranges: 
content_markdown: |-

                 #### **限流规则**

                 200/s/apikey
left_code_blocks:
    -
        code_block: 
        title: Java
        language: java
right_code_blocks:
    - code_block: |-
        {
          "msgInfo": {
            "code": "",
            "msg": ""
          },
          "msg": "",
          "data": {},
          "code": 200
        }
      title: Response
      language: json
---