# **資料庫**

## **PostgreSQL**

![](/assets/postgresql.png)

### 典範案例

* [經濟部中央地質調查所 — 地質騰雲網運用多套開源軟體](/use-case/di-zhi-teng-yun-wang-yun-yong-duo-tao-kai-yuan-ruan-ti.md)
* [經濟部水利署 — 水利雲受推崇開源軟體扮演幕後功臣](/shui-li-yun-shou-tui-chong-kai-yuan-ruan-ti-ban-yan-mu-hou-gong-chen.md)
* [經濟部中央地質調查所 — 地質騰雲網運用多套開源軟體](/use-case/di-zhi-teng-yun-wang-yun-yong-duo-tao-kai-yuan-ruan-ti.md)

### 組織介紹

PostgreSQL是由散佈在全球的數百名開發者（包含非營利組織團體，學術研究機構及國際企業體）志願貢獻與共同開發的專案成果，歷經22年來持續發展。長久以來被用於要求極端嚴謹的商業應用／科學研究環境及政府組織中。PostgreSQL為BSD版權協議發佈，允許在商業或非商業應用的兩種環境下，皆能享有自由取得且不受限制的使用權。PostgreSQL 具有高度擴展性，且完整遵從國際 ISO-SQL 規範的開發方向，是當前最先進的開放原始碼 \(OSS\) 的物件關聯型資料庫管理系統 \(ORDBMS\)。

### 軟體介紹

PostgreSQL是一套功能強大、開放原始碼物件關聯資料庫系統，在系統可靠性、資料完整性和正確性獲得極佳評價，並具備先進資料庫系統功能。

* 多版本並行控制：每個使用者都提供了一個資料庫的快照，其修改都是在自己本地端資料，其他使用者看不到除了自己以外的本地端資料，直到使用者把所有修改更新到資料庫中，這時其他使用者才能看到你的修改。
* 三種資料庫隔離方式：可序列化、可重複讀取和授權讀取。最主要的目的就是不讓每個使用者的修改影響到彼此，透過這機制不僅降低讀寫鎖定機制的依賴，也保證了資料庫高品質的符合 ACID 原則。
* 程序式程式設計：允許使用基本的SQL語句寫成函式執行，但由於缺乏流程控制等功能，所以引入其它程式語言編寫函式的功能，包刮 Plain SQL、PL/pgSQL、C/C++ 或 Java和 R統計語言。
* 使用者定義物件：使用者可為資料庫內幾乎所有的物件定義新的類型，包括索引、函式、資料域、資料類別和會話（編碼轉換）等。
* 繼承：資料表的結構和屬性可從一個「父」表中繼承，資料會在兩者間共享，所以任何繼承資料表如果有做插入或刪除的動作，則父表也會有所更動，同樣地，當父表有動作，其他繼承資料表也會有所更動。

### 應用

PostgreSQL資料庫為目前最廣泛使用的開放原始碼資料庫之一，從研發至今，歷經相當多年長時間的更新與改良，功能完整且具備許多商用級特性，可充分滿足企業級應用需求。PostgreSQL的開發社群人員遍及世界各地，提供充足的研發能量，持續加入許多新技術與功能，除了系統效能與運算能力提升外，在架構上也支援分散運算、異地備援與巨量資料處理等機制，並相容ISO/ANSI SQL等國際標準。

日本電信電話株式會社（簡稱NTT）為日本最大的電信服務公司，出資和美國 EnterpriseDB 公司合作，共同發展 PostgreSQL 適用於大規模系統的技術開發。以促進 NTT 與一般企業用戶的 PostgreSQL 導入使用率，應用標準且開源的 PostgreSQL 資料庫管理系統在 NTT 企業中，目前在NTT企業團隊中擁有數百個處理系統，引進 PostgreSQL 資料庫系統用於顧客付費相關的主系統。

### 資料來源：

* The world's most advanced open source database [https://www.postgresql.org/](https://www.postgresql.org/)
* PostgreSQL 中文-Mammoth [http://postgresql.wisdomfish.org/](http://postgresql.wisdomfish.org/)
* DSpace的PostgreSQL資料庫架構與操作 [http://blog.pulipuli.info/2008/01/dspacepostgresql.html](http://blog.pulipuli.info/2008/01/dspacepostgresql.html)
* 開放原始碼 PostgreSQL 資料庫系統簡介 [https://www.ipro.tw/ict-news/1302-postgresql-about.html](https://www.ipro.tw/ict-news/1302-postgresql-about.html)
* 不一樣的Node.js：用JavaScript打造高效能的前後台網頁程式 第二版 [https://books.google.com.tw/books?id=YyMqCwAAQBAJ&printsec=frontcover&hl=zh-TW\#v=onepage&q&f=false](https://books.google.com.tw/books?id=YyMqCwAAQBAJ&printsec=frontcover&hl=zh-TW#v=onepage&q&f=false)
* PostgreSQL 國際中文社群網誌
  [http://postgresql-chinese.blogspot.tw/2008/10/nttpostgresql30.html](http://postgresql-chinese.blogspot.tw/2008/10/nttpostgresql30.html)
* ostgreSQL的商業功能，摘要說明 [http://www.thinkpower.com.tw/CrystalDB.html](http://www.thinkpower.com.tw/CrystalDB.html)
* Node.js 資料庫應用 [https://lrs.itsa.org.tw/file.php/595/104%E6%95%99%E6%9D%90--%E7%B6%B2%E8%B7%AF%E5%8F%8A%E5%B9%B3%E5%8F%B0%E6%9C%8D%E5%8B%99\_%E9%AB%98%E9%9B%84%E5%A4%A7%E5%AD%B8%E5%BC%B5%E4%BF%9D%E6%A6%AE/Part\_A-\_%E5%B9%B3%E5%8F%B0%E6%9C%8D%E5%8B%99%E8%AA%B2%E7%A8%8B%E6%95%99%E6%9D%90/2.%E6%95%99%E6%9D%90%E6%8A%95%E5%BD%B1%E7%89%87/12\_Node.js%E7%9A%84%E8%B3%87%E6%96%99%E5%BA%AB%E6%87%89%E7%94%A8.pdf](https://lrs.itsa.org.tw/file.php/595/104教材--網路及平台服務_高雄大學張保榮/Part_A-_平台服務課程教材/2.教材投影片/12_Node.js的資料庫應用.pdf)



