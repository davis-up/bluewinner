# TBLDTL 634 進價計算基準 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '634'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|634|Purchase price based on|進價計算基準|C1 = Default Value for purchase price based on for creating new supplier|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '634'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|634|0|Order Date|Order Date|2|null|null|null|null|null|null|null|null|null|null|2008-09-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 02|634|1|Delivery Date|Delivery Date|2|null|null|null|null|null|null|null|null|null|null|2008-09-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

