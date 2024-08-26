# TBLDTL 28 販賣方式 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '28'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|28|Sold by|販賣方式|Define sold weight product by piece or weight.|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '28'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|28|0|Weight|Weight|2|null|null|null|null|null|null|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 02|28|1|Piece|Piece|2|null|null|null|null|null|null|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

