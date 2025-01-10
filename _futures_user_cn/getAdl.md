---
title: 获取ADL信息
position_number: 13
type: get
description: /trade/position/adl
content_markdown: |-

                #### **限流规则**

                200/s/apikey
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/user/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
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
          "data": [
            {
              "longQuantile": 0, //多头adl
              "shortQuantile": 0, //空头adl
              "symbol": "" //交易对
            }
          ],
          "code": 200
        }
      title: Response
      language: json
---