# TBLDTL 700 Global Parameter 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '700'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|700|Global Parameter|Global Parameter|TBDENTCD : NG reason code,TBDEDESC : NG reason description|15|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '700'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 15|700|1|NPP Control By Sub Code|NPP Control By Sub Code|2|1|null|null|null|null|null|null|null|null|null|2012-04-11 10:38:43.0|2013-10-18 12:02:56.0|F000033546|
|02 / 15|700|10|Dummy typology|null|2|null|null|null|null|MOST|F|null|null|null|null|2012-09-04 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|03 / 15|700|11|stop reason|stop reason|2|8|null|null|null|null|null|null|null|null|null|2012-11-06 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|04 / 15|700|12|Purge|Purge|2|15|null|null|null|null|null|null|null|null|null|2013-09-05 11:38:40.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 15|700|13|Set Final Assortment Date|null|2|1|null|null|null|null|null|null|null|null|null|2014-01-22 18:56:00.0|2014-01-22 18:56:00.0|SSAdmin|
|06 / 15|700|14|Store Default For Item Modification|null|2|null|null|null|null|006|null|null|null|null|null|2014-01-22 18:56:00.0|2014-01-22 18:56:00.0|SSAdmin|
|07 / 15|700|15|Java Path|Java Path|2|null|null|null|null|/opt/oracle/product/11.2/jdk/bin|null|null|null|null|null|2014-04-09 14:45:53.0|2014-04-09 14:45:53.0|WF-TEST|
|08 / 15|700|16|Default Stop reason for ItemModification|Default Stop reason for ItemModification|2|null|null|null|null|1|null|null|null|null|null|2014-05-09 21:06:23.0|2015-05-29 19:00:49.0|SSFIX_25550|
|09 / 15|700|2|W supplier|W supplier|2|1|null|null|null|null|null|null|null|null|null|2012-05-16 08:38:16.0|2013-08-22 20:48:35.0|WF-TEST|
|10 / 15|700|3|Exception day of new item creation|Exception day of new item creation|2|null|null|null|null|null|null|null|null|null|null|2012-08-31 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|11 / 15|700|4|Modify logistic item flag|Modify logistic item flag|2|0|null|null|null|null|null|null|null|null|null|2012-05-16 08:39:02.0|2013-08-22 20:48:35.0|WF-TEST|
|12 / 15|700|5|GDS barcode checking|GDS barcode checking|2|null|null|null|null|Y|null|null|null|null|null|2012-04-11 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|13 / 15|700|7|Order parameter|Order parameter|2|1|0|null|null|null|null|null|null|null|null|2012-04-11 00:00:00.0|2013-08-19 15:55:43.0|F000033546|
|14 / 15|700|8|SecureTanfer|SecureTanfer|2|null|null|null|null|twwfprod,10.142.147.50|/opt/workflow/pre_upload/|/opt/workflow/pre_upload/|null|null|null|2010-01-21 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|15 / 15|700|9|Bonita request|Bonita Request|2|100|null|null|null|null|null|null|null|null|null|2012-06-23 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|

