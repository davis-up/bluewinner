
# [SUPGLD] Supplier


```sql
   
    SELECT
        B.*
    FROM SUPGLD B WHERE 0=0  AND SUPSUPCD = '5298'

```

|SEQ|SUPSUPCD|SUPTYP|SUPEDESC|SUPLDESC|SUPTELNO|SUPFAXNO|SUPSTPPMTR|SUPADDR1|SUPADDR2|SUPADDR3|SUPRMT|SUPLGFLAG|SUPCRE|SUPUPD|SUPUSR|SUPTAXABLE|SUPSTATE|SUPTRNPS|SUPSTPBUSDATE|SUPSTPBUSR|SUPSTPPMTSD|SUPSTPPMTED|SUPCREUSR|SUPCSTNO|SUPPANNO|SUPMUNICIPAL|SUPCITY|SUPREGION|SUPGLN|SUPMSMENO|SUPSERVTAXNO|SUPEXCISEID|SUPSUPCDWEB|SUPSTPPMTDEP|SUPSTPBUSDEP|SUPBUSENT|SUPTEXKEY|SUPCROSSDP|SUPMINORDBY|SUPMINQTY|SUPMINAMT|SUPZIPCD|SUPMAIL|SUPRTNTELNO|SUPRTNFAXNO|SUPPAYCD|SUPBANKCD|SUPBANKACCD|SUPEFT|SUPMIXPACK|SUPRTNMEDIA|SUPCTRFG|SUPLEGALREP|SUPFRADD|SUPFRCOM|SUPRECONP|SUPRECONE|SUPFROZENSTATUS|SUPFROZENDATE|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|5298|C|Procter & Gamble Taiwan,Ltd|寶僑家品股份有限公司|02-87806388|02-87869084|null|台北市信義路５段１０６號７樓|null|null|5298|null|2009-05-08 19:00:00.0|2020-09-18 17:06:57.0|P4PAUT72A|1|null|2020-09-18 20:00:56.0|null|null|null|null|MIGRATION|null|null|null|null|null|4714706900019|null|null|null|5298|null|null|null|null|0|null|null|null|１１０|null|02-87220872|02-87869083|null|null|null|null|N|3|N|null|_|0|Amy|chan.a.24@pg.com|null|null|


# [SUPATT] Supplier - Attribute


```sql
   
    SELECT
        B.*
    FROM SUPATT B WHERE 0=0 AND SUASUPCD = '5298'
    -- FETCH FIRST 5 ROWS ONLY

```

|SEQ|SUASUPCD|SUACLCD|SUACLCD|SUACD|SUACD|SUASDATE|SUAALPH|SUANUM|SUADATE|SUATIME|SUAEDATE|SUACRE|SUACREUSR|SUAUPD|SUAUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|5298|OAOT|OAOT|TAXC|TAXC|2018-11-27 00:00:00.0|P|null|null|null|2049-12-31 00:00:00.0|2018-11-26 17:31:43.0|F000008539|2018-11-26 17:31:43.0|F000008539|


# [ATTVAL] Supplier - Attribute - Value


```sql
   
    SELECT
        A.*
    FROM ATTVAL A
        INNER JOIN SUPATT B ON A.ATTCLCD = B.SUACLCD  AND A.ATTCD = B.SUACD
    WHERE 0=0
    AND B.SUASUPCD = '5298'
    -- FETCH FIRST 5 ROWS ONLY

```

|SEQ|ATTCLCD|ATTCD|ATTSHORT|ATTDESC|ATTVTYP|ATTALPH|ATTNUM|ATTDATE|ATTTIME|ATTDEF|ATTCRE|ATTUPD|ATTUSR|ATTCREUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|OAOT|TAXC|Other Add On Tax Cod|For Supplier Attribute|1|P|null|null|null|0|2018-03-27 01:17:29.0|2018-11-14 18:31:17.0|CM11632|victorshih|


# [ATTCLASS] ATTVAL - ATTCLASS


```sql
   
    SELECT
        C.*
    FROM P4P.ATTVAL A
        INNER JOIN P4P.SUPATT B   ON A.ATTCLCD = B.SUACLCD  AND A.ATTCD = B.SUACD
        INNER JOIN P4P.ATTCLASS C ON A.ATTCLCD = C.ATCCLCD
    WHERE 0=0
      AND B.SUASUPCD = '5298'


```

|SEQ|ATCCLCD|ATCSHORT|ATCDESC|ATCUNIQ|ATCMAN|ATCITM|ATCSUP|ATCSTO|ATCCRE|ATCUPD|ATCUSR|ATCCREUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|OAOT|Other Add On Tax|Other Add On Tax|1|0|0|1|1|2018-03-27 01:12:46.0|2018-11-14 18:31:12.0|CM11632|victorshih|


# [SUPDEP] Supplier - Dept


