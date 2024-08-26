# TBLDTL 48 原產國 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '48'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|48|Country of Origin|原產國|Define the origin country for item by using ISO key 3166; C1=Country Seq. of PC weight scale|296|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '48'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 40|48|ABW|Aruba|阿路巴|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 40|48|AFG|Afghanistan|阿富汗|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 40|48|AGO|Angola|安哥拉|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 40|48|AIA|Anguilla|安圭拉|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 40|48|ALA|Aland Islands|芬蘭|2|null|null|null|null|62|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:37.0|PMD9058|
|06 / 40|48|ALB|Albania|阿爾巴尼亞|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|07 / 40|48|AND|Andorra|安道爾共和國|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|08 / 40|48|ANT|Netherlands Antilles|荷屬安地列斯|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|09 / 40|48|ARE|United Arab Emirates|阿拉伯聯合大公國|2|null|null|null|null|50|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:37.0|PMD9058|
|10 / 40|48|ARG|Argentina|阿根廷|2|null|null|null|null|18|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:35.0|PMD9058|
|11 / 40|48|ARM|Armenia|亞美尼亞|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|12 / 40|48|ASM|American Samoa|美屬薩摩亞|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|13 / 40|48|ATA|Antarctica|南極洲|2|null|null|null|null|64|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:37.0|PMD9058|
|14 / 40|48|ATF|French Southern Territories|法國南部和南極的領土|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|15 / 40|48|ATG|Antigua and Barbuda|安地卡及巴布達|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|16 / 40|48|AUS|Australia|澳大利亞|2|null|null|null|null|4|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:34.0|PMD9058|
|17 / 40|48|AUT|Austria|奧地利|2|null|null|null|null|68|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:38.0|PMD9058|
|18 / 40|48|AZE|Azerbaijan|亞塞拜然|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|19 / 40|48|BDI|Burundi|蒲隆地|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|20 / 40|48|BEL|Belgium|比利時|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|21 / 40|48|BEN|Benin|貝南|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|22 / 40|48|BFA|Burkina Faso|有吉納法索|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|23 / 40|48|BGD|Bangladesh|孟加拉|2|null|null|null|null|49|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:37.0|PMD9058|
|24 / 40|48|BGR|Bulgaria|保加利亞|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|25 / 40|48|BHR|Bahrain|巴林|2|null|null|null|null|26|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:35.0|PMD9058|
|26 / 40|48|BHS|Bahamas|巴哈馬|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|27 / 40|48|BIH|Bosnia and Herzegovina|波希尼亞及赫塞哥維那|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|28 / 40|48|BLM|Saint Barthelemy|聖巴托洛繆島|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|29 / 40|48|BLR|Belarus|白俄羅斯|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|30 / 40|48|BLZ|Belize|貝里斯|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|31 / 40|48|BMU|Bermuda|百慕達|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|32 / 40|48|BOL|Bolivia|玻利維亞|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|33 / 40|48|BRA|Brazil|巴西|2|null|null|null|null|25|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:35.0|PMD9058|
|34 / 40|48|BRB|Barbados|巴貝多|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|35 / 40|48|BRN|Brunei Darussalam|汶萊|2|null|null|null|null|47|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:36.0|PMD9058|
|36 / 40|48|BTN|Bhutan|不丹|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|37 / 40|48|BVT|Bouvet Island (Bouvetoya)|布維島|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|38 / 40|48|BWA|Botswana|波札那|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|39 / 40|48|CAF|Central African Republic|中非共和國|2|null|null|null|null|null|null|null|null|null|null|2009-03-27 00:00:00.0|2015-05-29 19:00:49.0|SSFIX_25550|
|40 / 40|48|CAN|Canada|加拿大|2|null|null|null|null|43|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:36.0|PMD9058|

