# TBLDTL 5 銷售型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '5'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|5|Type of sales|銷售型態|N1 = Default SC value, C1 = Attribute code for consignment,TBDCHA2 = Y , then it is allowed to create order through the HHT Order On Demand function;TBDCHA2 =N or blank, then it is NOT allowed to create order|33|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '5'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 33|5|0|Nat Brand Return Except Sample|品牌性可退貨商品樣品除外|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|02 / 33|5|1|Nat. Brand Non Returnable|品牌性商品但不可退貨|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|03 / 33|5|2|Nat. Brand Returnable|品牌性商品並可退貨|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|04 / 33|5|3|International Non Returnable|有國際合約商品但不可退貨|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|05 / 33|5|4|International Returnable|有國際合約商品並可退貨|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|06 / 33|5|5|Import|進口商品(經由後勤進口部)|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|07 / 33|5|6|Local|區域性商品|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|08 / 33|5|7|Consignment|寄賣商品|2|0|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|09 / 33|5|8|Supplier Catalogue|廠商型錄販賣商品|2|0|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|10 / 33|5|9|Clearance Sales|出清商品|2|null|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|11 / 33|5|A|Virtual|虛設單品|2|0|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|12 / 33|5|B|Central Display|集中陳列商品|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|13 / 33|5|C|Carrefour Item|家福商品|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|14 / 33|5|D|Carrefour Discount|家福超值|2|null|null|null|null|null|Y|null|null|null|null|2011-12-28 10:23:15.0|2021-05-25 23:53:56.0|SYSTEM|
|15 / 33|5|E|Consignment (DC)|寄賣商品 (DC)|2|null|null|null|null|null|N|null|null|null|null|2015-11-18 10:43:16.0|2021-05-25 23:53:56.0|SYSTEM|
|16 / 33|5|F|No.1 Item|超低價商品|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|17 / 33|5|G|Raw Material (No Sales)|生鮮原物料 (非販賣用)|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2023-02-22 11:00:21.0|F000172066|
|18 / 33|5|H|Processed Item (No Purchase)|生鮮自製品 (非進貨用)|2|0|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2023-02-22 11:00:00.0|F000172066|
|19 / 33|5|I|Fresh Processed Food Sticker|生鮮加工貼紙用|2|null|null|null|null|null|N|null|null|null|null|2020-04-09 09:26:20.0|2021-05-25 23:53:56.0|SYSTEM|
|20 / 33|5|J|Booking Return Except Sample|預結可退貨商品樣品除外|2|0|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|21 / 33|5|K|Booking Non Returnable|預結商品但不可退貨|2|0|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|22 / 33|5|L|Booking Returnable|預結商品可退貨|2|0|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|23 / 33|5|M|Mix CON/DC|混合進貨方式|2|null|null|null|null|null|Y|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|24 / 33|5|O|Organic|有機商品|2|null|null|null|null|null|Y|null|null|null|null|2013-05-20 09:46:55.0|2021-05-25 23:53:56.0|SYSTEM|
|25 / 33|5|P|Carrefour Premium|家福精選|2|null|null|null|null|null|Y|null|null|null|null|2011-12-28 10:23:45.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|26 / 33|5|R|Reserved Brand|家福超值獨賣品牌|2|null|null|null|null|null|Y|null|null|null|null|2012-07-19 18:38:28.0|2021-05-25 23:53:56.0|SYSTEM|
|27 / 33|5|S|Service|服務費單品|2|0|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|28 / 33|5|T|B2B Item|B2B 專用商品|2|null|null|null|null|null|N|null|null|null|null|2017-11-08 18:09:16.0|2021-05-25 23:53:56.0|SYSTEM|
|29 / 33|5|U|Group Buy|團購商品|2|0|null|null|null|null|N|null|null|null|null|2020-11-03 17:36:28.0|2021-05-25 23:53:56.0|SYSTEM|
|30 / 33|5|V|Virtual Top-Up|虛擬儲值|2|null|null|null|null|null|N|null|null|null|null|2009-03-27 00:00:00.0|2021-05-25 23:53:56.0|SYSTEM|
|31 / 33|5|W|Shiraz|Shiraz|2|null|null|null|null|null|Y|null|null|null|null|2021-01-04 13:38:58.0|2021-05-25 23:53:56.0|SYSTEM|
|32 / 33|5|Y|Jasons|Jasons|2|null|null|null|null|null|Y|null|null|null|null|2021-07-26 09:18:58.0|2021-07-26 09:18:58.0|victorshih|
|33 / 33|5|Z|Exclusive Item For EC|EC獨賣商品|2|null|null|null|null|null|Y|null|null|null|null|2017-02-08 17:08:52.0|2021-05-25 23:53:56.0|SYSTEM|