```sql
   
    SELECT
        B.*
    FROM P4P.SUPGLD A
        INNER JOIN P4P.SUPDEP B ON B.SUDSUPCD = A.SUPSUPCD
    WHERE 0=0
      AND A.SUPSUPCD = '5298'


```

|SEQ|SUDDPCD|SUDSUPCD|SUDSPEC|SUDTELNO|SUDFAXNO|SUDCONT|SUDORDDAY|SUDNATURE|SUDEOM|SUDCUTTM|SUDSTPPMTR|SUDORDPER|SUDLEADTM|SUDPYMT|SUDRBPCT|SUDCRBPCT|SUDDELDAY|SUDMAIL|SUDCRE|SUDUPD|SUDUSR|SUDACTLOC|SUDSTPBUSDATE|SUDSTPBUSR|SUDSTPPMTSD|SUDSTPPMTED|SUDCREUSR|SUDMOTHERSUP|SUDNEGOTYP|SUDMEDIA|SUDSTPPMTSTO|SUDPPBASEON|SUDSTPBUSSTO|SUDRRMEDIA|SUDRCVASN|SUDAUTASN|SUDSUPCUTN|SUDCOPCUT|SUDCOPCUTN|SUDPAYTM|SUDSUPGLN|SUDRTNTELNO|SUDRTNFAXNO|SUDRTNWD|SUDMIXPACK|SUDRTNMEDIA|SUDVALIDFLAG|SUDRTNAMTLIMIT|SUDCONEXPDATE|SUDFRADD|SUDFRCOM|SUDRECONP|SUDRECONE|SUDFROZENSTATUS|SUDFROZENDATE|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 06|76|5298|1|02-87806388|02-87869084|null|null|N|Y|15:00|null|null|null|1|0|0|null|null|2020-03-09 15:15:37.0|2020-09-18 17:06:57.0|P4PAUT72A|null|null|null|null|null|F000008539|null|3|null|null|0|null|E|0|0|null|null|null|0|4714706900019|02-87220872|02-87869083|null|N|3|null|null|null|_|0|Amy|chan.a.24@pg.com|null|null|
|02 / 06|30|5298|1|02-87806388|02-87869084|Milton Liang|null|N|Y|19:00|null|null|null|60|0|0|null|null|2009-05-08 19:00:00.0|2024-03-14 21:32:58.0|PKSUPFROZE|null|2009-05-08 00:00:00.0|5|null|null|MIGRATION|null|3|null|null|0|null|null|0|0|null|07:00|null|0|null|02-87220872|02-87869083|null|null|3|null|null|null|_|0|Amy|chan.a.24@pg.com|1|2024-03-14 21:32:58.0|
|03 / 06|41|5298|1|02-87806388|02-87869084|null|null|N|Y|15:00|null|null|null|60|0|0|null|null|2009-05-08 19:00:00.0|2024-03-14 21:32:58.0|PKSUPFROZE|null|2009-05-08 00:00:00.0|5|null|null|MIGRATION|null|3|null|null|0|null|null|0|0|null|07:00|null|0|null|02-87220872|02-87869083|null|null|3|null|null|null|_|0|Amy|chan.a.24@pg.com|1|2024-03-14 21:32:58.0|
|04 / 06|11|5298|1|02-87220714|02-87869083|張銘和Magic|12345|D|Y|18:00|null|1|1|80|21.67|0|123456|liang.m@pg.com|2009-05-08 19:00:00.0|2024-03-14 21:32:58.0|PKSUPFROZE|null|2009-05-08 00:00:00.0|5|null|null|MIGRATION|null|3|null|null|0|null|null|0|0|null|07:00|null|0|null|02-87220872|02-87869083|null|null|3|null|null|null|_|0|Amy|chan.a.24@pg.com|1|2024-03-14 21:32:58.0|
|05 / 06|12|5298|1|02-87220714|02-87869083|張銘和Magic|12345|D|N|18:00|null|1|1|8|17.63|0|23456|chang.m.8@pg.com|2009-05-08 19:00:00.0|2024-02-02 18:44:40.0|P4PAUT72A|null|null|null|null|null|MIGRATION|null|3|null|null|0|null|E|0|0|null|07:00|null|0|null|02-87220872|02-87869083|null|Y|1|null|0|null|_|0|Hanna|chan.a.24@pg.com|null|null|
|06 / 06|10|5298|1|02-87806388|02-87869084|Milton Liang|12345|D|Y|18:00|04|1|1|80|6|0|123456|liang.m@pg.com|2009-05-08 19:00:00.0|2024-03-14 21:32:58.0|PKSUPFROZE|null|2009-05-08 00:00:00.0|5|2009-05-08 00:00:00.0|2049-12-31 00:00:00.0|MIGRATION|null|3|null|2009-05-08 00:00:00.0|0|null|null|0|0|null|07:00|null|0|null|02-87220872|02-87869083|null|null|3|null|null|null|_|0|Amy|chan.a.24@pg.com|1|2024-03-14 21:32:58.0|


