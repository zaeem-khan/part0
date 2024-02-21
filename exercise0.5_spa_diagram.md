[![](https://mermaid.ink/img/pako:eNq9Uz1PwzAU_CuW58RpQ4Woh04gGOhEJ2SGh_1K3SaOsV8KqOp_x24qFuhQCdWTfe987_xxO647g1zyiO89Oo23Ft4CtMqxNDwEstp6cMReQ_cRMfwuJHCb8aFypJWz2YBLdn-3YCsiH2VVReqNxSh0FCtsonUbK5a2wk9ofYPgfRU9DEKgyW6B8Ec_g8O8TOrHPpI9LOaPzHS6b9HRwDL45-b_MdiCdakcz3OZNrClbfBSBtdn-lvDFqIO1tOlbBogSDY7d57RnUo_1lF-ay4V32wULxRPYnhY16N6Uo7qsh4vxhN5dS3rqahvps-K7wshxMuJg_GCtxjSzZkUhV0mKU4rbLMoy_Ih9VFun3jQU_f05TSXFHoseO9z82NsuFxCExOKxlIX5kO2DhHbfwMK2isp?type=png)](https://mermaid.live/edit#pako:eNq9Uz1PwzAU_CuW58RpQ4Woh04gGOhEJ2SGh_1K3SaOsV8KqOp_x24qFuhQCdWTfe987_xxO647g1zyiO89Oo23Ft4CtMqxNDwEstp6cMReQ_cRMfwuJHCb8aFypJWz2YBLdn-3YCsiH2VVReqNxSh0FCtsonUbK5a2wk9ofYPgfRU9DEKgyW6B8Ec_g8O8TOrHPpI9LOaPzHS6b9HRwDL45-b_MdiCdakcz3OZNrClbfBSBtdn-lvDFqIO1tOlbBogSDY7d57RnUo_1lF-ay4V32wULxRPYnhY16N6Uo7qsh4vxhN5dS3rqahvps-K7wshxMuJg_GCtxjSzZkUhV0mKU4rbLMoy_Ih9VFun3jQU_f05TSXFHoseO9z82NsuFxCExOKxlIX5kO2DhHbfwMK2isp)

# sequenceDiagram
    participant browser
    participant server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server-->>browser: HTML document
    deactivate server
    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: css file
    deactivate server
    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>browser: javascript file
    deactivate server
    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>browser: {"content":"kk","date":"2024-02-21T14:36:29.289Z"},...]
    deactivate server