---
title: Cancel Stop Limit
position_number: 8
type: post
description: /v1/future-u/trade/entrust/cancel-profit-stop
remark: Content-Type = application/x-www-form-urlencoded && application/json
parameters:
    -
        name: profitId
        type: integer
        mandatory: true
        default: N/A
        description: Stop limit ID
        ranges:
content_markdown: |-

                #### **Limit Flow Rules**

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
          "data": true,
          "code": 200
        }
      title: Response
      language: json
---