# [SUPSTO] Supplier - Store


```sql
   
    SELECT
        C.*
     FROM P4P.SUPGLD A
        INNER JOIN P4P.SUPDEP B ON B.SUDSUPCD = A.SUPSUPCD
        INNER JOIN P4P.SUPSTO C ON C.SUSSUPCD = A.SUPSUPCD AND C.SUSDPCD  = B.SUDDPCD
    WHERE 0=0
      AND A.SUPSUPCD = '5298'
    FETCH FIRST 5 ROWS ONLY

```

|SEQ|SUSDPCD|SUSDPCD|SUSSUPCD|SUSSUPCD|SUSSTOCD|SUSCUTTM|SUSSTPPMTR|SUSPYMT|SUSCRBPCT|SUSTELNO|SUSFAXNO|SUSCONT|SUSORDDAY|SUSDELDAY|SUSORDPER|SUSORDCLDAY|SUSLEADTM|SUSDELTIM|SUSSAFSTKDAY|SUSMEDIA|SUSCRE|SUSUPD|SUSUSR|SUSTAXNO|SUSNSONM|SUSSTPPMTSD|SUSSTPPMTED|SUSCREUSR|SUSPPBASEON|SUSSTPBUSDATE|SUSSTPBUSR|SUSSUPCUTN|SUSCOPCUT|SUSCOPCUTN|SUSMINQTY|SUSMINAMT|SUSRRMEDIA|SUSRCVASN|SUSAUTASN|SUSMAIL|SUSRTNTELNO|SUSRTNFAXNO|SUSFGTADD|SUSFGCOM|SUSVALIDFLAG|SUSCONEXPDATE|SUSRTNMEDIA|SUSRECONP|SUSRECONE|SUSGFCD|SUSRTNSUPCD|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|10|10|5298|5298|006|18:00|04|80|0|02-87806388|02-87869084|Milton Liang|12345|123456|1|null|1|null|null|E|2009-05-31 12:47:26.0|2020-09-18 17:06:57.0|P4PAUT72A|21238199|I01|2009-05-08 00:00:00.0|2049-12-31 00:00:00.0|DUPLI-031|0|2009-05-08 00:00:00.0|5|null|07:00|null|null|null|E|0|0|null|02-87220872|02-87869083|_|0|null|null|3|Amy|chan.a.24@pg.com|null|null|
|02 / 05|10|10|5298|5298|010|18:00|04|80|0|02-87806388|02-87869084|Milton Liang|12345|123456|1|null|1|null|null|E|2009-05-08 19:00:00.0|2020-09-18 17:06:57.0|P4PAUT72A|97161311|I01|2009-05-08 00:00:00.0|2049-12-31 00:00:00.0|MIGRATION|0|2009-05-08 00:00:00.0|5|null|07:00|null|null|null|E|0|0|null|02-87220872|02-87869083|_|0|null|null|3|Amy|chan.a.24@pg.com|null|null|
|03 / 05|10|10|5298|5298|013|18:00|04|80|0|02-87806388|02-87869084|Milton Liang|12345|123456|1|1|1|null|1|E|2009-05-08 19:00:00.0|2020-09-18 17:06:57.0|P4PAUT72A|21238199|I01|2009-05-08 00:00:00.0|2049-12-31 00:00:00.0|MIGRATION|0|2009-05-08 00:00:00.0|5|null|07:00|null|null|null|E|0|0|null|02-87220872|02-87869083|_|0|null|null|3|Amy|chan.a.24@pg.com|null|null|
|04 / 05|10|10|5298|5298|015|18:00|04|80|0|02-87806388|02-87869084|Milton Liang|12345|123456|1|0|1|null|1|E|2009-05-08 19:00:00.0|2020-09-18 17:06:57.0|P4PAUT72A|21238199|I01|2009-05-08 00:00:00.0|2049-12-31 00:00:00.0|MIGRATION|0|2009-05-08 00:00:00.0|5|null|07:00|null|null|null|E|0|0|null|02-87220872|02-87869083|_|0|null|null|3|Amy|chan.a.24@pg.com|null|null|
|05 / 05|10|10|5298|5298|016|18:00|04|80|0|02-87806388|02-87869084|Milton Liang|12345|123456|1|0|1|null|1|E|2009-05-08 19:00:00.0|2020-09-18 17:06:57.0|P4PAUT72A|21238199|I01|2009-05-08 00:00:00.0|2049-12-31 00:00:00.0|MIGRATION|0|2009-05-08 00:00:00.0|5|null|07:00|null|null|null|E|0|0|null|02-87220872|02-87869083|_|0|null|null|3|Amy|chan.a.24@pg.com|null|null|


# [ITMSUP] Supplier - Item


```sql
   
    SELECT
        B.*
     FROM P4P.SUPGLD A
        INNER JOIN P4P.ITMSUP B ON B.ITUSUPCD = A.SUPSUPCD

    WHERE 0=0
      AND A.SUPSUPCD = '5298'
    FETCH FIRST 5 ROWS ONLY

```

