# TBLDTL 538 特殊字元控制 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '538'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|538|Special Character|特殊字元控制|C1 = special character;C2 = To define as “1” if the special character maintained in CHA1 is applicable to remove from the Supplier related table details as well by CWF application|280|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '538'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 40|538|1|–|Special Character1|2|null|null|null|null|–|null|null|null|null|null|2011-03-08 10:54:11.0|2017-09-20 00:47:47.0|SYSTEM|
|02 / 40|538|10|坂|Special Character10|2|null|null|null|null|坂|null|null|null|null|null|2011-05-04 09:35:07.0|2017-09-20 00:47:47.0|SYSTEM|
|03 / 40|538|100|楽|Special Character100|2|null|null|null|null|楽|null|null|null|null|null|2016-05-17 11:08:00.0|2017-09-20 00:47:47.0|SYSTEM|
|04 / 40|538|101|寛|Special Character101|2|null|null|null|null|寛|null|null|null|null|null|2016-05-17 11:08:21.0|2017-09-20 00:47:47.0|SYSTEM|
|05 / 40|538|102|横|Special Character102|2|null|null|null|null|横|null|null|null|null|null|2016-05-17 11:08:46.0|2017-09-20 00:47:47.0|SYSTEM|
|06 / 40|538|103|廸|Special Character103|2|null|null|null|null|廸|null|null|null|null|null|2016-05-17 11:09:09.0|2017-09-20 00:47:47.0|SYSTEM|
|07 / 40|538|104|歳|Special Character104|2|null|null|null|null|歳|null|null|null|null|null|2016-05-18 10:28:25.0|2017-09-20 00:47:47.0|SYSTEM|
|08 / 40|538|105|黄|Special Character105|2|null|null|null|null|黄|null|null|null|null|null|2016-05-24 09:49:17.0|2017-09-20 00:47:47.0|SYSTEM|
|09 / 40|538|106|‧|Special Character106|2|null|null|null|null|‧|null|null|null|null|null|2016-05-30 15:55:47.0|2017-09-20 00:47:47.0|SYSTEM|
|10 / 40|538|107|缷|Special Character107|2|null|null|null|null|缷|null|null|null|null|null|2016-06-02 10:05:46.0|2017-09-20 00:47:47.0|SYSTEM|
|11 / 40|538|108|粧|Special Character108|2|null|null|null|null|粧|null|null|null|null|null|2016-06-02 16:24:43.0|2017-09-20 00:47:47.0|SYSTEM|
|12 / 40|538|109|酰|Special Character109|2|null|null|null|null|酰|null|null|null|null|null|2016-06-15 10:35:18.0|2017-09-20 00:47:47.0|SYSTEM|
|13 / 40|538|11|塩|Special Character11|2|null|null|null|null|塩|null|null|null|null|null|2011-05-04 09:35:26.0|2017-09-20 00:47:47.0|SYSTEM|
|14 / 40|538|110|沢|Special Characeter110|2|null|null|null|null|沢|null|null|null|null|null|2016-06-23 14:33:57.0|2017-09-20 00:47:47.0|SYSTEM|
|15 / 40|538|111|í|Special Character111|2|null|null|null|null|í|null|null|null|null|null|2016-07-21 10:19:05.0|2017-09-20 00:47:47.0|SYSTEM|
|16 / 40|538|112|腈|Special Character112|2|null|null|null|null|腈|null|null|null|null|null|2016-08-01 14:06:20.0|2017-09-20 00:47:47.0|SYSTEM|
|17 / 40|538|113|盗|Special Character113|2|null|null|null|null|盗|null|null|null|null|null|2016-08-01 14:06:59.0|2017-09-20 00:47:47.0|SYSTEM|
|18 / 40|538|114|麦|Special Character114|2|null|null|null|null|麦|null|null|null|null|null|2016-08-02 09:40:48.0|2017-09-20 00:47:47.0|SYSTEM|
|19 / 40|538|115|戸|Special Character115|2|null|null|null|null|戸|null|null|null|null|null|2016-08-12 09:27:04.0|2017-09-20 00:47:47.0|SYSTEM|
|20 / 40|538|116|・|Specail Character116|2|null|null|null|null|・|null|null|null|null|null|2016-08-22 12:00:31.0|2017-09-20 00:47:47.0|SYSTEM|
|21 / 40|538|117|犇|Special Character117|2|null|null|null|null|犇|null|null|null|null|null|2016-08-25 12:07:40.0|2017-09-20 00:47:47.0|SYSTEM|
|22 / 40|538|118|畑|Special Character118|2|null|null|null|null|畑|null|null|null|null|null|2016-08-25 12:08:02.0|2017-09-20 00:47:47.0|SYSTEM|
|23 / 40|538|119|倂|Special Character119|2|null|null|null|null|倂|null|null|null|null|null|2016-08-25 12:08:23.0|2017-09-20 00:47:47.0|SYSTEM|
|24 / 40|538|12|揾|Special Character12|2|null|null|null|null|揾|null|null|null|null|null|2011-05-04 09:35:44.0|2017-09-20 00:47:47.0|SYSTEM|
|25 / 40|538|120|緑|Special Character120|2|null|null|null|null|緑|null|null|null|null|null|2016-08-26 10:03:49.0|2017-09-20 00:47:47.0|SYSTEM|
|26 / 40|538|121|ō|Special Character121|2|null|null|null|null|ō|null|null|null|null|null|2016-08-29 09:51:14.0|2017-09-20 00:47:47.0|SYSTEM|
|27 / 40|538|122|覚|Special Character122|2|null|null|null|null|覚|null|null|null|null|null|2016-09-12 10:28:40.0|2017-09-20 00:47:47.0|SYSTEM|
|28 / 40|538|123|鲁|Special Character123|2|null|null|null|null|鲁|null|null|null|null|null|2016-09-12 10:29:10.0|2017-09-20 00:47:47.0|SYSTEM|
|29 / 40|538|124|浜|Special Character124|2|null|null|null|null|浜|null|null|null|null|null|2016-09-19 10:42:10.0|2017-09-20 00:47:47.0|SYSTEM|
|30 / 40|538|125|橮|Special Character125|2|null|null|null|null|橮|null|null|null|null|null|2016-09-23 09:27:52.0|2017-09-20 00:47:47.0|SYSTEM|
|31 / 40|538|126|Ø|Special Character216|2|null|null|null|null|Ø|null|null|null|null|null|2016-10-17 18:02:00.0|2017-09-20 00:47:47.0|SYSTEM|
|32 / 40|538|127|™|Special Character127|2|null|null|null|null|™|null|null|null|null|null|2016-10-27 11:08:07.0|2017-09-20 00:47:47.0|SYSTEM|
|33 / 40|538|128|蠺|Special Character128|2|null|null|null|null|蠺|null|null|null|null|null|2016-11-03 17:18:27.0|2017-09-20 00:47:47.0|SYSTEM|
|34 / 40|538|129|门|Special Character129|2|null|null|null|null|门|null|null|null|null|null|2016-11-10 15:39:16.0|2017-09-20 00:47:47.0|SYSTEM|
|35 / 40|538|13|敎|Special Character13|2|null|null|null|null|敎|null|null|null|null|null|2011-05-04 09:36:03.0|2017-09-20 00:47:47.0|SYSTEM|
|36 / 40|538|130|贴|Special Character130|2|null|null|null|null|贴|null|null|null|null|null|2016-11-10 15:39:47.0|2017-09-20 00:47:47.0|SYSTEM|
|37 / 40|538|131|芈|Special Character131|2|null|null|null|null|芈|null|null|null|null|null|2016-11-16 10:22:12.0|2017-09-20 00:47:47.0|SYSTEM|
|38 / 40|538|132|咔|Special Character132|2|null|null|null|null|咔|null|null|null|null|null|2016-11-18 15:49:01.0|2017-09-20 00:47:47.0|SYSTEM|
|39 / 40|538|133|ê|Special Character133|2|null|null|null|null|ê|null|null|null|null|null|2016-12-07 10:51:33.0|2017-09-20 00:47:47.0|SYSTEM|
|40 / 40|538|134|螨|Special Character134|2|null|null|null|null|螨|null|null|null|null|null|2016-12-08 10:27:51.0|2017-09-20 00:47:47.0|SYSTEM|

