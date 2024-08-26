# TBLDTL 54 Unit of Measure of Shelf Life Limit 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '54'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|54|Unit of Measure of Shelf Life Limit|Unit of Measure of Shelf Life Limit|Define unit of measure of shelf life limit.|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '54'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|54|D|Days|Days|2|1|null|null|null|null|null|null|null|null|null|2012-08-30 18:33:49.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 02|54|P|Percent (%)|Percent (%)|2|null|null|null|null|null|null|null|null|null|null|2012-08-30 18:33:49.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

