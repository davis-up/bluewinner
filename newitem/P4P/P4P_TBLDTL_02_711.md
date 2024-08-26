# TBLDTL 711 AWF申請單建立與資料修改控制依部門 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '711'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|711|Department not allowed to create data|AWF申請單建立與資料修改控制依部門|TBDENTCD : DepartmentTBDNUM1 : 1 = not allow to create / maintain data through workflowTBDNUM2 : 1 = not allow to generate internal barcodeTBDNUM3 : 1 = allow to change item from green to red item|33|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '711'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 33|711|10|Beverages|Beverages|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2022-03-08 15:03:52.0|F000036143|
|02 / 33|711|11|Cleaning|Cleaning|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2022-03-08 15:04:01.0|F000036143|
|03 / 33|711|12|Cosmetics|Cosmetics|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-09-24 19:11:29.0|F000036143|
|04 / 33|711|14|Dry Grocery|Dry Grocery|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2022-08-25 10:54:29.0|F000036143|
|05 / 33|711|15|Self-Service Perishables|Self-Service Perishables|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2022-03-08 15:04:17.0|F000036143|
|06 / 33|711|20|Ready To Eat|Ready To Eat|2|0|null|1|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|07 / 33|711|21|Fish|Fish|2|0|null|1|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|08 / 33|711|22|Fruit & Vegetables|Fruit & Vegetables|2|0|null|1|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|09 / 33|711|23|Bakery|Bakery|2|0|null|1|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|10 / 33|711|24|Butchery|Butchery|2|0|null|1|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|11 / 33|711|25|Dry Product|Dry Product|2|0|null|1|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|12 / 33|711|26|Restaurant|Restaurant|2|0|null|1|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2013-08-22 20:48:35.0|WF-TEST|
|13 / 33|711|30|Do-It-Yourself|Do-It-Yourself|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:10:53.0|F000036143|
|14 / 33|711|31|Housekeeping|Housekeeping|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2022-01-18 18:17:20.0|F000036143|
|15 / 33|711|32|Culture Stationery|Culture Stationery|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:11:21.0|F000036143|
|16 / 33|711|33|Leisure|Leisure|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:11:35.0|F000036143|
|17 / 33|711|34|Gardening|Gardening|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:11:48.0|F000036143|
|18 / 33|711|35|Cars|Cars|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:12:01.0|F000036143|
|19 / 33|711|36|Car Service|Car Service|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:12:15.0|F000036143|
|20 / 33|711|40|Big Appliance|Big Appliance|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:12:27.0|F000036143|
|21 / 33|711|41|Small Household Appliance|Small Household Appliance|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:12:42.0|F000036143|
|22 / 33|711|42|Photo Cine Optical|Photo Cine Optical|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:13:13.0|F000036143|
|23 / 33|711|43|HIFI Sound|HIFI Sound|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:13:29.0|F000036143|
|24 / 33|711|44|TV Video|TV Video|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:13:55.0|F000036143|
|25 / 33|711|45|Computers|Computers|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:14:12.0|F000036143|
|26 / 33|711|46|Telephone Services & Appliance|Telephone Services & Appliance|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:14:26.0|F000036143|
|27 / 33|711|48|Appliance Extention Warranty|Appliance Extention Warranty|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:14:42.0|F000036143|
|28 / 33|711|49|Appliance Service|Appliance Service|2|0|1|null|null|null|null|null|null|null|null|2012-05-02 00:00:00.0|2021-01-12 14:15:05.0|F000036143|
|29 / 33|711|60|Shoes|Shoes|2|0|1|null|null|null|null|null|null|null|null|2012-07-27 00:00:00.0|2021-01-12 14:15:25.0|F000036143|
|30 / 33|711|61|Permanent|Permanent|2|0|1|null|null|null|null|null|null|null|null|2012-07-27 00:00:00.0|2021-01-12 14:15:41.0|F000036143|
|31 / 33|711|62|Seasonal|Seasonal|2|0|1|null|null|null|null|null|null|null|null|2012-07-27 00:00:00.0|2021-01-12 14:15:57.0|F000036143|
|32 / 33|711|65|Household Linen|Household Linen|2|0|1|null|null|null|null|null|null|null|null|2012-07-27 00:00:00.0|2021-01-12 14:16:15.0|F000036143|
|33 / 33|711|66|Personal Accessories|Personal Accessories|2|0|0|null|null|null|null|null|null|null|null|2012-07-27 00:00:00.0|2022-01-18 16:17:32.0|F000036143|

