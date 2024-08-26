# TBLDTL 640 Supplier pay group code desc 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '640'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|640|Supplier pay group code desc|null|TBDNUM1  : Default value of pay group for new supplier creation (0 = Default),TBDENTCD  : Supplier pays group code,TBDEDESC  : Supplier pays group description|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '640'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|640|101|Pay group description1|Pay group description1|2|null|null|null|null|null|null|null|null|null|null|2013-05-15 19:21:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 02|640|102|Pay group description2|Pay group description2|2|null|null|null|null|null|null|null|null|null|null|2013-05-15 19:21:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

