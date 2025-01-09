---
title: 获取token接口
position_number: 4
split: '-------------------------------------'
type: post
description: /v1/spot/ws-token
parameters:
    -
        name:
        type: string
        mandatory: false
        default:
        description:
        ranges:
content_markdown: |-
  备注：
  
  accessToken有效期是2天，重新调用接口获取token会重置有效期。
  
  accessToken = listenKey
left_code_blocks:
    -
        code_block:
        title:
        language: json
right_code_blocks:
    -
        code_block: |-
                {
                    "code": 200,
                    "msg": "SUCCESS",
                    "msgInfo": [],
                    "data": {
                        "accessToken": "xxxxxx",
                        "refreshToken": "xxxxxx"
                    }
                }
        title: Response
        language: json
---
