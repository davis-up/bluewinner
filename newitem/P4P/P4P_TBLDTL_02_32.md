# TBLDTL 32 價格牌格式 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '32'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|32|Shelf Tag Size|價格牌格式|The Numeric Value 1 used for define the default shelf tag size on the shelf tag size modification screen. 1= Small,2 = Large|4|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '32'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 04|32|L|Large|Large|2|2|1|null|null|null|null|null|null|null|null|2008-04-29 00:00:00.0|2023-03-07 09:32:18.0|F000172052|
|02 / 04|32|S|Small|Small|2|1|2|null|null|null|null|null|null|null|null|2008-04-29 00:00:00.0|2023-03-07 09:32:27.0|F000172052|
|03 / 04|32|X|XL|XL|2|3|3|null|null|null|null|null|null|null|null|2017-05-25 16:59:17.0|2023-03-07 09:32:42.0|F000172052|
|04 / 04|32|Y|XXL|XXL|2|null|4|null|null|null|null|null|null|null|null|2017-10-18 01:21:52.0|2023-03-07 09:32:49.0|F000172052|

