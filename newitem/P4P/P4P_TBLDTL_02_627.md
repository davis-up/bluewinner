# TBLDTL 627 供應商型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '627'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|627|Supplier Type Setup|供應商型態|N1 = Transfer to PS : 0 - No/ 1 - Yes , N2 = Transfer to Mandala : 0 - No/1 - Yes, N3 = Transfer to CPC : 0 - No/1 - Yes , C1 = Set ID for Merchandise Vendor for interface to PeopleSoft, C2 = Supplier Type Code used for interface to CPC (C - Commercial = C/ E - Expense = E/ I - consider Expense = E), C3 = Prefix for Supplier Code used for interface to CPC|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '627'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|627|C|Commercial|Commercial|2|1|1|1|null|TWMER|C|8|TWMER|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 03|627|E|Expense|Expense|2|1|1|1|null|TWMER|E|1|TWMER|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 03|627|I|Internal Commercial|Internal Commercial|2|1|1|0|null|TWMER|E|1|TWMER|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|

