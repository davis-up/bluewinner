# TBLDTL 21 縣市 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '21'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|21|City|縣市|C1 = Parent Parameter No of Upper Level. 37-State/1-Region,C2 = Upper Level code|27|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '21'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 27|21|001|Taipei City|臺北市|2|null|null|null|null|1|1,2|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 27|21|002|Keelung  City|基隆市|2|null|null|null|null|1|0|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 27|21|003|New Taipei City|新北市|2|null|null|null|null|1|1,2|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 27|21|004|Yilan County|宜蘭縣|2|null|null|null|null|1|1|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 27|21|005|Hsinchu City|新竹市|2|null|null|null|null|1|3|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|06 / 27|21|006|Hsinchu County|新竹縣|2|null|null|null|null|1|3|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|07 / 27|21|007|Taoyuan City|桃園市|2|null|null|null|null|1|3|null|null|null|null|2009-03-27 00:00:00.0|2016-08-01 09:26:32.0|F000033546|
|08 / 27|21|008|Miaoli County|苗栗縣|2|null|null|null|null|1|3|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|09 / 27|21|009|Taichung City|臺中市|2|null|null|null|null|1|4|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|10 / 27|21|010|Taichung County|臺中縣|2|null|null|null|null|1|4|null|null|null|null|2013-05-31 11:47:57.0|2015-05-29 19:00:49.0|SSFIX_25550|
|11 / 27|21|011|Changhua County|彰化縣|2|null|null|null|null|1|6|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|12 / 27|21|012|Nantou County|南投縣|2|null|null|null|null|1|4|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|13 / 27|21|013|Chiayi City|嘉義市|2|null|null|null|null|1|5|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|14 / 27|21|014|Chiayi County|嘉義縣|2|null|null|null|null|1|5|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|15 / 27|21|015|Yunlin County|雲林縣|2|null|null|null|null|1|5|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|16 / 27|21|016|Tainan City|臺南市|2|null|null|null|null|1|5|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|17 / 27|21|017|Tainan County|臺南縣|2|null|null|null|null|1|5|null|null|null|null|2013-05-31 11:48:26.0|2015-05-29 19:00:49.0|SSFIX_25550|
|18 / 27|21|018|Kaohsiung City|高雄市|2|null|null|null|null|1|6|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|19 / 27|21|019|Kaohsiung County|高雄縣|2|null|null|null|null|1|6|null|null|null|null|2013-05-31 11:48:53.0|2015-05-29 19:00:49.0|SSFIX_25550|
|20 / 27|21|020|Penghu County|澎湖縣|2|null|null|null|null|1|0|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|21 / 27|21|021|Pingtung County|屏東縣|2|null|null|null|null|1|6|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|22 / 27|21|022|Taitung County|臺東縣|2|null|null|null|null|1|6|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|23 / 27|21|023|Hualien County|花蓮縣|2|null|null|null|null|1|5|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|24 / 27|21|024|Kinmen County|金門縣|2|null|null|null|null|1|0|0|null|null|null|2009-03-27 00:00:00.0|2018-03-26 18:39:02.0|victorshih|
|25 / 27|21|025|Lienchiang County|連江縣|2|null|null|null|null|1|0|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|26 / 27|21|026|南海諸島|南海諸島|2|null|null|null|null|1|0|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|27 / 27|21|027|釣魚台列嶼|釣魚台列嶼|2|null|null|null|null|1|0|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

