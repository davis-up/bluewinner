# TBLDTL 716 重量單位 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '716'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|716|Weight Unit|重量單位|Weight Unit|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '716'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|716|cm|Centimeter|公分|2|null|null|null|null|null|null|null|null|null|null|2014-02-19 17:46:36.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 03|716|m|meter|公尺|2|null|null|null|null|null|null|null|null|null|null|2014-09-25 15:36:57.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 03|716|mm|millimeter|公厘|2|null|null|null|null|null|null|null|null|null|null|2014-02-14 14:33:17.0|2015-05-29 19:00:49.0|SSFIX_25550|

