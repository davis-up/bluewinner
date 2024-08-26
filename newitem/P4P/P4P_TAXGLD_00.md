
# TAXGLD


```sql
   
    SELECT * FROM TAXGLD
     FETCH FIRST 40 ROWS ONLY

```

|SEQ|TAXTAXCD|TAXTAXTYP|TAXSDATE|TAXDESC|TAXRATE|TAXREFUND|TAXEDATE|TAXLOC|TAXCRE|TAXUPD|TAXUSR|TAXCREUSR|TAXSUPINV|TAXNATURECD|TAXCDAMT|TAXNUM1|TAXNUM2|TAXALPH1|TAXALPH2|TAXCDCUS|TAXPOS|TAXVATSP|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 05|1|1|2008-10-22 00:00:00.0|VAT 5%|5|1|2010-08-02 00:00:00.0|null|2008-10-21 13:47:55.0|2010-08-02 18:57:26.0|victorshih|golf|N|null|null|null|null|null|null|null|null|0|
|02 / 05|0|1|2008-10-06 00:00:00.0|VAT 0%|0|1|2010-08-02 00:00:00.0|null|2008-10-05 15:26:26.0|2010-08-02 18:57:26.0|victorshih|SSAdmin|N|null|null|null|null|null|null|null|null|0|
|03 / 05|0|1|2010-08-03 00:00:00.0|VAT 0%|0|1|2049-12-31 00:00:00.0|null|2010-08-02 18:57:26.0|2010-08-02 19:03:39.0|sharonlee|victorshih|Y|null|SGSC1|null|null|null|null|SGSC3|12|0|
|04 / 05|1|1|2010-08-03 00:00:00.0|VAT 5%|5|1|2049-12-31 00:00:00.0|null|2010-08-02 18:57:26.0|2010-08-02 19:03:39.0|sharonlee|victorshih|Y|null|SGSC0|null|null|null|null|SGSC2|11|1|
|05 / 05|P|C|2018-03-27 00:00:00.0|VAT 5% For Add On Tax|5|1|2049-12-31 00:00:00.0|null|2018-03-26 18:43:17.0|2018-03-26 18:43:17.0|victorshih|victorshih|Y|null|null|null|null|null|null|null|null|0|


- TAXGLD [com.ss.c4.p4p.referential.model.TaxModel]
  - TAXTAXCD
    - Value : 1
    - PK
    - 說明 : taxCode
    - comment : Tax Code
  - TAXTAXTYP
    - Value : 1
    - 說明 : taxType
    - [TBLDTL = 30 : Tax Type 稅率型態](P4P_TBLDTL_02_30.md)
    - comment : Tax Type *Table 30
  - TAXSDATE
    - Value : 2008-10-22 00:00:00.0
    - PK
    - 說明 : startDate
    - comment : Tax Start Date
  - TAXDESC
    - Value : VAT 5%
    - 說明 : taxDescription
    - comment : Tax Code Description
  - TAXRATE
    - Value : 5
    - 說明 : taxRate
    - comment : Tax Rate
  - TAXREFUND
    - Value : 1
    - 說明 : taxRefund
    - comment : Refundable (1=Yes/0=No)
  - TAXEDATE
    - Value : 2010-08-02 00:00:00.0
    - 說明 : endDate
    - comment : Tax End Date
  - TAXLOC
    - Value : null
    - 說明 : taxlocation
    - [TBLDTL = 30 : Tax Type 稅率型態](P4P_TBLDTL_02_30.md)
    - comment : Tax Location depends on Tax Location Level in Table 30
  - TAXCRE
    - Value : 2008-10-21 13:47:55.0
    - 說明 : cred
    - comment : Creation Date
  - TAXUPD
    - Value : 2010-08-02 18:57:26.0
    - 說明 : lastUpd
    - comment : Date of last update
  - TAXUSR
    - Value : victorshih
    - 說明 : lastUser
    - comment : Last User
  - TAXCREUSR
    - Value : golf
    - 說明 : creUser
    - comment : Creation User
  - TAXSUPINV
    - Value : N
    - 說明 : chargedOnSupplierInvoice
    - comment : Charged on supplier invoice (Y/N)
  - TAXNATURECD
    - Value : null
    - 說明 : natureCode
    - comment : Nature code for IMA
  - TAXCDAMT
    - Value : null
    - 說明 : codeAmount
    - comment : Code Amount for Thales
  - TAXNUM1
    - Value : null
    - 說明 : numeric1
    - comment : Numeric 1 (Reserve for future purpose)
  - TAXNUM2
    - Value : null
    - 說明 : numeric2
    - comment : Numeric 2 (Reserve for future purpose)
  - TAXALPH1
    - Value : null
    - 說明 : alphaNumeric1
    - comment : Alphanumeric 1 (Reserve for future purpose)
  - TAXALPH2
    - Value : null
    - 說明 : alphaNumeric2
    - comment : Alphanumeric 2 (Reserve for future purpose)
  - TAXCDCUS
    - Value : null
    - 說明 : codeAmountOfCustomer
    - comment : Code Amount of Customer Return
  - TAXPOS
    - Value : null
    - 說明 : posAccumulator
    - comment : POS Accumulator
  - TAXVATSP
    - Value : 0
    - 說明 : vatIncluded
    - comment : VAT Included in Selling Price (1-Yes/0-No)
