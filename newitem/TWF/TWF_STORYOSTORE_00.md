
# Story HBR

- 部門：10
- Business Format : HYP

```sql
   
SELECT ST.* FROM STOGLD ST
    INNER JOIN (
        select DISTINCT WSTSTOCD as SC  from WSTORYTYPO  where 1=1
            AND WSTDEPCD = '10'
            AND WSTCD = 'HBR' AND WSTBIZFORMAT =  'HYP'
        UNION
        select TBDENTCD SC from tbldtl where TBDTBNO = 727 and TBDNUM1 = 1
    ) C ON ST.STOSTOCD = C.SC
 WHERE 0=0
       AND ST.STOTYPE <> 'O'
FETCH FIRST 5 ROWS ONLY

```

|SEQ|STOSTOCD|STOEDESC|STOLDESC|STOREGION|STOTYPE|STOSHORT|STOORDABLE|STOBRCD|STOBREDESC|STOBRLDESC|STOLADDR1|STOLADDR2|STOEADDR1|STOEADDR2|STOSTATE|STOWELID|STOTAXID|STOCASHIER|STOFORMAT|STOCATE|STOMKT|STOTAXLOC|STOCITY|STOCRE|STOUPD|STOUSR|STOCREUSR|STOMUNICIPAL|STOPRINTER|STOTRANS|STOAREACD|STOARO|STOITMDESC|STOCHANGEPP|STORETURN|STOADJORD|STOCOSTCAL|STOCYSTART|STOCYEND|STOAUTOORD|STODEFINEL|STODEFINEE|STOGLN|STODAYSSEARCH|STOPPDECIMAL|STOSPDECIMAL|STOWGSHORT|STOPRICELEN|STONONSCHORD|STOLGORDBY|STOWGTYP|STOTAB|STOBUCD|STOPSSTO|STORETURNPRITOL|STOSTOPOS|STOPSGL|STOPSAP|STOPSHO|STOPSBC|STOPSTZ|STOPSCOUNTRY|STOPSCOUNTRYCD|STOPSORIGIN|STOPSSETID|STOPSINTINF|STOALERTTIME1|STOALERTTIME2|STOALERTTIME3|STOALERTCOLOR1|STOALERTCOLOR2|STOALERTCOLOR3|STOSPLTLGTPO|STOTOLEBTWSUG|STOINPUTMRP|STOMRPDIFFPO|STOALERTNSP|STOPRINTDCOD|STODEFAULTLOC|STORECRETURNWH|STOSTKCONSIGN|STOSTKLOC|STOMERGELIST|STOSTKADJIMA|STPSTKADJFG|STOLOC|STOPOFT|STOPHONENO|STOFAXNO|STOSTICKPRINTER|STOBYPSRAWF|STOSEMIPRINTER|STOECBUS|BUSINESSFORMAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|006|Model Store|單品模範店|0|S|006|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|22662550|T|HYP|H|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:43:36.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900065|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|null|20|null|null|null|null|null|null|null|null|null|null|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|02 / 05|016|Chia Yi (CY)|嘉義店 (CY)|3|S|CY|1|null|null|null|600 嘉義市博愛路二段461號|null|461 PO-AI ROAD SEC.2 CHIA YI 600|null|null|null|22662550|T|HYP|H|A|null|013|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900164|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA015|0|0016|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|05-235-3606|05-286-3550|PR|null|PS|1|HYP|
|03 / 05|018|Ping Tung (PT)|屏東店 (PT)|4|S|PT|1|null|null|null|900 屏東市仁愛路188號|null|188 JEN-AI ROAD PING TUNG 900|null|null|null|22662550|T|HYP|H|A|null|021|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900188|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA013|0|0018|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|08-738-0310|08-736-0125|PR|null|PS|1|HYP|
|04 / 05|019|Love River (LR)|愛河店 (LR)|4|S|LR|1|null|null|null|803 高雄市河東路356號|null|356 HER-TUNG ROAD KAOHSIUNG 803|null|null|null|22662550|T|HYP|H|A|null|018|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900195|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA011|0|0019|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|07-272-5066|07-272-0342|PR|null|PS|1|HYP|
|05 / 05|01E|Fong Shan (FS)|鳳山店 (FS)|4|S|FS|1|null|null|null|830 高雄市鳳山區中山西路236號|null|236 CHUNGSHAN WEST ROAD  FONG SHAN|KAOHSUING COUNTY 830|null|null|22662550|T|HYP|H|A|null|018|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546901147|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA031|0|0114|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|07-740-1789|07-740-1779|PR|null|PS|1|HYP|


# Story J02

- 部門：10
- Business Format : SUP

```sql
   
SELECT ST.* FROM STOGLD ST
    INNER JOIN (
        select DISTINCT WSTSTOCD as SC  from WSTORYTYPO  where 1=1
            AND WSTDEPCD = '10'
            AND WSTCD = 'J02' AND WSTBIZFORMAT =  'SUP'
        UNION
        select TBDENTCD SC from tbldtl where TBDTBNO = 727 and TBDNUM1 = 1
    ) C ON ST.STOSTOCD = C.SC
 WHERE 0=0
       AND ST.STOTYPE <> 'O'
FETCH FIRST 5 ROWS ONLY

```

