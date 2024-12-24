---
title: Get Trading Pair Currency
position_number: 2
type: get
description: /v1/future-u/market/public/symbol/coins

parameters:
  - name:
    content:
content_markdown: Note：This method does not require a signature.
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