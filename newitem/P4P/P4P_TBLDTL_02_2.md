# TBLDTL 2 店型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '2'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|2|Store Type|店型態|Store Type|4|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '2'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 04|2|L|Logistic|Logistic|1|null|null|null|null|null|null|null|null|null|null|2007-05-23 15:10:20.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 04|2|M|Merchandise|Merchandise|1|null|null|null|null|null|null|null|null|null|null|2007-05-23 15:10:20.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|03 / 04|2|O|Office|Office|1|null|null|null|null|null|null|null|null|null|null|2007-05-23 15:10:20.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 04|2|S|Store|Store|1|null|null|null|null|null|null|null|null|null|null|2007-05-23 15:10:20.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

