# TBLDTL 727 單品修改申請預設店別 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '727'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|727|default Store release|單品修改申請預設店別|Default Store item modification|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '727'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|727|006|default Store item modification|Default Store item modification|2|1|null|null|null|null|null|null|null|null|null|2014-07-09 18:24:44.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 02|727|031|default Store item modification|Default Store item modification|2|1|null|null|null|null|null|null|null|null|null|2014-07-09 18:24:44.0|2015-05-29 19:00:49.0|SSFIX_25550|

