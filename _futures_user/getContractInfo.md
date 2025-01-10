---
title: Get Account Related Information
position_number: 1
type: get
description: /user/account/info
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
          "data": {
            "accountId": 0, //Account ID
            "allowOpenPosition": false, //Is it possible to open position
            "allowTrade": false, //Is it possible to trade
            "allowTransfer": false, //Is it possible to transfer
            "openTime": "", //Opening time
            "state": 0, //User status
            "userId": 0 //User ID
          },
          "code": 200
        }
      title: Response
      language: json
---