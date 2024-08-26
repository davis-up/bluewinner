# TBLDTL 629 停止合作原因 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '629'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|629|Stop Business Reason|停止合作原因|To define Stop Business Reason.|8|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '629'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 08|629|1|BANKRUPT|公司倒閉|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 08|629|2|VIOLATION|違約|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 08|629|3|SHORTAGE|缺貨|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 08|629|4|UNCOPORATION|不合作|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 08|629|5|NO TRADE|停止往來|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|06 / 08|629|6|BUSINESS NOT PROUD|業績不佳|2|null|null|null|null|null|null|null|null|null|null|2010-10-28 10:22:42.0|2015-05-29 19:00:49.0|SSFIX_25550|
|07 / 08|629|7|CONTRACT AND LAW LITIGATION|黑名單-合約及法律訴訟|2|null|null|null|null|null|null|null|null|null|null|2011-06-27 16:52:48.0|2015-05-29 19:00:49.0|SSFIX_25550|
|08 / 08|629|Z|Stop From GDS|由GDS停止|2|null|null|null|null|null|null|null|null|null|null|2010-04-19 14:28:51.0|2015-05-29 19:00:49.0|SSFIX_25550|

