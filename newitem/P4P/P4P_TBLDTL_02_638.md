# TBLDTL 638 Supplier Partnership 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '638'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|638|Supplier Partnership|Supplier Partnership|TBDCHA1  Identify partnership supplier and consignment code.,TBDCHA2  Identify return created for consignment supplier or partnership supplier,TBDCHA3   Generate interface file (Y/N)|4|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '638'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 04|638|C00|Consignment Not Manage Stock|寄賣無控管庫存|2|null|null|null|null|C00|C|null|N|null|null|2011-07-27 18:04:48.0|2016-03-21 14:44:18.0|F000033546|
|02 / 04|638|C01|Consignment Manage Stock|寄賣有控管庫存|2|null|null|null|null|C01|C|null|Y|null|null|2015-09-01 10:12:57.0|2016-03-21 14:44:28.0|F000033546|
|03 / 04|638|Mix|Mix|null|2|null|null|null|null|MIX|C|null|null|null|null|2011-07-27 18:04:48.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 04|638|P|Partnership|null|2|null|null|null|null|P|P|null|null|null|null|2011-07-27 18:04:48.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

