
# SUPATT


```sql
   
    SELECT * FROM SUPATT
     FETCH FIRST 10 ROWS ONLY

```

|SEQ|SUASUPCD|SUACLCD|SUACD|SUASDATE|SUAALPH|SUANUM|SUADATE|SUATIME|SUAEDATE|SUACRE|SUACREUSR|SUAUPD|SUAUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 10|F279|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|02 / 10|F780|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|03 / 10|F785|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|04 / 10|F787|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|05 / 10|F790|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|06 / 10|F794|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|07 / 10|F795|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|08 / 10|F799|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|09 / 10|F805|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|
|10 / 10|F806|CONS|C00|2009-05-08 00:00:00.0|null|0|null|null|2049-12-31 00:00:00.0|2009-05-08 19:00:00.0|MIGRATION|2009-09-01 10:51:50.0|SSFIX_1041|


- SUPATT [SupplierAttribute]
  - SUASUPCD
    - Value : F279
    - PK,FK (SUPGLD.SUPSUPCD), [SUPGLD](P4P_SUPGLD_00.md)
    - 說明 : supplierCode
    - comment : Supplier Code
  - SUACLCD
    - Value : CONS
    - PK,FK (ATTVAL.ATTCD), [ATTVAL](P4P_ATTVAL_00.md)
    - 說明 : attClassCode
    - comment : Attribute Class Code
  - SUACD
    - Value : C00
    - PK,FK (ATTVAL.ATTCD), [ATTVAL](P4P_ATTVAL_00.md)
    - 說明 : attValueCode
    - comment : Attribute Value Code
  - SUASDATE
    - Value : 2009-05-08 00:00:00.0
    - PK
    - 說明 : suppAttStartDate
    - comment : Start Date
  - SUAALPH
    - Value : null
    - 說明 : suppAttAlph
    - comment : Alphanumeric value
  - SUANUM
    - Value : 0
    - 說明 : suppAttNumber
    - comment : Number value
  - SUADATE
    - Value : null
    - 說明 : suppAttDate
    - comment : Date
  - SUATIME
    - Value : null
    - 說明 : suppAttTime
    - comment : Time
  - SUAEDATE
    - Value : 2049-12-31 00:00:00.0
    - 說明 : suppAttEndDate
    - comment : End Date
  - SUACRE
    - Value : 2009-05-08 19:00:00.0
    - 說明 : cred
    - comment : Creation Date
  - SUACREUSR
    - Value : MIGRATION
    - 說明 : creUser
    - comment : Creation User
  - SUAUPD
    - Value : 2009-09-01 10:51:50.0
    - 說明 : lastUpd
    - comment : Date of last update
  - SUAUSR
    - Value : SSFIX_1041
    - 說明 : lastUser
    - comment : Last User
