
# Table

## WITMSUBSUP

- `1u02_WITMSUBSUP` [2024-08-27 14:57]

```sql
        SELECT A.*
        FROM WITMSUBSUP A
           INNER JOIN WITMGLD  B ON A.WSUSITMID = B.WITMID
           -- INNER JOIN WREQGLD  C ON C.WRQREQNO = B.WITMREQNO
        WHERE 0=0
         AND B.WITMREQNO = 'CL240700002'
         --B.WITSREQNO
         --ORDER BY B.WITSID


```

|SEQ|WSUSID|WSUSITMID|WSUSSUBCD|WSUSSUPCD|WSUSNEGO|WSUSPACK|WSUSORDBY|WSUSPKLAY|WSUSLAYPAL|WSUSPKBOX|WSUSCRE|WSUSUPD|WSUSUSR|WSUSCREUSR|WSUSSUBIDMD|WSUSNEGO_C4|WSUSPACK_C4|WSUSORDBY_C4|WSUSPKLAY_C4|WSUSLAYPAL_C4|WSUSPKBOX_C4|WSUSSUBCDEDESC|WSUSSUBCD_C4|WSUSSUPCD_C4|WSUSSUBCDEDESC_C4|WSUSFORMID|WSUSSUPEDESC|WSUSSUPLDESC|WSUSSUPEDESC_C4|WSUSSUPLDESC_C4|WSUSSUBLDESC|WSUSSUBLDESC_C4|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |


----

## Description

- [`WSUSID`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Request Sub by sup. ID
- [`WSUSITMID`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Request Item ID
- [`WSUSSUBCD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Item Sub code
- [`WSUSSUPCD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Supplier Code
- [`WSUSNEGO`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Negotiation Type (1- Based on MRP, 2-Based on MOP, 3-Direct Entry)
- [`WSUSPACK`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Quantity per pack
- [`WSUSORDBY`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Order By(B-by box, L-by layer, P-by pallet)
- [`WSUSPKLAY`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Pack per layer
- [`WSUSLAYPAL`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Layer per pallet
- [`WSUSPKBOX`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Pack per box
- [`WSUSCRE`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Creation date
- [`WSUSUPD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Date of last update
- [`WSUSUSR`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Last user
- [`WSUSCREUSR`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Creation User
- [`WSUSSUBIDMD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Sub code ID from P4MD+
- [`WSUSSUBCDEDESC`] : 
  - UI :`YYY`
  - value :`null`
- [`WSUSFORMID`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Refer E-Form ID from table WMAPITM
- [`WSUSSUPEDESC`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Supplier English Description
- [`WSUSSUPLDESC`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Supplier Local Description
- [`WSUSSUBLDESC`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Sub code Local Description

