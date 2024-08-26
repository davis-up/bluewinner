# TBLDTL 712 新單品欄位預設值設定 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '712'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|712|Parameter Control|新單品欄位預設值設定|TBDENTCD : Entry (running number xxx),TBDEDESC : Description,TBDCHA1  : Column/Field Code ,TBDCHA2  : Value ,TBDCHA3  : Department |21|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '712'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 21|712|01|SP Type|SP Type|2|null|null|null|null|01|G|ALL|null|null|null|2012-05-10 15:16:17.0|2013-08-22 20:48:35.0|WF-TEST|
|02 / 21|712|04|Sensitiveness|Sensitiveness|2|null|null|null|null|02|4|ALL|null|null|null|2012-05-10 15:24:15.0|2013-08-22 20:48:35.0|WF-TEST|
|03 / 21|712|06|VAT Code|VAT Code|2|null|null|null|null|04|1|ALL|null|null|null|2012-05-10 15:34:43.0|2013-08-22 20:48:35.0|WF-TEST|
|04 / 21|712|07|Sold By|Sold By|2|null|null|null|null|05|null|null|null|null|null|2012-05-10 15:35:43.0|2013-08-22 20:48:35.0|WF-TEST|
|05 / 21|712|08|Shelf Tag Size|Shelf Tag Size|2|null|null|null|null|06|S|ALL|null|null|null|2012-05-10 15:36:45.0|2013-08-22 20:48:35.0|WF-TEST|
|06 / 21|712|09|Brand|Brand|2|null|null|null|null|07|null|null|null|null|null|2012-05-10 15:39:40.0|2013-08-22 20:48:35.0|WF-TEST|
|07 / 21|712|10|Specific Item|Specific Item|2|null|null|null|null|08|B|ALL|null|null|null|2012-05-10 15:42:13.0|2013-08-22 20:48:35.0|WF-TEST|
|08 / 21|712|11|Type Of Sales|Type Of Sales|2|null|null|null|null|09|2|ALL|null|null|null|2012-05-10 15:43:09.0|2013-08-22 20:48:35.0|WF-TEST|
|09 / 21|712|12|Capacity|Capacity|2|null|null|null|null|10|null|null|null|null|null|2012-05-10 15:48:16.0|2013-08-22 20:48:35.0|WF-TEST|
|10 / 21|712|13|Stock Unit|Stock Unit|2|null|null|null|null|11|null|ALL|null|null|null|2012-05-10 15:49:45.0|2013-08-22 20:48:35.0|WF-TEST|
|11 / 21|712|14|Country of Origin|Country of Origin|2|null|null|null|null|12|TWN|ALL|null|null|null|2012-05-10 15:50:52.0|2013-08-22 20:48:35.0|WF-TEST|
|12 / 21|712|15|Typology Code|Typology Code|2|null|null|null|null|13|1U|ALL|null|null|null|2012-05-10 15:51:10.0|2013-08-22 20:48:35.0|WF-TEST|
|13 / 21|712|16|Grade|Grade|2|null|null|null|null|14|1U|ALL|null|null|null|2012-05-10 15:52:17.0|2013-08-22 20:48:35.0|WF-TEST|
|14 / 21|712|17|Season|Season|2|null|null|null|null|15|0|ALL|null|null|null|2012-05-10 15:53:17.0|2013-08-22 20:48:35.0|WF-TEST|
|15 / 21|712|18|Unit Code|Unit Code|2|null|null|null|null|16|01|ALL|null|null|null|2012-05-11 08:55:12.0|2013-08-22 20:48:35.0|WF-TEST|
|16 / 21|712|19|Barcode Type|Barcode Type|2|null|null|null|null|17|1|ALL|null|null|null|2012-05-11 08:56:00.0|2013-08-22 20:48:35.0|WF-TEST|
|17 / 21|712|22|Typology Item|Typology Item|2|null|null|null|null|20|1|ALL|null|null|null|2012-09-04 17:22:54.0|2013-08-22 20:48:35.0|WF-TEST|
|18 / 21|712|23|Priority|Priority|2|null|null|null|null|21|0|ALL|null|null|null|2012-09-04 17:23:25.0|2013-08-22 20:48:35.0|WF-TEST|
|19 / 21|712|35|CONS|CONS|2|null|null|null|null|19|null|null|null|null|null|2012-05-22 14:58:37.0|2013-08-22 20:48:35.0|WF-TEST|
|20 / 21|712|37|Logistic Pack|Logistic Pack|2|1|1|1|null|23|cm|ALL|null|null|null|2013-12-03 15:14:29.0|2015-05-29 19:00:49.0|SSFIX_25550|
|21 / 21|712|40|Returable|Returable|2|null|null|null|null|22|1|ALL|null|null|null|2012-06-08 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|

