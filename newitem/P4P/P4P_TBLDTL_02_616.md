# TBLDTL 616 Typology – Typology and Concept 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '616'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|616|Typology – Typology and Concept|Typology – Typology and Concept|TBDENTCD  Typology code,TBDNUM1  Level of Typology code for calculating accumulate item |29|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '616'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 29|616|1J|1J|1J|2|null|null|null|null|SUP|JSN|null|null|null|null|2022-08-20 16:42:17.0|2022-08-20 16:42:17.0|ibmsupport|
|02 / 29|616|1S|1S|1S|2|null|null|null|null|SUP|SUP|null|null|null|null|2015-01-28 10:18:49.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 29|616|1U|1U|1U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:02:18.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|04 / 29|616|2J|2J|2J|2|null|null|null|null|SUP|JSN|null|null|null|null|2022-08-20 16:42:17.0|2022-08-20 16:42:17.0|ibmsupport|
|05 / 29|616|2S|2S|2S|2|null|null|null|null|SUP|SUP|null|null|null|null|2015-01-28 10:19:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|06 / 29|616|2U|2U|2U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:02:55.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|07 / 29|616|3J|3J|3J|2|null|null|null|null|SUP|JSN|null|null|null|null|2022-08-20 16:42:17.0|2022-08-20 16:42:17.0|ibmsupport|
|08 / 29|616|3S|3S|3S|2|null|null|null|null|SUP|SUP|null|null|null|null|2015-01-28 10:19:13.0|2015-05-29 19:00:49.0|SSFIX_25550|
|09 / 29|616|3U|3U|3U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:03:20.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|10 / 29|616|4J|4J|4J|2|null|null|null|null|SUP|JSN|null|null|null|null|2022-08-20 16:42:17.0|2022-08-20 16:42:17.0|ibmsupport|
|11 / 29|616|4S|4S|4S|2|null|null|null|null|SUP|SUP|null|null|null|null|2018-10-02 18:01:39.0|2018-10-02 18:01:39.0|victorshih|
|12 / 29|616|4U|4U|4U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:03:45.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|13 / 29|616|5J|5J|5J|2|null|null|null|null|SUP|JSN|null|null|null|null|2022-08-20 16:42:17.0|2022-08-20 16:42:17.0|ibmsupport|
|14 / 29|616|5S|5S|5S|2|null|null|null|null|SUP|SUP|null|null|null|null|2018-10-02 18:02:03.0|2018-10-02 18:02:03.0|victorshih|
|15 / 29|616|5U|5U|5U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:04:18.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|16 / 29|616|6S|6S|6S|2|null|null|null|null|SUP|SUP|null|null|null|null|2020-05-11 14:37:02.0|2020-05-11 14:37:02.0|victorshih|
|17 / 29|616|6U|6U|6U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:04:39.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|18 / 29|616|7U|7U|7U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:05:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|19 / 29|616|8U|8U|8U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:05:18.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|20 / 29|616|9U|9U|9U|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:05:40.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|21 / 29|616|B|B|B|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:06:04.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|22 / 29|616|M|M|M|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:06:34.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|23 / 29|616|MIN|MIN|MIN|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:07:19.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|24 / 29|616|MOST|MOST|MOST|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:08:06.0|2015-05-29 19:00:49.0|SSFIX_25550|
|25 / 29|616|MOSTJSN|MOSTJSN|MOSTJSN|2|null|null|null|null|SUP|JSN|null|null|null|null|2022-08-20 16:42:17.0|2022-08-20 16:42:17.0|ibmsupport|
|26 / 29|616|MOSTSUP|MOSTSUP|MOSTSUP|2|null|null|null|null|SUP|SUP|null|null|null|null|2015-01-28 10:20:17.0|2015-05-29 19:00:49.0|SSFIX_25550|
|27 / 29|616|S|S|S|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:06:56.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|28 / 29|616|SUP|SUP|SUP|2|null|null|null|null|HYP|HYP|null|null|null|null|2012-05-01 03:07:43.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|29 / 29|616|XS|XS|XS|2|null|null|null|null|SUP|SUP|null|null|null|null|2016-12-22 09:50:44.0|2016-12-22 09:50:44.0|F000033546|

