# TBLDTL 633 後勤標示設定 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '633'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|633|Logistic Flag Setup|後勤標示設定|C1 = Available for business is owned by Carrefour (Y/N), C2 = Available for business is not owned by Carrefour (Y/N)|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '633'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|633|L|Logistic Center|Logistic Center|2|null|null|null|null|Y|Y|null|null|null|null|2008-09-08 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 03|633|P|Purchase Office|Purchase Office|2|null|null|null|null|Y|N|null|null|null|null|2008-09-08 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|03 / 03|633|S|Internal Transfer|Internal Transfer|2|null|null|null|null|Y|Y|null|null|null|null|2008-09-08 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

