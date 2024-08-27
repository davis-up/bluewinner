
# 部門預設供應商列表 

- 部門：10

```sql
   
     SELECT
         sup.SUPSUPCD ,
         sup.SUPEDESC ,
         sup.SUPLDESC ,
         supdept.SUDNATURE

     FROM SUPGLD sup
            INNER JOIN SUPDEP supdept ON sup.SUPSUPCD = supdept.SUDSUPCD
            INNER JOIN TBLDTL TB ON TB.TBDTBNO = 713 AND sup.SUPSUPCD = TB.TBDENTCD
        WHERE 0=0
        -- sup.SUPSUPCD in (select tbdentcd from TBLDTL where tbdtbno = '713') // 713 後勤單品預設倉別
        AND SUDSTPBUSDATE IS NULL
        AND supdept.SUDDPCD = 10
        GROUP BY sup.SUPSUPCD , sup.SUPEDESC , sup.SUPLDESC , supdept.SUDNATURE
        ORDER BY sup.SUPSUPCD

        FETCH FIRST 5 ROWS ONLY

```

|SEQ|SUPSUPCD|SUPEDESC|SUPLDESC|SUDNATURE|
| -- | -- | -- | -- | -- |
|01 / 02|B326|CF DD-All Divisions-A to B|CF DD-直送全品項ＡｔｏＢ|W|
|02 / 02|G727|HD Stock-Returning DC|HD Stock-退貨倉|W|

