---
title: 获取所有交易对的指数价格
position_number: 12
type: get
description: /v1/future-u/market/public/q/index-price
parameters:
content_markdown: 注：**此方法不需要签名**
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
          "data": [
            {
              "p": 0, //价格
              "s": "", //交易对
              "t": 0 //时间
            }
          ],
          "code": 200
        }
      title: Response
      language: json
---