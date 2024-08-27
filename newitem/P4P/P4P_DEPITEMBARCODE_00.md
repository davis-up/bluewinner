
# 『MD 服務』 是否有 重複條碼 

- 條碼：3245415192712

```sql
   
     SELECT
         mdsub.ITSSUBCD ,  -- subCode
         mdbar.ITBUNCD  ,  -- unitCode
         mditm.ITMDPCD  ,  -- deptCode
         mditm.ITMITMCD ,  -- itmCode
         mdbar.ITBBAR
        FROM ITMBAR mdbar
            INNER JOIN ITMSUB  mdsub ON mdbar.ITBSUBID = mdsub.ITSSUBID
            INNER JOIN ITMGLD   mditm ON mdbar.ITBITMID = mditm.ITMITMID
        WHERE mdbar.ITBORGBAR = 3245415192712
        FETCH FIRST 5 ROWS ONLY

```

|SEQ|ITBBAR|ITBUNCD|ITSSUBCD|ITMDPCD|ITMITMCD|
| -- | -- | -- | -- | -- | -- |
|01 / 01|3245415192712|01|001|10|201069|

