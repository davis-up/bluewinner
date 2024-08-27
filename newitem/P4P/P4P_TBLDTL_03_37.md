
# 條碼列表

- 部門：10
- Business Format : <MS>

```sql
   
SELECT
    A.TBDENTCD ,  -- 條碼ID
    A.TBDEDESC ,  -- 條碼名
    A.TBDCHA1  ,  -- 條碼程式
    A.TBDNUM2    -- IsEditTypeIE( 1=不可修改)
FROM TBLDTL A WHERE A.TBDTBNO = 33
AND A.TBDENTCD NOT IN (SELECT '9'  FROM TBLDTL WHERE  TBDTBNO = 711 AND TBDENTCD = '10' AND tbdnum2 = 1)


```

|SEQ|TBDENTCD|TBDEDESC|TBDNUM2|TBDCHA1|
| -- | -- | -- | -- | -- |
|01 / 04|1|EAN-13|null|barcodeEan13Generator|
|02 / 04|2|EAN-8|null|barcodeEan8Generator|
|03 / 04|3|UPC-A|null|barcodeUpcAGenerator|
|04 / 04|4|UPC-E|null|barcodeUpcEGenerator|

