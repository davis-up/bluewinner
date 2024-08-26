# TBLDTL 626 business format 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '626'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|626|business format|null|business format|7|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '626'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 07|626|AUT|Other-Production Center|Other-Production Center|2|null|null|null|null|null|null|null|null|null|null|2022-02-22 21:36:23.0|2022-02-22 21:36:23.0|ibmsupport|
|02 / 07|626|CVS|Convenience Store|Convenience Store|2|null|null|null|null|null|null|null|null|null|null|2022-02-22 21:36:23.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|03 / 07|626|ECM|Electronic Commerce|Electronic Commerce|2|null|null|null|null|null|null|null|null|null|null|2022-02-22 21:36:23.0|2022-02-22 21:36:23.0|ibmsupport|
|04 / 07|626|HYP|HYP|HYP|2|1|1|null|null|null|null|null|null|null|null|2022-02-22 21:36:23.0|2022-02-22 21:36:23.0|ibmsupport|
|05 / 07|626|JSN|Jasons|Jasons|2|1|3|null|null|null|null|null|null|null|null|2022-02-22 21:36:23.0|2022-02-22 21:36:23.0|ibmsupport|
|06 / 07|626|OTH|Others Store|Others Store|2|null|null|null|null|null|null|null|null|null|null|2022-02-22 21:36:23.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|07 / 07|626|SUP|Supermarket|Supermarket|2|1|2|null|null|null|null|null|null|null|null|2022-02-22 21:36:23.0|2022-08-22 15:41:31.0|PMD-8443-pt1|

