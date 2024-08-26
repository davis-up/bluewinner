# TBLDTL 356 Relate to ITMSPEC in ITMGLD 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '356'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|356|Specific item|Relate to ITMSPEC in ITMGLD|C1 = P4 with specific item code, C2 = Mandala specific item code, C3 = Mandala specific item description ,C4 = TEXAS specific item code|3|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '356'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 03|356|B|Brand|Brand|2|null|null|null|null|B|B|Brand|A|null|null|2008-01-04 10:22:18.0|2024-05-07 21:40:54.0|BRID0617|
|02 / 03|356|C|Carrefour|Carrefour|2|null|null|null|null|C|C|Carrefour|ME|null|null|2008-01-04 10:22:18.0|2024-05-07 21:40:54.0|BRID0617|
|03 / 03|356|F|First Price|First Price|2|null|null|null|null|F|F|First Price|P1,P4|null|null|2008-01-04 10:22:18.0|2024-05-07 21:40:54.0|BRID0617|

