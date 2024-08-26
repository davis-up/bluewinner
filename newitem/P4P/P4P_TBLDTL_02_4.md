# TBLDTL 4 售價型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '4'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|4|Selling Price Type|售價型態|C1 = Controlled by Merchandise or Store - M/S|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '4'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|4|G|Green Item|售價由商品部控制|2|null|null|null|null|M|SUP|null|null|null|null|2009-03-27 00:00:00.0|2016-10-13 09:35:36.0|F000033546|
|02 / 02|4|R|Red Item|售價由各店自行決定|2|null|null|null|null|S|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

