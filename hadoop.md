# **大數據**

## **Hadoop**

![](/assets/Hadoop.png)

### 典範案例

* [經濟部水利署 — 水利雲受推崇開源軟體扮演幕後功臣](/shui-li-yun-shou-tui-chong-kai-yuan-ruan-ti-ban-yan-mu-hou-gong-chen.md)
* [中央研究院 — R軟體成統計分析市場主流](/man-zu-zhi-ming-ji-yin-ding-wei-xu-qiu-r-ruan-ti-cheng-tong-ji-fen-xi-shi-chang-zhu-liu.md)

### 組織介紹

Hadoop 源自於 Google 在2004年提出 Map/Reduce 和 Google File System 的啟發，Google 的 MapReduce 運算方法可以把應用程式分解為許多並行計算指令，跨大量的計算節點運行巨大的數據集。使用該框架的常見例子就是在網路數據上運行的搜索演算法。

Hadoop 最初只與網頁引擎技術有關，迅速發展成為分析大數據的雲端技術，目前屬於 Apache 軟體基金會的頂級開源計畫之一，在開放原始碼、社群基礎且完全免費的條件之下，被各種組織和產業廣為應用。

### 軟體介紹

Hadoop 用戶可以在不了解分散式底層細節的情況下，開發分散式程式。充分利用集群的威力進行高速運算、存儲和分析。雲端運算技術由最主要的兩個元件及架構組成：

* HDFS \(Hadoop Distributed File System\) 分散式檔案系統：由單一伺服器擴充到許多伺服器或電腦，形成雲端架構中的節點。這些節點所組成的大型分散式檔案系統，可以避免資料遺失或損壞而影響系統整體服務，不僅變更架構規模更加容易，還能提供更高的可靠性。
* MapReduce 分散式資料平行運算處理架構：是一種工作負載分散處理系統，將待處理的工作拆解成多個執行緒 \(thread\)，在上千台機器上平行處理巨量資料，有效的節省資料處理的時間。

Hadoop 無法完全解決巨量資料的難題，Apache 基金會開發了其他與 Hadoop 技術相關的開源套件，共同組成 Hadoop 體系，以應付巨量資料的其他需求。相關專案包含：「Pig」用來處理資料的 Script 語言撰寫、「Hive」可使用 SQL 語法查詢和大型資料的存取功能、「HBase」專門用在 Hadoop 以分散式儲存方式應付 PB 等級的資料處理。

### 應用

Hadoop 可以處理結構化及非結構化資料的型態資料，通訊紀錄、圖片、聲音和電子郵件…等，提供使用者更多隱含在資料裡的訊息以對應決策。技術已經得到廣泛運用，多數的雲端運算平台供應商皆以 Hadoop 架構為基礎，再開發各自的雲端運算服務。

* 網路零售業：Amazon 以 Hadoop 架構建置 Amazon EC2 雲端運算平台，讓使用者能彈性的租用雲端電腦運行所需應用的系統，透過簡易的服務介面，能適當的發揮效能並且為使用者節省運算時間及開發成本。Wal-Mart 則使用 Hadoop 來分析消費者搜尋行為，利用關鍵字的分析結果找出消費者需求，以規劃後續的行銷策略。並預計深入 Facebook, Twitter 分析消費者在社群網站上對商品的討論，以領先競爭者一步發現消費者需求，並主動寄送相關商品的促銷訊息。
* 社群網站：Facebook 建置超過600台伺服器的雲端運算系統，以處理每日產生的大量資料與系統紀錄。
* 搜尋引擎：Yahoo搜尋引擎，以 HBase 資料庫儲存全球各地的 web 資料，再利用 Hadoop MapReduce 分散處理這些資料，以處理1兆個網路連結以及高達 5 PB 的網頁內容，建立全球網際網路的網頁索引資料。
* 金融業：Visa 公司為降低詐騙及盜領等犯罪損失，利用 Hadoop 在作為信用卡付款驗證的系統 VisaNet 上，每天分析上億筆的交易資料，Hadoop 系統有效的將分析時間從耗費上月降至10多分鐘，迅速的發現可疑交易，並能通知銀行以阻止詐騙交易。

### 資料來源：

* Welcome to Apache™ Hadoop®! [http://hadoop.apache.org/](http://hadoop.apache.org/)
* 什麼是Hadoop [http://wiki.mbalib.com/zh-tw/Hadoop](http://wiki.mbalib.com/zh-tw/Hadoop)
* 雲端生活－雲端運算技術探討與發展趨勢 [https://www.fisc.com.tw/tc/knowledge/quarterly1.aspx?PKEY=dffd88ca-ce2b-4680-bb31-e46be1687159](https://www.fisc.com.tw/tc/knowledge/quarterly1.aspx?PKEY=dffd88ca-ce2b-4680-bb31-e46be1687159)
* Hadoop技術協助企業解決巨量資料難題 [https://www.ithome.com.tw/node/73977](https://www.ithome.com.tw/node/73977)
* 擴充Hadoop功能的軍火庫 [https://www.ithome.com.tw/node/73980](https://www.ithome.com.tw/node/73980)
* Big Data 大數據 大商機 大未來 [http://mmdays.com/2012/12/22/big-data-%E5%A4%A7%E8%B3%87%E6%96%99-%E5%A4%A7%E5%95%86%E6%A9%9F/](http://mmdays.com/2012/12/22/big-data-大資料-大商機/)



