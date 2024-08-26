# TBLDTL 38 收銀系統型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '38'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|38|Cashier System|收銀系統型態|Define type of cashier system that store uses.|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '38'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|38|C|Calypso|Calypso|2|null|null|null|null|null|null|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 03|38|S|SA|SA|2|null|null|null|null|null|null|null|null|null|null|2008-04-29 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|03 / 03|38|T|TPLinux|TPLinux|2|null|null|null|null|null|null|null|null|null|null|2013-10-03 18:45:39.0|2015-05-29 19:00:49.0|SSFIX_25550|