|SEQ|ITUITMID|ITUSUPCD|ITUSTPSUP|ITUSTPSUPRSN|ITUCRE|ITUUPD|ITUUSR|ITUCREUSR|ITUDSSUP|ITURETURN|ITURTNSHIP|ITURTNMEDIA|ITURTNTMP|ITURTNPMT|ITUGEXC|ITUREMIXPA|ITULOGBASK|ITURETURNSUPER|ITURTNTMPSUPER|ITURTNPMTSUPER|ITURETURNJASONS|ITURTNTMPJASONS|ITURTNPMTJASONS|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|564680|5298|null|null|2022-06-22 16:27:44.0|2024-05-03 20:17:15.0|P4PAUT41|PKNSAIPDMWF|null|0|null|null|0|0|null|null|N|0|0|0|0|0|0|
|02 / 05|564681|5298|null|null|2022-06-22 16:32:44.0|2024-05-03 20:17:13.0|P4PAUT41|PKNSAIPDMWF|null|0|null|null|0|0|null|null|N|0|0|0|0|0|0|
|03 / 05|577146|5298|null|null|2022-11-07 18:57:47.0|2024-05-03 20:17:19.0|P4PAUT41|PKNSAIPDMWF|null|0|null|null|0|0|null|null|null|0|0|0|0|0|0|
|04 / 05|577147|5298|null|null|2022-11-07 18:57:47.0|2024-05-03 20:17:20.0|P4PAUT41|PKNSAIPDMWF|null|0|null|null|0|0|null|null|null|0|0|0|0|0|0|
|05 / 05|577148|5298|null|null|2022-11-07 18:57:47.0|2024-05-03 20:17:21.0|P4PAUT41|PKNSAIPDMWF|null|0|null|null|0|0|null|null|null|0|0|0|0|0|0|


# [SUPBRAND] Supplier - Brand


```sql
   
    SELECT
        B.*
    FROM P4P.SUPGLD A
        INNER JOIN P4P.SUPBRAND B ON A.SUPSUPCD = B.SURSUPCD
    WHERE 0=0
      AND A.SUPSUPCD = '5298'


```

|SEQ|SURSUPCD|SURBRNDID|SURSBRNDID|SURCRE|SURUPD|SURUSR|SURCREUSR|
| -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|5298|3|2|2024-08-14 13:49:33.0|2024-08-14 14:35:38.0|TWscan-prod|TWscan-prod|
|02 / 05|5298|3|5|2024-08-14 13:49:14.0|2024-08-14 14:35:36.0|TWscan-prod|TWscan-prod|
|03 / 05|5298|3|20|2024-08-14 14:23:27.0|2024-08-14 14:35:37.0|TWscan-prod|TWscan-prod|
|04 / 05|5298|15|13|2024-08-14 14:14:26.0|2024-08-14 14:35:40.0|TWscan-prod|TWscan-prod|
|05 / 05|5298|15|14|2024-08-14 14:14:39.0|2024-08-14 14:35:39.0|TWscan-prod|TWscan-prod|


# [BRNDDTL] Brand Detail


```sql
   
    /**
     * SUPBRAND.SURBRNDID :主品牌
     */

    SELECT
         '主品牌' S1 , C.*
        FROM P4P.SUPGLD A
            INNER JOIN P4P.SUPBRAND B ON A.SUPSUPCD = B.SURSUPCD
            INNER JOIN P4P.BRNDDTL  C ON C.BNDID    = B.SURBRNDID
        WHERE 0=0
          AND A.SUPSUPCD = '5298'

    UNION

    /**
     * SUPBRAND.SURSBRNDID :子品牌
     */
    SELECT
        '子品牌' S1 ,C.*
        FROM P4P.SUPGLD A
            INNER JOIN P4P.SUPBRAND B ON A.SUPSUPCD = B.SURSUPCD
            INNER JOIN P4P.BRNDDTL  C ON C.BNDID    = B.SURSBRNDID
        WHERE 0=0
          AND A.SUPSUPCD = '5298'

```

|SEQ|S1|BNDID|BNDBRNDEDESC|BNDBRNDLDESC|BNDCRE|BNDUPD|BNDUSR|BNDCREUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 07|主品牌|3|P&G|寶僑|2024-08-14 13:45:23.0|2024-08-14 13:45:23.0|TWscan-prod|TWscan-prod|
|02 / 07|主品牌|15|P&G|寶僑中文|2024-08-14 14:14:26.0|2024-08-14 14:14:26.0|TWscan-prod|TWscan-prod|
|03 / 07|子品牌|2|Lenor|蘭諾|2024-08-14 13:45:45.0|2024-08-14 13:45:45.0|TWscan-prod|TWscan-prod|
|04 / 07|子品牌|5|Gillete|吉列|2024-08-14 13:49:14.0|2024-08-14 13:49:14.0|TWscan-prod|TWscan-prod|
|05 / 07|子品牌|13|蘭諾|蘭諾|2024-08-14 14:14:26.0|2024-08-14 14:14:26.0|TWscan-prod|TWscan-prod|
|06 / 07|子品牌|14|吉列|吉列|2024-08-14 14:14:39.0|2024-08-14 14:14:39.0|TWscan-prod|TWscan-prod|
|07 / 07|子品牌|20|Lenor|兰诺|2024-08-14 14:25:00.0|2024-08-14 14:25:00.0|TWscan-prod|TWscan-prod|


