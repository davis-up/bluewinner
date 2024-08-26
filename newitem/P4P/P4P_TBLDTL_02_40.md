# TBLDTL 40 庫存調整原因 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '40'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|40|Stock adjustment Reason|庫存調整原因|C1 = Adjust in=(+), Adjust out =(-), C2 = Include in gross margin Y=Yes, N=No, C3 = The movement type code for interface to Mandala, C4 = The movement type description for interface to Mandala, N1 = Adjust because of stock counting Y/N: 0 = No, 1 = Yes, N2 = 1, default adjustment code for stock adjustment created by HHT, N3 = 0 / blank, the adjustment reason code is applicable for all natures of items, = 1, the adjustment code cannot be selected for partnership items, = 2, the adjustment code cannot be selected for consignment items, = 3 the adjustment code cannot be selected for both partnership and consignment items.N4 = 0, send as UNKNOWN_LOSS, = 1, send as BK_ITEM_KNOWN_LOSS in PS BCI monthly interface|27|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '40'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 27|40|3|Inter Stores Transfer In|店間移撥 - 轉入|2|0|null|null|null|+|N|1|Inter Stores Transfer|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 27|40|4|Inter Stores Transfer Out|店間移撥 - 轉出|2|0|null|null|null|-|N|1|Inter Stores Transfer|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 27|40|5|RCV/RTN Adjustment|進/退貨庫存調整|2|1|null|null|null|+|N|7|Others|null|null|2009-03-27 00:00:00.0|2016-10-24 10:59:18.0|F000000959|
|04 / 27|40|6|Free Goods Thales|贈品Thales|2|0|null|null|null|+|Y|5|Free Product|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 27|40|7|Free Goods Minus Adjustment|贈品負調整|2|0|null|null|null|-|N|5|Free Product|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|06 / 27|40|8|Inter Department Transfer In|部門間移撥 - 轉入|2|null|null|null|null|+|Y|3|Inter Stores Transfer In|null|null|2011-06-20 17:55:34.0|2015-05-29 19:00:49.0|SSFIX_25550|
|07 / 27|40|9|Inter Department Transfer Out|部門間移撥 - 轉出|2|null|null|null|null|-|Y|4|Inter Stores Transfer Out|null|null|2011-06-20 17:56:07.0|2015-05-29 19:00:49.0|SSFIX_25550|
|08 / 27|40|B|Breakage|一般報廢|2|0|1|null|1|-|Y|6|Inventory|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|09 / 27|40|C|Cycle Count|週期盤點|2|1|null|null|0|+|Y|6|Inventory|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|10 / 27|40|D|Donate (Breakage)|捐贈(仍屬報廢)|2|0|null|null|1|-|Y|6|Inventory|null|null|2016-08-26 17:40:03.0|2017-11-24 16:07:05.0|F000000959|
|11 / 27|40|E|Expiry|即(過)期報廢|2|0|null|null|1|-|Y|6|Inventory|null|null|2016-10-17 13:45:06.0|2021-04-12 09:24:01.0|victorshih|
|12 / 27|40|F|Fall Back (Withdrawel)|下架報廢|2|0|null|null|1|-|Y|6|Inventory|null|null|2016-10-17 13:45:07.0|2017-11-24 16:08:14.0|F000000959|
|13 / 27|40|G|MD Requested|MD要求報廢|2|0|null|null|1|-|Y|6|Inventory|null|null|2016-10-17 13:45:07.0|2017-11-24 16:08:49.0|F000000959|
|14 / 27|40|H|Customer Return|顧客退貨(仍屬報廢)|2|0|null|null|null|-|Y|6|Inventory|null|null|2017-12-12 18:40:28.0|2017-12-12 18:40:28.0|F000000959|
|15 / 27|40|I|Inventory|大盤|2|1|null|null|0|+|Y|6|Inventory|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|16 / 27|40|K|Inter Location Transfer In|Inter Location Transfer In|2|0|null|null|null|+|N|3|Inter Stores Transfer In|null|null|2019-01-03 15:17:15.0|2019-01-08 10:59:20.0|F000000959|
|17 / 27|40|L|Inter Location Transfer Out|Inter Location Transfer Out|2|0|null|null|null|-|N|4|Inter Stores Transfer Out|null|null|2019-01-03 15:18:33.0|2019-01-08 10:59:05.0|F000000959|
|18 / 27|40|M|Adjustment from IMA|IMA調整|2|0|null|null|null|+|Y|6|Inventory|null|null|2010-03-31 13:55:26.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|19 / 27|40|N|Take Out Materials|生產原料領出|2|0|null|null|null|-|Y|9|Material requisition & Finished goods|null|null|2023-11-27 18:12:59.0|2023-11-27 18:12:59.0|F000172050|
|20 / 27|40|O|Product Entry|成品(半成品)入帳|2|0|null|null|null|+|Y|9|Material requisition & Finished goods|null|null|2023-11-27 18:13:56.0|2023-11-27 18:13:56.0|F000172050|
|21 / 27|40|P|Product Shipment|成品(半成品)出貨|2|0|null|null|null|-|Y|1|Inter Stores Transfer|null|null|2023-11-27 18:14:38.0|2023-12-06 15:24:06.0|F000172066|
|22 / 27|40|T|Theft|偷竊|2|0|null|null|1|-|Y|6|Inventory|null|null|2017-03-27 15:13:49.0|2017-11-24 16:09:09.0|F000000959|
|23 / 27|40|V|Adjustment For Sales Reversal|重收營業額銷售調整|2|0|null|null|null|+|N|R|Reversal Sales|null|null|2013-11-29 15:26:08.0|2015-05-29 19:00:49.0|SSFIX_25550|
|24 / 27|40|W|Adjustment For Clearance|出清調整|2|0|null|null|null|-|Y|6|Inventory|null|null|2014-09-19 09:18:00.0|2017-11-24 16:09:28.0|F000000959|
|25 / 27|40|X|Tasting|非贈品試吃報廢|2|0|null|null|null|-|Y|6|Inventory|null|null|2014-09-19 09:19:14.0|2017-11-24 16:09:39.0|F000000959|
|26 / 27|40|Y|Adjustment For Fresh Combination|生鮮改變型態調整|2|0|null|null|null|-|Y|6|Inventory|null|null|2014-09-19 09:21:04.0|2017-11-24 16:09:57.0|F000000959|
|27 / 27|40|Z|Adjustment For Consignment Item Sales|寄賣商品銷售調整|2|0|null|null|null|+|N|null|null|null|null|2011-09-04 11:19:10.0|2015-05-29 19:00:49.0|SSFIX_25550|

