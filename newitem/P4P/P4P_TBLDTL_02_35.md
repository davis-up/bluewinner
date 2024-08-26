# TBLDTL 35 Market Potential 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '35'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|35|Market Potential|Market Potential|Define how sensitive the selling price is.|7|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '35'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 07|35|A|Carrefour Hyper|家樂福量販店|2|null|null|null|null|null|null|null|null|null|null|2021-03-02 15:01:25.0|2021-03-24 00:47:38.0|victorshih|
|02 / 07|35|B|Carrefour Super|家樂福便利購店|2|null|null|null|null|null|null|null|null|null|null|2021-03-02 15:01:46.0|2022-08-22 15:41:31.0|PMD-8443-pt1|
|03 / 07|35|C|Shiraz Super|Shiraz便利購店|2|null|null|null|null|null|null|null|null|null|null|2021-03-02 15:02:16.0|2021-03-24 00:48:19.0|victorshih|
|04 / 07|35|D|Jasons Market|Jasons超市|2|null|null|null|null|null|null|null|null|null|null|2021-03-02 15:02:46.0|2021-07-19 17:58:29.0|victorshih|
|05 / 07|35|E|Carrefour Others|EC電子商務 與 中央廚房|2|null|null|null|null|null|null|null|null|null|null|2021-03-11 18:45:37.0|2021-03-24 00:50:15.0|victorshih|
|06 / 07|35|F|Unmanned Store|無人商店|2|null|null|null|null|null|null|null|null|null|null|2021-07-19 17:57:16.0|2021-07-19 17:57:16.0|victorshih|
|07 / 07|35|Z|Office (Migrate From Old P4MD)|辦公室(舊P4MD移轉未使用)|2|null|null|null|null|null|null|null|null|null|null|2021-03-24 00:42:50.0|2021-03-24 00:52:05.0|victorshih|

