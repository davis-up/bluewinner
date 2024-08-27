
# Typo 1U

- 部門：10
- 商品分類 : 001

```sql
   
SELECT ST.* FROM STOGLD ST
    INNER JOIN (
        SELECT C.tysstocd SC
          FROM TYPMSTGT A
            LEFT JOIN TYPCLUSTYP B   ON A.tyttypcd = B.tyctypcd
            LEFT JOIN TYPSTOMSCLUS C ON A.tytdpcd  = C.tysdpcd AND  A.tytmscd = C.tysmscd AND B.tyccluscd = C.tyscluscd
        WHERE 1 = 1 AND A.tytdpcd = '10'  AND　A.tytmscd = '001'
            AND A.tyttypcd in( '1U' ) AND C.tysisdel = 0
            AND trunc(sysdate) between B.tycsdate and B.tycedate
            AND trunc(sysdate) between C.tyssdate and C.tysedate
        UNION
        select TBDENTCD SC from tbldtl where TBDTBNO = 727 and TBDNUM1 = 1
    ) C ON ST.STOSTOCD = C.SC
FETCH FIRST 5 ROWS ONLY

```

|SEQ|STOSTOCD|STOEDESC|STOLDESC|STOREGION|STOTYPE|STOSHORT|STOORDABLE|STOBRCD|STOBREDESC|STOBRLDESC|STOLADDR1|STOLADDR2|STOEADDR1|STOEADDR2|STOSTATE|STOWELID|STOTAXID|STOCASHIER|STOFORMAT|STOCATE|STOMKT|STOTAXLOC|STOCITY|STOCRE|STOUPD|STOUSR|STOCREUSR|STOMUNICIPAL|STOPRINTER|STOTRANS|STOAREACD|STOARO|STOITMDESC|STOCHANGEPP|STORETURN|STOADJORD|STOCOSTCAL|STOCYSTART|STOCYEND|STOAUTOORD|STODEFINEL|STODEFINEE|STOGLN|STODAYSSEARCH|STOPPDECIMAL|STOSPDECIMAL|STOWGSHORT|STOPRICELEN|STONONSCHORD|STOLGORDBY|STOWGTYP|STOTAB|STOBUCD|STOPSSTO|STORETURNPRITOL|STOSTOPOS|STOPSGL|STOPSAP|STOPSHO|STOPSBC|STOPSTZ|STOPSCOUNTRY|STOPSCOUNTRYCD|STOPSORIGIN|STOPSSETID|STOPSINTINF|STOALERTTIME1|STOALERTTIME2|STOALERTTIME3|STOALERTCOLOR1|STOALERTCOLOR2|STOALERTCOLOR3|STOSPLTLGTPO|STOTOLEBTWSUG|STOINPUTMRP|STOMRPDIFFPO|STOALERTNSP|STOPRINTDCOD|STODEFAULTLOC|STORECRETURNWH|STOSTKCONSIGN|STOSTKLOC|STOMERGELIST|STOSTKADJIMA|STPSTKADJFG|STOLOC|STOPOFT|STOPHONENO|STOFAXNO|STOSTICKPRINTER|STOBYPSRAWF|STOSEMIPRINTER|STOECBUS|BUSINESSFORMAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|006|Model Store|單品模範店|0|S|006|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|22662550|T|HYP|H|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:43:36.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900065|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|null|20|null|null|null|null|null|null|null|null|null|null|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|02 / 05|013|Chung Hua (CH)|中華店 (CH)|4|S|CH|1|null|null|null|710 台南市永康區中華二路350號B1-1-8|null|B1-1-8 350 CHUNG-HUA 2ND ROAD|YONG KANG TAINAN 710|null|null|22662550|T|HYP|H|A|null|016|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900133|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA006|0|0013|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|06-275-6050|06-236-9352|PR|null|PS|1|HYP|
|03 / 05|015|Chung Cheng (CC)|中正店 (CC)|4|S|CC|1|null|null|null|710 台南市永康區中正南路358號|null|358 CHUNG-CHENG SOUTH ROAD|YONG KANG TAINAN 710|null|null|22662550|T|HYP|H|A|null|016|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900157|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA009|0|0015|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|06-253-8481|06-254-6742|PR|null|PS|1|HYP|
|04 / 05|016|Chia Yi (CY)|嘉義店 (CY)|3|S|CY|1|null|null|null|600 嘉義市博愛路二段461號|null|461 PO-AI ROAD SEC.2 CHIA YI 600|null|null|null|22662550|T|HYP|H|A|null|013|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900164|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA015|0|0016|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|05-235-3606|05-286-3550|PR|null|PS|1|HYP|
|05 / 05|018|Ping Tung (PT)|屏東店 (PT)|4|S|PT|1|null|null|null|900 屏東市仁愛路188號|null|188 JEN-AI ROAD PING TUNG 900|null|null|null|22662550|T|HYP|H|A|null|021|2009-03-27 00:00:00.0|2021-03-03 23:06:29.0|CRID0551|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900188|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWA013|0|0018|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P5|L|0|1|0|1|M|6|L|null|08-738-0310|08-736-0125|PR|null|PS|1|HYP|


