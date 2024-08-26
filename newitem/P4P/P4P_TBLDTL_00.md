# TBLDTL

```sql
      SELECT * FROM TBLDTL
  FETCH FIRST 1 ROWS ONLY

````

|SEQ|TBDTBNO|TBDENTCD|TBDEDESC|TBDLDESC|TBDACCES|TBDNUM1|TBDNUM2|TBDNUM3|TBDNUM4|TBDCHA1|TBDCHA2|TBDCHA3|TBDCHA4|TBDDAT1|TBDDAT2|TBDCRE|TBDUPD|TBDUSR|TBDCMNT|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|01 / 01|48|PER|Peru|秘魯|2|null|null|null|null|53|null|null|null|null|null|2009-03-27 00:00:00.0|2023-11-27 17:28:37.0|PMD9058|Define the origin country for item by using ISO key 3166|


- TBDTBNO
  - Value : 48
  - EngName : tableNumber
- TBDENTCD
  - Value : PER
  - EngName : entryCode
- TBDEDESC
  - Value : Peru
  - EngName : engDesc
- TBDLDESC
  - Value : 秘魯
  - EngName : localDesc
- TBDACCES
  - Value : 2
  - EngName : accessType
- TBDNUM1
  - Value : null
  - EngName : numVal1
- TBDNUM2
  - Value : null
  - EngName : numVal2
- TBDNUM3
  - Value : null
  - EngName : numVal3
- TBDNUM4
  - Value : null
  - EngName : numVal4
- TBDCHA1
  - Value : 53
  - EngName : charVal1
- TBDCHA2
  - Value : null
  - EngName : charVal2
- TBDCHA3
  - Value : null
  - EngName : charVal3
- TBDCHA4
  - Value : null
  - EngName : charVal4
- TBDDAT1
  - Value : null
  - EngName : dateVal1
- TBDDAT2
  - Value : null
  - EngName : dateVal2
- TBDCRE
  - Value : 2009-03-27 00:00:00.0
  - EngName : creDate
- TBDUPD
  - Value : 2023-11-27 17:28:37.0
  - EngName : updDate
- TBDUSR
  - Value : PMD9058
  - EngName : user
- TBDCMNT
  - Value : Define the origin country for item by using ISO key 3166


---


|SEQ|TBHTBNO|說明|資料量|SEQ|TBHTBNO|說明|資料量|
|:--:|:--:|:--|:--:|:--:|:--:|:--|:--:|
|1 / 393 |[***1***](./P4P_TBLDTL_02_1.md)  |Region Code 區域碼 |51  |2 / 393 |[***2***](./P4P_TBLDTL_02_2.md)  |Store Type 店型態 |4  |
|3 / 393 |[***4***](./P4P_TBLDTL_02_4.md)  |Selling Price Type 售價型態 |2  |4 / 393 |[***5***](./P4P_TBLDTL_02_5.md)  |Type of sales 銷售型態 |33  |
|5 / 393 |[***6***](./P4P_TBLDTL_02_6.md)  |Season Code 季節代碼 |18  |6 / 393 |[***7***](./P4P_TBLDTL_02_7.md)  |Sensitiveness Code 敏感性商品碼 |8  |
|7 / 393 |10  |Stop Item Reason 停止單品原因 |23  |8 / 393 |[***11***](./P4P_TBLDTL_02_11.md)  |Stop Payment Reason 止付原因 |15  |
|9 / 393 |15  |Mapping between program and role Mapping table for program and role |7  |10 / 393 |16  |Tab of Items that can buy and sell 標籤設定 - 可進貨可銷售單品 |26  |
|11 / 393 |17  |Tab of Items that can buy but not sell 標籤設定 - 可進貨不可銷售單品 |26  |12 / 393 |18  |Tab of Items that can sell but not buy 標籤設定 - 不可進貨可銷售單品 |26  |
|13 / 393 |19  |Tab of Items that can not buy and sell 標籤設定 - 不可進貨不可銷售單品 |26  |14 / 393 |[***21***](./P4P_TBLDTL_02_21.md)  |City 縣市 |27  |
|15 / 393 |22  |Postcode / District 郵遞區號 / 區域 |368  |16 / 393 |[***24***](./P4P_TBLDTL_02_24.md)  |Business Entity 公司型態 |1  |
|17 / 393 |[***25***](./P4P_TBLDTL_02_25.md)  |Stock Unit 庫存單位 |82  |18 / 393 |26  |SNI SNI - Siemens Nixdorf Information |21  |
|19 / 393 |[***27***](./P4P_TBLDTL_02_27.md)  |Item Type 單品型態 |5  |20 / 393 |[***28***](./P4P_TBLDTL_02_28.md)  |Sold by 販賣方式 |2  |
|21 / 393 |29  |Unit Code 銷售碼 |99  |22 / 393 |[***30***](./P4P_TBLDTL_02_30.md)  |Tax Type 稅率型態 |2  |
|23 / 393 |31  |Media of Sale Promotion 促銷原因 |12  |24 / 393 |[***32***](./P4P_TBLDTL_02_32.md)  |Shelf Tag Size 價格牌格式 |4  |
|25 / 393 |[***33***](./P4P_TBLDTL_02_33.md)  |Barcode Type 條碼型態 |5  |26 / 393 |[***34***](./P4P_TBLDTL_02_34.md)  |Store Format 店規模 |5  |
|27 / 393 |[***35***](./P4P_TBLDTL_02_35.md)  |Market Potential |7  |28 / 393 |[***36***](./P4P_TBLDTL_02_36.md)  |Store Category 店類別 |7  |
|29 / 393 |[***38***](./P4P_TBLDTL_02_38.md)  |Cashier System 收銀系統型態 |3  |30 / 393 |[***39***](./P4P_TBLDTL_02_39.md)  |Scale System 磅秤系統型態 |2  |
|31 / 393 |[***40***](./P4P_TBLDTL_02_40.md)  |Stock adjustment Reason 庫存調整原因 |27  |32 / 393 |41  |Capacity Ratio 容量比率 |89  |
|33 / 393 |[***42***](./P4P_TBLDTL_02_42.md)  |Capacity Unit 容量 |75  |34 / 393 |43  |Tab for Store Maintenance 標籤設定 - 店資料維護 |10  |
|35 / 393 |44  |Replenishment Type |5  |36 / 393 |46  |Item  parameter default 單品預設參數 |11  |
|37 / 393 |[***47***](./P4P_TBLDTL_02_47.md)  |Shelf Life UOM |5  |38 / 393 |[***48***](./P4P_TBLDTL_02_48.md)  |Country of Origin 原產國 |296  |
|39 / 393 |49  |Order By 訂貨層級 |4  |40 / 393 |50  |Type of Division 處別 |7  |
|41 / 393 |[***51***](./P4P_TBLDTL_02_51.md)  |Alert color before cut-off time cut-off time警示顏色 |3  |42 / 393 |[***52***](./P4P_TBLDTL_02_52.md)  |Location ID in store |5  |
|43 / 393 |53  |Unit of Measure |5  |44 / 393 |[***54***](./P4P_TBLDTL_02_54.md)  |Unit of Measure of Shelf Life Limit |2  |
|45 / 393 |55  |Sorting Rules |4  |46 / 393 |57  |Food Attribute |4  |
|47 / 393 |58  |Airproof Attribute |2  |48 / 393 |59  |Receiver email defined By Selling Price 緊急變價電子郵件通知收件人設定 |3  |
|49 / 393 |60  |DM Organizer DM促销组织者 |8  |50 / 393 |61  |control shelftag print qty for MLC items MLC單品價格牌列印張數邏輯控制 |1  |
|51 / 393 |62  |Alert Message for Breakage VS Returnable 庫存調整警告資訊 |2  |52 / 393 |63  |Negotiation type |2  |
|53 / 393 |101  |Order Proposal Management Setup 建議訂單管理參數 |5  |54 / 393 |102  |Time(Mins) to alert before cut-off time  cut-off time警示時間 |1  |
|55 / 393 |103  |Maximum order quantity by MS 最大訂貨數量依分類 |2659  |56 / 393 |104  |Order acknowledgement status 訂單回傳狀態 |5  |
|57 / 393 |106  |Country information 國家資料 |12  |58 / 393 |107  |User Region control (Maximum 4 region) COS/NSO+ 下單需新增員編於此並設定Store Format |35  |
|59 / 393 |108  |Store data group type 店群組類別 |6  |60 / 393 |110  |Email unix environment |5  |
|61 / 393 |111  |Checking Time before Cut-Off Time |1  |62 / 393 |113  |Time slot on IST request received time |7  |
|63 / 393 |[***150***](./P4P_TBLDTL_02_150.md)  |Supplier(Warehouse)Feature Referential 物流型態 |4  |64 / 393 |[***151***](./P4P_TBLDTL_02_151.md)  |Supplier(Warehouse) Feature Setup 倉庫物流型態與對應衛星倉設定 |161  |
|65 / 393 |152  |Consignment item validation |1  |66 / 393 |153  |Satellite Warehouse 衛星倉代碼與名稱 |11  |
|67 / 393 |200  |Commission Contract Status |8  |68 / 393 |201  |Pro-forma grouping for printing |1  |
|69 / 393 |204  |Tolerance for invoice matching amount |1  |70 / 393 |205  |Maximum %VAT for Invoice |2  |
|71 / 393 |207  |Sales upload mailing setup |2  |72 / 393 |209  |Generate grossmargin sequence filename |1  |
|73 / 393 |210  |Generate daily matched sequence filename |1  |74 / 393 |211  |Type of proforma |10  |
|75 / 393 |212  |Country information for ZCS ZCS國別資料 |35  |76 / 393 |214  |Control autogen proforma by department |42  |
|77 / 393 |216  |Invoice amount decimal and rounding 發票小數及進位參數 |3  |78 / 393 |217  |Invoice Type 發票型熊 |2  |
|79 / 393 |218  |Check in birt report for ZC(CON0006) |1  |80 / 393 |219  |Control Inc/Exc ZC+ ITM gen cyc list |2  |
|81 / 393 |220  |Specific day for payement cycle Specific day for payement cycle’ |1  |82 / 393 |300  |Parameter Setup for Fee and Rebate Fee and Rebate參數 |27  |
|83 / 393 |301  |National contract status |6  |84 / 393 |302  |Fee Type |202  |
|85 / 393 |303  |Role Profile Mapping |3  |86 / 393 |304  |Interface out to peoplesoft Code Sub Event |6  |
|87 / 393 |305  |Interface out to peoplesoft Code Amount |7  |88 / 393 |306  |Invoice template description |11  |
|89 / 393 |308  |EDI Invoice Field Description |9  |90 / 393 |309  |IMA dept. and P4 dept. mapping |42  |
|91 / 393 |310  |Tax and TXN_Type code by Income type |5  |92 / 393 |311  |Invoice date by Income type |4  |
|93 / 393 |312  |Multi Cut of Date in period |1  |94 / 393 |313  |FRS Permission Group |3  |
|95 / 393 |314  |National Contract form |3  |96 / 393 |315  |Fee and Rebate Type |202  |
|97 / 393 |316  |NC. Description |10  |98 / 393 |317  |Fee PA Description |2  |
|99 / 393 |318  |FRS upload parameter |6  |100 / 393 |319  |Invoice Distribution City |20  |
|101 / 393 |320  |Decimal rounding 小數進位 |3  |102 / 393 |321  |Action Parameter |19  |
|103 / 393 |[***322***](./P4P_TBLDTL_02_322.md)  |Mapping TaxId by Supplier by Department |15163  |104 / 393 |323  |Mapping Local language for Vat System  |4  |
|105 / 393 |324  |FRS Parameter for PS |13  |106 / 393 |325  |Element  of Control tool |8  |
|107 / 393 |326  |Rebate and PNL Type |156  |108 / 393 |[***327***](./P4P_TBLDTL_02_327.md)  |Department Group |11  |
|109 / 393 |351  |Store Group Type Group type of stores |8  |110 / 393 |352  |Store Group Group of stores |27  |
|111 / 393 |353  |Rotation Class Categories of sales quantity ranges |2  |112 / 393 |[***354***](./P4P_TBLDTL_02_354.md)  |Grade 等級 |1179  |
|113 / 393 |355  |Collection Code Relate to ITMCOLNO in ITMGLD |80  |114 / 393 |[***356***](./P4P_TBLDTL_02_356.md)  |Specific item Relate to ITMSPEC in ITMGLD |3  |
|115 / 393 |357  |Rej Bad Extract Rejection and Bad Extraction |4  |116 / 393 |358  |Item Order Parameter Interfacing Control 單品訂貨參數介面檔控制 |12  |
|117 / 393 |359  |Control the file generation |1  |118 / 393 |360  |Reason code Description SC2維護原因 |20  |
|119 / 393 |400  |Booking Status SBS預售狀態 |8  |120 / 393 |401  |Warehouse Code Setup SBS倉庫設定 |3  |
|121 / 393 |402  |System Lock Time for Interfacing SBS+系統鎖定與訂單檔產出時間 |8  |122 / 393 |403  |Default parameter for booking item |2  |
|123 / 393 |404  |Available Stock Interface Time |1  |124 / 393 |407  |SBS Parameter SBS參數 |12  |
|125 / 393 |408  |Generate SBS+ Report |3  |126 / 393 |409  |SBS Upload Parameter |2  |
|127 / 393 |410  |the lead time of delivery by store |155  |128 / 393 |411  |Picking Methods for the SBS Booking |4  |
|129 / 393 |412  |Discount Types for SBS Transaction |4  |130 / 393 |413  |Payment Types for SBS Transaction |4  |
|131 / 393 |414  |Hide columns in SBS0005 and report |12  |132 / 393 |470  |Interface for IST_InterfaceOutbound |3  |
|133 / 393 |498  |FTP Directory and Host Setup |1  |134 / 393 |499  |Exclude Store by Group for MT |4  |
|135 / 393 |500  |Batch process status 批次作業狀態 |4  |136 / 393 |501  |Local Language for P/O printing P/O列印中文 |30  |
|137 / 393 |502  |Rejection details extraction Rejection資料匯出 |207  |138 / 393 |503  |Global Parameter for PS PS介面檔參數 |13  |
|139 / 393 |504  |PS Parameter by income type |3  |140 / 393 |505  |PS Parameter by income type |4  |
|141 / 393 |506  |Report parameter type 報表參數型態 |10  |142 / 393 |507  |Report parameter default value 報表參數預設值 |2  |
|143 / 393 |508  |Report default type 報表預設型態 |2  |144 / 393 |509  |Group Code For Master Data Interface Master File介面檔群組與傳送參數 |14  |
|145 / 393 |510  |Set up Master Data Interface Criteria Master File介面檔產生條件參數 |6  |146 / 393 |511  |Tax Number Type For PeopleSoft PS統一編號型態 |10  |
|147 / 393 |512  |Global parameter for Interface to WI WI介面檔參數 |3  |148 / 393 |513  |Global parameter for rcv. from Demarca Demarca介面檔參數 |2  |
|149 / 393 |514  |The criteria for CPC data interface CPC介面檔參數 |3  |150 / 393 |515  |Define file param for Interface to CPC CPC介面檔參數 |1  |
|151 / 393 |[***516***](./P4P_TBLDTL_02_516.md)  |End of Day Parameter EOD參數 |1  |152 / 393 |517  |EOD Exception Profile |19  |
|153 / 393 |518  |Conversion Character Set 介面檔字元編碼轉換控制 |27  |154 / 393 |519  |Default Item Value 單品預設參數 |2  |
|155 / 393 |520  |User password parameter 帳號密碼參數 |1  |156 / 393 |521  |Country Parameter Setup 國別參數設定 |58  |
|157 / 393 |522  |Path of generate file translation |1  |158 / 393 |523  |Internal Barcode Parameter 內部條碼參數 |6  |
|159 / 393 |524  |Item Deletion Parameters 單品刪除參數 |5  |160 / 393 |[***525***](./P4P_TBLDTL_02_525.md)  |Global Tax Setup 系統稅別設定 |1  |
|161 / 393 |526  |Barcode with department 部門條碼設定 |17  |162 / 393 |527  |Default values for TEXAS TEXAS預設參數 |3  |
|163 / 393 |528  |Assortment request status |18  |164 / 393 |529  |The default values for interface purpose |2  |
|165 / 393 |530  |Model Store 模範原型店 |1  |166 / 393 |531  |Item Restructure control 單品組織異動控制 |2  |
|167 / 393 |532  |Check CM+ |7  |168 / 393 |533  |Total month checking non movement item |2  |
|169 / 393 |534  |Parameter for Report Extraction |12  |170 / 393 |535  |Transaction Type between P4CM+ and P4CM |9  |
|171 / 393 |536  |Grouping transaction type |5  |172 / 393 |[***538***](./P4P_TBLDTL_02_538.md)  |Special Character 特殊字元控制 |280  |
|173 / 393 |539  |Displayed in extraction reports |4  |174 / 393 |540  |Create Data for Now Store |2  |
|175 / 393 |541  |Round decimal function on AVGSALE |1  |176 / 393 |542  |for qualified manufacture date/exp date |2  |
|177 / 393 |543  |Master data file interface option |12  |178 / 393 |544  |Default Stop reason of Auto Release |1  |
|179 / 393 |545  |Transfer media for return report 退貨單傳送方式 |3  |180 / 393 |546  |Control the Batch launching Parameter |1  |
|181 / 393 |547  |Cal method to generate the Int file |1  |182 / 393 |548  |Control number fields Master Data Ext. |41  |
|183 / 393 |549  |No. of days in advance 提前下传天数 |1  |184 / 393 |550  |Item Level for Target SKU calculation |1  |
|185 / 393 |[***551***](./P4P_TBLDTL_02_551.md)  |Common controls for CWF |6  |186 / 393 |552  |trigger to launch data comparison |1  |
|187 / 393 |553  |discrepancy of auto updating to TP Linux |1  |188 / 393 |555  |DDL for Request Type of IST 移撥清單型態 |3  |
|189 / 393 |556  |Expiry-N days for clearance control |36  |190 / 393 |557  |Best Before Date Rule for Semi-Product 半成品最佳使用期限規則 |49  |
|191 / 393 |558  |Control EXD pop-up reminder in POS |1  |192 / 393 |560  |Special server for receive file via FTP |1  |
|193 / 393 |561  |shelf tag printing WebUI and logic apply |1  |194 / 393 |562  |shelf tag printing priority and color |5  |
|195 / 393 |563  |item characteristic type |10  |196 / 393 |564  |logo type to be printed on shelf tag |5  |
|197 / 393 |565  |EC Business Model Store |1  |198 / 393 |566  |No Expiry Products 無效期商品設定 |3797  |
|199 / 393 |567  |Products Expiry Risk Warning Days 單品效期風險警示天數 |16  |200 / 393 |568  |Consign Products Broadcast List Criteria 寄賣商品推播清單 |2  |
|201 / 393 |569  |Risk Management No Broadcast Criteria 風險管理不推播參數設定 |24  |202 / 393 |570  |Approach Flag 處理方式 |3  |
|203 / 393 |571  |Clearance Area Threshold 出清區閾值 |1  |204 / 393 |572  |Expiry Category 效期類別 |7  |
|205 / 393 |573  |Warehouse MLC 倉庫MLC |3  |206 / 393 |574  |不列入MLC維護指標計算設定 |4  |
|207 / 393 |575  |列印貨架號碼標籤 |4  |208 / 393 |576  |MLC單品維護異動來源 |3  |
|209 / 393 |577  |OOS Reason 缺貨原因 |10  |210 / 393 |578  |Scan OOS Criterion 刷缺標準 |116  |
|211 / 393 |579  |缺貨處理結果 |3  |212 / 393 |580  |單品狀態 |2  |
|213 / 393 |581  |出倉作業-表單狀態 |4  |214 / 393 |582  |是否可調整缺貨原因 |1  |
|215 / 393 |583  |備貨補貨表單類型 |7  |216 / 393 |584  |Task Assignment-Job Task 數位派工-工作項目 |10  |
|217 / 393 |585  |Task Assignment-Job Status 數位派工-任務狀態 |4  |218 / 393 |586  |Task Assignment-Logistic Status 數位派工-到貨來源 |3  |
|219 / 393 |587  |Task Assignment-Job Task 數位派工-設定TOP組別 |5  |220 / 393 |588  |Task Assignment-Job Task 數位派工-HRIS Hyper店部門代碼對應TOP組別與處別 |59  |
|221 / 393 |589  |Task Assignment-Job Task 數位派工-HRIS Super店部門代碼對應TOP組別與處別 |8  |222 / 393 |590  |Task Assignment Job code 數位派工- 設定HRIS職等代碼資料 |12  |
|223 / 393 |591  |Task Assignment-Job code 數位派工- 設定後場工作項目 |1  |224 / 393 |593  |Task Assignment-Job code 數位派工- 設定報表中文字 |4  |
|225 / 393 |594  |Centric authority Centric查詢權限設定 |55  |226 / 393 |595  |不可刪除權限群組 |4  |
|227 / 393 |596  |Centric Mobile 自動指派權限設定For Hyper |543  |228 / 393 |597  |Centric Mobile 自動指派權限設定For super |77  |
|229 / 393 |600  |Selling Promotion Parameter-Others(CONS) 促銷售價參數 - 其它(CONS) |3  |230 / 393 |[***601***](./P4P_TBLDTL_02_601.md)  |Pricing Decimal and Rounding Method 價格小數位數及進位基準 |5  |
|231 / 393 |602  |Selling Promotion Parameter 促銷售價參數 |8  |232 / 393 |603  |Pre-Referential Parameter Pre-Referential參數 |36  |
|233 / 393 |604  |Voucher Type |2  |234 / 393 |605  |Selling Promotion Parameter - Others 促銷售價參數 - 其它 |3  |
|235 / 393 |606  |Default value for NSA++ NSA++預設參數 |14  |236 / 393 |607  |Permission Group |8  |
|237 / 393 |608  |Menu function list |9  |238 / 393 |609  |TP Linux Selling Promotion TP Linux售價參數 |24  |
|239 / 393 |610  |TP Linux customer type TP Linux顧客型態 |32  |240 / 393 |611  |Packaging Maintenance |2  |
|241 / 393 |612  |TP Linux - Media Type Parameter TP Linux - Payment Media參數 |52  |242 / 393 |613  |Activity Log Table |2160  |
|243 / 393 |614  |Activity Log Last Updated Time |2  |244 / 393 |615  |TP Linux Group code |20  |
|245 / 393 |[***616***](./P4P_TBLDTL_02_616.md)  |Typology – Typology and Concept |29  |246 / 393 |[***617***](./P4P_TBLDTL_02_617.md)  |Typology – Role |1  |
|247 / 393 |618  |Typology – Cluster |32  |248 / 393 |619  |TP Linux - Parameter by Promotion Type |24  |
|249 / 393 |620  |Attribute class for item link |1  |250 / 393 |621  |Typology Maintenance Typology維護 |4  |
|251 / 393 |622  |Data extraction 資料擷取 |2  |252 / 393 |623  |Orderable Store |82  |
|253 / 393 |624  |Department Control for Average Sales 部門Average Sales控制 |42  |254 / 393 |[***626***](./P4P_TBLDTL_02_626.md)  |business format |7  |
|255 / 393 |[***627***](./P4P_TBLDTL_02_627.md)  |Supplier Type Setup 供應商型態 |3  |256 / 393 |[***628***](./P4P_TBLDTL_02_628.md)  |Specific Supplier |3  |
|257 / 393 |[***629***](./P4P_TBLDTL_02_629.md)  |Stop Business Reason 停止合作原因 |8  |258 / 393 |630  |Payment Mode 付款方式 |14  |
|259 / 393 |631  |Bank Code Set Up 銀行資料設定 |5215  |260 / 393 |[***632***](./P4P_TBLDTL_02_632.md)  |Supplier Default Value 供應商預設參數 |7  |
|261 / 393 |[***633***](./P4P_TBLDTL_02_633.md)  |Logistic Flag Setup 後勤標示設定 |3  |262 / 393 |[***634***](./P4P_TBLDTL_02_634.md)  |Purchase price based on 進價計算基準 |2  |
|263 / 393 |635  |Minimum Order Type 最小訂貨型態 |3  |264 / 393 |[***636***](./P4P_TBLDTL_02_636.md)  |Supplier Payment Term 供應商付款條件 |3  |
|265 / 393 |637  |Priority/Best Price by Tier |7  |266 / 393 |[***638***](./P4P_TBLDTL_02_638.md)  |Supplier Partnership |4  |
|267 / 393 |639  |Block for modification on returning list 退貨清單修改參數控制 |2  |268 / 393 |[***640***](./P4P_TBLDTL_02_640.md)  |Supplier pay group code desc |2  |
|269 / 393 |641  |Bank Inf Bank Acc Code Rel |4  |270 / 393 |642  |Negotiation type |4  |
|271 / 393 |643  |TPLinux-Card Bincode for Mobile Payment. TPLinux-Bincode Group for Mobile Payment |39  |272 / 393 |644  |apply to all store exclude Jasons store |2  |
|273 / 393 |651  |Store code for automatic typo assortment |1  |274 / 393 |661  |Communication Description |12  |
|275 / 393 |662  |Location Code and Location Description |5  |276 / 393 |663  |Communication Location Description |7  |
|277 / 393 |664  |Type Code and Type Description |9  |278 / 393 |[***700***](./P4P_TBLDTL_02_700.md)  |Global Parameter |15  |
|279 / 393 |701  |Application Form 申請表單名稱與代碼 |6  |280 / 393 |[***702***](./P4P_TBLDTL_02_702.md)  |NG reason  E-Codi 退回原因 |3  |
|281 / 393 |703  |GDS NG Reason GDS 退回原因 |7  |282 / 393 |704  |Control GDS data compared screen GDS 與 MD資料比對控制 |4  |
|283 / 393 |705  |User Role 使用者角色 |5  |284 / 393 |706  |Flow shortname  表單流程簡稱 |22  |
|285 / 393 |707  |Page Display 表單中文名稱顯示與使用者權限 |26  |286 / 393 |[***711***](./P4P_TBLDTL_02_711.md)  |Department not allowed to create data AWF申請單建立與資料修改控制依部門 |33  |
|287 / 393 |[***712***](./P4P_TBLDTL_02_712.md)  |Parameter Control 新單品欄位預設值設定 |21  |288 / 393 |[***713***](./P4P_TBLDTL_02_713.md)  |Defalut Supplier 後勤單品預設倉別 |2  |
|289 / 393 |[***714***](./P4P_TBLDTL_02_714.md)  |default Store AWF店分配與預設店別 |403  |290 / 393 |715  |Priority 表單優先權名稱與代碼 |3  |
|291 / 393 |[***716***](./P4P_TBLDTL_02_716.md)  |Weight Unit 重量單位 |3  |292 / 393 |[***717***](./P4P_TBLDTL_02_717.md)  |Specific Item in Role 單品建立依特定單品代碼與使用角色 |4  |
|293 / 393 |[***718***](./P4P_TBLDTL_02_718.md)  |VAT by Store 預設稅別依店別 |3  |294 / 393 |719  |E-Form Action Status GDS 表單狀態 |8  |
|295 / 393 |720  |request status 申請單狀態 |10  |296 / 393 |721  |Default values for columns in Item modif 單品修改申請欄位預設值 |3  |
|297 / 393 |722  |Default value Item Logistic modification 後勤單品修改申請欄位預設值 |2  |298 / 393 |723  |Default value NPP 進售價修改申請欄位預設值 |2  |
|299 / 393 |724  |Default value PPP 促銷進售價申請欄位預設值 |1  |300 / 393 |725  |Default value StopRelease 店分配修改申請欄位預設值 |1  |
|301 / 393 |726  |Default display unit 陳列單位預設值依分類 |441  |302 / 393 |[***727***](./P4P_TBLDTL_02_727.md)  |default Store release 單品修改申請預設店別 |2  |
|303 / 393 |728  |AWF exclusion store for PSP creation |1  |304 / 393 |[***730***](./P4P_TBLDTL_02_730.md)  |Show supplier on PPP grid 促銷進價供應商顯示設定 |2  |
|305 / 393 |731  |Default PP/SP 進售價申請相關設定 |5  |306 / 393 |732  |Division not pass to Pricing Team 不需全國價格策略審核依處別 |1  |
|307 / 393 |733  |Define Dept not allow pass Pricing Team 不需全國價格策略審核依部門 |44  |308 / 393 |734  |Number of day for re-cal PPP end date 促銷進價延後生效天數設定 |5  |
|309 / 393 |735  |GDS check Item modi comparison GDS 單品修改申請資料比對設定 |16  |310 / 393 |737  |Vat |1  |
|311 / 393 |738  |Work Flow Error for upload 匯入錯誤碼與描述設定 |8  |312 / 393 |739  |default Store release |1  |
|313 / 393 |740  |Label Label change new local language For AWF |26  |314 / 393 |741  |Modify add PURGEWORK in pakage PKWFPURGE |15  |
|315 / 393 |742  |Modify add PURGELOG in pakage PKWFPURGE |8  |316 / 393 |743  |On process over time for WMAPITM |1  |
|317 / 393 |744  |Item Category |3  |318 / 393 |745  |Temporary Type |3  |
|319 / 393 |746  |Link Type |8  |320 / 393 |747  |Control to SKU Calculation |1  |
|321 / 393 |748  |Classify food or non food |2  |322 / 393 |749  |Document Type |2  |
|323 / 393 |750  |Define Dept not allow pass Pricing Team |7  |324 / 393 |751  |License Type |17  |
|325 / 393 |752  |Item Level |6  |326 / 393 |754  |Parameter Setup for File Link Path |5  |
|327 / 393 |755  |Control RWF Functional |3  |328 / 393 |762  |Number of day to stop the promo pack |1  |
|329 / 393 |[***770***](./P4P_TBLDTL_02_770.md)  |Mandatory Field Contr by Department |2  |330 / 393 |802  |Logistic Return Reason 後勤退貨原因 |4  |
|331 / 393 |803  |Good exchange criteria 換貨條件 |2  |332 / 393 |[***804***](./P4P_TBLDTL_02_804.md)  |Return Condition 退貨條件 |12  |
|333 / 393 |[***805***](./P4P_TBLDTL_02_805.md)  |Return Media 退貨方式 |15  |334 / 393 |806  |Charge To |2  |
|335 / 393 |807  |WMS Code |1  |336 / 393 |808  |Warehouse rule and Chceking |5  |
|337 / 393 |809  |Freight Company 貨運公司代碼與名稱 |27  |338 / 393 |810  |Over Stock |2  |
|339 / 393 |811  |Stop Item |3  |340 / 393 |812  |Return half of amount from purchase |2  |
|341 / 393 |813  |Return Location |1  |342 / 393 |814  |AllowDsptchQtyAndRecvQtyMoreThanTheReqst |1  |
|343 / 393 |815  |Control for create Non Schedule Order |1  |344 / 393 |816  |Central Return General Parameter |1  |
|345 / 393 |817  |Pallet Packing Status 集板狀態 |2  |346 / 393 |828  |Purge For SBS+ POS Transaction SBS+ POS資料保留期間設定 |2  |
|347 / 393 |900  |P4CM+ Return Reason Code |23  |348 / 393 |901  |Alert type for an automatic order 自動訂單警示型態 |8  |
|349 / 393 |902  |Country Information for P4CM+ |68  |350 / 393 |904  |HHT menu can be performed during EOD HHT功能控制(EOD) |6  |
|351 / 393 |905  |Priority price up/down in shelf tag INF 價格牌排序及旗標參數 |3  |352 / 393 |906  |AccManageSysWebSer for TIM |1  |
|353 / 393 |907  |Extraction validation period |1  |354 / 393 |908  |Default no. of days on Item expiry risk 商品過期風險天數預設值 |7  |
|355 / 393 |909  |Parameter for Merchandise Location code MLC商品位置碼參數 |2  |356 / 393 |910  |MRP Reject Reason Code |2  |
|357 / 393 |911  |Blocking Stock Reason 庫存凍結原因 |3  |358 / 393 |912  |Block Stock Status 庫存凍結狀態 |2  |
|359 / 393 |913  |StockAdjustment_Consignment_Bydept 寄賣商品庫存調整依部門參數設定 |9  |360 / 393 |914  |Block modification pre-sales order Pre-Sales預售單修改控制 |1  |
|361 / 393 |915  |Update ONYR from DCOD integration |1  |362 / 393 |916  |Code Amount for Monthly Sales Interface |4  |
|363 / 393 |917  |Rejection data for automatic trigger Rejection Data自動重送參數設定 |30  |364 / 393 |918  |Automatic trigger rejection data to CM+ 自動重送CM+ Rejection Data |144  |
|365 / 393 |920  |Coefficient promotion depend on end days PSP變異系數依結束日更新參數 |2  |366 / 393 |921  |rep/screen lock while inventory process |14  |
|367 / 393 |923  |Allowable Clearance Discount HHT出清折數設定 |10  |368 / 393 |924  |Shelf tag format for shelf tag size 'A' |6  |
|369 / 393 |925  |Extend warranty item & Bad for new item |5  |370 / 393 |926  |To contain Bank information |5  |
|371 / 393 |927  |To define the POP shelf tag size POP大小對應參數 |6  |372 / 393 |928  |Dept Code Allowed for Order On Demand |8  |
|373 / 393 |931  |Weighing Scale System Parameter Setup |1  |374 / 393 |932  |Department of Product Center 生產中心部門 |5  |
|375 / 393 |933  |Production Center |1  |376 / 393 |934  |SCO Alert Code and Weight Control SCO 警語及重量控制 |42  |
|377 / 393 |1000  |Number of days setup for purging-CMS CMS資料保留期間設定 |15  |378 / 393 |[***1001***](./P4P_TBLDTL_02_1001.md)  |Control Supplier Frozen Process |1  |
|379 / 393 |1005  |Interface table purging 介面檔資料保留期間設定 |98  |380 / 393 |1006  |Purge the data by  modules 功能模組資料保留期間設定 |9  |
|381 / 393 |1010  |Data Retention Day for Pre-Referential Pre-Referential資料保留期間設定 |3  |382 / 393 |1011  |Data Purging for typology tables Typology資料保留期間設定 |2  |
|383 / 393 |1012  |Data Retention for FIFO table purging FIFO資料保留期間設定 |4  |384 / 393 |1013  |JCA Store Order Files Transfer Setup JCA 分店訂單檔案傳輸設定 |12  |
|385 / 393 |2000  |3in1UserRole 3in1UserRole權限設定 |8  |386 / 393 |9000  |List of specific parameter table number 特殊參數表列表 |44  |
|387 / 393 |9001  |List of stores belong to this MD 商品部 / 店介面檔設定 |417  |388 / 393 |9002  |List of interface file for Mandala Mandala介面檔列表 |24  |
|389 / 393 |9003  |List of stores allow to overlap type M  允許促銷型態重覆列表(依店) |407  |390 / 393 |9004  |Store and buffer minutes use in process CYC結束緩衝時間控制 |1  |
|391 / 393 |9005  |Daily supplier data changed report 每日供應商報表參數 |3  |392 / 393 |[***9006***](./P4P_TBLDTL_02_9006.md)  |Shelf Life Limit Formula 允收天數計算式 |2  |
|393 / 393 |9100  |CM+ACL Control CM+ 權限控管 |2  |--|--|--|--|

---

