---
title: 获取交易对币种
position_number: 2
type: get
description: /market/public/symbol/coins

parameters:
  - name:
    content:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
  - code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/future-u/market/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
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
        "data": [],
        "code": 200
      }
    title: Response
    language: json
---