|SEQ|STOSTOCD|STOEDESC|STOLDESC|STOREGION|STOTYPE|STOSHORT|STOORDABLE|STOBRCD|STOBREDESC|STOBRLDESC|STOLADDR1|STOLADDR2|STOEADDR1|STOEADDR2|STOSTATE|STOWELID|STOTAXID|STOCASHIER|STOFORMAT|STOCATE|STOMKT|STOTAXLOC|STOCITY|STOCRE|STOUPD|STOUSR|STOCREUSR|STOMUNICIPAL|STOPRINTER|STOTRANS|STOAREACD|STOARO|STOITMDESC|STOCHANGEPP|STORETURN|STOADJORD|STOCOSTCAL|STOCYSTART|STOCYEND|STOAUTOORD|STODEFINEL|STODEFINEE|STOGLN|STODAYSSEARCH|STOPPDECIMAL|STOSPDECIMAL|STOWGSHORT|STOPRICELEN|STONONSCHORD|STOLGORDBY|STOWGTYP|STOTAB|STOBUCD|STOPSSTO|STORETURNPRITOL|STOSTOPOS|STOPSGL|STOPSAP|STOPSHO|STOPSBC|STOPSTZ|STOPSCOUNTRY|STOPSCOUNTRYCD|STOPSORIGIN|STOPSSETID|STOPSINTINF|STOALERTTIME1|STOALERTTIME2|STOALERTTIME3|STOALERTCOLOR1|STOALERTCOLOR2|STOALERTCOLOR3|STOSPLTLGTPO|STOTOLEBTWSUG|STOINPUTMRP|STOMRPDIFFPO|STOALERTNSP|STOPRINTDCOD|STODEFAULTLOC|STORECRETURNWH|STOSTKCONSIGN|STOSTKLOC|STOMERGELIST|STOSTKADJIMA|STPSTKADJFG|STOLOC|STOPOFT|STOPHONENO|STOFAXNO|STOSTICKPRINTER|STOBYPSRAWF|STOSEMIPRINTER|STOECBUS|BUSINESSFORMAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|006|Model Store|單品模範店|0|S|006|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|22662550|T|HYP|H|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:43:36.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900065|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|null|20|null|null|null|null|null|null|null|null|null|null|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|02 / 02|031|Logistics|後勤|0|L|LGS|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|031|C|HYP|L|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:41:26.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|11:00|0|null|null|4717546900102|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|TWY900|20|null|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|


# Story CS2

- 部門：10
- Business Format : JSN

```sql
   
SELECT ST.* FROM STOGLD ST
    INNER JOIN (
        select DISTINCT WSTSTOCD as SC  from WSTORYTYPO  where 1=1
            AND WSTDEPCD = '10'
            AND WSTCD = 'CS2' AND WSTBIZFORMAT =  'JSN'
        UNION
        select TBDENTCD SC from tbldtl where TBDTBNO = 727 and TBDNUM1 = 1
    ) C ON ST.STOSTOCD = C.SC
 WHERE 0=0
       AND ST.STOTYPE <> 'O'
FETCH FIRST 5 ROWS ONLY

```

|SEQ|STOSTOCD|STOEDESC|STOLDESC|STOREGION|STOTYPE|STOSHORT|STOORDABLE|STOBRCD|STOBREDESC|STOBRLDESC|STOLADDR1|STOLADDR2|STOEADDR1|STOEADDR2|STOSTATE|STOWELID|STOTAXID|STOCASHIER|STOFORMAT|STOCATE|STOMKT|STOTAXLOC|STOCITY|STOCRE|STOUPD|STOUSR|STOCREUSR|STOMUNICIPAL|STOPRINTER|STOTRANS|STOAREACD|STOARO|STOITMDESC|STOCHANGEPP|STORETURN|STOADJORD|STOCOSTCAL|STOCYSTART|STOCYEND|STOAUTOORD|STODEFINEL|STODEFINEE|STOGLN|STODAYSSEARCH|STOPPDECIMAL|STOSPDECIMAL|STOWGSHORT|STOPRICELEN|STONONSCHORD|STOLGORDBY|STOWGTYP|STOTAB|STOBUCD|STOPSSTO|STORETURNPRITOL|STOSTOPOS|STOPSGL|STOPSAP|STOPSHO|STOPSBC|STOPSTZ|STOPSCOUNTRY|STOPSCOUNTRYCD|STOPSORIGIN|STOPSSETID|STOPSINTINF|STOALERTTIME1|STOALERTTIME2|STOALERTTIME3|STOALERTCOLOR1|STOALERTCOLOR2|STOALERTCOLOR3|STOSPLTLGTPO|STOTOLEBTWSUG|STOINPUTMRP|STOMRPDIFFPO|STOALERTNSP|STOPRINTDCOD|STODEFAULTLOC|STORECRETURNWH|STOSTKCONSIGN|STOSTKLOC|STOMERGELIST|STOSTKADJIMA|STPSTKADJFG|STOLOC|STOPOFT|STOPHONENO|STOFAXNO|STOSTICKPRINTER|STOBYPSRAWF|STOSEMIPRINTER|STOECBUS|BUSINESSFORMAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 02|006|Model Store|單品模範店|0|S|006|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|22662550|T|HYP|H|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:43:36.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900065|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|null|20|null|null|null|null|null|null|null|null|null|null|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|02 / 02|031|Logistics|後勤|0|L|LGS|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|031|C|HYP|L|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:41:26.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|11:00|0|null|null|4717546900102|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|TWY900|20|null|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|

