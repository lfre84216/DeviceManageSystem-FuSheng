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
- 設備出借流程 (使用員工證或手動輸入身分->勾選要使用之設備->點選借出即可)
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
### 登入註冊<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/7.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/8.png">
<br>

### 使用者介面<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/1.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/2.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/3.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/4.png">
<br>

### 管理者介面<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/5.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/6.png">
<br>

## 製作過程與困難點
在實作該專案的過程中，有嘗試想要實際讓資料庫可以被外部來連接，<br>
達成實際直接遠端資料庫的功能，<br>
所以在網路這方面有另外研究了關於虛擬伺服器的功能，<br>
讓實作出來的程式也能透過外部裝置來進行連線。
