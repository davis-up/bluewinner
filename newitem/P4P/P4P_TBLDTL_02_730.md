# TBLDTL 730 促銷進價供應商顯示設定 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '730'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|730|Show supplier on PPP grid|促銷進價供應商顯示設定|Show supplier on PPP grid|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '730'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|730|01|Logistic item|Logistic item|1|null|null|null|null|1|null|null|null|null|null|2013-01-18 10:45:16.0|2013-08-22 20:48:35.0|WF-TEST|
|02 / 02|730|02|Normal item|Normal item|1|null|null|null|null|1|null|null|null|null|null|2013-01-18 10:45:16.0|2013-08-22 20:48:35.0|WF-TEST|

