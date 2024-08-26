# TBLDTL 770 Mandatory Field Contr by Department 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '770'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|770|Mandatory Field Contr by Department|Mandatory Field Contr by Department|Mandatory Field Controlled by Department in New Item Creation (E-Codi)				    TBDCHA1: Null / ALL / List of dept codes separated by comma (,)                             > Null = this field is not mandatory                             > 'ALL' = this field is mandatory for all departments                             > List of dept codes (e.g. 10,11,12) = this field is mandatory for specific departments only|2|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '770'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|770|001|Collection No|Collection No|2|null|null|null|null|null|null|null|null|null|null|2016-12-07 04:27:05.0|2016-12-07 04:27:05.0|SYSTEM|
|02 / 02|770|002|Shelf Life|Shelf Life|2|null|null|null|null|null|null|null|null|null|null|2016-12-07 04:28:26.0|2016-12-07 04:28:26.0|SYSTEM|

