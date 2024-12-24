---
title: 撤销所有止盈止损
position_number: 9
type: post
description: /v1/future-u/trade/entrust/cancel-all-profit-stop
remark: Content-Type = application/x-www-form-urlencoded && application/json
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: 
        description: 交易对，例如btc_usdt
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
          "data": true,
          "code": 200
        }
      title: Response
      language: json
---