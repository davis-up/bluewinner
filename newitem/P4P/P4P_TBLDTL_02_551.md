# TBLDTL 551 Common controls for CWF 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '551'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|551|Common controls for CWF|Common controls for CWF|to have all the common controls for CWF application|6|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '551'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 06|551|1|Common controls for CWF|Common controls for CWF|2|null|null|null|null|null|null|null|null|null|null|2016-10-13 00:13:45.0|2016-10-13 00:13:45.0|SYSTEM|
|02 / 06|551|BB|ItemRelease control basedon flowtyp Nego|ItemRelease control basedon flowtyp Nego|2|null|null|null|null|null|null|null|null|null|null|2017-11-29 01:02:19.0|2017-11-29 01:02:19.0|SYSTEM|
|03 / 06|551|IC|Common Weight Control|Common Weight Control|2|1|null|null|null|null|null|null|null|null|null|2022-12-20 21:48:08.0|2022-12-20 21:48:08.0|PMD-8712|
|04 / 06|551|IM|Common Weight Control|Common Weight Control|2|1|null|null|null|null|null|null|null|null|null|2022-12-20 21:48:08.0|2023-03-06 10:40:53.0|F000172050|
|05 / 06|551|XX|Log. Replen.team controlfor stop/release|Log. Replen.team controlfor stop/release|2|null|null|null|null|null|null|null|null|null|null|2017-11-29 01:02:19.0|2017-11-29 01:02:19.0|SYSTEM|
|06 / 06|551|YY|stop/Release 2 step to MD+ on flow type|stop/Release 2 step to MD+ on flow type|2|null|null|null|null|null|null|null|null|null|null|2017-11-29 01:02:19.0|2017-11-29 01:02:19.0|SYSTEM|

