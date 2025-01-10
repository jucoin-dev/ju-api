---
title: 获取账户相关信息
position_number: 1
type: get
description: /user/account/info
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
          "data": {
            "accountId": 0, //帐户id
            "allowOpenPosition": false, //是否可开仓
            "allowTrade": false, //是否可以交易
            "allowTransfer": false, //是否可以划转
            "openTime": "", //开通时间
            "state": 0, //用户状态
            "userId": 0 //用户id
          },
          "code": 200
        }
      title: Response
      language: json
---