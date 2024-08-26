# TBLDTL 805 退貨方式 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '805'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|805|Return Media|退貨方式|Note:Entry code usage in PT805 should be 1 digit only.a.The list of Return Media value's has to be maintained in PT805,b.The Return Model for the corresponding Return Media shall be maintained in TBDCHA1,c.The value’s shall be separated by ','d. The initial character of interface file’s name is maintained in TBDCHA2.|15|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '805'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 15|805|1|Vendor taking|廠商到店自取|2|null|null|null|null|N|null|null|null|null|null|2013-08-01 18:51:01.0|2017-08-17 19:05:02.0|F000000959|
|02 / 15|805|2|Freight|寄貨運|2|null|null|null|null|N|null|null|null|null|null|2013-08-01 18:51:01.0|2017-08-17 19:04:25.0|F000000959|
|03 / 15|805|3|WMS|退家福統倉|2|null|null|null|null|Y|null|null|null|null|null|2013-08-01 18:51:01.0|2017-08-17 19:04:07.0|F000000959|
|04 / 15|805|4|Agency Return|統倉代收代退|2|null|null|null|null|N|null|null|null|null|null|2017-08-17 19:03:41.0|2017-08-17 19:03:41.0|F000000959|
|05 / 15|805|5|No Return|特殊品不可退|2|null|null|null|null|N|null|null|null|null|null|2017-08-17 19:06:25.0|2017-08-17 19:20:59.0|F000000959|
|06 / 15|805|6|LI DC|退LI聯一倉|2|null|null|null|null|N|LI|null|null|null|null|2019-01-29 18:50:10.0|2020-03-11 00:56:16.0|CRID0465|
|07 / 15|805|7|LZ DC|退LZ蘆竹倉|2|null|null|null|null|N|LZ|null|null|null|null|2019-01-29 18:50:42.0|2020-03-11 00:56:16.0|CRID0465|
|08 / 15|805|8|KS DC|退KS岡山乾倉|2|null|null|null|null|N|KS|null|null|null|null|2019-01-29 18:51:35.0|2020-03-11 00:56:16.0|CRID0465|
|09 / 15|805|9|YM Frozen DC|退YM北凍倉|2|null|null|null|null|N|YMF|null|null|null|null|2019-01-29 18:52:03.0|2021-06-22 14:30:39.0|victorshih|
|10 / 15|805|A|KH DC|退KH南凍倉|2|null|null|null|null|N|KH|null|null|null|null|2019-06-04 14:00:59.0|2020-03-11 00:56:16.0|CRID0465|
|11 / 15|805|B|Shiraz TY DC|退TY大園倉|2|null|null|null|null|N|TY|null|null|null|null|2021-03-09 15:15:27.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|12 / 15|805|C|YM DC|退YM楊梅倉|2|null|null|null|null|N|YM|null|null|null|null|2021-06-22 14:31:32.0|2021-06-22 14:31:32.0|victorshih|
|13 / 15|805|D|EG DC|退EG長榮倉|2|null|null|null|null|N|EG|null|null|null|null|2022-05-06 15:37:39.0|2022-05-06 15:40:00.0|victorshih|
|14 / 15|805|E|ZF DC|退ZF忠富倉|2|null|null|null|null|N|ZF|null|null|null|null|2022-07-11 15:46:21.0|2022-07-11 15:46:21.0|F000000959|
|15 / 15|805|F|HD DC|退HD環東倉|2|null|null|null|null|N|HD|null|null|null|null|2024-05-07 11:19:41.0|2024-05-07 11:19:41.0|PMD-9491|

