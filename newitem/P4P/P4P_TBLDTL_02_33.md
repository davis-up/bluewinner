# TBLDTL 33 條碼型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '33'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|33|Barcode Type|條碼型態|C1 = name of barcode generatorC3 = Y, major barcode disallow; N, major barcode allow|5|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '33'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|33|1|EAN-13|EAN-13|2|null|null|null|null|barcodeEan13Generator|01|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 05|33|2|EAN-8|EAN-8|2|null|null|null|null|barcodeEan8Generator|02|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 05|33|3|UPC-A|UPC-A|2|null|null|null|null|barcodeUpcAGenerator|03|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 05|33|4|UPC-E|UPC-E|2|null|null|null|null|barcodeUpcEGenerator|03|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 05|33|9|PLU|PLU|2|null|null|null|null|barcodePluGenerator|00|null|null|null|null|2008-04-29 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

