---
title: 撤销计划委托
position_number: 2
type: post
description: /v1/future-u/trade/entrust/cancel-plan
remark: Content-Type = application/x-www-form-urlencoded && application/json
parameters:
    -
        name: entrustId
        type: integer
        mandatory: true
        default: N/A
        description: 计划委托id
        ranges:
content_markdown: |-

               #### **限流规则**

               200/s/apikey
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/future-u/trade/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
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