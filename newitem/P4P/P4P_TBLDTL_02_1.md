# TBLDTL 1 區域碼 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '1'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|1|Region Code|區域碼|Region Code|51|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '1'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 40|1|0|General Office|一般辦公室|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 40|1|1|Taipei North Region|北北區|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 40|1|10|South 1 Area|南區 第一區|2|null|null|null|null|null|null|null|null|null|null|2017-07-03 17:51:47.0|2021-05-13 17:08:21.0|L2_MD_8113|
|04 / 40|1|11|South 2 Area|南區 第二區|2|null|null|null|null|null|null|null|null|null|null|2018-07-02 15:26:48.0|2021-05-13 17:08:21.0|L2_MD_8113|
|05 / 40|1|12|South 3 Area|南區 第三區|2|null|null|null|null|null|null|null|null|null|null|2020-12-24 15:17:39.0|2021-05-13 17:08:21.0|L2_MD_8113|
|06 / 40|1|13|AS01 Area|AS01 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:14:48.0|2021-05-13 17:08:21.0|L2_MD_8113|
|07 / 40|1|14|AS02 Area|AS02 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:15:22.0|2021-05-13 17:08:21.0|L2_MD_8113|
|08 / 40|1|15|AS03 Area|AS03 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:15:48.0|2021-05-13 17:08:21.0|L2_MD_8113|
|09 / 40|1|16|AS04 Area|AS04 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:16:11.0|2021-05-13 17:08:21.0|L2_MD_8113|
|10 / 40|1|17|AS05 Area|AS05 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:16:33.0|2021-05-13 17:08:21.0|L2_MD_8113|
|11 / 40|1|18|AS06 Area|AS06 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:16:58.0|2021-05-13 17:08:21.0|L2_MD_8113|
|12 / 40|1|19|AS07 Area|AS07 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:17:23.0|2021-05-13 17:08:21.0|L2_MD_8113|
|13 / 40|1|2|Taipei South Region|北南區|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|14 / 40|1|20|AS08 Area|AS08 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:17:48.0|2021-05-13 17:08:21.0|L2_MD_8113|
|15 / 40|1|21|AS09 Area|AS09 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:18:18.0|2021-05-13 17:08:21.0|L2_MD_8113|
|16 / 40|1|22|AS10 Area|AS10 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:18:53.0|2021-05-13 17:08:21.0|L2_MD_8113|
|17 / 40|1|23|AS11 Area|AS11 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:19:12.0|2021-05-13 17:08:21.0|L2_MD_8113|
|18 / 40|1|24|AS12 Area|AS12 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:19:45.0|2021-05-13 17:08:21.0|L2_MD_8113|
|19 / 40|1|25|AS13 Area|AS13 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:20:07.0|2021-05-13 17:08:21.0|L2_MD_8113|
|20 / 40|1|26|AS14 Area|AS14 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:20:43.0|2021-05-13 17:08:21.0|L2_MD_8113|
|21 / 40|1|27|JR1 Area|JR1 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:21:17.0|2021-05-11 18:11:41.0|L2_MD_8113|
|22 / 40|1|28|JR2 Area|JR2 Area|2|null|null|null|null|null|null|null|null|null|null|2021-01-12 11:21:35.0|2021-05-11 18:11:41.0|L2_MD_8113|
|23 / 40|1|29|A01 Area|A01 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:54:36.0|2021-10-28 10:54:36.0|victorshih|
|24 / 40|1|3|Central Region|中區|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|25 / 40|1|30|A02 Area|A02 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:54:52.0|2021-10-28 10:54:52.0|victorshih|
|26 / 40|1|31|A03 Area|A03 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:55:08.0|2021-10-28 10:55:08.0|victorshih|
|27 / 40|1|32|A04 Area|A04 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:55:27.0|2021-10-28 10:55:27.0|victorshih|
|28 / 40|1|33|A05 Area|A05 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:55:51.0|2021-10-28 10:55:51.0|victorshih|
|29 / 40|1|34|A06 Area|A06 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:56:11.0|2021-10-28 10:56:11.0|victorshih|
|30 / 40|1|35|A07 Area|A07 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:56:45.0|2021-10-28 10:56:45.0|victorshih|
|31 / 40|1|36|A08 Area|A08 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:57:15.0|2021-10-28 10:57:15.0|victorshih|
|32 / 40|1|37|A09 Area|A09 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:57:37.0|2021-10-28 10:57:37.0|victorshih|
|33 / 40|1|38|A10 Area|A10 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:58:03.0|2021-10-28 10:58:03.0|victorshih|
|34 / 40|1|39|A11 Area|A11 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:58:27.0|2021-10-28 10:58:27.0|victorshih|
|35 / 40|1|4|South Region|南區|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|36 / 40|1|40|A12 Area|A12 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:58:45.0|2021-10-28 10:58:45.0|victorshih|
|37 / 40|1|41|A13 Area|A13 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:59:03.0|2021-10-28 10:59:03.0|victorshih|
|38 / 40|1|42|A14 Area|A14 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:59:27.0|2021-10-28 10:59:27.0|victorshih|
|39 / 40|1|43|A15 Area|A15 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 10:59:49.0|2021-10-28 10:59:49.0|victorshih|
|40 / 40|1|44|A16 Area|A16 Area|2|null|null|null|null|null|null|null|null|null|null|2021-10-28 11:00:10.0|2021-10-28 11:00:10.0|victorshih|

