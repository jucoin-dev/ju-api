---
title: Update Orders
position_number: 2
type: post
description: /v1/future-u/trade/order/update
remark: Content-Type = application/x-www-form-urlencoded && application/json
parameters:
    -
        name: orderId
        type: number
        mandatory: true
        default: 
        description: Order ID
        ranges:
    -
        name: price
        type: number
        mandatory: true
        default: 
        description: Target price
        ranges:
    -
        name: origQty
        type: number
        mandatory: true
        default: 
        description: Target quantity (cont)
        ranges:
    -
        name: triggerProfitPrice
        type: number
        mandatory: false
        default: N/A
        description: Profit target price
        ranges:
    -
        name: triggerStopPrice
        type: number
        mandatory: false
        default: N/A
        description: Stop-Loss price
        ranges:
    -
        name: triggerPriceType
        type: string
        mandatory: false
        default: LATEST_PRICE
        description: Trigger price type
        ranges: INDEX_PRICE(Index price)；MARK_PRICE(Mark price)；LATEST_PRICE(latest price)
    -
        name: profitDelegateOrderType
        type: string
        mandatory: false
        default: N/A
        description: Take-Profit order type
        ranges: LIMIT；MARKET
    -
        name: profitDelegateTimeInForce
        type: string
        mandatory: false
        default: N/A
        description: Take-Profit order validity method
        ranges: GTC;IOC;FOK;GTX
    -
        name: profitDelegatePrice
        type: number
        mandatory: false
        default: N/A
        description: Take-Profit order price
        ranges: 
    -
        name: stopDelegateOrderType
        type: string
        mandatory: false
        default: N/A
        description: Stop-Loss order type
        ranges: LIMIT；MARKET
    -
        name: stopDelegateTimeInForce
        type: string
        mandatory: false
        default: N/A
        description: Stop-Loss order validity method
        ranges: GTC;IOC;FOK;GTX
    -
        name: stopDelegatePrice
        type: number
        mandatory: false
        default: N/A
        description: Stop-Loss order price
        ranges: 
    -
        name: followUpOrder
        type: boolean
        mandatory: false
        default: N/A
        description: 
        ranges: If true, it indicates chase order
content_markdown: |-

              #### **Limit Flow Rules**

              200/s/apikey
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/future-u/trade/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
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
        "data": {},
        "code": 200
      }
    title: Response
    language: json
---