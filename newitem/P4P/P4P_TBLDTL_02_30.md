# TBLDTL 30 稅率型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '30'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|30|Tax Type|稅率型態|N1 = Applicable for 0-Same Tax Location, 1- Crosse Tax location, 2-No Checking,N2 = Tax rate different by Item - 1-Yes, 0-No,N3 = Inc/Exc in selling price - 1-Include, 0-Exclude,N4 = Tax Location Level - 1-State, 2-Municipal, 3-City, 4- Region,C1 = P-Primary Tax/S-Substitute Tax/A-Add on Tax/N-Not Applicable,C2 = On top of which tax type,C3 = Tax rate base on - S-Supplier location, T-Store Location,C4 = Applicable for Intra-Company Transaction-Y-Yes, N-No|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '30'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|30|1|VAT|VAT|2|2|1|1|null|P|null|null|N|null|null|2009-03-27 00:00:00.0|2016-05-17 17:33:08.0|F000000959|
|02 / 02|30|C|Purchase For Add On Tax|Purchase For Add On Tax|2|2|1|null|null|C|null|null|N|null|null|2018-03-26 18:41:45.0|2018-03-26 18:41:58.0|victorshih|

