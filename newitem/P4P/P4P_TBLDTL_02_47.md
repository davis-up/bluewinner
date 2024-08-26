# TBLDTL 47 Shelf Life UOM 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '47'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|47|Shelf Life UOM|Shelf Life UOM|N1 = Number of day for each UOM. N2 = Tolerance period of Manufacture and Expiry Date|5|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '47'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|47|D|Day|日|2|1|0|null|null|null|null|null|null|null|null|2008-08-20 16:43:34.0|2022-03-25 19:49:50.0|F000172050|
|02 / 05|47|H|Hour|小時|2|0.042|0|null|null|null|null|null|null|null|null|2008-08-20 16:43:34.0|2022-03-25 19:50:01.0|F000172050|
|03 / 05|47|M|Month|月|2|30|5|null|null|null|null|null|null|null|null|2016-02-24 13:27:22.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|04 / 05|47|W|Week|週|2|7|0|null|null|null|null|null|null|null|null|2008-08-20 16:43:34.0|2022-03-25 19:50:14.0|F000172050|
|05 / 05|47|Y|Year|年|2|365|5|null|null|null|null|null|null|null|null|2016-02-24 13:27:35.0|2020-11-20 11:20:54.0|CRID0483|

