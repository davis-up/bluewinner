# TBLDTL 714 AWF店分配與預設店別 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '714'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|714|default Store|AWF店分配與預設店別|TBDNUM1: Defaulted store for store selection of workflow new item creationscreen (0 or blank: No, 1: Yes )TBDNUM2: Released Store to P4MD+ for new item creation (future release) onvalidation date when validation date < Store assortment date – 1 ( 0 or blank:No, 1: Yes )TBDNUM3: Store which is allowed to create PPP for DS supplier for Promotionprice modification( 0 or blank: No, 1: Yes )If no store has TBDNUM3 = 1, system will generate all stores based on storeassortment as defaulted and allow user to remove/untickTBDNUM4: For stop/Release logistic item,  system should allow to stop/releasestores based on the value set up  ( 0 or blank: No, 1: Yes )|403|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '714'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 40|714|006|006|006|2|1|1|1|0|1|1|0|null|null|null|2012-05-29 00:00:00.0|2014-02-21 11:15:13.0|F000079381|
|02 / 40|714|011|011|011|2|0|0|0|0|null|null|null|null|null|null|2015-07-16 19:11:08.0|2015-07-16 19:11:08.0|SSFIX-25487|
|03 / 40|714|012|012|012|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:08:59.0|2013-10-27 16:49:45.0|F000033546|
|04 / 40|714|013|013|013|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:09:11.0|2013-10-27 16:49:52.0|F000033546|
|05 / 40|714|015|015|015|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:09:25.0|2013-10-27 16:49:59.0|F000033546|
|06 / 40|714|016|016|016|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:09:40.0|2013-10-27 16:50:06.0|F000033546|
|07 / 40|714|018|018|018|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:09:55.0|2013-10-27 16:50:13.0|F000033546|
|08 / 40|714|019|019|019|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:10:08.0|2013-10-27 16:50:22.0|F000033546|
|09 / 40|714|01A|01A|01A|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:10:21.0|2013-10-27 16:50:34.0|F000033546|
|10 / 40|714|01B|01B|01B|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:10:35.0|2013-10-27 16:50:44.0|F000033546|
|11 / 40|714|01E|01E|01E|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:10:51.0|2013-10-27 16:50:52.0|F000033546|
|12 / 40|714|01G|01G|01G|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:11:09.0|2013-10-27 16:51:01.0|F000033546|
|13 / 40|714|01H|01H|01H|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:11:22.0|2013-10-27 16:51:09.0|F000033546|
|14 / 40|714|01I|01I|01I|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:11:34.0|2015-05-29 19:00:49.0|SSFIX_25550|
|15 / 40|714|021|021|021|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:11:46.0|2013-10-27 16:51:29.0|F000033546|
|16 / 40|714|022|022|022|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:11:57.0|2013-10-27 16:51:39.0|F000033546|
|17 / 40|714|023|023|023|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:12:07.0|2013-10-27 16:51:47.0|F000033546|
|18 / 40|714|026|026|026|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:12:22.0|2013-10-27 16:51:56.0|F000033546|
|19 / 40|714|02D|02D|02D|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:12:35.0|2013-10-27 16:52:06.0|F000033546|
|20 / 40|714|02E|02E|02E|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:12:51.0|2013-10-27 16:52:13.0|F000033546|
|21 / 40|714|02F|02F|02F|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:13:03.0|2013-10-27 16:52:21.0|F000033546|
|22 / 40|714|02G|02G|02G|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:13:14.0|2013-10-27 16:52:32.0|F000033546|
|23 / 40|714|02H|02H|02H|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:13:26.0|2013-10-27 16:52:40.0|F000033546|
|24 / 40|714|02I|02I|02I|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:13:39.0|2013-10-27 16:52:48.0|F000033546|
|25 / 40|714|02J|02J|02J|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:13:54.0|2013-10-27 16:52:56.0|F000033546|
|26 / 40|714|02K|02K|02K|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:14:06.0|2013-10-27 16:53:04.0|F000033546|
|27 / 40|714|02L|02L|02L|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:14:19.0|2015-05-29 19:00:49.0|SSFIX_25550|
|28 / 40|714|02M|02M|02M|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:14:29.0|2013-10-27 16:53:21.0|F000033546|
|29 / 40|714|02N|02N|02N|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:14:41.0|2013-10-27 16:53:30.0|F000033546|
|30 / 40|714|031|031|031|2|1|1|1|0|0|1|null|null|null|null|2012-05-29 00:00:00.0|2014-02-21 11:15:33.0|F000079381|
|31 / 40|714|041|041|041|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:14:53.0|2013-10-27 16:53:40.0|F000033546|
|32 / 40|714|042|042|042|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:15:06.0|2013-10-27 16:53:49.0|F000033546|
|33 / 40|714|044|044|044|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:15:30.0|2013-10-27 16:54:07.0|F000033546|
|34 / 40|714|047|047|047|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:15:56.0|2013-10-27 16:54:15.0|F000033546|
|35 / 40|714|048|048|048|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:16:20.0|2013-10-27 16:54:27.0|F000033546|
|36 / 40|714|049|049|049|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:16:31.0|2013-10-27 16:54:36.0|F000033546|
|37 / 40|714|04A|04A|04A|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:17:14.0|2013-10-27 16:54:45.0|F000033546|
|38 / 40|714|04B|04B|04B|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:17:27.0|2013-10-27 16:54:56.0|F000033546|
|39 / 40|714|04C|04C|04C|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:17:38.0|2013-10-27 16:55:04.0|F000033546|
|40 / 40|714|04D|04D|04D|2|0|0|0|0|null|null|null|null|null|null|2012-12-07 14:17:53.0|2015-05-29 19:00:49.0|SSFIX_25550|

