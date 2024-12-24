---
title: 获取跟单交易对信息
position_number: 1
type: get
display: 0
split: '-------------------------------------'
description: /v1/spot/public/copy-trade/symbol
parameters:
  
content_markdown: >-
    
left_code_blocks:
    -
        code_block:
        title: Java
        language: java
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: |-
                {
                  "code": 200,
                  "mc": "SUCCESS",
                  "msgInfo": [],
                  "data": [{
                      symbolId: 1,       //市场id
                      symbol: "btc_usdt" //市场
                  }]
                }            
        title: Response
        language: json
---
