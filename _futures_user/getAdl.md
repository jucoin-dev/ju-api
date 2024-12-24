---
title: Get ADL Information
position_number: 13
type: get
description: /v1/future-u/user/position/adl
content_markdown: |-

               #### **Limit Flow Rules**

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
              "longQuantile": 0, //long position adl
              "shortQuantile": 0, //Short position adl
              "symbol": "" //Trading pair
            }
          ],
          "code": 200
        }
      title: Response
      language: json
---