
# ITMSUB


```sql
   
    SELECT * FROM ITMSUB
     FETCH FIRST 10 ROWS ONLY

```

|SEQ|ITSSUBID|ITSSUBCD|ITSITMID|ITSEDESC|ITSLDESC|ITSSTOP|ITSSTITMR|ITSCRE|ITSUPD|ITSUSR|ITSCREUSR|ITSDELFLAG|ITSROTCLS|ITSPRDCHR|ITSESTOP|ITSALLSTOP|ITSTYPO|ITSPKDATE|ITSSPMSG1|ITSSPMSG2|ITSSUPLDESC|ITSSUPEDESC|ITSRETURN|ITSRTNTMP|ITSRTNPMT|ITSWHCHK|ITSMIXPACK|ITSITMLV|ITSUSEDATE|ITSUSEDATEUOM|ITSCNCD|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 10|13587|001|9602|Towfu Cake|滷肉豆乾|null|null|2009-05-08 19:00:00.0|2024-03-07 20:10:17.0|SPOTACTION|MIGRATION|N|null|null|null|null|1|null|null|null|null|null|1|1|1|null|null|null|null|null|null|
|02 / 10|13588|001|10731|Towfu Cake|五香方乾|null|null|2009-05-08 19:00:00.0|2024-03-07 20:10:09.0|SPOTACTION|MIGRATION|N|3|null|null|null|1|null|null|null|null|null|1|1|1|null|null|null|null|null|null|
|03 / 10|874604|001|590432|S-2L|黑色 S-2L|null|null|2023-04-25 16:17:49.0|2023-04-25 16:17:50.0|PKNSAIPURWF|PKNSAIBARWF|N|null|null|null|null|0|null|null|null|null|null|null|null|null|null|null|null|null|null|null|
|04 / 10|832244|001|564340|107223|原味(純)雞肉鬆|null|null|2022-06-20 13:18:31.0|2024-04-26 15:23:37.0|PKNSAIBARWF|PKNSAIBARWF|N|null|null|null|null|0|null|null|null|null|null|null|null|null|null|null|null|null|null|null|
|05 / 10|927814|001|622126|Coupon|喬亞+烘焙折20|null|null|2024-04-23 17:51:51.0|2024-04-23 17:51:51.0|F000041553|F000041553|N|null|null|null|null|0|null|null|null|null|null|0|0|0|null|null|null|null|null|null|
|06 / 10|617423|001|422363|年節用400g/包|炭燒飛魚子_專櫃|null|null|2018-01-16 20:13:27.0|2022-09-29 16:02:35.0|P4PAUT43Y|PKNSAIBARWF|N|null|null|null|null|0|null|null|null|null|null|null|null|null|null|null|null|null|null|null|
|07 / 10|808970|001|549112|Mayura Wagyu |巧克力和牛紐約|null|null|2021-12-16 10:52:42.0|2023-10-11 17:38:43.0|PKP4TPWF|PKNSAIBARWF|N|3|null|null|2023-10-05 00:00:00.0|1|N|null|null|null|null|0|0|0|N|N|null|null|null|null|
|08 / 10|874605|001|590433|M-2L|混色 M-2L|null|null|2023-04-25 16:17:49.0|2023-04-25 16:17:51.0|PKNSAIPURWF|PKNSAIBARWF|N|null|null|null|null|0|null|null|null|null|null|null|null|null|null|null|null|null|null|null|
|09 / 10|9934|001|1819|Sparkling White|家福凱芙氣泡甜|null|null|2009-05-08 19:00:00.0|2024-03-21 20:34:00.0|SPOTACTION|MIGRATION|N|null|null|null|null|0|null|null|null|null|null|1|1|1|null|null|null|null|null|null|
|10 / 10|809239|001|549251|Membership Day|四月會員日|2022-04-15 00:00:00.0|0|2021-12-21 10:19:19.0|2022-04-14 14:21:13.0|F000041553|F000009360|N|null|null|2049-12-31 00:00:00.0|2022-04-15 00:00:00.0|0|null|null|null|null|null|0|0|0|null|null|null|null|null|null|


- ITMSUB
  - ITSSUBID
    - Value : 13587
    - PK
    - comment : Item Sub code ID
  - ITSSUBCD
    - Value : 001
    - comment : Item Sub code
  - ITSITMID
    - Value : 9602
    - FK (ITMGLD.ITMITMID), [ITMGLD](P4P_ITMGLD_00.md)
    - comment : Item ID
  - ITSEDESC
    - Value : Towfu Cake
    - comment : Sub Code English Description
  - ITSLDESC
    - Value : 滷肉豆乾
    - comment : Sub Code Local Description
  - ITSSTOP
    - Value : null
    - comment : Start Stop Date
  - ITSSTITMR
    - Value : null
    - comment : Stop Item Reason Code *Table 10
  - ITSCRE
    - Value : 2009-05-08 19:00:00.0
    - comment : Creation date
  - ITSUPD
    - Value : 2024-03-07 20:10:17.0
    - comment : Date of last update
  - ITSUSR
    - Value : SPOTACTION
    - comment : Last user
  - ITSCREUSR
    - Value : MIGRATION
    - comment : Creation User
  - ITSDELFLAG
    - Value : N
    - comment : Request for deletion flag (Y/N)
  - ITSROTCLS
    - Value : null
    - comment : Rotation Class *Table 353
  - ITSPRDCHR
    - Value : null
    - comment : Product Characteristic
  - ITSESTOP
    - Value : null
    - comment : End Stop Date
  - ITSALLSTOP
    - Value : null
    - comment : The latest date that all stores of sub codes stopped
  - ITSTYPO
    - Value : 1
    - comment : Typo flag
  - ITSPKDATE
    - Value : null
    - comment : Flag for Packed by Date(Y/N)
  - ITSSPMSG1
    - Value : null
    - comment : Special message1 (check mandatory field in TBDNUM1 of PT50)
  - ITSSPMSG2
    - Value : null
    - comment : Special message2
  - ITSSUPLDESC
    - Value : null
    - comment : Supplier sub code local name
  - ITSSUPEDESC
    - Value : null
    - comment : Supplier sub code English name
  - ITSRETURN
    - Value : 1
    - comment : Returnable for nonstop item ( 0=No, 1=Yes )
  - ITSRTNTMP
    - Value : 1
    - comment : Returnable for Temporary stop ( 0=No, 1=Yes )
  - ITSRTNPMT
    - Value : 1
    - comment : Returnable for Permanent stop ( 0=No, 1=Yes )
  - ITSWHCHK
    - Value : null
    - comment : warehouse checking mark ( Y/N )
  - ITSMIXPACK
    - Value : null
    - comment : Return mix packing ( Y/N )
  - ITSITMLV
    - Value : null
    - comment : Item Level *Table 752
  - ITSUSEDATE
    - Value : null
    - comment : Use by date
  - ITSUSEDATEUOM
    - Value : null
    - comment : Use by date unit
  - ITSCNCD
    - Value : null
    - comment : CN Code
