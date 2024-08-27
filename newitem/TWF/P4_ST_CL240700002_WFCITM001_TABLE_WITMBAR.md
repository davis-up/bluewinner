
# Table

## WITMBAR

- `1u02_WITMBAR` [2024-08-27 14:57]

```sql
    SELECT * FROM WITMBAR  WHERE 0=0  AND WBARREQNO = 'CL240700002'
```

|SEQ|WBARID|WBARREQNO|WBARITMID|WBARSUBCD|WBARSUBCDEDESC|WBARSUBCDLDESC|WBARUNTCD|WBARBARTYP|WBARINEX|WBARBARCD|WBARMJBAR|WBARNPP|WBARNSP|WBARGROSSMAR|WBARTYPOFLAG|WBARTYPOCD|WBARTYPOSDATE|WBARTYPOEDATE|WBARTYPSOTOPRS|WBARBCQTY|WBARFRQTY|WBARSNI|WBARSSTOP|WBARESTOP|WBARSTOPRS|WBARCRE|WBARUPD|WBARUSR|WBARCREUSR|WBARSUBIDMD|WBARSUBCDEDESC_C4|WBARSUBCDLDESC_C4|WBARUNTCD_C4|WBARBARTYP_C4|WBARINEX_C4|WBARBARCD_C4|WBARMJBAR_C4|WBARNPP_C4|WBARNSP_C4|WBARGROSSMAR_C4|WBARTYPOFLAG_C4|WBARTYPOCD_C4|WBARTYPOSDATE_C4|WBARTYPOEDATE_C4|WBARTYPSOTOPRS_C4|WBARBCQTY_C4|WBARFRQTY_C4|WBARSNI_C4|WBARSSTOP_C4|WBARESTOP_C4|WBARSTOPRS_C4|WBARFORMID|WBARWORKID|WBARITMBARID|WBARTYPOSUP|WBARTYPSUPCD|WBARTYPOSUPSDATE|WBARTYPOSUPEDATE|WBARTYPOJSN|WBARTYPJSNCD|WBARTYPOJSNSDATE|WBARTYPOJSNEDATE|WBARSTORYHYP|WBARSTORYSUP|WBARSTORYJSN|WBARTYPJSNSOTOPRS|WBARTYPSUPSOTOPRS|WBARTYPOSUP_C4|WBARTYPSUPCD_C4|WBARTYPOSUPSDATE_C4|WBARTYPOSUPEDATE_C4|WBARTYPOJSN_C4|WBARTYPJSNCD_C4|WBARTYPOJSNSDATE_C4|WBARTYPOJSNEDATE_C4|WBARSTORYHYP_C4|WBARSTORYSUP_C4|WBARSTORYJSN_C4|WBARTYPJSNSOTOPRS_C4|WBARTYPSUPSOTOPRS_C4|WBARGWEIGHT|WBARNWEIGHT|WBARGWEIGHT_C4|WBARNWEIGHT_C4|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|2686693|CL240700002|2622043|001|LOTTE Chicken|雞午餐肉|01|1|E|7672622751009|Y|128|159|15.4717|1|2U|2024-07-11 00:00:00.0|2049-12-31 00:00:00.0|null|null|null|null|null|null|null|2024-07-10 16:53:21.0|2024-07-10 16:53:21.0|buyer_UST|buyer_UST|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|0.374|0.34|null|null|


----

## Description

- [`WBARID`] : 
  - UI :`YYY`
  - value :`2686693`
  - comment: Request Barcode ID
- [`WBARREQNO`] : 
  - UI :`YYY`
  - value :`CL240700002`
  - comment: Request No.
- [`WBARITMID`] : 
  - UI :`YYY`
  - value :`2622043`
  - comment: Request item ID
- [`WBARSUBCD`] : 
  - UI :`YYY`
  - value :`001`
  - comment: Item Sub code
- [`WBARSUBCDEDESC`] : 
  - UI :`YYY`
  - value :`LOTTE Chicken`
  - comment: Sub code Local Description
- [`WBARSUBCDLDESC`] : 
  - UI :`YYY`
  - value :`雞午餐肉`
  - comment: Sub code English Description
- [`WBARUNTCD`] : 
  - UI :`YYY`
  - value :`01`
  - comment: Item Unit code
