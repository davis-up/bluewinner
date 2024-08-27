
# Table

## WITMSUBSTOSUP

- `1u02_WITMSUBSTOSUP` [2024-08-27 14:57]

```sql
        SELECT A1.*
        FROM WITMSUBSTOSUP A1
           INNER JOIN WITMSUBSUP A ON A.WSUSID = A1.WSTPSUSID
           INNER JOIN WITMGLD  B ON A.WSUSITMID = B.WITMID
        WHERE 0=0
          AND B.WITMREQNO = 'CL240700002'


```

|SEQ|WSTPID|WSTPSUSID|WSTPSUBCD|WSTPSUPCD|WSTPSTOCD|WSTPPACK|WSTPORDBY|WSTPPKLAY|WSTPLAYPAL|WSTPPKBOX|WSTPCRE|WSTPUPD|WSTPUSR|WSTPCREUSR|WSTPPACK_C4|WSTPORDBY_C4|WSTPPKLAY_C4|WSTPLAYPAL_C4|WSTPPKBOX_C4|WSTPSUBCD_C4|WSTPSUPCD_C4|WSTPSTOCD_C4|WSTPSUBCDDESC|WSTPSUBCDDESC_C4|WSTPMARKD|WSTPMARKD_C4|WSTPSUPEDESC|WSTPSUPLDESC|WSTPSUPEDESC_C4|WSTPSUPLDESC_C4|WSTPSUBLDESC|WSTPSUBLDESC_C4|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |


----

## Description

- [`WSTPID`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Request Sub by store by sup. ID
- [`WSTPSUSID`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Request Sub code by sup. ID
- [`WSTPSUBCD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Item Sub code
- [`WSTPSUPCD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Supplier Code
- [`WSTPSTOCD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Store Code
- [`WSTPPACK`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Quantity per pack
- [`WSTPORDBY`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Order By(B-by box, L-by layer, P-by pallet)
- [`WSTPPKLAY`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Pack per layer
- [`WSTPLAYPAL`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Layer per pallet
- [`WSTPPKBOX`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Pack per box
- [`WSTPCRE`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Creation date
- [`WSTPUPD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Date of last update
- [`WSTPUSR`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Last user
- [`WSTPCREUSR`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Creation User
- [`WSTPSUBCDDESC`] : 
  - UI :`YYY`
  - value :`null`
- [`WSTPMARKD`] : 
  - UI :`YYY`
  - value :`null`
- [`WSTPSUPEDESC`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Supplier English Description
- [`WSTPSUPLDESC`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Supplier Local Description
- [`WSTPSUBLDESC`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Sub code Local Description

