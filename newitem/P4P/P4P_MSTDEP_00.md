
# MSTDEP

- `MSTDEP_部門` [2024-07-22 11:18]
  - MSDDPCD : 部門代號
  - MSDUSETYP : Typology Flag, typoFlag
  - MSDREQWEIGHT : deptWeight
  - MSDDVCD : [TBLDTL].TBDENTCD
- [[ST] WSReferential-department](https://wf-dev.int.uni-prosperity.com.tw/WSReferential/services/labelValue/department)


```sql
   
    SELECT * FROM MSTDEP
     --FETCH FIRST 10 ROWS ONLY

```

|SEQ|MSDDPCD|MSDEDESC|MSDLDESC|MSDDVCD|MSDSTAT|MSDCRE|MSDUPD|MSDUSR|MSDCREUSR|MSDAUTODEL|MSDISHIDACD|MSDREQWEIGHT|MSDUSECPM|MSDINCRNYC|MSDGENORD|MSDFULLPACK|MSDUSETYP|MSDSHELFLIMIT|MSDSHELFLIMITUOM|MSDUSETYPALLO|MSDCTRFG|MSDMTAX|MSDFNF|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 46|10|Beverages|菸酒飲料|1|1|2009-05-08 19:00:00.0|2021-09-15 13:12:18.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|02 / 46|11|Cleaning|家用清潔用品|1|1|2009-05-08 19:00:00.0|2021-09-24 13:38:44.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|03 / 46|12|Cosmetics|生活藥粧|1|1|2009-05-08 19:00:00.0|2021-09-24 13:38:44.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|0|N|N|null|
|04 / 46|14|Dry Grocery|乾性食品|1|1|2009-05-08 19:00:00.0|2021-11-11 15:38:53.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|05 / 46|15|Self-Service Perishables|日配食品|1|1|2009-05-08 19:00:00.0|2021-09-24 13:38:44.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|06 / 46|20|Ready To Eat|熟食課|2|1|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|1|0|N|Y|1|null|null|0|N|null|null|
|07 / 46|21|Fish|鮮魚課|2|1|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|1|0|N|Y|1|null|null|0|N|null|null|
|08 / 46|22|Fruit & Vegetables|蔬果課|2|1|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|1|0|N|Y|1|null|null|0|N|null|null|
|09 / 46|23|Bakery|麵包課|2|1|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|1|0|N|Y|1|null|null|0|N|null|null|
|10 / 46|24|Butchery|精肉課|2|1|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|1|0|N|Y|1|null|null|0|N|null|null|
|11 / 46|25|Dry Product|乾貨|2|1|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|1|0|N|Y|0|null|null|0|N|null|null|
|12 / 46|26|Restaurant|餐廳課|2|1|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|1|0|N|Y|0|null|null|0|N|null|null|
|13 / 46|30|Do-It-Yourself|自己動手做|3|1|2009-05-08 19:00:00.0|2018-07-30 09:41:31.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|14 / 46|31|Housekeeping|家用品貨|3|1|2009-05-08 19:00:00.0|2023-01-30 16:48:14.0|F000000959|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|15 / 46|32|Culture Stationery|文物書籍|3|1|2009-05-08 19:00:00.0|2018-07-30 09:41:31.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|16 / 46|33|Leisure|休閒用品|3|1|2009-05-08 19:00:00.0|2018-07-30 09:41:31.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|17 / 46|34|Gardening|園藝|3|1|2009-05-08 19:00:00.0|2018-07-30 09:41:31.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|18 / 46|35|Cars|汽車百貨|3|1|2009-05-08 19:00:00.0|2018-07-30 09:41:31.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|19 / 46|36|Car Service|汽車保養|3|1|2009-05-08 19:00:00.0|2018-07-30 09:41:31.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|0|null|null|0|N|N|null|
|20 / 46|40|Big Appliance|大家電|4|1|2009-05-08 19:00:00.0|2012-08-18 10:50:49.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|21 / 46|41|Small Household Appliance|小家電|4|1|2009-05-08 19:00:00.0|2012-08-18 10:50:48.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|22 / 46|42|Photo Cine Optical|光學/辦公室器材|4|1|2009-05-08 19:00:00.0|2012-08-18 10:50:47.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|23 / 46|43|HIFI Sound|音響|4|1|2009-05-08 19:00:00.0|2012-08-18 10:50:47.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|24 / 46|44|TV Video|電視/錄影機|4|1|2009-05-08 19:00:00.0|2012-08-18 10:50:46.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|25 / 46|45|Computers|電腦|4|1|2009-05-08 19:00:00.0|2012-05-26 10:18:24.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|26 / 46|46|Telephone Services & Appliance|電信服務|4|1|2009-05-08 19:00:00.0|2010-11-10 10:22:57.0|F000033546|MIGRATION|Y|1|N|1|0|N|Y|0|null|null|null|null|null|null|
|27 / 46|47|Maintenance Service|保養服務|4|1|2009-05-08 19:00:00.0|2018-05-31 12:11:25.0|victorshih|MIGRATION|Y|1|N|1|0|Y|N|0|null|null|0|N|N|null|
|28 / 46|48|Appliance Extention Warranty|家電延長保固|4|1|2009-05-08 19:00:00.0|2010-11-10 10:22:57.0|F000033546|MIGRATION|Y|1|N|1|0|N|Y|0|null|null|null|null|null|null|
|29 / 46|49|Appliance Service|家電服務|4|1|2009-05-08 19:00:00.0|2010-11-10 10:22:57.0|F000033546|MIGRATION|Y|1|N|1|0|N|Y|0|null|null|null|null|null|null|
|30 / 46|51|Fish (Raw Material)|鮮魚課(原料)|2|0|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|0|0|N|Y|0|null|null|0|N|null|null|
|31 / 46|52|F/V (Raw Material)|蔬果課(Raw Material)|2|0|2009-05-08 19:00:00.0|2015-05-05 09:27:08.0|F000033546|MIGRATION|Y|1|Y|0|0|N|Y|0|null|null|0|N|null|null|
|32 / 46|60|Shoes|鞋類|6|1|2009-05-08 19:00:00.0|2012-05-26 10:18:42.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|33 / 46|61|Permanent|一般性紡織品|6|1|2009-05-08 19:00:00.0|2012-07-21 11:43:25.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|34 / 46|62|Seasonal|季節性服飾|6|1|2009-05-08 19:00:00.0|2012-07-21 11:43:22.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|35 / 46|63|Jewelry|金飾|6|0|2009-05-08 19:00:00.0|2009-05-09 00:14:01.0|nellyng|MIGRATION|N|1|N|0|0|Y|N|0|null|null|null|null|null|null|
|36 / 46|65|Household Linen|紡織類家飾|6|1|2009-05-08 19:00:00.0|2023-01-30 16:47:52.0|F000000959|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|0|N|N|null|
|37 / 46|66|Personal Accessories|個人配件|6|1|2009-05-08 19:00:00.0|2021-09-24 13:39:03.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|0|N|N|null|
|38 / 46|72|Expense|會計|8|1|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|N|null|N|0|0|Y|N|0|null|null|null|null|null|null|
|39 / 46|79|Home Delivery|宅配外送|7|1|2009-05-08 19:00:00.0|2010-04-13 11:47:29.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|0|null|null|null|null|null|null|
|40 / 46|80|Management|管理課|8|1|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|N|null|N|0|0|Y|N|0|null|null|null|null|null|null|
|41 / 46|90|Computer|電腦課|9|0|2009-05-08 19:00:00.0|2009-05-08 19:00:00.0|MIGRATION|MIGRATION|N|null|N|0|0|Y|N|0|null|null|null|null|null|null|
|42 / 46|78|Gift Card Top Up Value|禮物卡加值金|7|1|2010-04-13 11:45:27.0|2010-04-13 11:46:20.0|victorshih|victorshih|Y|1|N|1|1|N|Y|0|null|null|null|null|null|null|
|43 / 46|76|Free goods and gifts| 贈品和禮品|7|1|2013-02-18 09:28:10.0|2024-03-12 11:18:25.0|F000172066|F000033546|Y|1|N|1|1|N|Y|0|null|null|0|N|N|null|
|44 / 46|75|Member & Financial Service|會員及金融服務|7|1|2013-11-07 10:06:43.0|2013-11-07 10:06:43.0|F000033546|F000033546|Y|1|N|1|1|N|Y|0|null|null|0|N|null|null|
|45 / 46|77|Service merchandise sales|服務銷售商品|7|1|2015-01-13 11:46:22.0|2024-03-12 11:18:25.0|F000172066|F000033546|Y|1|N|1|1|N|Y|0|null|null|0|N|N|null|
|46 / 46|50|Cross Border eCommerce-Grocery|境外電子商務-雜貨|1|1|2016-05-12 14:26:12.0|2017-08-29 16:21:42.0|F000000959|F000033546|Y|1|N|1|0|N|Y|1|null|null|0|N|N|null|


- MSTDEP [DepartmentModel]
  - MSDDPCD
    - Value : 10
    - PK
    - 說明 : code
    - 中文 : 部門代碼
    - comment : Department code
  - MSDEDESC
    - Value : Beverages
    - 說明 : engDesc
    - 中文 : 部門英文名稱
    - comment : Department English description
  - MSDLDESC
    - Value : 菸酒飲料
    - 說明 : localDesc
    - 中文 : 部門中文名稱
    - comment : Department Local description
  - MSDDVCD
    - Value : 1
    - FK (MSTDIV.MSVDVCD), [MSTDIV](P4P_MSTDIV_00.md)
    - 說明 : divisionCode
    - comment : Division code
  - MSDSTAT
    - Value : 1
    - 說明 : activeStatus
    - comment : Active Status (1-Yes, 0-No)
  - MSDCRE
    - Value : 2009-05-08 19:00:00.0
    - 說明 : cred
    - comment : Creation date
  - MSDUPD
    - Value : 2021-09-15 13:12:18.0
    - 說明 : lastUpd
    - comment : Date of last update
  - MSDUSR
    - Value : victorshih
    - 說明 : lastUser
    - comment : Last user
  - MSDCREUSR
    - Value : MIGRATION
    - 說明 : creUser
    - comment : Creation User
  - MSDAUTODEL
    - Value : Y
    - 說明 : autoDeleteFlag
    - comment : Automatic Delete Flag (Y/N)
  - MSDISHIDACD
    - Value : 1
    - 說明 : ishidaCode
    - comment : Weighting scale
  - MSDREQWEIGHT
    - Value : N
    - 說明 : requireInputWeight
    - 中文 : deptWeight
    - comment : To indicate whether the department is allowed to have weighted items (Y/N)
  - MSDUSECPM
    - Value : 1
    - 說明 : useCpm
    - 中文 : useCPM
    - comment : To indicate whether the order parameter in the particular department is using CMP to control. (0-NOT USED, 1-USED)
  - MSDINCRNYC
    - Value : 1
    - 說明 : includeRNYC
    - comment : To indicate whether order is using RNYC to calculate (1-Yes, 0-No)
  - MSDGENORD
    - Value : N
    - 說明 : genScheduleOrder
    - comment : To indicate whether automatic order generates when shelf capacity = 0 (Y/N)
  - MSDFULLPACK
    - Value : Y
    - 說明 : calCondition
    - comment : Calculated condition (Y/N) Y- Use the new rounding criteria on quantity per pack
  - MSDUSETYP
    - Value : 1
    - 說明 : useTyp
    - 中文 : useTyp
    - comment : To indicate all items under department are controlled by typology. (0-NOT USED, 1-USED)
  - MSDSHELFLIMIT
    - Value : null
    - 說明 : shelfLife
    - comment : Shelf life limit of store receiving
  - MSDSHELFLIMITUOM
    - Value : null
    - 說明 : shelfLifeUOM
    - [TBLDTL = 54 : Unit of Measure of Shelf Life Limit](P4P_TBLDTL_02_54.md)
    - comment : Shelf life limit unit * table 54
  - MSDUSETYPALLO
    - Value : 0
    - comment : To indicate at department level to define whether the department using space allocation. (0-NOT USED, 1-USED)
  - MSDCTRFG
    - Value : N
    - comment : Central return Flag (Y/N)
  - MSDMTAX
    - Value : N
    - comment : Multi-Tax Rate flag (Y/N)
  - MSDFNF
    - Value : null
    - [TBLDTL = 748 : Classify food or non food](P4P_TBLDTL_02_748.md)
    - comment : Classify food or non food department *Table 748
