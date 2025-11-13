# C# 自學計畫 24 週確認表

使用方式
- 每週勾選核對清單，填寫日期與備註。
- 建議將本表加入你的 repo 並每週提交更新（可搭配 GitHub Projects/Issues 追蹤）。

狀態欄位說明
- [X] 學：本週主題學習完成（含筆記）
- [ ] 作：本週實作/練習完成
- [ ] 測：本週驗收測試或自我檢核通過

| 週次 | 主題 | 產出/練習 | 驗收標準 | 狀態 | 預定日期 | 完成日期 | 備註 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 環境建置、.NET CLI、專案/解決方案、Top-level statements、Console I/O、基本除錯 | 建立 .NET 8 Console 專案，印出 Hello 與讀取姓名；以斷點除錯執行 | 可使用 `dotnet new/build/run`；能下斷點、檢視變數；專案結構清楚 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 2 | 型別與運算子、控制流程；.editorconfig + dotnet format | 四則運算 CLI（含除以零處理）；加入 .editorconfig 並格式化 | 正確處理輸入與例外；`dotnet format` 無變更 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 3 | Nullable Reference Types（NRT）、null 安全技巧 | 啟用 NRT；為輸入與資料模型加上 null 檢查 | 專案無 NRT 警告（或有意識地抑制並說明理由） | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 4 | 迴圈、小型 CLI 專案、xUnit 初探 | 九九乘法表、1~100 總和；為其中 1 個函式寫 xUnit 測試 | 測試可執行通過；涵蓋邏輯邊界 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 5 | 方法、重載、參數設計；GCD、Try* 與 tuple 回傳 | 實作 GCD；示範 `TryDivide`（回傳 bool + out）與 tuple 回傳對照 | 單元測試涵蓋正常/邊界/錯誤情境 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 6 | ref/out/in；string 與 StringBuilder、格式化與效能 | 比較大量字串串接 vs StringBuilder；撰寫格式化輸出 | 量測差異（簡單 Benchmark/碼表）；能選用正確工具 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 7 | 類別、屬性、建構子、存取修飾詞 | Person、Product 類別（自動屬性、不同建構子） | 封裝正確、不可變欄位合理；基本測試通過 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 8 | 繼承與多型 | Animal/Dog/Cat 覆寫 Speak()；在集合中多型呼叫 | 以介面/基底型別在集合中運作正確 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 9 | 介面與抽象；struct vs class；records（選修） | 實作 ILogger（Console/File）；Point struct；試用 record | 能以介面替換實作；理解值/參考語意差異 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 10 | 集合基礎、泛型入門 | 陣列、List、Dictionary 操作；實作簡易 `Stack<T>` | 泛型 `Stack<T>` 透過測試驗證 push/pop/peek | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 11 | LINQ 基礎、延遲/即時執行 | 使用 Where/Select/OrderBy/GroupBy；控制 ToList 的時機 | 能解釋延遲執行；查詢結果正確且效能合理 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 12 | 例外處理策略、enum 應用 | 模擬常見錯誤（除零、檔案不存在）；自訂例外；星期 enum | 正確使用 try/catch/finally、重新擲回；enum 映射正確 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 13 | 檔案 IO、檔案/目錄、編碼 | File/Directory/Path 操作；FileLogger（寫入日誌） | 可靠寫檔與讀檔；檔案路徑與編碼處理正確 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 14 | JSON 序列化/反序列化（System.Text.Json） | 商品 DTO 匯入/匯出；命名策略與日期格式設定 | 讀寫 JSON 正確；能處理錯誤/缺欄位 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 15 | WinForms 基礎或 Console UI 優化 | 登入介面（帳號/密碼/登入按鈕/訊息）；本機驗證 | 基本事件處理正常；輸入驗證與錯誤提示完善 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 16 | 委派與事件 | 倒數計時器；事件訂閱/退訂與觸發流程 | 事件在結束時正確觸發；解除訂閱避免記憶體泄漏 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 17 | Lambda 與 LINQ 進階 | 複合查詢（投影、分組、join）；小型查詢工具 | 能以 Lambda 流暢撰寫 LINQ；結果與測試一致 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 18 | async/await、Task、取消、IProgress（async streams 選修） | 模擬下載（延遲）、取消、進度回報 | UI/Console 不被阻塞；取消與進度回報正確 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 19 | HttpClient、超時/取消/重試（Polly 選修） | 呼叫公開 API（如 JSONPlaceholder），解析並顯示/存檔 | 正確設定超時；可取消；錯誤可觀測與處理 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 20 | SQLite + EF Core（或 Dapper）CRUD | 建立資料表並完成 CRUD；讀取用 NoTracking（必要時） | Migration/連線設定正確；CRUD 測試通過 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 21 | DI 與設定、Logging 抽換 | 建立 DI 容器；以介面注入 Logger；加入 Serilog | 以 DI 切換實作不改呼叫端；Log 輸出可設定 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 22 | 單元測試策略、可測性重構 | 強化 xUnit 測試；抽換依賴以便測試（介面/注入） | 關鍵模組具良好覆蓋；測試穩定可重複 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 23 | GitHub Actions CI、覆蓋率與分析 | 建立 CI 工作流程（還原/建置/測試）；產出覆蓋率報告 | PR 自動跑測試；失敗能快速定位問題 | [ ] 學 [ ] 作 [ ] 測 |  |  |  |
| 24 | 期末整合專案與驗收 | 商品管理系統：CRUD + JSON 匯入匯出 + 非同步 + DB + 日誌 + 測試 + CI | Demo 可運作；README 清楚；能解釋設計決策（DI/非同步/錯誤處理/資料層） | [ ] 學 [ ] 作 [ ] 測 |  |  |  |

附註
- UI 路線可選 WinForms / WPF / .NET MAUI；若目標後端，可改第 15 週為 ASP.NET Core Web API 入門並調整後續整合。
- 若處理帳密資料：教學示例請勿存明碼，至少以雜湊（SHA-256+salt）記錄，並標註教學用途。
