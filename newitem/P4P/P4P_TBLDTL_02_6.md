# TBLDTL 6 季節代碼 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '6'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|6|Season Code|季節代碼|N1 = Default SC value. TBDCHA3: To maintain the number of days to be considered for the advanced average sales calculation.|18|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '6'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 18|6|0|Permanent|永久常置性|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|02 / 18|6|1|Perm. Opt. (CON+CAT)|永久選擇性|2|0|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|03 / 18|6|2|Temporary|暫時性(尚未定義好)|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|04 / 18|6|3|One Shot Promotion Item|促銷檔期性商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|05 / 18|6|4|Winter Item|冬季商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|06 / 18|6|5|Spring Item|春季商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|07 / 18|6|6|Summer Item|夏季商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|08 / 18|6|7|Fall Item|秋天商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|09 / 18|6|8|CNY|農曆過年節慶商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|10 / 18|6|9|Dragon Boat|端午節節慶商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|11 / 18|6|A|Moon Festival|中秋節節慶商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|12 / 18|6|B|Halloween|萬聖節節慶商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|13 / 18|6|C|Xmas|聖誕節節慶商品|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|14 / 18|6|D|Repeat Promotion|不定期促銷|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|15 / 18|6|F|Back To School Item|開學季商品|2|null|null|null|null|null|null|null|null|null|null|2010-03-17 14:46:40.0|2017-05-10 18:31:00.0|SYSTEM|
|16 / 18|6|J|Jasons|Jasons|2|null|null|null|null|null|null|null|null|null|null|2021-07-26 09:22:14.0|2021-07-26 09:22:14.0|victorshih|
|17 / 18|6|N|No1. Items|最低價品牌|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2017-05-10 18:31:00.0|SYSTEM|
|18 / 18|6|S|Shiraz|Shiraz|2|null|null|null|null|null|null|null|null|null|null|2020-12-24 10:45:07.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

