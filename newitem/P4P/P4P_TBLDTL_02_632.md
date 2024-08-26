# TBLDTL 632 供應商預設參數 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '632'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|632|Supplier Default Value|供應商預設參數|To define the default value to display in page for each parameter table.|7|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '632'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 07|632|1|Supplier Type|Supplier Type|0|null|null|null|null|C|null|null|null|null|null|2008-10-14 15:12:54.0|2013-09-11 19:10:14.0|SSFIX-14007|
|02 / 07|632|2|Payment Mode|Payment Mode|0|null|null|null|null|1|null|null|null|null|null|2008-10-14 15:12:54.0|2013-09-11 19:10:14.0|SSFIX-14007|
|03 / 07|632|3|Specific Supplier|Specific Supplier|0|null|null|null|null|1|null|null|null|null|null|2008-10-14 15:12:54.0|2013-09-11 19:10:14.0|SSFIX-14007|
|04 / 07|632|4|Supplier Nature|Supplier Nature|0|null|null|null|null|CE|I|D|W|null|null|2008-10-14 15:12:54.0|2013-09-11 19:10:14.0|SSFIX-14007|
|05 / 07|632|5|Negotiation Type|Negotiation Type|0|null|null|null|null|3|null|null|null|null|null|2008-10-14 15:12:54.0|2013-09-11 19:10:14.0|SSFIX-14007|
|06 / 07|632|6|Cut Off Time (SUP0002B)|Cut Off Time (SUP0002B)|0|null|null|null|null|18:00|null|null|null|null|null|2008-10-24 16:43:02.0|2013-09-11 19:10:14.0|SSFIX-14007|
|07 / 07|632|7|PP Base On (SUP0002B)|null|2|null|null|null|null|0|null|null|null|null|null|2008-06-23 00:00:00.0|2013-09-11 19:10:14.0|SSFIX-14007|

