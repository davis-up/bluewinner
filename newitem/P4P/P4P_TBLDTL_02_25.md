# TBLDTL 25 庫存單位 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '25'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|25|Stock Unit|庫存單位|The smallest unit measurement |82|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '25'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 40|25|BOTTLE瓶|BOTTLE瓶|BOTTLE瓶|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|02 / 40|25|BOX盒|BOX盒|BOX盒|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|03 / 40|25|BOX箱|BOX箱|BOX箱|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|04 / 40|25|Bag包|Bag包|Bag包|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|05 / 40|25|Bag袋|Bag袋|Bag袋|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|06 / 40|25|BoX盒|BoX盒|BoX盒|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|07 / 40|25|Bottle瓶|Bottle瓶|Bottle瓶|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|08 / 40|25|Bowl碗|Bowl碗|Bowl碗|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|09 / 40|25|Box盒|Box盒|Box盒|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|10 / 40|25|Box箱|Box箱|Box箱|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|11 / 40|25|Bucket桶|Bucket桶|Bucket桶|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|12 / 40|25|Bucket筒|Bucket筒|Bucket筒|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|13 / 40|25|Bunch把|Bunch把|Bunch把|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|14 / 40|25|CAN罐|CAN罐|CAN罐|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|15 / 40|25|CARD卡|CARD卡|CARD卡|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|16 / 40|25|Can桶|Can桶|Can桶|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|17 / 40|25|Can罐|Can罐|Can罐|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|18 / 40|25|Card卡|Card卡|Card卡|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|19 / 40|25|Ctn箱|Ctn箱|Ctn箱|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|20 / 40|25|Cup杯|Cup杯|Cup杯|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|21 / 40|25|KG公斤|KG公斤|KG公斤|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|22 / 40|25|Kg公斤|Kg公斤|Kg公斤|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|23 / 40|25|Loaf條|Loaf條|Loaf條|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|24 / 40|25|L公升|L公升|L公升|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|25 / 40|25|PACK包|PACK包|PACK包|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|26 / 40|25|PC串|PC串|PC串|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|27 / 40|25|PC付|PC付|PC付|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|28 / 40|25|PC件|PC件|PC件|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|29 / 40|25|PC份|PC份|PC份|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|30 / 40|25|PC個|PC個|PC個|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|31 / 40|25|PC副|PC副|PC副|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|32 / 40|25|PC包|PC包|PC包|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|33 / 40|25|PC卡|PC卡|PC卡|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|34 / 40|25|PC只|PC只|PC只|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|35 / 40|25|PC台|PC台|PC台|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|36 / 40|25|PC塊|PC塊|PC塊|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|37 / 40|25|PC尺|PC尺|PC尺|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|38 / 40|25|PC尾|PC尾|PC尾|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|39 / 40|25|PC幅|PC幅|PC幅|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|
|40 / 40|25|PC床|PC床|PC床|0|null|null|null|null|null|null|null|null|null|null|2009-05-08 23:43:30.0|2015-05-29 19:00:49.0|SSFIX_25550|

