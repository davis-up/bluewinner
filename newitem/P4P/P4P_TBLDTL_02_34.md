# TBLDTL 34 店規模 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '34'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|34|Store Format|店規模|C1 = For Malaysia use only, to indicate that the NPP/PPP and logistic information, DC surcharge and DC Discount, of the secondary supplier will be removed or update to zero for the specific store format: Y-Remove, null not remove |5|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '34'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|34|AUT|Other-Production Center|Other-Production Center|2|null|null|null|null|null|null|null|null|null|null|2010-01-28 16:16:37.0|2015-11-05 17:14:43.0|F000033546|
|02 / 05|34|CVS|Convenience Store|Convenience Store|2|null|null|null|null|null|null|null|null|null|null|2018-09-14 14:58:29.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|03 / 05|34|ECM|Electronic Commerce|eCommerce|2|null|null|null|null|null|null|null|null|null|null|2015-11-05 16:55:34.0|2015-11-05 17:14:51.0|F000033546|
|04 / 05|34|HYP|Hyper|Hyper|2|1|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-11-05 17:15:01.0|F000033546|
|05 / 05|34|SUP|Supermarket|Supermarket|2|1|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