# [MSTDEP] Dept


```sql
   
    SELECT
        C.*
    FROM P4P.SUPGLD A
        INNER JOIN P4P.SUPDEP B ON B.SUDSUPCD = A.SUPSUPCD
        INNER JOIN P4P.MSTDEP C ON B.SUDDPCD  = C.MSDDPCD
    WHERE 0=0
      AND A.SUPSUPCD = '5298'


```

|SEQ|MSDDPCD|MSDEDESC|MSDLDESC|MSDDVCD|MSDSTAT|MSDCRE|MSDUPD|MSDUSR|MSDCREUSR|MSDAUTODEL|MSDISHIDACD|MSDREQWEIGHT|MSDUSECPM|MSDINCRNYC|MSDGENORD|MSDFULLPACK|MSDUSETYP|MSDSHELFLIMIT|MSDSHELFLIMITUOM|MSDUSETYPALLO|MSDCTRFG|MSDMTAX|MSDFNF|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 06|10|Beverages|菸酒飲料|1|1|2009-05-08 19:00:00.0|2021-09-15 13:12:18.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|02 / 06|11|Cleaning|家用清潔用品|1|1|2009-05-08 19:00:00.0|2021-09-24 13:38:44.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|03 / 06|12|Cosmetics|生活藥粧|1|1|2009-05-08 19:00:00.0|2021-09-24 13:38:44.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|0|N|N|null|
|04 / 06|30|Do-It-Yourself|自己動手做|3|1|2009-05-08 19:00:00.0|2018-07-30 09:41:31.0|victorshih|MIGRATION|Y|1|N|1|1|N|Y|1|null|null|0|N|N|null|
|05 / 06|41|Small Household Appliance|小家電|4|1|2009-05-08 19:00:00.0|2012-08-18 10:50:48.0|victorshih|MIGRATION|Y|1|N|1|0|N|Y|1|null|null|null|null|null|null|
|06 / 06|76|Free goods and gifts| 贈品和禮品|7|1|2013-02-18 09:28:10.0|2024-03-12 11:18:25.0|F000172066|F000033546|Y|1|N|1|1|N|Y|0|null|null|0|N|N|null|


# [STOGLD] Store


```sql
   
    SELECT
        D.*
     FROM P4P.SUPGLD A
        INNER JOIN P4P.SUPDEP B ON B.SUDSUPCD = A.SUPSUPCD
        INNER JOIN P4P.SUPSTO C ON C.SUSSUPCD = A.SUPSUPCD AND C.SUSDPCD  = B.SUDDPCD
        INNER JOIN P4P.STOGLD D ON C.SUSSTOCD = D.STOSTOCD
    WHERE 0=0
      AND A.SUPSUPCD = '5298'
    FETCH FIRST 5 ROWS ONLY

```

