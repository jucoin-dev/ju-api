---
title: Get token
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
  Note：
  
  The accessToken is valid for 2 days. Calling the endpoint again will reset the validity period. 
  
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
                    "mc": "SUCCESS",
                    "msgInfo": [],
                    "data": {
                        "accessToken": "xxxxxx",
                        "refreshToken": "xxxxxx"
                    }
                }
        title: Response
        language: json
---
