# **資料庫**

## **MongoDB**

![](/assets/mongodb.png)

### 典範案例

* [內政部營建署著手打造 SDS 架構](/use-case/di-zhi-teng-yun-wang-yun-yong-duo-tao-kai-yuan-ruan-ti/ying-jian-shu-zhu-shou-da-zao-sds-jia-gou.md)

### 組織介紹

是 2007 年由 10gen 公司開發的一套開源 NoSQL 資料庫，屬於文件導向資料庫類型，希望能夠結合關係資料庫與非關係資料庫雙方的優點，適合用在網頁應用程式、網路架構的環境底下。2013 年更名為 MongoDB Inc.，讓大家能由公司名稱直接就聯想到其代表性產品。

### 軟體介紹

MongoDB 是一款由 C++ 編寫的高性能、開源、無模式的常用非關係型資料庫產品，是非關係資料庫當中功能最豐富、最像關係資料庫的資料庫。它擴展了關係型資料庫的眾多功能，例如：輔助索引、範圍查詢、排序等。

MongoDB 主要解決的是巨量數據的訪問效率問題，它作為分散式數據崛起後，使用較多的一款非結構資料庫，它的主要功能特性如下：

* 集合導向的儲存：適合存儲物件類型資料及 JSON 形式的數據。
* 動態查詢：支援豐富的查詢表達式。查詢指令使用 JSON 形式的標記，可輕易查詢文件中內嵌的對象及數組。
* 完整的索引支援：包括文件內嵌對象及數組。MongoDB 的查詢優化器會分析查詢表達式，並生成一個高效的查詢計劃。
* 查詢監視：包含一個監視工具用於分析資料庫操作的性能。
* 複製及自動故障轉移：MongoDB 資料庫支援伺服器之間的數據複製，支援主-從模式及伺服器之間的相互複製。複製的主要目標是提供冗餘及自動故障轉移。
* 高效的傳統存儲方式：支援二進位數據及大型對象（如圖片或視頻）。
* 自動分片：支援雲級別的伸縮性，自動分片功能支援水平的資料庫集群，可動態添加額外的機器。

### 應用

MongoDB 已經有 900 萬下載，使用者包括財富 500 公司如 eBay, Cisco, MetLife, Adobe…等。相比傳統關係資料庫，MongoDB 對於大數據，高並發以及高可靠性支援更好。適用於各種應用場景如 CRM，內容管理，事件紀錄，商情分析，手機應用，社交等。

* 網站實時數據：MongoDB 非常適合即時的插入，更新與查詢，並具備網站實時數據存儲所需的複製及高度伸縮性。
* 數據緩存：由於性能很高，MongoDB 也適合作為信息基礎設施的緩存層。在系統重啟之後，由 MongoDB 搭建的持久化緩存層可以避免下層的數據源過量。
* 大尺寸、低價值數據存儲：使用傳統的關係型資料庫存儲一些數據時可能會比較昂貴，在此之前，很多時候程式員往往會選擇傳統的文件進行存儲。
* 高伸縮性場景：MongoDB 非常適合由數十或數百台伺服器組成的資料庫。MongoDB 的路線圖中已經包含對 MapReduce 引擎的內置支援。
* 對象或 JSON 數據存儲：MongoDB 的 BSON 數據格式非常適合文件化格式的存儲及查詢。

實際案例：中國東方航空 2015 年初開始打造全新航空電商系統，選用了可橫向擴展的 MongoDB 資料庫，7 月部分系統已上線，預估目標要能承載一天 10 億次資料庫查詢，而開放的部分先供旅行社以及平板平臺做航班搜尋，以 3 臺伺服器撐住每日 500 萬次查詢量。

### 資料來源：

* MongoDB for GIANT Ideas [https://www.mongodb.com/](https://www.mongodb.com/)
* MongoDB資料庫開發應用（1）--MongoDB資料庫的基礎知識和使用 [http://www.zendei.com/article/357.html](http://www.zendei.com/article/357.html)
* mongodb快速入門 [http://www.itread01.com/content/1507611383.html](http://www.itread01.com/content/1507611383.html)
* MongoDB學習筆記 MongoDB介紹及安裝 [https://read01.com/zh-tw/jjGO2o.html\#.WeQrzVuCyM8](https://read01.com/zh-tw/jjGO2o.html#.WeQrzVuCyM8)
* 東方航空用MongoDB挑戰1天10億次網站查詢 [https://www.ithome.com.tw/news/98087](https://www.ithome.com.tw/news/98087)



