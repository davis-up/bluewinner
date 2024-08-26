# TBLDTL 804 退貨條件 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '804'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|804|Return Condition|退貨條件|N1 : allow user to free key-in comment ( 0: No, 1: Yes ),C1 : exclude for over stock calculation (Y/N)|12|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '804'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 12|804|1|No Return|不可退|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:27:17.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 12|804|10|Complete Original  Accessary, Document A|完整原廠配件外箱|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:30:58.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 12|804|11|Original Cover Box|原外箱|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:31:15.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 12|804|12|Original Product Package|須附商品原包裝|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:31:37.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 12|804|2|Accept Breakage and Good Product|良壞可退|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:27:41.0|2015-05-29 19:00:49.0|SSFIX_25550|
|06 / 12|804|3|Only Good Product|只收良品|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:27:57.0|2015-05-29 19:00:49.0|SSFIX_25550|
|07 / 12|804|4|Only Breakage(incl. Near/Over Expire Dat|只收壞品含即期過期|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:28:38.0|2016-03-01 15:35:32.0|F000000959|
|08 / 12|804|5|Only Breakage(incl. Product Defective |只收壞品含故障瑕疵|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:29:09.0|2016-03-01 15:36:29.0|F000000959|
|09 / 12|804|6|Only Intact Stock Product|只退未拆封庫存機|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:29:31.0|2015-05-29 19:00:49.0|SSFIX_25550|
|10 / 12|804|7|MD Special Reutrn|MD特退通知|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:29:43.0|2015-05-29 19:00:49.0|SSFIX_25550|
|11 / 12|804|8|Supplier Special Demands (Refer to Logis|廠商特殊要求查後勤卡車|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:30:05.0|2016-03-01 15:39:27.0|F000000959|
|12 / 12|804|9|Vender Need Check Product|廠商到店對點封箱|2|null|null|null|null|null|null|null|null|null|null|2015-05-14 17:30:25.0|2015-05-29 19:00:49.0|SSFIX_25550|

