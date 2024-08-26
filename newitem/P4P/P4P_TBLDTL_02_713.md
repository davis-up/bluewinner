# TBLDTL 713 後勤單品預設倉別 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '713'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|713|Defalut Supplier|後勤單品預設倉別|TBDENTCD : Warehouse supplier|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '713'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|713|B326|B326|B326|2|null|null|null|null|null|null|null|null|null|null|2012-05-22 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|02 / 02|713|G727|G727|G727|2|null|null|null|null|null|null|null|null|null|null|2024-04-29 09:42:44.0|2024-04-29 09:42:58.0|F000172066|