# Typo 1J

- 部門：10
- 商品分類 : 001

```sql
   
SELECT ST.* FROM STOGLD ST
    INNER JOIN (
        SELECT C.tysstocd SC
          FROM TYPMSTGT A
            LEFT JOIN TYPCLUSTYP B   ON A.tyttypcd = B.tyctypcd
            LEFT JOIN TYPSTOMSCLUS C ON A.tytdpcd  = C.tysdpcd AND  A.tytmscd = C.tysmscd AND B.tyccluscd = C.tyscluscd
        WHERE 1 = 1 AND A.tytdpcd = '10'  AND　A.tytmscd = '001'
            AND A.tyttypcd in( '1J' ) AND C.tysisdel = 0
            AND trunc(sysdate) between B.tycsdate and B.tycedate
            AND trunc(sysdate) between C.tyssdate and C.tysedate
        UNION
        select TBDENTCD SC from tbldtl where TBDTBNO = 727 and TBDNUM1 = 1
    ) C ON ST.STOSTOCD = C.SC
FETCH FIRST 5 ROWS ONLY

```

|SEQ|STOSTOCD|STOEDESC|STOLDESC|STOREGION|STOTYPE|STOSHORT|STOORDABLE|STOBRCD|STOBREDESC|STOBRLDESC|STOLADDR1|STOLADDR2|STOEADDR1|STOEADDR2|STOSTATE|STOWELID|STOTAXID|STOCASHIER|STOFORMAT|STOCATE|STOMKT|STOTAXLOC|STOCITY|STOCRE|STOUPD|STOUSR|STOCREUSR|STOMUNICIPAL|STOPRINTER|STOTRANS|STOAREACD|STOARO|STOITMDESC|STOCHANGEPP|STORETURN|STOADJORD|STOCOSTCAL|STOCYSTART|STOCYEND|STOAUTOORD|STODEFINEL|STODEFINEE|STOGLN|STODAYSSEARCH|STOPPDECIMAL|STOSPDECIMAL|STOWGSHORT|STOPRICELEN|STONONSCHORD|STOLGORDBY|STOWGTYP|STOTAB|STOBUCD|STOPSSTO|STORETURNPRITOL|STOSTOPOS|STOPSGL|STOPSAP|STOPSHO|STOPSBC|STOPSTZ|STOPSCOUNTRY|STOPSCOUNTRYCD|STOPSORIGIN|STOPSSETID|STOPSINTINF|STOALERTTIME1|STOALERTTIME2|STOALERTTIME3|STOALERTCOLOR1|STOALERTCOLOR2|STOALERTCOLOR3|STOSPLTLGTPO|STOTOLEBTWSUG|STOINPUTMRP|STOMRPDIFFPO|STOALERTNSP|STOPRINTDCOD|STODEFAULTLOC|STORECRETURNWH|STOSTKCONSIGN|STOSTKLOC|STOMERGELIST|STOSTKADJIMA|STPSTKADJFG|STOLOC|STOPOFT|STOPHONENO|STOFAXNO|STOSTICKPRINTER|STOBYPSRAWF|STOSEMIPRINTER|STOECBUS|BUSINESSFORMAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|006|Model Store|單品模範店|0|S|006|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|22662550|T|HYP|H|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:43:36.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900065|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|null|20|null|null|null|null|null|null|null|null|null|null|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|02 / 05|031|Logistics|後勤|0|L|LGS|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|031|C|HYP|L|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:41:26.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|11:00|0|null|null|4717546900102|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|TWY900|20|null|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|03 / 05|813|Mia C’bon Chu Pei (0R)|竹北高鐵店 (0R)|28|S|0R|1|null|null|null|302 新竹縣竹北市文興路二段2號|null|No. 2 ,Section 1,Wenxing Rd, Chu-Bei |City, Hsin Chu County 302|null|null|22662550|T|SUP|S|D|null|006|2022-05-05 00:06:21.0|2022-10-24 15:59:07.0|md8706|victorshih|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546916776|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWP813|0|0445|TW080|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|1|0|1|M|6|L|null|03-657-9028|null|PR|0|PS|1|JSN|
|04 / 05|814|Mia C’bon Beyond (0L)|永和比漾店 (0L)|27|S|0L|1|null|null|null|234 新北市永和區中山路一段238號B2F|null|B2F, No.238 Chong Shan Rd. 1st Section, |Yong-Ho District, New Taipei City 234|null|null|22662550|T|SUP|S|D|null|003|2022-05-26 00:11:40.0|2023-08-31 17:51:58.0|F000172061|victorshih|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546916783|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWP814|0|0446|TW080|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|1|0|1|M|6|L|null|02-8231-5950|null|PR|0|PS|1|JSN|
|05 / 05|815|Mia C’bon Hoping (0A)|台北和平店 (0A)|27|S|0A|1|null|null|null|106 台北市大安區羅斯福路2段41-49號B1|null|B1F, No. 41-49 & B2F No.41 Rosevelt Rd. |2nd Section, Taipei City 106|null|null|22662550|T|SUP|S|D|null|001|2022-04-07 00:09:32.0|2022-10-24 16:01:57.0|md8706|victorshih|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546916790|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWP815|0|0447|TW080|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|1|0|1|M|6|L|null|02-2396-9625|null|PR|0|PS|1|JSN|


