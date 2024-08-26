# TBLDTL 718 預設稅別依店別 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '718'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|718|VAT by Store|預設稅別依店別|VAT by Store|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '718'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|718|006|006|006|2|1|null|null|null|null|null|null|null|null|null|2012-10-22 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|02 / 03|718|07K|07K|07K|2|0|null|null|null|null|null|null|null|null|null|2018-03-29 12:13:00.0|2018-03-29 12:13:16.0|victorshih|
|03 / 03|718|836|836|836|2|0|null|null|null|null|null|null|null|null|null|2023-10-02 13:31:32.0|2023-10-02 13:31:32.0|F000172054|

