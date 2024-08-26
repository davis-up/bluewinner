# TBLDTL 327 Department Group 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '327'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|327|Department Group|Department Group|TBDCHAR1:Department Group|11|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '327'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 11|327|00|Division Total|Division Total|1|null|null|null|null|10,11,12,14,15,20,21,22,23,24,25,26,30,31,32,33,34,35,36,40,41,42,43,44,45,46,47,48,49,51,52,60,61|62,63,65,66,72,75,76,78,79,80,90|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|02 / 11|327|01|Grocery|Grocery|1|null|null|null|null|10,11,12,14,15|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|03 / 11|327|02|Fresh|Fresh|1|null|null|null|null|20,21,22,23,24,25,26|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|04 / 11|327|03|Bazaar|Bazaar|1|null|null|null|null|30,31,32,33,34,35,36|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|05 / 11|327|04|Appliance|Appliance|1|null|null|null|null|40,41,42,43,44,45,46,47,48,49|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|06 / 11|327|06|Textile|Textile|1|null|null|null|null|60,61,62,63,65,66|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|07 / 11|327|07|Dept 75,76,77,79|Dept 75,76,77,79|1|null|null|null|null|75,76,78,79|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|08 / 11|327|0A|Food|Food|1|null|null|null|null|20|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|09 / 11|327|0B|Non Food|Non Food|1|null|null|null|null|40|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|10 / 11|327|0C|Total without 49,79|Total without 49,79|1|null|null|null|null|10,11,12,14,15,20,21,22,23,24,25,26,30,31,32,33,34,35,36,40,41,42,43,44,45,46,47,48,51,52,60,61,62|63,65,66,72,75,76,78,80,90|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|
|11 / 11|327|4A|Appliance without 49|Appliance without 49|1|null|null|null|null|40,41,42,43,44,45,46,47,48|null|null|null|null|null|2014-09-12 04:34:23.0|2015-05-29 18:06:55.0|SSFIX_25550|