|SEQ|STOSTOCD|STOEDESC|STOLDESC|STOREGION|STOTYPE|STOSHORT|STOORDABLE|STOBRCD|STOBREDESC|STOBRLDESC|STOLADDR1|STOLADDR2|STOEADDR1|STOEADDR2|STOSTATE|STOWELID|STOTAXID|STOCASHIER|STOFORMAT|STOCATE|STOMKT|STOTAXLOC|STOCITY|STOCRE|STOUPD|STOUSR|STOCREUSR|STOMUNICIPAL|STOPRINTER|STOTRANS|STOAREACD|STOARO|STOITMDESC|STOCHANGEPP|STORETURN|STOADJORD|STOCOSTCAL|STOCYSTART|STOCYEND|STOAUTOORD|STODEFINEL|STODEFINEE|STOGLN|STODAYSSEARCH|STOPPDECIMAL|STOSPDECIMAL|STOWGSHORT|STOPRICELEN|STONONSCHORD|STOLGORDBY|STOWGTYP|STOTAB|STOBUCD|STOPSSTO|STORETURNPRITOL|STOSTOPOS|STOPSGL|STOPSAP|STOPSHO|STOPSBC|STOPSTZ|STOPSCOUNTRY|STOPSCOUNTRYCD|STOPSORIGIN|STOPSSETID|STOPSINTINF|STOALERTTIME1|STOALERTTIME2|STOALERTTIME3|STOALERTCOLOR1|STOALERTCOLOR2|STOALERTCOLOR3|STOSPLTLGTPO|STOTOLEBTWSUG|STOINPUTMRP|STOMRPDIFFPO|STOALERTNSP|STOPRINTDCOD|STODEFAULTLOC|STORECRETURNWH|STOSTKCONSIGN|STOSTKLOC|STOMERGELIST|STOSTKADJIMA|STPSTKADJFG|STOLOC|STOPOFT|STOPHONENO|STOFAXNO|STOSTICKPRINTER|STOBYPSRAWF|STOSEMIPRINTER|STOECBUS|BUSINESSFORMAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|006|Model Store|單品模範店|0|S|006|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|22662550|T|HYP|H|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:43:36.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900065|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|null|20|null|null|null|null|null|null|null|null|null|null|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|02 / 05|010|South Region Office|南區辦公室|0|O|010|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|006|C|HYP|L|Z|null|003|2009-03-27 00:00:00.0|2021-04-09 16:08:54.0|L2_MD_8018|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|11:00|0|null|null|4717546900102|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|TWA912|20|null|null|null|null|null|null|null|null|null|null|null|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|1|HYP|
|03 / 05|013|Chung Hua (CH)|中華店 (CH)|4|S|CH|1|null|null|null|710 台南市永康區中華二路350號B1-1-8|null|B1-1-8 350 CHUNG-HUA 2ND ROAD|YONG KANG TAINAN 710|null|null|22662550|T|HYP|H|A|null|016|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900133|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA006|0|0013|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|06-275-6050|06-236-9352|PR|null|PS|1|HYP|
|04 / 05|015|Chung Cheng (CC)|中正店 (CC)|4|S|CC|1|null|null|null|710 台南市永康區中正南路358號|null|358 CHUNG-CHENG SOUTH ROAD|YONG KANG TAINAN 710|null|null|22662550|T|HYP|H|A|null|016|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900157|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA009|0|0015|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|06-253-8481|06-254-6742|PR|null|PS|1|HYP|
|05 / 05|016|Chia Yi (CY)|嘉義店 (CY)|3|S|CY|1|null|null|null|600 嘉義市博愛路二段461號|null|461 PO-AI ROAD SEC.2 CHIA YI 600|null|null|null|22662550|T|HYP|H|A|null|013|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900164|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA015|0|0016|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|05-235-3606|05-286-3550|PR|null|PS|1|HYP|


# [ITMGLD] ITEM_Has_Brand


```sql
   
    SELECT
        C.*
    FROM P4P.SUPGLD A
        INNER JOIN P4P.ITMSUP B ON B.ITUSUPCD = A.SUPSUPCD
        INNER JOIN P4P.ITMGLD C ON B.ITUITMID = C.ITMITMID
    WHERE 0=0
      AND A.SUPSUPCD = '5298'
      AND C.ITMITMCD = '110002'
      AND C.ITMLBRAND IS NOT NULL


```

|SEQ|ITMITMID|ITMDPCD|ITMITMCD|ITMMSCD|ITMSPEC|ITMEDESC|ITMLDESC|ITMSHNM|ITMSTKUN|ITMPACK|ITMCAPA|ITMCAPUT|ITMCAPML|ITMCOLNO|ITMSPTYP|ITMTYPSEL|ITMSEACD|ITMSENSIT|ITMTAX|ITMWEIGHT|ITMPCWGH|ITMGRADE|ITMCORIG|ITMRBPCT|ITMINPMON|ITMSTOP|ITMSTOPRS|ITMARO|ITMORDDAY|ITMORDPER|ITMLEADTM|ITMDELDAY|ITMMSUPCD|ITMDSSUP|ITMCRE|ITMUPD|ITMUSR|ITMCREUSR|ITMDELFLAG|ITMTYP|ITMSHELF|ITMDCAPUT|ITMDCAPA|ITMESTOP|ITMSUBTAX|ITMBRAND|ITMSUBBRAND|ITMRETURN|ITMWARRANTY|ITMSHELFLIFE|ITMCOMPLETE|ITMTAB|ITMINTBAR|ITMSHELFVALUE|ITMALLSTOP|ITMITMCDWEB|ITMSCAPA|ITMNPACK|ITMLGFLAG|ITMINGUN|ITMWGHING|ITMWGHINGUN|ITMWGHSTK|ITMINGQTYSTK|ITMTYPO|ITMUSEDATE|ITMUSEDATEUOM|ITMSHELFLIMITUOM|ITMSHELFLIMIT|ITMRTNTMP|ITMRTNPMT|ITMSUPLDESC|ITMSUPEDESC|ITMSUPCAPA|ITMSUPCAPUT|ITMSUPSTKUN|ITMWHCHK|ITMMIXPACK|ITMLGREQ|ITMGEXCF|ITMITMCAT|ITMITMLV|ITMLBRAND|ITMEBRAND|ITMLSBRAND|ITMESBRAND|ITMPROORG|ITMTAXCAT|ITMTAXSUBCAT|ITMDOCTYPE|ITMDOCNAME|ITMFOODATT|ITMAIRPFATT|ITMQTYBOX|ITMNQTYBOX|ITMPKBOX|ITMNPKBOX|ITMCNCD|ITMBRDORI|ITMITMCHAR|ITMCHARSDAT|ITMCHAREDAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|374968|12|110002|110|B|GLT PROSHIELD CHILL MANUAL RAZOR|吉列鋒護冰爽刮鬍刀架|吉列鋒護冰爽刀架|PC支|6|1 PC支|PC支|1|null|G|3|0|4|1|N|null|3U|DEU|0|2016-10-15 00:00:00.0|2023-12-17 00:00:00.0|2|0|1234567|1|2|1234567|F459|5298|2016-10-14 16:06:41.0|2024-08-14 14:28:26.0|TWscan-prod|PKNSAIPDMWF|N|3|S|PC支|1|2049-12-31 00:00:00.0|null|null|null|0|0|null|1|ABCDEFGHIJSTOKLQRP|null|null|2023-07-13 00:00:00.0|null|1|null|null|null|null|null|null|null|1|null|null|null|null|0|0|null|null|null|null|null|N|N|0|null|null|null|寶僑|P&G|蘭諾2|Lenor2|null|null|null|null|null|null|null|6|null|1|null|null|null|null|null|null|


