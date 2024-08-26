# TBLDTL 27 單品型態 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '27'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|27|Item Type|單品型態|N1 = Can Buy-1/ Cannot Buy-0, N2 = Can Sell-1/ Cannot Sell -0, N3 = Parameter  number for tab control, C1 = Raw Material - Y/ Commercial - N|5|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '27'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|27|0|Raw Material|原物料|2|1|0|17|null|Y|209xx,219xx,229xx,239xx,249xx,259xx|null|null|null|null|2008-04-29 00:00:00.0|2014-12-09 13:48:45.0|F000000959|
|02 / 05|27|1|Fresh Product|自製品|2|0|1|18|null|N|20xxx,23xxx,24xxx,25xxx|209xx,239xx,249xx,259xx|null|null|null|2008-04-29 00:00:00.0|2014-12-09 13:52:19.0|F000000959|
|03 / 05|27|2|Fish & Vegetable|生鮮|2|1|1|16|null|N|21xxx,22xxx|219xx,229xx|null|null|null|2008-04-29 00:00:00.0|2014-12-09 14:00:16.0|F000000959|
|04 / 05|27|3|Commercial|一般|2|1|1|16|null|N|ALL|20xxx,21xxx,22xxx,23xxx,24xxx,25xxx|null|null|null|2008-04-29 00:00:00.0|2014-12-09 13:59:56.0|F000000959|
|05 / 05|27|4|Generic|Generic|2|0|0|19|null|N|null|null|null|null|null|2008-04-29 00:00:00.0|2008-08-08 00:00:00.0|ITEM|


---


部門 : 熟食課 [23] , 商品組織分類 : 調味品 [905] , ***單品型態: Raw Material 原物料 [0]***

檢查碼: 239xx

- 規則:
  1. TBDCHA2 含有檢查碼 且 TBDCHA3無含有檢查碼  , 此 規則優先。
  2. TBDCHA2 是 『ALL』。


```sql
        
    SELECT
        TBDENTCD, TBDEDESC, TBDLDESC
       ,TBDCHA2 , INSTR(NVL(TBDCHA2,'X'), '239xx') TBDNUM2
       ,TBDCHA3 , INSTR(NVL(TBDCHA3,'X'), '239xx') TBDNUM3
    FROM TBLDTL
    WHERE TBDTBNO = '27'

```

|SEQ|TBDENTCD|TBDEDESC|TBDLDESC|TBDNUM2|TBDNUM3|TBDCHA2|TBDCHA3|
| -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|0|Raw Material|原物料|19|0|209xx,219xx,229xx,239xx,249xx,259xx|null|
|02 / 05|1|Fresh Product|自製品|0|7|20xxx,23xxx,24xxx,25xxx|209xx,239xx,249xx,259xx|
|03 / 05|2|Fish & Vegetable|生鮮|0|0|21xxx,22xxx|219xx,229xx|
|04 / 05|3|Commercial|一般|0|0|ALL|20xxx,21xxx,22xxx,23xxx,24xxx,25xxx|
|05 / 05|4|Generic|Generic|0|0|null|null|



---


部門 : 精肉課 [24] , 商品組織分類 : 家福牛肉 [060] , ***單品型態: Fresh Product 自製品 [1]***

檢查碼: 24xxx

- 規則:
  1. TBDCHA2 含有檢查碼 且 TBDCHA3無含有檢查碼  , 此 規則優先。
  2. TBDCHA2 是 『ALL』。


```sql
        
    SELECT
        TBDENTCD, TBDEDESC, TBDLDESC
       ,TBDCHA2 , INSTR(NVL(TBDCHA2,'X'), '24xxx') TBDNUM2
       ,TBDCHA3 , INSTR(NVL(TBDCHA3,'X'), '24xxx') TBDNUM3
    FROM TBLDTL
    WHERE TBDTBNO = '27'

```

|SEQ|TBDENTCD|TBDEDESC|TBDLDESC|TBDNUM2|TBDNUM3|TBDCHA2|TBDCHA3|
| -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|0|Raw Material|原物料|0|0|209xx,219xx,229xx,239xx,249xx,259xx|null|
|02 / 05|1|Fresh Product|自製品|13|0|20xxx,23xxx,24xxx,25xxx|209xx,239xx,249xx,259xx|
|03 / 05|2|Fish & Vegetable|生鮮|0|0|21xxx,22xxx|219xx,229xx|
|04 / 05|3|Commercial|一般|0|25|ALL|20xxx,21xxx,22xxx,23xxx,24xxx,25xxx|
|05 / 05|4|Generic|Generic|0|0|null|null|



---


部門 : 鮮魚課 [21] , 商品組織分類 : 鮭魚 [034] , ***單品型態: Fish & Vegetable 生鮮 [2]***

檢查碼: 21xxx

- 規則:
  1. TBDCHA2 含有檢查碼 且 TBDCHA3無含有檢查碼  , 此 規則優先。
  2. TBDCHA2 是 『ALL』。


```sql
        
    SELECT
        TBDENTCD, TBDEDESC, TBDLDESC
       ,TBDCHA2 , INSTR(NVL(TBDCHA2,'X'), '21xxx') TBDNUM2
       ,TBDCHA3 , INSTR(NVL(TBDCHA3,'X'), '21xxx') TBDNUM3
    FROM TBLDTL
    WHERE TBDTBNO = '27'

```

|SEQ|TBDENTCD|TBDEDESC|TBDLDESC|TBDNUM2|TBDNUM3|TBDCHA2|TBDCHA3|
| -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|0|Raw Material|原物料|0|0|209xx,219xx,229xx,239xx,249xx,259xx|null|
|02 / 05|1|Fresh Product|自製品|0|0|20xxx,23xxx,24xxx,25xxx|209xx,239xx,249xx,259xx|
|03 / 05|2|Fish & Vegetable|生鮮|1|0|21xxx,22xxx|219xx,229xx|
|04 / 05|3|Commercial|一般|0|7|ALL|20xxx,21xxx,22xxx,23xxx,24xxx,25xxx|
|05 / 05|4|Generic|Generic|0|0|null|null|



---


部門 : 菸酒飲料 [10] , 商品組織分類 : 可樂 [000] , ***單品型態: Commercial 一般 [3]***

檢查碼: 10xxx

- 規則:
  1. TBDCHA2 含有檢查碼 且 TBDCHA3無含有檢查碼  , 此 規則優先。
  2. TBDCHA2 是 『ALL』。


```sql
        
    SELECT
        TBDENTCD, TBDEDESC, TBDLDESC
       ,TBDCHA2 , INSTR(NVL(TBDCHA2,'X'), '10xxx') TBDNUM2
       ,TBDCHA3 , INSTR(NVL(TBDCHA3,'X'), '10xxx') TBDNUM3
    FROM TBLDTL
    WHERE TBDTBNO = '27'

```

|SEQ|TBDENTCD|TBDEDESC|TBDLDESC|TBDNUM2|TBDNUM3|TBDCHA2|TBDCHA3|
| -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|0|Raw Material|原物料|0|0|209xx,219xx,229xx,239xx,249xx,259xx|null|
|02 / 05|1|Fresh Product|自製品|0|0|20xxx,23xxx,24xxx,25xxx|209xx,239xx,249xx,259xx|
|03 / 05|2|Fish & Vegetable|生鮮|0|0|21xxx,22xxx|219xx,229xx|
|04 / 05|3|Commercial|一般|0|0|ALL|20xxx,21xxx,22xxx,23xxx,24xxx,25xxx|
|05 / 05|4|Generic|Generic|0|0|null|null|


