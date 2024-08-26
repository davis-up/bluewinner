# TBLDTL 636 供應商付款條件 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '636'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|636|Supplier Payment Term|供應商付款條件|To define payment term based on goods receiving date or invoice date.|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '636'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|636|0|Good receiving|Good receiving|2|null|null|null|null|G|null|null|null|null|null|2010-12-22 20:21:03.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 03|636|1|Invoice Date|Invoice Date|2|null|null|null|null|I|null|null|null|null|null|2010-12-22 20:21:03.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 03|636|2|Invoice Receiving Date|Invoice Receiving Date|2|null|null|null|null|IR|null|null|null|null|null|2010-12-22 20:21:03.0|2015-05-29 19:00:49.0|SSFIX_25550|