# [ITMGLD] ITEM


```sql
   
    SELECT
        A.*
    FROM P4P.ITMGLD A

    WHERE 0=0
      AND A.ITMITMCD = '110002'


```

|SEQ|ITMITMID|ITMDPCD|ITMITMCD|ITMMSCD|ITMSPEC|ITMEDESC|ITMLDESC|ITMSHNM|ITMSTKUN|ITMPACK|ITMCAPA|ITMCAPUT|ITMCAPML|ITMCOLNO|ITMSPTYP|ITMTYPSEL|ITMSEACD|ITMSENSIT|ITMTAX|ITMWEIGHT|ITMPCWGH|ITMGRADE|ITMCORIG|ITMRBPCT|ITMINPMON|ITMSTOP|ITMSTOPRS|ITMARO|ITMORDDAY|ITMORDPER|ITMLEADTM|ITMDELDAY|ITMMSUPCD|ITMDSSUP|ITMCRE|ITMUPD|ITMUSR|ITMCREUSR|ITMDELFLAG|ITMTYP|ITMSHELF|ITMDCAPUT|ITMDCAPA|ITMESTOP|ITMSUBTAX|ITMBRAND|ITMSUBBRAND|ITMRETURN|ITMWARRANTY|ITMSHELFLIFE|ITMCOMPLETE|ITMTAB|ITMINTBAR|ITMSHELFVALUE|ITMALLSTOP|ITMITMCDWEB|ITMSCAPA|ITMNPACK|ITMLGFLAG|ITMINGUN|ITMWGHING|ITMWGHINGUN|ITMWGHSTK|ITMINGQTYSTK|ITMTYPO|ITMUSEDATE|ITMUSEDATEUOM|ITMSHELFLIMITUOM|ITMSHELFLIMIT|ITMRTNTMP|ITMRTNPMT|ITMSUPLDESC|ITMSUPEDESC|ITMSUPCAPA|ITMSUPCAPUT|ITMSUPSTKUN|ITMWHCHK|ITMMIXPACK|ITMLGREQ|ITMGEXCF|ITMITMCAT|ITMITMLV|ITMLBRAND|ITMEBRAND|ITMLSBRAND|ITMESBRAND|ITMPROORG|ITMTAXCAT|ITMTAXSUBCAT|ITMDOCTYPE|ITMDOCNAME|ITMFOODATT|ITMAIRPFATT|ITMQTYBOX|ITMNQTYBOX|ITMPKBOX|ITMNPKBOX|ITMCNCD|ITMBRDORI|ITMITMCHAR|ITMCHARSDAT|ITMCHAREDAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 07|594327|11|110002|110|B|SNG BEADS BL 1B BL 2R |熊寶貝多效護衣芳香豆-藍風鈴組合包|熊寶貝多效護衣芳香|PC瓶|1|950 ml毫升|ml毫升|1|null|G|1|0|4|1|N|null|2U|TWN|8.5|2023-06-06 00:00:00.0|null|null|0|1234567|1|3|1234567|E379|0552|2023-06-05 19:40:03.0|2024-05-07 20:08:42.0|SPOTACTION|PKNSAIPDMWF|N|3|S|ml毫升|100|null|null|null|null|0|null|Y|1|ABCDEFGHIJSTOKLQRP|null|3|null|null|950|null|null|null|null|null|null|null|1|null|null|D|729|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|6|null|6|null|null|TWN|null|null|null|
|02 / 07|374968|12|110002|110|B|GLT PROSHIELD CHILL MANUAL RAZOR|吉列鋒護冰爽刮鬍刀架|吉列鋒護冰爽刀架|PC支|6|1 PC支|PC支|1|null|G|3|0|4|1|N|null|3U|DEU|0|2016-10-15 00:00:00.0|2023-12-17 00:00:00.0|2|0|1234567|1|2|1234567|F459|5298|2016-10-14 16:06:41.0|2024-08-14 14:28:26.0|TWscan-prod|PKNSAIPDMWF|N|3|S|PC支|1|2049-12-31 00:00:00.0|null|null|null|0|0|null|1|ABCDEFGHIJSTOKLQRP|null|null|2023-07-13 00:00:00.0|null|1|null|null|null|null|null|null|null|1|null|null|null|null|0|0|null|null|null|null|null|N|N|0|null|null|null|寶僑|P&G|蘭諾2|Lenor2|null|null|null|null|null|null|null|6|null|1|null|null|null|null|null|null|
|03 / 07|23815|22|110002|110|B|Cherry(Jumbo)|櫻桃(Jumbo)|櫻桃(Jumbo)|Kg公斤|1|1 Kg公斤|Kg公斤|1|F2|R|2|0|4|0|Y|0|1U|NZL|0|2006-02-01 00:00:00.0|null|null|0|null|null|null|null|D228|null|2009-05-08 19:00:00.0|2024-02-08 14:03:51.0|AutoRelease|MIGRATION|N|2|L|TKg台斤|1|null|null|null|null|1|0|null|1|ABCDEFGHIJSTOKLQRP|2|null|null|null|1|null|null|null|null|null|null|null|1|null|null|null|null|1|1|null|null|null|null|null|N|N|0|null|null|null|null|null|null|null|null|null|null|null|null|null|null|1|null|1|null|null|null|null|null|null|
|04 / 07|584765|21|110002|110|B|Tempula piece|特級日式天婦羅片185g (原料)|特級日式天婦羅片|Box盒|15|1 Box盒|Box盒|1|F0|G|2|0|4|1|Y|1|SPE|TWN|0|2023-02-18 00:00:00.0|null|null|0|null|null|null|null|C422|null|2023-02-17 16:52:48.0|2024-03-26 18:44:45.0|PKNSAIPDMWF|PKNSAIPDMWF|N|2|S|Box盒|1|null|null|null|null|1|null|Y|1|ABCDEFGHIJSOKLQRP|null|1|null|null|1|null|null|null|null|null|null|null|0|null|null|D|242|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|15|null|1|null|null|null|null|null|null|
|05 / 07|243224|14|110002|110|C|C-Grape Pie|家福葡萄派|家福葡萄派|Box盒|10|168 g克|g克|1|null|G|C|0|5|1|N|null|2U|TWN|0|2013-06-13 00:00:00.0|null|null|0|1234567|1|3|1234567|E379|B365|2013-06-13 14:13:20.0|2024-02-01 21:31:41.0|SPOTACTION|PKNSAIPDM|N|3|L|g克|100|null|null|null|null|0|0|D|1|ABCDEFGHIJSTOKLQRP|null|300|null|null|168|null|null|null|null|null|null|null|1|null|null|D|199|0|0|null|null|null|null|null|N|N|1|null|null|null|null|null|null|null|null|null|null|null|null|null|null|10|null|1|null|null|null|null|null|null|
|06 / 07|622525|44|110002|110|B|Pokemon Card Scarlet Violet|寶可夢卡牌 朱紫 變幻假面 收藏家組合|變幻假面收藏家組|BOX盒|1|1 Box盒|Box盒|1|null|G|K|1|4|1|N|null|SPE|JPN|3.5|2024-04-27 00:00:00.0|null|null|0|null|null|null|null|H219|null|2024-04-26 18:48:57.0|2024-05-07 09:23:05.0|PKNSAIPDMWF|PKNSAIPDMWF|N|3|S|Box盒|1|null|null|null|null|0|null|null|1|ABCDEFGHIJSOKLQRP|null|null|null|null|1|null|null|null|null|null|null|null|0|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|1|null|1|null|null|null|null|null|null|
|07 / 07|579310|20|110002|110|B|Vicenzi Puff Pastry|侑-鹹蛋黃千層酥-專櫃|鹹蛋黃千層酥|PACK包|1|1 Pack包|Pack包|1|F3|G|7|1|4|1|N|null|CON|TWN|0|2022-11-25 00:00:00.0|null|null|0|null|null|null|null|H964|null|2022-11-24 18:22:50.0|2023-02-15 09:35:03.0|PMD8713-1|PKNSAIPDMWF|N|2|S|Pack包|1|null|null|null|null|1|null|Y|1|ABCDEFGHIJSOKLQRP|null|1|null|null|1|null|null|null|null|null|null|null|0|null|null|D|242|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|null|1|null|1|null|null|TWN|null|null|null|

