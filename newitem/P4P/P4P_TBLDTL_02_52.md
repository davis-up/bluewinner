# TBLDTL 52 Location ID in store 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '52'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|52|Location ID in store|Location ID in store|C1 = Migration(M),Sale(S),All(A)|5|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '52'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|52|E|E-commerce|E-commerce|2|null|null|null|null|E|null|null|null|null|null|2015-01-28 22:31:38.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 05|52|L|Global Location|Global Location|2|null|null|null|null|A|null|null|null|null|null|2010-07-30 14:11:34.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 05|52|O|Outside Storage|Outside Storage|2|null|null|null|null|null|null|null|null|null|null|2010-06-14 17:28:25.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 05|52|R|In-store Storage|In-store Storage|2|null|null|null|null|null|null|null|null|null|null|2010-06-14 17:27:53.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 05|52|S|Sales Area|Sales Area|2|null|null|null|null|null|null|null|null|null|null|2010-06-14 17:28:08.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

