# TBLDTL 1001 Control Supplier Frozen Process 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '1001'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|1001|Control Supplier Frozen Process|Control Supplier Frozen Process|Define parameter for supplier frozen process.If EC1, Char Value1 updated from Y to N, the suppliers in intermediate state of frozen process will not proceed any more. NUM Value 1~3 is blank or null,the corresponding job will fail to run.|1|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '1001'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|1001|1|Ctrl activate/de-activate frozen process|Ctrl activate/de-activate frozen process|2|120|7|1|null|Y|null|null|null|null|null|2021-01-06 22:21:59.0|2024-03-14 09:15:02.0|PMD-9017|

