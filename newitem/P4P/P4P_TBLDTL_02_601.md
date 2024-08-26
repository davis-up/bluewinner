# TBLDTL 601 價格小數位數及進位基準 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '601'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|601|Pricing Decimal and Rounding Method|價格小數位數及進位基準|Define decimal digit and rounding method of pricing.|5|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '601'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|601|1|Purchase price decimal|Purchase price decimal|2|2|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2013-09-11 19:10:16.0|SSFIX-14007|
|02 / 05|601|2|Selling price decimal|Selling price decimal|2|0|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2013-09-11 19:10:16.0|SSFIX-14007|
|03 / 05|601|3|Rounding method|Rounding method|2|3|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2013-09-11 19:10:16.0|SSFIX-14007|
|04 / 05|601|4|Round to value|Round to value|2|1|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2013-09-11 19:10:16.0|SSFIX-14007|
|05 / 05|601|5|Gross net weight decimal|Gross net weight decimal|2|3|null|null|null|null|null|null|null|null|null|2022-12-20 00:00:00.0|2022-12-20 00:00:00.0|TWF-2141|

