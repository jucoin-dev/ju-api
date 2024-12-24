---
title: Get User's Step Rate
position_number: 8
type: get
description: /v1/future-u/user/user/step-rate
parameters:
    -
content_markdown: |-
  
              #### **Limit Flow Rules**

              200/s/apikey
left_code_blocks:
    -
        code_block: "public void getStepRate() {\r\n\tString text = HttpUtil.get(URL + \"/v1/future-u/user/user/step-rate\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    - code_block: |-
        {
          "msgInfo": {
            "code": "",
            "msg": ""
          },
          "msg": "success",
          "data": {
            "makerFee":"0.00004",
            "takerFee": "0.00001"
          },
          "code": 200
        }
      title: Response
      language: json
---
