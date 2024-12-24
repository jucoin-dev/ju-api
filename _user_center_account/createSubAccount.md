---
title: create a sub-account
position_number: 2
type: post
description: /api/user/account
parameters:
    -
        name: accountName
        type: string
        mandatory: true
        default:
        description: sub-account name
        ranges:

content_markdown:
left_code_blocks:
    -
        code_block: |-
            public String createSubAccount(){


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
                  "msg": "SUCCESS",
                  "msgInfo": [
                    {}
                  ],
                  "data": true  //true: success; false/null: unsuccess
                }
        title: Response
        language: json
---
