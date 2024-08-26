# TBLDTL 29 銷售碼 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '29'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|29|Unit Code|銷售碼|N1 = Applicable for Retail Qty|99|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '29'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 40|29|01|Single|單|2|1|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|02 / 40|29|02|Twin|雙|2|2|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|03 / 40|29|03|Three|三|2|3|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|04 / 40|29|04|Four|四|2|4|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|05 / 40|29|05|Five|五|2|5|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|06 / 40|29|06|Half Dozen|六/半打|2|6|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|07 / 40|29|07|Seven|七|2|7|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|08 / 40|29|08|Eight|八|2|8|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|09 / 40|29|09|Nine|九|2|9|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|10 / 40|29|10|Ten|十|2|10|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|11 / 40|29|11|Eleven|十一|2|11|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|12 / 40|29|12|One Dozen|十二/一打|2|12|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|13 / 40|29|13|Thirteen|十三|2|13|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|14 / 40|29|14|Fourteen|十四|2|14|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|15 / 40|29|15|Fifteen|十五|2|15|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|16 / 40|29|16|Sixteen|十六|2|16|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|17 / 40|29|17|Seventeen|十七|2|17|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|18 / 40|29|18|Eighteen|十八|2|18|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|19 / 40|29|19|Nineteen|十九|2|19|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|20 / 40|29|20|Twenty|二十|2|20|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|21 / 40|29|21|Twenty-One|二十一|2|21|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|22 / 40|29|22|Twenty-Two|二十二|2|22|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|23 / 40|29|23|Twenty-Three|二十三|2|23|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|24 / 40|29|24|TWO DOZENS|二十四/二打|2|24|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|25 / 40|29|25|Twenty-Five|二十五|2|25|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|26 / 40|29|26|Twenty-Six|二十六|2|26|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|27 / 40|29|27|Twenty-Seven|二十七|2|27|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|28 / 40|29|28|Twenty-Eight|二十八|2|28|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|29 / 40|29|29|Twenty-Nine|二十九|2|29|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|30 / 40|29|30|Thirty|三十|2|30|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|31 / 40|29|31|Thirty-One|三十一|2|31|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|32 / 40|29|32|Thirty-Two|三十二|2|32|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|33 / 40|29|33|Thirty-Three|三十三|2|33|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|34 / 40|29|34|Thirty-Four|三十四|2|34|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|35 / 40|29|35|Thirty-Five|三十五|2|35|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|36 / 40|29|36|THREE DOZEN|三十六/三打|2|36|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|37 / 40|29|37|Thirty-Seven|三十七|2|37|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|38 / 40|29|38|Thirty-Eight|三十八|2|38|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|39 / 40|29|39|Thirty-Nine|三十九|2|39|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|
|40 / 40|29|40|Fourty|四十|2|40|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 18:27:46.0|SSFIX_25550|

