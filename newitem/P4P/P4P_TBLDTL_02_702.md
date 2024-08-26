# TBLDTL 702 E-Codi 退回原因 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '702'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|702|NG reason |E-Codi 退回原因|TBDENTCD : NG reason code,TBDEDESC : NG reason description|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '702'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|702|1|Application not be approved|LApplication not be approved|2|0|1|1|1|1|1|1|1|null|null|2012-04-23 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|02 / 03|702|2|GDS: Refused by Manager|LGDS: Refused by Manager|2|1|1|1|1|1|1|1|1|null|null|2012-04-23 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|03 / 03|702|3|Cancelled by MD Buyer|Cancelled by MD Buyer|2|1|1|1|1|1|1|1|1|null|null|2019-07-17 13:49:28.0|2019-07-17 13:50:51.0|F000036143|

