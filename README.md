# DeviceManageSystem-FuSheng-
實際協助-復盛設備管理系統(Device-Manage-System)

## 實作目的
在復盛股份有限公司，進行大學企業實習，<br>
與主管討論開發專案，決定要製作一個實際的設備管理系統，<br>
幫復盛IT資訊部門做管理設備之電子化，<br>
同時降低人員的管理成本。

## 設計理念與技術
主要使用C# ASP.NET MVC的網頁程式來製作專案，<br>
讓網路設備組管理人員透過Fusheng帳號進行SSO登入，<br>
公司使用設備人員僅須利用員工證刷卡，<br>
即可進行身分確認並完成電子設備出借之動作。
- C# ASP.NET MVC
- HTML+CSS
- Boostarp CSS UI Framework
- JavaScript+jQuery
- AJAX
- JSON
- Card Reader

## 主要實作功能
實作功能包含完整的管理設備出借之流程，<br>
管理人員能夠透過公司帳號直接使用網頁管理者身分登入，<br>
接著僅需新增設備，使用人員就可以直接透過員工證使用設備。<br>
- 設備出借流程 (使用員工證或手動輸入身分->勾選要使用之設備->點選出借即可)
- 設備歸還流程 (確認歸還之設備->勾選歸還之設備->點選歸還即可)
- 設備後台管理 (可新增設備、修改設備當前狀態)
- 出借後台管理 (可查看出借之紀錄)
- 多國語系 (支援繁體中文、簡體中文、英文)
- 資料特定欄位排序 (可點選欄位名稱進行資料排序)
- 資料即時搜尋 (不須經由網頁刷新即可搜尋出特定設備)
- 動作提示訊息 (網頁介面前端右下角狀態)
- SSO單一登入 (統一使用復盛人員資訊進行登入)
- Excel報表匯出 (含設備資訊與出借紀錄)

## 相關程式畫面
### 模擬登入(實際轉為復盛公司SSO登入)<br>
<img src="https://github.com/lfre84216/DeviceManageSystem-FuSheng-/blob/main/1.png">
<br>

### 設備出借<br>
<img src="https://github.com/lfre84216/DeviceManageSystem-FuSheng-/blob/main/2.png">
<br>

### 設備歸還<br>
<img src="https://github.com/lfre84216/DeviceManageSystem-FuSheng-/blob/main/3.png">
<br>

### 設備管理<br>
<img src="https://github.com/lfre84216/DeviceManageSystem-FuSheng-/blob/main/4.png">
<br>

### 設備管理修改<br>
<img src="https://github.com/lfre84216/DeviceManageSystem-FuSheng-/blob/main/5.png">
<br>

### 出借記錄<br>
<img src="https://github.com/lfre84216/DeviceManageSystem-FuSheng-/blob/main/6.png">
<br>

## 製作過程與困難點
當時在串接SSO的時候，不太了解實作原理，<br>
主要是先判斷未獲得Session值時，<br>
先連入公司的Login View URL(該URL後方會加入身分驗證成功後導向的特定網址參數，對應該專案特定的Action)，<br>
所以登入公司帳號後，即可導向回原設備管理系統的Action，<br>
同時帶入回傳的JSON資料，取得Session值。<br><br>
另外，在復盛公司進行實作專案，<br>
是我第一次加入公司進行實習，<br>
在這邊特別感謝復盛IT的Richie詳細的教我程式撰寫方面的問題，<br>
以及復盛IT的Rexx帶領我熟悉公司環境。<br>
