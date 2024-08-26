# TBLDTL 51 Alert color before cut-off time 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '51'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|51|Alert color before cut-off time|cut-off time警示顏色|TBDENTCD  : The color code,TBDEDESC  : The color description|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '51'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|51|1|Green|Green|2|null|null|null|null|null|null|null|null|null|null|2010-05-20 00:57:10.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 03|51|2|Blue|Blue|2|null|null|null|null|null|null|null|null|null|null|2010-05-20 00:57:10.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 03|51|3|Red|Red|2|null|null|null|null|null|null|null|null|null|null|2010-05-20 00:57:10.0|2015-05-29 19:00:49.0|SSFIX_25550|

