
# ATTVAL


```sql
   
    SELECT * FROM ATTVAL
     FETCH FIRST 10 ROWS ONLY

```

|SEQ|ATTCLCD|ATTCD|ATTSHORT|ATTDESC|ATTVTYP|ATTALPH|ATTNUM|ATTDATE|ATTTIME|ATTDEF|ATTCRE|ATTUPD|ATTUSR|ATTCREUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 10|STOD|OPN|Store Open Date|Open Date|3|null|null|2023-01-01 00:00:00.0|null|1|2009-03-27 00:00:00.0|2023-05-22 09:29:10.0|F000000959|MIGRATION|
|02 / 10|STCD|CLO|Store Closed Date|Store Last Sales Date|3|null|null|2049-12-31 00:00:00.0|null|0|2009-03-27 00:00:00.0|2023-04-24 11:02:11.0|F000000959|MIGRATION|
|03 / 10|CONS|C00|Consignment|Consignment Supplier/Item with Posting|2|null|0|null|null|1|2009-03-27 00:00:00.0|2018-11-14 18:31:17.0|CM11632|MIGRATION|
|04 / 10|CHKY|CAR|Carrefour|Carrefour|5|null|null|null|null|1|2009-03-27 00:00:00.0|2018-11-14 18:31:17.0|CM11632|MIGRATION|
|05 / 10|SAR|SAL|Sales Area|Sales Area in Square Meters|2|null|0|null|null|0|2009-03-27 00:00:00.0|2018-11-14 18:31:17.0|CM11632|MIGRATION|
|06 / 10|SAR|STA|Storage Area|Storage Area in Square Meters|2|null|0|null|null|0|2009-03-27 00:00:00.0|2018-11-14 18:31:17.0|CM11632|MIGRATION|
|07 / 10|CONS|7|7|7|2|null|0|null|null|0|2009-03-27 20:00:00.0|2018-11-14 18:31:17.0|CM11632|MIGRATION|
|08 / 10|IMP|Y|inv match for inter|inv matching for inter purchase|5|null|null|null|null|0|2010-03-31 15:39:37.0|2018-11-14 18:31:17.0|CM11632|F000001609|
|09 / 10|IMP|N|inv normatch to inte|inv no matching for inter purchase|5|null|null|null|null|1|2010-03-31 15:39:37.0|2018-11-14 18:31:17.0|CM11632|F000001609|
|10 / 10|UIMA|Y|Use IMA|Use IMA|5|null|null|null|null|0|2010-03-31 15:42:09.0|2018-11-14 18:31:17.0|CM11632|F000001609|


- ATTVAL [AttributeCodeModel]
  - ATTCLCD
    - Value : STOD
    - PK,FK (ATTCLASS.ATCCLCD), [ATTCLASS](P4P_ATTCLASS_00.md)
    - 說明 : attributeClassModel, [ATTCLASS](P4P_ATTCLASS_00.md)
    - comment : Attribute class code
  - ATTCD
    - Value : OPN
    - PK
    - 說明 : attrValCode
    - comment : Attribute Value Code
  - ATTSHORT
    - Value : Store Open Date
    - 說明 : attrValShortName
    - comment : Attribute Value Short Name
  - ATTDESC
    - Value : Open Date
    - 說明 : attrValName
    - comment : Attribute Value Name
  - ATTVTYP
    - Value : 3
    - 說明 : attrValType
    - comment : Value Type (1 = Alphanumeric Value, 2 = Number, 3 = Date, 4 = Time)
  - ATTALPH
    - Value : null
    - 說明 : attrValAlph
    - comment : Alphanumeric Value
  - ATTNUM
    - Value : null
    - 說明 : attrValNumber
    - comment : Number
  - ATTDATE
    - Value : 2023-01-01 00:00:00.0
    - 說明 : attrValDate
    - comment : Date
  - ATTTIME
    - Value : null
    - 說明 : attrValTime
    - comment : Time
  - ATTDEF
    - Value : 1
    - 說明 : attrValDef
    - comment : Is this value allocated to its link (item, supplier, store) by default during generation (1:yes, 0:no)
  - ATTCRE
    - Value : 2009-03-27 00:00:00.0
    - 說明 : cred
    - comment : Creation date
  - ATTUPD
    - Value : 2023-05-22 09:29:10.0
    - 說明 : lastUpd
    - comment : Date of last update
  - ATTUSR
    - Value : F000000959
    - 說明 : lastUser
    - comment : Last user
  - ATTCREUSR
    - Value : MIGRATION
    - 說明 : creUser
    - comment : Creation user


 # 寄賣列表


 ```sql
    
 SELECT ATTCD , ATTDESC , ATTSHORT
 FROM ATTVAL
 WHERE ATTCLCD = 'CONS'
 ORDER BY ATTCD


 ```

|SEQ|ATTCD|ATTSHORT|ATTDESC|
| -- | -- | -- | -- |
|01 / 03|7|7|7|
|02 / 03|C00|Consignment|Consignment Supplier/Item with Posting|
|03 / 03|C01|Consignment|Consignment Supplier/Item without Posting|

