# **大數據**

## **Spark**

![](/assets/Spark.png)

### 典範案例

* [經濟部水利署 — 水利雲受推崇開源軟體扮演幕後功臣](/shui-li-yun-shou-tui-chong-kai-yuan-ruan-ti-ban-yan-mu-hou-gong-chen.md)
* [中央研究院 — R軟體成統計分析市場主流](/man-zu-zhi-ming-ji-yin-ding-wei-xu-qiu-r-ruan-ti-cheng-tong-ji-fen-xi-shi-chang-zhu-liu.md)

### 組織介紹

Apache Spark 是一個圍繞速度、易用性和複雜分析構建的大數據處理框架。Spark 在2009年由 Matei Zaharia 在加州大學柏克萊分校AMPLab 開創，2010年透過 BSD 授權條款開源釋出。2013年該專案被捐贈給 Apache 軟體基金會並切換授權條款至 Apache2.0。2014年 Spark 成為 Apache 的頂級專案，有超過400多位貢獻家投入 Spark 開發，讓其成為基金會以及巨量資料眾多開源專案中最活躍得專案。

### 軟體介紹

Spark 是一個彈性的運算框架，包含多個緊密集成的組件。適合做 Spark Streaming 資料流處理、Spark SQL 互動分析、ML Lib 機器學習等應用，因此 Spark 可成為一個用途廣泛的大數據運算平台，負責多個工作機器之間或一個計算集群上調度、分發和監控由計算任務組成的應用。Spark 允許用戶將資料載入至叢集記憶體內儲存，並多次重覆運算，非常適合用於機器學習演算法。

* Spark Core：Spark 的核心功能實現，包括︰SparkContext 的初始化、部署模式、存儲體系、任務提交與執行、計算引擎等。
* Spark SQL：作為 Apache Spark 大數據框架的一部分，主要用於結構化數據處理和對 Spark 數據執行類 SQL 的查詢。通過 Spark SQL，可以針對不同格式的數據執行 ETL 操作然後完成特定的查詢操作。
* Spark Streaming：是 Spark 核心 API 的一個擴充，它對即時資料串流的處理具有可擴充性、高資料量、可容錯性等特點。
* MLlib：是 Spark 擴展的機器學習庫。提供多種類型的機器學習算法，包括分類、回歸、群集和協同過濾，並支持模型評估和數據導入功能。也提供一個低層的機器學習原語，包括一個通用的梯度下降優化算法。
* GraphX：是 Spark 上的分散式圖形處理框架。它提供了一組 API，可用於表達圖表計算並可以模擬 Pregel 抽象化。GraphX 還對這種抽象化提供了優化運行。

### 應用

Spark 設計具有一種泛用性，剛好將運算模組和底層架構切開，讓擅長大資料分析的社群來協助開發各種大資料分析模組，又能讓擅長叢集運算和底層架構的專家來優化底層資源管理，也因此吸引了大批開發者參與。

2015年 IBM 宣布將大規模資助 Spark，微軟、Google 也應用 Spark 建置數據雲端分析服務與機器學習平台，顯示 Spark 現在已成為許多企業與技術人員愛用的大數據資料分析框架。不少跨國大型網路服務業者如 Twitter, eBay, Uber, Netflix 等都是 Spark 使用者，也有汽車業如 Toyota 也使用 Spark 來分析資料。

* 遊戲領域：從即時的潛在遊戲事件中迅速地探勘出有價值的模式，以創造出巨大的商業利益，比如用戶回傳率情況、如何制定定向廣告以及如何自動調整遊戲的複雜度等。
* 電子商務領域：即時交易數據將被傳遞到k均值算法或者 ALS 等協同過濾流算法中。這些運算結果將和顧客評論等非結構化數據結合起來，用於不斷改進交易模式以適應新趨勢的發展。
* 金融或證券領域：Spark堆棧技術可以被應用到信用詐騙和風險管控系統中。通過獲取大量的歷史數據和其他一些外洩數據以及一些連接/請求信息（IP地理信息或時間信息），可以取得非常好的模型結果。

### 資料來源：

* Lightning-fast cluster computing [https://spark.apache.org/](https://spark.apache.org/)
* 維基百科 Apache Spark [https://zh.wikipedia.org/wiki/Apache\_Spark](https://zh.wikipedia.org/wiki/Apache_Spark)
* Apache Spark 介紹 [http://pythonsparkhadoop.blogspot.tw/2016/11/apache-spark.html](http://pythonsparkhadoop.blogspot.tw/2016/11/apache-spark.html)
* Spark是什麼？用Spark進行數據分析 [http://www.bigdatafinance.tw/index.php/tech/coding/253-spark-spark](http://www.bigdatafinance.tw/index.php/tech/coding/253-spark-spark)
* spark架構和調整 [https://ifun01.com/8AOBEFH.html](https://ifun01.com/8AOBEFH.html)
* 【Spark研究】用Apache Spark進行大數據處理第二部分：Spark SQL [https://read01.com/zh-tw/P5nKN.html\#.WeRJKluCyM8](https://read01.com/zh-tw/P5nKN.html#.WeRJKluCyM8)
* 大資料技術新秀Spark如何通吃批次和串流資料分析能力 [https://www.ithome.com.tw/news/103290](https://www.ithome.com.tw/news/103290)
* 微軟雲端大數據宣布投入更多Spark應用開發 [https://www.bnext.com.tw/article/39838/BN-2016-06-07-025724-216](https://www.bnext.com.tw/article/39838/BN-2016-06-07-025724-216)
* 事實上，Spark是一項非常值得學習的技術 [https://kknews.cc/zh-tw/news/4b2pev.html](https://kknews.cc/zh-tw/news/4b2pev.html)



