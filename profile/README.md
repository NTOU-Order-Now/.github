# Order Now 
convenient, easy-to-use, and user-friendly food ordering platform


[View product](https://github.com/orgs/NTOU-Order-Now/projects/3)

## Documents
[SRD](https://docs.google.com/document/d/1cDQtjMbSaG90kuzeX0CxduzchRwdxvLS8CkxThgKghY/edit?tab=t.0)
[SDD](https://docs.google.com/document/d/1K23yAGst5DzZO4r-wZECXxlBDo70b6HL1Xv5dIrOVxA/edit?tab=t.0)
[STD](https://docs.google.com/document/d/1N5iF8bUXvtXqkwYkaIcBPecmmWRXf2qavU8zvCiGaRI/edit?tab=t.0)

### 基本需求
- [x] 系統使用者分為老闆和顧客兩種
- [x] 顧客可註冊帳號，註冊資訊包含基本資料(姓名、密碼、年齡、性別等)
- [x] 老闆可上架菜單，包含餐點名稱、單價、照片和說明。
- [x] 老闆可設定套餐，包含套餐名稱、價格、包含之餐點、照片和說明
- [x] 顧客可瀏覽早餐店的所有菜單
- [x] 顧客在可接受點餐時間內可點選多項餐點(包含套餐)，加入點菜單
- [x] 顧客可在點菜單上設定預定取餐時間，並送出點菜單
- [x] 老闆可即時收到顧客之點菜單，並設定接受或拒絕
- [x] 接受之點菜單將自動產生取餐序號，並加入至餐點製作清單
- [x] 老闆可以設定某一個點菜單已製作完成，並在畫面上明顯的顯示此狀態

### 進階需求
- [ ] 整合簡易客戶評價系統，顧客可對餐點進行評分
- [ ] 顧客可設定常用餐點清單，快速下單
- [x] 老闆可設定每週可接受點餐時間
- [x] 系統提供基本資料分析功能，呈現各餐點銷售情況
- [ ] 餐點狀態即時通知功能
- [x] 支援RWD (響應式網頁設計)
- [ ] 支援第三方登入(如Google、Facebook)
- [ ] 支援多語言介面(中文、英文)

### 額外需求
- [x] 系統並非只有單一商店，而是有多間商店可以點餐、註冊


## 預計功能實現

- 用websocket+ message queue 實現即時通知
- 使用redis當作快取來優化socket server 和 MQ之間的 lantency 和 throughput
- 用firebase 支援第三方登入
- 實作忘記密碼、email驗證功能
- 評價系統(已完成後端)
- 使用message queue優化 Imgur uploading process
- 提高後端 throughput 和 降低 前後端 lantency
- 使用playwright實作E2E testing 並加入CI/CD pipeline
- 完成剩餘的整合測試
- 開放內用點餐及內用接單功能
- 語言切換


## Future plan

- 改為微服務架構
- 使用K6 + Grafana + Prometheus 建立可觀測性