- [`WBARBARTYP`] : 
  - UI :`YYY`
  - value :`1`
  - comment: Original Barcode Type(1-EAN 13, 2-EAN 8, 3-UPCA, 4-UPCE, 9-PLU, EAN-14) *Table 33
- [`WBARINEX`] : 
  - UI :`YYY`
  - value :`E`
  - comment: Internal/External Barcode (I/E)
- [`WBARBARCD`] : 
  - UI :`YYY`
  - value :`7672622751009`
  - comment: Item Bar code
- [`WBARMJBAR`] : 
  - UI :`YYY`
  - value :`Y`
  - comment: Major Barcode Flag(Y-for 1 major barcode, Blank for the others)
- [`WBARNPP`] : 
  - UI :`YYY`
  - value :`128`
  - comment: Item NPP
- [`WBARNSP`] : 
  - UI :`YYY`
  - value :`159`
  - comment: Item NSP
- [`WBARGROSSMAR`] : 
  - UI :`YYY`
  - value :`15.4717`
  - comment: % Gross Margin
- [`WBARTYPOFLAG`] : 
  - UI :`YYY`
  - value :`1`
  - comment:

```txt
Typology Flag
(1: Yes,0: No)

```

- [`WBARTYPOCD`] : 
  - UI :`YYY`
  - value :`2U`
  - comment: Typology code * Table 616
- [`WBARTYPOSDATE`] : 
  - UI :`YYY`
  - value :`2024-07-11 00:00:00.0`
  - comment: Typology Start Date
- [`WBARTYPOEDATE`] : 
  - UI :`YYY`
  - value :`2049-12-31 00:00:00.0`
  - comment: Typology End Date
- [`WBARTYPSOTOPRS`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Typology Stop Item Reason
- [`WBARBCQTY`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Basic Goods
- [`WBARFRQTY`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Free Goods
- [`WBARSNI`] : 
  - UI :`YYY`
  - value :`null`
  - comment:

```txt
SNI Code* Table26
0 = Normal (Default)
1 = Open price
2 = Negative

```

- [`WBARSSTOP`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Start Stop Date by Sub Code
- [`WBARESTOP`] : 
  - UI :`YYY`
  - value :`null`
  - comment: End Stop Date by Sub Code
- [`WBARSTOPRS`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Stop Item Reason Code *Table 10
- [`WBARCRE`] : 
  - UI :`YYY`
  - value :`2024-07-10 16:53:21.0`
  - comment: Creation date
- [`WBARUPD`] : 
  - UI :`YYY`
  - value :`2024-07-10 16:53:21.0`
  - comment: Date of last update
- [`WBARUSR`] : 
  - UI :`YYY`
  - value :`buyer_UST`
  - comment: Last user
- [`WBARCREUSR`] : 
  - UI :`YYY`
  - value :`buyer_UST`
  - comment: Creation User
- [`WBARSUBIDMD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Sub code ID from P4MD+
- [`WBARFORMID`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Refer E-Form ID from table WMAPITM
- [`WBARWORKID`] : 
  - UI :`YYY`
  - value :`null`
- [`WBARITMBARID`] : 
  - UI :`YYY`
  - value :`null`
- [`WBARTYPOSUP`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Super Typology Flag
- [`WBARTYPSUPCD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Super Typology Code
- [`WBARTYPOSUPSDATE`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Super Typology Start Date
- [`WBARTYPOSUPEDATE`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Super Typology End Date
- [`WBARTYPOJSN`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Jasons Typology Flag
- [`WBARTYPJSNCD`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Jasons Typology Code
- [`WBARTYPOJSNSDATE`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Jasons Typology Start Date
- [`WBARTYPOJSNEDATE`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Jasons Typology End Date
- [`WBARSTORYHYP`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Hyper Story Code
- [`WBARSTORYSUP`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Super Story Code
- [`WBARSTORYJSN`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Jasons Story Code
- [`WBARTYPJSNSOTOPRS`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Jasons Typology Stop Item Reason
- [`WBARTYPSUPSOTOPRS`] : 
  - UI :`YYY`
  - value :`null`
  - comment: Super Typology Stop Item Reason
- [`WBARGWEIGHT`] : 
  - UI :`YYY`
  - value :`0.374`
  - comment: Gross Weight
- [`WBARNWEIGHT`] : 
  - UI :`YYY`
  - value :`0.34`
  - comment: Net Weight

