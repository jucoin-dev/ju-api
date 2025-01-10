---
title: 获取交易对的深度信息
position_number: 10
type: get
description: /market/public/q/depth
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: 交易对
        ranges:
    -
        name: level
        type: integer
        mandatory: true
        default: N/A
        description: "档位（min:1,max:50）\t"
        ranges:
content_markdown: >-

  #### **限流规则**

  1/s/ip
  <br>
  注：此方法不需要签名

left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/future-u/market/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
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
            "a": [], //卖单
            "b": [], //买单
            "s": "", //交易对
            "t": 0, //时间
            "u": 0 //updateId
          },
          "code": 200
        }
      title: Response
      language: json
---