---
title: See Leverage Stratification of All Trading Pairs
position_number: 6
type: get
description: /market/public/leverage/bracket/list
parameters:
content_markdown: Note：This method does not require a signature.
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
              "leverageBrackets": [
                {
                  "bracket": 0, //Level
                  "maintMarginRate": 0, //Maintain margin rate
                  "maxLeverage": 0, //Maximum leverage
                  "maxNominalValue": 0, //Maximum notional value
                  "maxStartMarginRate": 0, //Maximum initial margin rate
                  "minLeverage": 0, //Minimum leverage
                  "startMarginRate": 0, //Initial margin rate
                  "symbol": "" //Trading pair
                }
              ],
              "symbol": ""
            }
          ],
          "code": 200
        }
      title: Response
      language: json
---