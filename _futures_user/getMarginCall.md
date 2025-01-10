---
title: Get Margin Call Information
position_number: 18
type: get
description: /trade/position/break-list
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: Trading pair (see the margin call of all trading pairs if don't pass parameters)
        ranges:
content_markdown: |-

               #### **Limit Flow Rules**

               200/s/apikey
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/v1/future-u/trade/position/break-list\");\r\n\tSystem.out.println(text);\r\n}"
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
              "breakPrice": 0,    //Margin call price. 0 means no margin call
              "calMarkPrice": 0,  //Mark price
              "contractType": "", //Futures type: PERPETUAL;PREDICT
              "entryPrice": 0,    //Open position average price
              "isolatedMargin": 0,//Isolated Margin
              "leverage": 0,      //Leverage
              "positionSide": "", //Position side:LONG;SHORT
              "positionSize": 0,  //Position quantity (Cont)
              "positionType": "", //Position type:CROSSED;ISOLATED
              "symbol": ""        //Symbol
            }
          ],
          "code": 200
        }
      title: Response
      language: json
---