# Typo 1S

- 部門：10
- 商品分類 : 001

```sql
   
SELECT ST.* FROM STOGLD ST
    INNER JOIN (
        SELECT C.tysstocd SC
          FROM TYPMSTGT A
            LEFT JOIN TYPCLUSTYP B   ON A.tyttypcd = B.tyctypcd
            LEFT JOIN TYPSTOMSCLUS C ON A.tytdpcd  = C.tysdpcd AND  A.tytmscd = C.tysmscd AND B.tyccluscd = C.tyscluscd
        WHERE 1 = 1 AND A.tytdpcd = '10'  AND　A.tytmscd = '001'
            AND A.tyttypcd in( '1S' ) AND C.tysisdel = 0
            AND trunc(sysdate) between B.tycsdate and B.tycedate
            AND trunc(sysdate) between C.tyssdate and C.tysedate
        UNION
        select TBDENTCD SC from tbldtl where TBDTBNO = 727 and TBDNUM1 = 1
    ) C ON ST.STOSTOCD = C.SC
FETCH FIRST 5 ROWS ONLY

```

|SEQ|STOSTOCD|STOEDESC|STOLDESC|STOREGION|STOTYPE|STOSHORT|STOORDABLE|STOBRCD|STOBREDESC|STOBRLDESC|STOLADDR1|STOLADDR2|STOEADDR1|STOEADDR2|STOSTATE|STOWELID|STOTAXID|STOCASHIER|STOFORMAT|STOCATE|STOMKT|STOTAXLOC|STOCITY|STOCRE|STOUPD|STOUSR|STOCREUSR|STOMUNICIPAL|STOPRINTER|STOTRANS|STOAREACD|STOARO|STOITMDESC|STOCHANGEPP|STORETURN|STOADJORD|STOCOSTCAL|STOCYSTART|STOCYEND|STOAUTOORD|STODEFINEL|STODEFINEE|STOGLN|STODAYSSEARCH|STOPPDECIMAL|STOSPDECIMAL|STOWGSHORT|STOPRICELEN|STONONSCHORD|STOLGORDBY|STOWGTYP|STOTAB|STOBUCD|STOPSSTO|STORETURNPRITOL|STOSTOPOS|STOPSGL|STOPSAP|STOPSHO|STOPSBC|STOPSTZ|STOPSCOUNTRY|STOPSCOUNTRYCD|STOPSORIGIN|STOPSSETID|STOPSINTINF|STOALERTTIME1|STOALERTTIME2|STOALERTTIME3|STOALERTCOLOR1|STOALERTCOLOR2|STOALERTCOLOR3|STOSPLTLGTPO|STOTOLEBTWSUG|STOINPUTMRP|STOMRPDIFFPO|STOALERTNSP|STOPRINTDCOD|STODEFAULTLOC|STORECRETURNWH|STOSTKCONSIGN|STOSTKLOC|STOMERGELIST|STOSTKADJIMA|STPSTKADJFG|STOLOC|STOPOFT|STOPHONENO|STOFAXNO|STOSTICKPRINTER|STOBYPSRAWF|STOSEMIPRINTER|STOECBUS|BUSINESSFORMAT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|006|Model Store|單品模範店|0|S|006|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|22662550|T|HYP|H|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:43:36.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546900065|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|null|20|null|null|null|null|null|null|null|null|null|null|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|02 / 05|031|Logistics|後勤|0|L|LGS|0|null|null|null|251 台北縣淡水鎮民權路27號後棟5樓|null|5F, Back Building,No.27, Min-Chuan Rd.,|Tam Hsui, Taipei, Taiwan, R.O.C 251|null|null|031|C|HYP|L|A|null|003|2009-03-27 00:00:00.0|2021-03-24 00:41:26.0|victorshih|MIGRATION|null|RP|0|02|0|B|N|N|4|0|22:00|11:00|0|null|null|4717546900102|60|2|0|1|0|1|0|D|ABCDEFGHIJ|1|TWY900|20|null|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|0|0|1|M|6|L|null|null|null|null|0|PS|0|HYP|
|03 / 05|05E|Yonghe Yongan (YY)|永和永安店 (YY)|33|S|YY|1|null|null|null|234 新北市永和區中和路499號之1~2號,499之5~55號|null|No.449-1~2, 449-5~55, Zhonghe Rd.,|Yonghe City, Taipei County 234, Taiwan|null|null|22662550|T|SUP|S|B|null|003|2009-11-09 02:25:30.0|2021-11-01 12:10:54.0|md8395|victorshih|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546901543|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWP502|0|0154|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P4|L|0|1|0|1|M|6|L|null|02-2232-7755|02-2923-1122|PR|0|PS|1|SUP|
|04 / 05|05S|Jongho Jingan (JA)|中和景安店 (JA)|38|S|JA|1|null|null|null|235 新北市中和區景平路353號B1|null|B1F., No.353, Jingping Rd., Zhonghe Dist|, New Taipei City 235, Taiwan (R.O.C.)|null|null|22662550|T|SUP|S|B|null|003|2013-04-28 09:17:08.0|2021-11-01 12:10:54.0|md8395|F000033546|null|RP|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546902588|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWP505|0|0159|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P4|L|0|1|0|1|M|6|L|null|02-2240-9628|02-2240-9728|PR|0|PS|1|SUP|
|05 / 05|05T|FongyuanFongNan (FN)|豐原豐南店 (FN)|42|S|FN|1|null|null|null|420 台中市豐原區豐南街118號|null|No. 118, Fengnan St., Fengyuan Dist.,|Taichung City 420, Taiwan (R.O.C.)|null|null|22662550|T|SUP|S|B|null|009|2013-04-28 09:22:51.0|2021-11-01 12:10:54.0|md8395|F000033546|null|RF|0|02|0|B|N|N|4|0|22:00|12:00|0|null|null|4717546902595|60|1|1|1|0|1|0|D|ABCDEFGHIJ|1|TWP507|0|0160|TW010|TW011|000|TWD|E08|TAIWAN|TW|S|TWMER|0|5|15|30|3|2|1|0|50|0|1|0|P3|L|0|1|0|1|M|6|L|null|04-2528-0897|04-2528-0893|PR|0|PS|1|SUP|

