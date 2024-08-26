
# MSTMS


```sql
   
    SELECT * FROM MSTMS
     FETCH FIRST 10 ROWS ONLY

```

|SEQ|MSTDPCD|MSTMSCD|MSTEDESC|MSTLDESC|MSTPARENT|MSTLEVEL|MSTSQTY|MSTMAXC|MSTTOL|MSTTAR|MSTCRE|MSTUPD|MSTUSR|MSTCREUSR|MSTMRK|MSTMAXO|MSTUNIT|MSTSHELFLIMIT|MSTSHELFLIMITUOM|MSTSTKDPCT|MSTLGREQ|MSTLICNFLG|MSTLICNTYPE|MSTWEIGHTCONTROL|MSTSHELFLIFEFLAG|MSTSHELFLIFELMTFLAG|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 10|10|0|Soft Drinks|飲料|null|1|null|null|null|null|2009-05-08 19:00:00.0|2011-01-03 16:50:19.0|SS-FIX4710|MIGRATION|null|null|null|null|null|null|null|null|null|null|null|null|
|02 / 10|10|00|Carbonate|碳酸飲料|0|2|null|null|null|null|2009-05-08 19:00:00.0|2011-01-03 16:50:19.0|SS-FIX4710|MIGRATION|null|null|null|null|null|null|null|null|null|null|null|null|
|03 / 10|10|000|Cola|可樂|00|3|10|100|0|0|2009-05-08 19:00:00.0|2013-11-13 19:07:49.0|F000001609|MIGRATION|null|3000|B|null|null|null|0|null|null|Y|Y|Y|
|04 / 10|10|001|Tonic Ginger|碳酸汽水|00|3|13|100|0|0|2009-05-08 19:00:00.0|2013-11-13 19:07:49.0|F000001609|MIGRATION|null|2000|B|null|null|null|0|null|null|Y|Y|Y|
|05 / 10|10|002|Soda And Sarsaparilla|加味汽水及沙士|00|3|27|100|0|0|2009-05-08 19:00:00.0|2013-11-13 19:07:49.0|F000001609|MIGRATION|null|3000|B|null|null|null|0|null|null|Y|Y|Y|
|06 / 10|10|01|Fruit Juice|果汁|0|2|null|null|null|null|2009-05-08 19:00:00.0|2011-01-03 16:50:19.0|SS-FIX4710|MIGRATION|null|null|null|null|null|null|null|null|null|null|null|null|
|07 / 10|10|010|Mixed Vegetable Juice|混和蔬菜果汁|01|3|10|100|null|null|2009-05-08 19:00:00.0|2011-01-03 16:50:19.0|SS-FIX4710|MIGRATION|null|2000|B|null|null|null|null|null|null|Y|Y|Y|
|08 / 10|10|011|Apple Juice|蘋果汁|01|3|12|100|null|null|2009-05-08 19:00:00.0|2011-01-03 16:50:19.0|SS-FIX4710|MIGRATION|null|2000|B|null|null|null|null|null|null|Y|Y|Y|
|09 / 10|10|012|Orange Juice|柳橙汁|01|3|12|100|null|null|2009-05-08 19:00:00.0|2011-01-03 16:50:19.0|SS-FIX4710|MIGRATION|null|2000|B|null|null|null|null|null|null|Y|Y|Y|
|10 / 10|10|013|Grape Juice|葡萄汁|01|3|15|100|0|0|2009-05-08 19:00:00.0|2011-01-03 16:50:19.0|SS-FIX4710|MIGRATION|null|2000|B|null|null|null|null|null|null|Y|Y|Y|


- MSTMS [com.ss.c4.p4p.referential.model.MdStructureModel]
  - MSTDPCD
    - Value : 10
    - PK,FK (MSTDEP.MSDDPCD), [MSTDEP](P4P_MSTDEP_00.md)
    - 說明 : deptCode
    - 中文 : 部門代碼
    - comment : Department code
  - MSTMSCD
    - Value : 0
    - PK
    - 說明 : mdStructureCode
    - 中文 : 商品組織分類代碼
    - comment : Merchandise structure code
  - MSTEDESC
    - Value : Soft Drinks
    - 說明 : msEngDesc
    - 中文 : 英文名稱
    - comment : MS English description
  - MSTLDESC
    - Value : 飲料
    - 說明 : msLocalDesc
    - 中文 : 中文名稱
    - comment : MS Local description
  - MSTPARENT
    - Value : null
    - 說明 : msParent
    - comment : Parent MS
  - MSTLEVEL
    - Value : 1
    - 說明 : level
    - comment : 1=GFM, 2=FML,3=SFM
  - MSTSQTY
    - Value : null
    - 說明 : structureQty
    - comment : No. of items as plan (only input at SFM level and sum up to upper level)
  - MSTMAXC
    - Value : null
    - 說明 : maxCommercMargin
    - comment : Max Commercial Margin% (only input in Sub Family level)
  - MSTTOL
    - Value : null
    - 說明 : sellingPriceTolerance
    - comment : Selling Price Tolerance% (only input in Sub Family level)
  - MSTTAR
    - Value : null
    - 說明 : targetMargin
    - comment : Target Margin% (only input in Sub Family level)
  - MSTCRE
    - Value : 2009-05-08 19:00:00.0
    - 說明 : cred
    - comment : Creation date
  - MSTUPD
    - Value : 2011-01-03 16:50:19.0
    - 說明 : lastUpd
    - comment : Date of last update
  - MSTUSR
    - Value : SS-FIX4710
    - 說明 : lastUser
    - comment : Last user
  - MSTCREUSR
    - Value : MIGRATION
    - 說明 : creUser
    - comment : Creation User
  - MSTMRK
    - Value : null
    - 說明 : markUp
    - comment : Mark up % (only input in Family level)
  - MSTMAXO
    - Value : null
    - 說明 : maxOrderQty
    - comment : Maximum Order Quantity
  - MSTUNIT
    - Value : null
    - 說明 : unitOfMeasure
    - comment : Unit of Measure*Table 53
  - MSTSHELFLIMIT
    - Value : null
    - 說明 : shelfLifeMST
    - comment : Shelf life limit of store receiving
  - MSTSHELFLIMITUOM
    - Value : null
    - 說明 : shelfLifeUOMMST
    - comment : Shelf life limit unit * table 54
  - MSTSTKDPCT
    - Value : null
    - 說明 : stockDay
  - MSTLGREQ
    - Value : null
    - comment : Logistic box define (Y/N)
  - MSTLICNFLG
    - Value : null
    - comment : License flag (Y/N)
  - MSTLICNTYPE
    - Value : null
    - comment : License Type *Table 760
  - MSTWEIGHTCONTROL
    - Value : null
    - 中文 : mstweightcontrol
    - comment : Weight Control Flag
  - MSTSHELFLIFEFLAG
    - Value : null
    - 中文 : mdhShelfLifeFlag
  - MSTSHELFLIFELMTFLAG
    - Value : null
    - 中文 : mdhShelfLifeLimitFlag
