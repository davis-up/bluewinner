# TBLDTL 151 倉庫物流型態與對應衛星倉設定 

---

```sql
            SELECT
       A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, COUNT(1) S1, A.TBHCMNT
    FROM TBLHDR A
        INNER JOIN TBLDTL B ON A.TBHTBNO = B.TBDTBNO
    WHERE A.TBHTBNO = '151'
    GROUP BY A.TBHTBNO , A.TBHEDESC, A.TBHLDESC, A.TBHCMNT
    ORDER BY A.TBHTBNO

```

|SEQ|TBHTBNO|TBHEDESC|TBHLDESC|TBHCMNT|S1|
| -- | -- | -- | -- | -- | -- |
|01 / 01|151|Supplier(Warehouse) Feature Setup|倉庫物流型態與對應衛星倉設定|N1: Warehouse feature (Parameter 150) , N2: SSD Default value for warehouse supplier , C1: Logistics Supplying Flow for interface to Mandala. P=Picking (STD On Stock),X=Cross dock (XD),F=Flow-trough (FT),V=Virtual Flow-trough,D=Direct) , C2: List of Satellite Warehouse code separated by ','|161|


---


```sql
            SELECT * FROM TBLDTL WHERE TBDTBNO = '151'
    FETCH FIRST 40 ROWS ONLY

```

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 40|151|7653|7653|7653|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2023-09-13 18:58:17.0|F000172066|
|02 / 40|151|7655|7655|7655|2|2|null|null|null|X|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-04 19:13:41.0|md9069|
|03 / 40|151|7656|7656|7656|2|2|null|null|null|X|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-04 19:13:41.0|md9069|
|04 / 40|151|9623|9623|9623|2|1|null|null|null|P|9,8,7,6,5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|05 / 40|151|9625|9625|9625|2|2|null|null|null|X|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-04 19:13:41.0|md9069|
|06 / 40|151|A689|A689|A689|2|1|null|null|null|P|5,6,7,8,9,A,B,C,D,E,G|null|null|null|null|2009-03-27 00:00:00.0|2023-09-13 18:48:37.0|F000172066|
|07 / 40|151|A690|A690|A690|2|2|null|null|null|X|5,A,B|null|null|null|null|2009-03-27 00:00:00.0|2023-07-17 17:47:06.0|F000172058|
|08 / 40|151|B075|B075|B075|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|09 / 40|151|B157|B157|B157|2|1|null|null|null|P|9,8,7,6,5,A,B|null|null|null|null|2009-03-27 00:00:00.0|2020-06-17 18:55:53.0|victorshih|
|10 / 40|151|B307|B307|B307|2|2|null|null|null|X|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-05 17:14:44.0|F000172058|
|11 / 40|151|B326|B326|B326|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|12 / 40|151|C190|C190|C190|2|2|null|null|null|X|5,B,G|null|null|null|null|2009-03-27 00:00:00.0|2023-10-11 12:09:19.0|md9249|
|13 / 40|151|C349|C349|C349|2|2|null|null|null|X|5,B,G|null|null|null|null|2009-03-27 00:00:00.0|2023-09-13 18:49:40.0|F000172066|
|14 / 40|151|C350|C350|C350|2|2|null|null|null|X|5,B,G|null|null|null|null|2009-03-27 00:00:00.0|2023-10-11 12:09:19.0|md9249|
|15 / 40|151|C379|C379|C379|2|2|null|null|null|X|5,B,G|null|null|null|null|2009-03-27 00:00:00.0|2023-10-12 14:09:51.0|md9251|
|16 / 40|151|C433|C433|C433|2|1|null|null|null|P|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-04 19:13:41.0|md9069|
|17 / 40|151|C502|C502|C502|2|1|null|null|null|P|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|18 / 40|151|C534|C534|C534|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|19 / 40|151|C537|C537|C537|2|1|null|null|null|P|9,8,7,6,5,A,B|null|null|null|null|2009-03-27 00:00:00.0|2020-06-17 18:56:32.0|victorshih|
|20 / 40|151|C548|C548|C548|2|1|null|null|null|P|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|21 / 40|151|C557|C557|C557|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|22 / 40|151|C560|C560|C560|2|1|null|null|null|P|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|23 / 40|151|C563|C563|C563|2|2|null|null|null|X|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-04 19:13:41.0|md9069|
|24 / 40|151|C786|C786|C786|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|25 / 40|151|C837|C837|C837|2|1|null|null|null|P|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|26 / 40|151|C838|C838|C838|2|2|null|null|null|X|5,B,G|null|null|null|null|2009-03-27 00:00:00.0|2023-10-11 12:09:19.0|md9249|
|27 / 40|151|D002|D002|D002|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|28 / 40|151|D172|D172|D172|2|1|null|null|null|P|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|29 / 40|151|D173|D173|D173|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|30 / 40|151|D174|D174|D174|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|31 / 40|151|D313|D313|D313|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|32 / 40|151|D409|D409|D409|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2017-05-09 15:25:11.0|F000000959|
|33 / 40|151|D410|D410|D410|2|2|null|null|null|X|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-04 19:13:41.0|md9069|
|34 / 40|151|D576|D576|D576|2|2|null|null|null|X|5,B|null|null|null|null|2009-03-27 00:00:00.0|2023-05-04 19:13:41.0|md9069|
|35 / 40|151|D589|D589|D589|2|1|null|null|null|P|5,6,7,8,9,A,B,C,D,E,G|null|null|null|null|2009-03-27 00:00:00.0|2023-09-13 18:49:05.0|F000172066|
|36 / 40|151|D592|D592|D592|2|2|null|null|null|X|5,A|null|null|null|null|2009-03-27 00:00:00.0|2016-09-06 11:23:28.0|L2_PMD1601|
|37 / 40|151|E050|E050|E050|2|1|null|null|null|P|9,8,7,6,5,A,B|null|null|null|null|2009-03-27 00:00:00.0|2020-06-17 18:57:09.0|victorshih|
|38 / 40|151|E051|E051|E051|2|1|null|null|null|P|9,8,7,6,5,A,B,C,D,E,G|null|null|null|null|2009-03-27 00:00:00.0|2023-09-13 18:49:22.0|F000172066|
|39 / 40|151|E228|E228|E228|2|2|null|null|null|X|5,B,G|null|null|null|null|2009-03-27 00:00:00.0|2023-10-11 12:09:19.0|md9249|
|40 / 40|151|E379|E379|E379|2|2|null|null|null|X|5,B,G|null|null|null|null|2009-03-27 00:00:00.0|2023-09-13 18:49:53.0|F000172066|

