# TBLDTL 354 等級 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '354'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|354|Grade|等級|C1 = Grade CodeC2 = Store Format for Story (HYP/SUP)C3 = Business format|1220|


---


```sql
        
    SELECT * FROM (
        SELECT * FROM TBLDTL WHERE TBDTBNO = '354' AND  instr(TBDCHA3,',') =0
        FETCH FIRST 2 ROWS ONLY
    )
    UNION ALL
    SELECT * FROM (
        SELECT * FROM TBLDTL WHERE TBDTBNO = '354' AND  instr(TBDCHA3,',') >0
        FETCH FIRST 2 ROWS ONLY
    )

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 04|354|1BM|1BM|1BM|2|null|null|null|null|1BM|HYP|HYP|null|null|null|2024-06-19 13:37:56.0|2024-06-19 13:37:56.0|PMD-9555|
|02 / 04|354|1EL|1EL|1EL|2|null|null|null|null|1EL|HYP|HYP|null|null|null|2024-06-19 13:37:56.0|2024-06-19 13:37:56.0|PMD-9555|
|03 / 04|354|CAT|CAT|CAT|2|null|null|null|null|CAT|null|HYP,SUP,JSN|1|null|null|2009-05-11 12:28:21.0|2022-08-23 15:18:00.0|CRID0588|
|04 / 04|354|CAT1|CAT1|CAT1|2|null|null|null|null|CAT1|SUP|HYP,SUP|null|null|null|2023-06-20 18:40:48.0|2023-06-26 11:53:26.0|md9141|

