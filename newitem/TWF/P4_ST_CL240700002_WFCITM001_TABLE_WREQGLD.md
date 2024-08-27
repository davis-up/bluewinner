
# Table

## WREQGLD

- `1u02_WREQGLD` [2024-08-27 14:57]

```sql
    SELECT * FROM WREQGLD  WHERE 0=0  AND WRQREQNO = 'CL240700002'
```

|SEQ|WRQREQNO|WRQSTATUS|WRQSUBMIT|WRQSOURCE|WRQUUID|WRQREQFROM|WRQPRI|WRQAPP|WRQREL|WRQNGFLAG|WRQNGRS|WRQCRE|WRQUPD|WRQUSR|WRQCREUSR|WRQFLOWTYP|WRQITMTYP|WRQFORMID|WRQASTFLAG|WRQNGRSCD|WRQUSRNAME|WRQDELEGEEUSR|WRQASSIGNUSR|WRQASSIGNDATE|WRQORGREQNO|WRQCANFLAG|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|CL240700002|0|null|C|null|null|0|IC|null|null|null|2024-07-10 16:44:04.0|2024-07-10 16:44:04.0|buyer_UST|buyer_UST|M|L|null|null|null|UST team UST team|null|null|null|null|null|


----

## Description

- [`WRQREQNO`] : 
  - UI :`申請單號`
  - value :`CL240700002`
  - comment: Request No.
- [`WRQSTATUS`] : 
  - UI :`申請狀態`
  - value :`0`
  - comment:

```txt
Status  (PT 720)
0- saved
1- submitted
2- validated(released to MD)
3- cancelled
4- rejected(mark NG)
5- Wait to release all stores
6- Wait to re-confirm
7- Wait for all GDS Request
8- Fail from released to MD
9- Wait to compare PSP
A- Wait for submit from E-form screen

```

- [`WRQSUBMIT`] : 
  - UI :`送審狀態`
  - value :`null`
  - comment:

```txt
Submit Status
0-waiting submit by Div mgr.
1-waiting submit by Logistic mgr.
2-waiting submit by Pricing mgr.
3-end submit
4-waiting release to md (E-Form).
5-comparing PSP.
6-waiting submit by Tax mgr.

```

- [`WRQSOURCE`] : 
  - UI :``
  - value :`C`
  - comment:

```txt
Source data
C = E-codi
F = E-form

```

- [`WRQUUID`] : 
  - UI :``
  - value :`null`
  - comment: Unique  ID  from Bonita
- [`WRQREQFROM`] : 
  - UI :``
  - value :`null`
  - comment: Request No. from E-from
- [`WRQPRI`] : 
  - UI :`優先順序`
  - value :`0`
  - comment:

```txt
Priority*Table 715
0 = Normal
1 = High
2 = Urgent

```

- [`WRQAPP`] : 
  - UI :`申請格式`
  - value :`IC`
  - comment:

```txt
Application Form * 701
[ IC - Item Creation
  IM - Item Modification
  NP - NPP/NSP
  PP - PPP/PSP
  SR - Stop/Release ]

```

- [`WRQREL`] : 
  - UI :``
  - value :`null`
  - comment: Released Date
- [`WRQNGFLAG`] : 
  - UI :`[Manager] 審核 NG：[1:Yes],[0:NO]`
  - value :`null`
  - comment: NG Flag (1-Yes, 0-No)
- [`WRQNGRS`] : 
  - UI :`[Manager] NG 原因`
  - value :`null`
  - comment: NG Reason by E-codi * default table 702
- [`WRQCRE`] : 
  - UI :``
  - value :`2024-07-10 16:44:04.0`
  - comment: Creation date
- [`WRQUPD`] : 
  - UI :``
  - value :`2024-07-10 16:44:04.0`
  - comment: Date of last update
- [`WRQUSR`] : 
  - UI :``
  - value :`buyer_UST`
  - comment: Last user
- [`WRQCREUSR`] : 
  - UI :``
  - value :`buyer_UST`
  - comment: Creation User
- [`WRQFLOWTYP`] : 
  - UI :``
  - value :`M`
  - comment:

```txt
Flow Type:
for item
S=for red item,
M=for green item
for price
PP = PP Only
SP = SP Only
BP = Both Price

```

- [`WRQITMTYP`] : 
  - UI :``
  - value :`L`
  - comment: Item Type N=Normal, L=Logistic
- [`WRQFORMID`] : 
  - UI :``
  - value :`null`
  - comment: Refer E-Form ID from table WMAPITM
- [`WRQASTFLAG`] : 
  - UI :``
  - value :`null`
  - comment:

```txt
Store assortment Date Flag
F- Future
I- Immiediate

```

- [`WRQNGRSCD`] : 
  - UI :`[Manager] NG [代碼]`
  - value :`null`
  - comment: NG Reason Code
- [`WRQUSRNAME`] : 
  - UI :``
  - value :`UST team UST team`
  - comment: User Name
- [`WRQDELEGEEUSR`] : 
  - UI :``
  - value :`null`
  - comment: Delegee User
- [`WRQASSIGNUSR`] : 
  - UI :``
  - value :`null`
  - comment: Assign User
- [`WRQASSIGNDATE`] : 
  - UI :``
  - value :`null`
  - comment: Assign Date
- [`WRQORGREQNO`] : 
  - UI :`原申請單號`
  - value :`null`
  - comment: Original Request No
- [`WRQCANFLAG`] : 
  - UI :``
  - value :`null`
  - comment: Cancel Flag

