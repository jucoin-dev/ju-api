---
title: Delete user account apiKey
position_number: 4
type: delete
description: /api/user/account/api-key/{apikeyId}
parameters:
    -
        name: apikeyId
        type: string
        mandatory: true
        default:
        description: apiKey id
        ranges:

content_markdown:
left_code_blocks:
    -
        code_block: |-
            public String deleteApiKey(){


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
                  "data": true    //true: success; false/null: unsuccess
                }
        title: Response
        language: json
---
