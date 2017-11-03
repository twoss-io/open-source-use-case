# **資料庫**

## **MariaDB**

![](/assets/MariaDB.png)

### 組織介紹

MariaDB是從MySQL獨立出來的另一套衍生資料庫，而且都來自相同的創始人Michael Widenius和其他創始人在1994年開始開發MySQL，2008年將MySQL賣給了昇陽電腦，傳為開源軟體商業化的經典案例。

2年後，MySQL更推出大受歡迎的5.5版，但甲骨文卻收購了昇陽電腦。

為保證仍有開源可用的兼容MySQL的分支可用，Michael Widenius在創立了MariaDB的同時，還成立了非營利組織MariaDB基金會為MariaDB項目、用戶和開發者社區提供基礎架構支援。目前MariaDB是發展最快的MySQL分支版本，新版本發佈速度已經超過了商用的MySQL版本，在開源數據庫領域擁有較強的技術影響力。

### 軟體介紹

一個資料庫應用程序分成主應用程序和存儲資料的聚集。每個資料庫都使用一個或多個API來創建、訪問、管理、搜尋和複製資料。資料庫還使用非關係資料源，例如目標或文件。然而，大型資料集常因為檢索緩慢和需要寫入其他資料源，資料庫證明是其最好的選擇。關係資料庫管理系統或RDBMS，將資料儲存在各種表中。而表之間的關係則是使用主鍵和外鍵來建立。

RDBMS提供了以下功能：

* 能夠實現與表，列和索引的資料源
* 確保引用的多個表中的行完整性
* 自動更新指標
* 解釋SQL查詢和操作從表操作採購數據

MariaDB的重要特點是：

所有MariaDB的是根據GPL，LGPL，或者BSD。

* MariaDB的包括存儲引擎，包括高性能存儲引擎的廣泛選擇，用於與其他RDBMS資料源工作
* MariaDB的使用標準和流行的查詢語言
* MariaDB的運行在多種操作系統，並支持多種編程語言
* MariaDB的提供了PHP，最流行的Web開發語言之一的支持
* MariaDB的提供加萊拉集群技術
* MariaDB的還提供了許多操作和的MySQL命令不可用，並消除/替換功能，影響性能產生負面影響

### 應用

MariaDB擁有約1200萬名全球用戶，其中包括Booking.com、惠普、維珍移動和維基百科。它的解決方案在私有、公共和混合雲部署中使用，在許多Linux發行版中都是預設的，比如Red Hat、Ubuntu和SUSE，這使得6000萬用戶的數量進一步增加。

2017年MariaDB基金會宣佈，騰訊雲正式成為MariaDB基金會白金會員，這是基金會最高級別會員。意味騰訊雲在開源領域的步伐正在不斷深入，從IaaS的開源進入到PaaS的開源。在騰訊內部，一直有一個數據庫內核團隊，在MySQL和MariaDB基礎上之上做出改進優化，騰訊雲完成了主備節點鎖拆分、動態調整各種級別複製參數，以及binlog寫優化等；發現並解決了死結引起的innodb 600S crash問題、memory barrier引起的hang問題以及字符串問題等影響資料庫穩定的問題。未來，騰訊雲還將投入更多精力到內核研發上，並會合併之前的一些內部穩定使用功能發佈開源版本。

### 資料來源：

* MariaDB \| Open Source Database \(RDBMS\) for the Enterprise [https://mariadb.com/](https://mariadb.com/)
* 維基百科 MariaDB [https://zh.wikipedia.org/wiki/MariaDB](https://zh.wikipedia.org/wiki/MariaDB)
* MariaDB 10新版大躍進 [https://www.ithome.com.tw/news/86622](https://www.ithome.com.tw/news/86622)
* MariaDB的介紹 [http://www.w3ii.com/zh-TW/mariadb/mariadb\_introduction.html](http://www.w3ii.com/zh-TW/mariadb/mariadb_introduction.html)
* MariaDB 基金會發布 MariaDB 10 的通用版 [https://ifun01.com/8V8ZFD4.html](https://ifun01.com/8V8ZFD4.html)
* 百度百科 MariaDB [https://baike.baidu.com/item/MariaDB\#reference-\[1\]-2521908-wrap](https://baike.baidu.com/item/MariaDB#reference-[1]-2521908-wrap)
* Google棄甲骨文MySQL，將大規模導入MariaDB [https://blog.pumo.com.tw/archives/630](https://blog.pumo.com.tw/archives/630)
* 騰訊雲正式成為MariaDB基金會白金會員 [http://sina.com.hk/news/article/20170619/0/5/2/%E9%A8%B0%E8%A8%8A%E9%9B%B2%E6%AD%A3%E5%BC%8F%E6%88%90%E7%82%BAMariaDB%E5%9F%BA%E9%87%91%E6%9C%83%E7%99%BD%E9%87%91%E6%9C%83%E5%93%A1-7571666.html](http://sina.com.hk/news/article/20170619/0/5/2/騰訊雲正式成為MariaDB基金會白金會員-7571666.html)



