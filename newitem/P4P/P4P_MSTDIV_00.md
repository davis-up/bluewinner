
# MSTDIV


```sql
   
    SELECT * FROM MSTDIV
     --FETCH FIRST 10 ROWS ONLY

```

|SEQ|MSVDVCD|MSVEDESC|MSVLDESC|MSVCRE|MSVUPD|MSVUSR|MSVCREUSR|
| -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 08|1|Grocery|雜貨|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|
|02 / 08|2|Fresh|生鮮|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|
|03 / 08|3|Hard Goods|日用百貨|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|
|04 / 08|4|Appliance|家電|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|
|05 / 08|6|Textile|服飾|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|
|06 / 08|7|Service|服務|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|
|07 / 08|8|Management|管理|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|
|08 / 08|9|Computer|電腦|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|


- MSTDIV [DivisionModel]
  - MSVDVCD
    - Value : 1
    - PK
    - 說明 : divisionCode
    - comment : Division code
  - MSVEDESC
    - Value : Grocery
    - 說明 : divisionEngDesc
    - comment : Division English description
  - MSVLDESC
    - Value : 雜貨
    - 說明 : divisionLocalDesc
    - comment : Division Local description
  - MSVCRE
    - Value : 2009-05-08 19:00:00.0
    - 說明 : cred
    - comment : Creation date
  - MSVUPD
    - Value : 2009-05-08 19:00:00.0
    - 說明 : lastUpd
    - comment : Date of last update
  - MSVUSR
    - Value : MIGRATION
    - 說明 : lastUser
    - comment : Last user
  - MSVCREUSR
    - Value : MIGRATION
    - 說明 : creUser
    - comment : Creation User
