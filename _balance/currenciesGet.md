---
title: Get currency information
position_number: 1
type: get
description: /v1/spot/public/currencies
parameters:
    -
        name: version
        type: string
        mandatory: false
        default:
        description:
        ranges:
content_markdown:
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
              "msg": "string",
              "msgInfo": [
                {}
              ],
              "data": {
                  "time":0,
                  "version":"",
                  "currencies": [
                          {
                              "id": 11,                
                              "currency": "usdt",      
                              "displayName": "",    
                              "type": "",           
                              "nominalValue": "",   
                              "fullName": "usdt",       
                              "logo": null,             
                              "cmcLink": null,          
                              "weight": 100,            
                              "maxPrecision": 6,        
                              "depositStatus": 1,       
                              "withdrawStatus": 1,      
                              "convertEnabled": 1,      
                              "transferEnabled": 1,     
                              "isChainExist": 1,        
                              "plates": [],              
                              "isListing": 1,           
                              "withdrawCloseReason": ""  
                          }
                  ]

                }
            }
        title: Response
        language: json
---

