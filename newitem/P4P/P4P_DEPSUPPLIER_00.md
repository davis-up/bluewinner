
# 部門供應商列表 

- 部門：10
- SUDRBPCT : 佣金
- SUACLCD: 類別
- SUACD: 寄賣代碼
- S1 : 寄賣
   - 數字 0 則無寄賣

```sql
   
        SELECT
            sup.SUPSUPCD ,                -- supplierCode
            sup.SUPEDESC ,                -- supplierEDesc
            sup.SUPLDESC ,                -- supplierLDesc
            supdept.SUDNATURE ,           -- supplierNature
            supdept.SUDRBPCT  ,           -- rebate
            COUNT(patt.SUACD) S1,         -- consignment
            patt.SUACLCD,
            patt.SUACD
        FROM SUPGLD sup
            INNER JOIN SUPDEP supdept   ON sup.SUPSUPCD = supdept.SUDSUPCD
            LEFT  JOIN SUPATT patt ON sup.SUPSUPCD = patt.SUASUPCD
                AND SYSDATE BETWEEN patt.SUASDATE AND patt.SUAEDATE
                AND ( patt.SUACLCD = 'CONS')
        WHERE supdept.SUDDPCD = '10'

            AND ( SUDNATURE <> 'W' )
            AND (
                    SUDSTPBUSDATE IS NULL
                    OR trunc(sysdate) < trunc(SUDSTPBUSDATE)
                )
        GROUP BY sup.SUPSUPCD,
            sup.SUPEDESC,
            sup.SUPLDESC,
            supdept.SUDNATURE,
            supdept.SUDRBPCT,
            patt.SUACLCD,
            patt.SUACD
        ORDER BY SUPSUPCD

        FETCH FIRST 5 ROWS ONLY

```

|SEQ|SUPSUPCD|SUPEDESC|SUPLDESC|SUDNATURE|SUDRBPCT|SUACLCD|SUACD|S1|
| -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|0003|TIED|DC--泰德利股份有限公司|D|14.05|null|null|0|
|02 / 05|0004|SAPPORO|DC--東順興|D|8.28|null|null|0|
|03 / 05|0501|Swire Coca-Cola(S&D)Limited Taiwan Branc|英屬維京群島商太古食品股份有限公司台灣分|D|3.25|null|null|0|
|04 / 05|0505|Kolin Food Corporation|客錸食品股份有限公司|D|3.75|null|null|0|
|05 / 05|0509|I MEI|DC--瑞盟行銷|D|6.4|null|null|0|



|SEQ|SUPSUPCD|SUPEDESC|SUPLDESC|SUDNATURE|SUDRBPCT|SUACLCD|SUACD|S1|
| -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|C606|Uni-President Organics Corp.|統一生機開發股份有限公司|N|0|CONS|C00|1|
|02 / 05|E046|Seeds Enterprise Co.Ltd.|西祺企業股份有限公司|N|0.5|CONS|C00|1|
|03 / 05|F263|Seeds Enterprise Co.Ltd.|西祺企業股份有限公司|N|1|CONS|C00|1|
|04 / 05|G557|Sommet International INC.|嵩亮國際企業股份有限公司|N|0|CONS|C00|1|
|05 / 05|H105|Creation Wine & Sprit Inc.|威廉彼特國際股份有限公司|N|0|CONS|C00|1|
