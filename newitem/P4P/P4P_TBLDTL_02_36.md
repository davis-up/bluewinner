# TBLDTL 36 店類別 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '36'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|36|Store Category|店類別|Define store category that sells items.|7|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '36'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 07|36|C|Convenience Store|Convenience Store|2|null|null|null|null|null|null|null|null|null|null|2018-09-14 15:00:05.0|2018-09-14 15:00:05.0|victorshih|
|02 / 07|36|E|Electronic Commerce|電子商務|2|null|null|null|null|null|null|null|null|null|null|2015-11-05 16:57:45.0|2015-11-05 16:57:45.0|F000033546|
|03 / 07|36|H|Hyper|量販型態|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 07|36|L|Logistic|後勤|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 07|36|M|Mini-Hyper|小型量販型態|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|06 / 07|36|P|Production Center|中央廚房|2|null|null|null|null|null|null|null|null|null|null|2010-01-28 16:25:15.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|07 / 07|36|S|Supermarket|超市型態|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

