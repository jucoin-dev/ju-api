---
title: 获取全交易对的买一卖一行情信息
position_number: 19
type: get
description: /v1/future-u/market/public/q/ticker/books
parameters:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
  -
    code_block: "public void getTickerBokk() {\r\n\tString text = HttpUtil.get(URL + \"/data/api//v1/future-u/market/public/q/ticker/books?symbol=btc_usdt\");\r\n\tSystem.out.println(text);\r\n}"
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
            "ap": "", //卖一价格
            "aq": "", //卖一数量
            "bp": "", //买一价格
            "bq": "", //买一数量
            "s": "", //交易对
            "t": 0 //时间
          }
        ],
        "code": 200
      }
    title: Response
    language: json
---