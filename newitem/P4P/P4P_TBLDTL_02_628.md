# TBLDTL 628 Specific Supplier 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '628'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|628|Specific Supplier|null|To define Specific Supplier (Maximum length of TBDENTCD is 1 character).|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '628'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|628|1|Direct|Direct|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 03|628|2|Wholesale|Wholesale|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 03|628|3|Import|Import|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

