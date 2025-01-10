---
title: 获取客户端IP
position_number: 1
type: get
description: /public/client
parameters:
    -
        name:
        type: number
        mandatory: false
        default:
        description:
        ranges:
content_markdown: 注：此方法不需要签名
left_code_blocks:
    -
        code_block: |-
            public String getClient(){


            }
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
                  "msgInfo": null
                  "data": {
                    "ip": 192.168.1.1  
                  }
                }
        title: Response
        language: json
---
