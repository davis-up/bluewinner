# Table

- 參數表 [TBLDTL ParameterDetailModel](./P4P/P4P_TBLDTL_01.md)
- Business Format [TBLDTL 626](./P4P/P4P_TBLDTL_02_626.md)
  - 篩選條件 TBDNUM1 = 1

|TBDENTCD|TBDEDESC|TBDNUM1|TBDNU2|
|:--:|:--:|:--:|:--:|
|代碼|名稱|篩選條件|代號|
|HYP|HYP|1|1|
|JSN|Jasons (現在改成 Mia C'bon),代碼將會改成 MIA|1|3|
|SUP|Supermarket|1|2|

- 稅别資料取得 [TAXGLD 和 TBLDTL 30 Tax Type 稅率型態](./P4P/P4P_TAXGLD_00.md)
- 寄賣列表 [ATTVAL](./P4P/P4P_ATTVAL_00.md)
- 有效部門 [MSTDEP 和 BLDTL 711 AWF申請單建立與資料修改控制依部門](./P4P/P4P_MSTDEP_00.md)
- 商品組織 [MSTMS](./P4P/P4P_MSTMS_00.md)
- Typology Typo 列表 [TYPMSTGT 依據 BusinessFormat[Hyper,Super,Mia]、部門、商品組織](./P4P/P4P_TYPMSTGT_00.md)
- Story 列表 [WSTORYTYPO 依據 BusinessFormat[Hyper,Super,Mia]、部門](./TWF/TWF_WSTORYTYPO_00.md)
  - WSTORYTYPO 是舊系統，請改用新系統
- Typology Typo 店家列表[依據 Typo 、 BusinessFormat[Hyper,Super,Mia]、部門、商品組織、TBLDTL 727 單品修改申請預設店別](./P4P/P4P_TYPOSTORE_00.md)
- Story 店家列表[依據 Story 、 BusinessFormat[Hyper,Super,Mia]、部門、TBLDTL 727 單品修改申請預設店別](./TWF/TWF_STORYOSTORE_00.md)
- 部門 有效供應商列表[供應商SUPGLD、部門SUPDEP、SUPATT](./P4P/P4P_DEPSUPPLIER_00.md)
- 部門 預設供應商列表[供應商SUPGLD、部門SUPDEP、TBLDTL 713 後勤單品預設倉別](./P4P/P4P_DEPSUPPLIER_01.md)
- 部門 條碼列表[TBLDTL 33 、 TBLDTL 711](./P4P/P4P_TBLDTL_03_37.md)
- 驗證 條碼 在『MD 服務』是否有重複[ITMBAR](./P4P/P4P_DEPITEMBARCODE_00.md)
- Supplier 供應商
  - [供應商品牌與Sub-品牌 UPBRAND](./P4P/P4P_SUPGLD_03.md#supbrand-supplier---brand)
  - [品牌名 BRNDDTL](./P4P/P4P_SUPGLD_03.md#brnddtl-brand-detail)

## TWF

- 申請單 CL240700002
  - [WREQGLD](./TWF/P4_ST_CL240700002_WFCITM001_TABLE_WREQGLD.md)
  - [WITMGLD](./TWF/P4_ST_CL240700002_WFCITM001_TABLE_WITMGLD.md)
  - [WITMBAR](./TWF/P4_ST_CL240700002_WFCITM001_TABLE_WITMBAR.md)
    - [WITMSUBSUP](./TWF/P4_ST_CL240700002_WFCITM001_TABLE_WITMSUP.md)
    - [WITMSUBSTOSUP](./TWF/P4_ST_CL240700002_WFCITM001_TABLE_WITMSUBSTOSUP.md)
  - [WITMSUP](./TWF/P4_ST_CL240700002_WFCITM001_TABLE_WITMSUP.md)
  - [WITMSTO](./TWF/P4_ST_CL240700002_WFCITM001_TABLE_WITMSTO.md)
