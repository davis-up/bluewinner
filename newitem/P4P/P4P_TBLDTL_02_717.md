# TBLDTL 717 單品建立依特定單品代碼與使用角色 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '717'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|717|Specific Item in Role|單品建立依特定單品代碼與使用角色|Specific Item in Role|4|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '717'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 04|717|1|Specific Item|Specific Item|1|null|null|null|null|buyer|C|null|null|null|null|2012-06-27 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|02 / 04|717|2|Specific Item|Specific Item|1|null|null|null|null|buyer|B|null|null|null|null|2012-06-26 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|03 / 04|717|3|Specific Item|Specific Item|1|null|null|null|null|manager|C|null|null|null|null|2012-06-28 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|04 / 04|717|4|Specific Item|Specific Item|2|null|null|null|null|buyer|F|null|null|null|null|2013-02-18 08:13:41.0|2013-08-22 20:48:35.0|WF-TEST|

