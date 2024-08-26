# TBLDTL 9006 允收天數計算式 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '9006'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|9006|Shelf Life Limit Formula|允收天數計算式|Shelf Life Limit Formula|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '9006'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|9006|1|Local shelf life limit|本地允收公式|2|3|2|null|null|null|null|null|null|null|null|2023-02-15 18:03:10.0|2023-02-15 21:30:43.0|CRID0640|
|02 / 02|9006|2|Import shelf life limit|進口允收公式|2|2|1|null|null|null|null|null|null|null|null|2023-02-15 18:03:10.0|2023-02-15 21:30:43.0|CRID0640|

