# TBLDTL 7 敏感性商品碼 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '7'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|7|Sensitiveness Code|敏感性商品碼|To show how sensitive the selling price is|8|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '7'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 08|7|0|Temp|Temp|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 08|7|1|VS-Unbeatable / Top 100 Red|VS-無敵商品/百大紅色商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2016-05-16 13:39:18.0|F000033546|
|03 / 08|7|2|HW-HousewifeWallet/SeasonalSensitivity|HW-主婦荷包/季節性敏感|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 08|7|3|LP-Everyday Low Price/In Promotion|LP-天天便宜促銷|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 08|7|4|NS-Non Sensitivity/Normal Comparable|NS-非敏感可比較|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|06 / 08|7|5|NC-Non Comparable|NC-不可比較商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|07 / 08|7|6|HC-Housewife Wallet by City|HC-區域主婦荷包|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|08 / 08|7|A|RM-Raw Material|RM-原物料|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

