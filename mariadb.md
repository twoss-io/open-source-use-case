# **資料庫**

## **MariaDB**

![](/assets/MariaDB.png)

### 典範案例

* [內政部營建署著手打造 SDS 架構](/use-case/di-zhi-teng-yun-wang-yun-yong-duo-tao-kai-yuan-ruan-ti/ying-jian-shu-zhu-shou-da-zao-sds-jia-gou.md)

### 組織介紹

MariaDB 是從 MySQL 獨立出來的另一套衍生資料庫，而且都來自相同的創始人 Michael Widenius 和其他創始人在 1994 年開始開發MySQL，2008年將 MySQL 賣給了昇陽電腦，傳為開源軟體商業化的經典案例。

2 年後，MySQL 更推出大受歡迎的 5.5 版，但甲骨文卻收購了昇陽電腦。為保證仍有開源可用的兼容 MySQL 的分支可用，Michael Widenius 在創立了 MariaDB 的同時，還成立了非營利組織 MariaDB 基金會為 MariaDB 項目、使用者和開發者社群提供基礎架構支援。目前 MariaDB 是發展最快的 MySQL 分支版本，新版本發佈速度已經超過了商用的 MySQL 版本，在開源資料庫領域擁有較強的技術影響力。

### 軟體介紹

一個資料庫應用程序分成主應用程序和存儲資料的聚集。每個資料庫都使用一個或多個 API 來創建、訪問、管理、搜尋和複製資料。資料庫還使用非關係資料源，例如目標或文件。然而，大型資料集常因為檢索緩慢和需要寫入其他資料源，資料庫證明是其最好的選擇。關係資料庫管理系統或 RDBMS，將資料儲存在各種表中。而表之間的關係則是使用主鍵和外鍵來建立。

RDBMS 提供了以下功能：

* 能夠實現與表、列和索引的資料源。
* 確保引用的多個表中的完整性。
* 自動更新指標。
* 解釋 SQL 查詢和從表操作採購數據。

MariaDB 的重要特點是：

* 所有 MariaDB 的是根據 GPL, LGPL，或者 BSD。
* 為了與其他 RDBMS 資料源搭配使用，可選擇各種儲存引擎使用，並包括高性能存儲引擎。
* 使用標準和流行的查詢語言。
* 運行在多種操作系統，並支援多種編程語言。
* 提供了 PHP，最流行的 Web 開發語言之一的支援。
* 提供加 Galera 集群技術。
* 提供了許多 MySQL 無法使用的操作及命令，並消除、替代了負面表現的影響。

### 應用

MariaDB 擁有約 1200 萬名全球使用者，其中包括 Booking.com、惠普、維珍移動和維基百科。它的解決方案在私有、公共和混合雲部署中使用，在許多 Linux 發行版中都是預設的，比如 Red Hat、Ubuntu 和 SUSE，這使得 6000 萬使用者的數量進一步增加。

2017 年 MariaDB 基金會宣佈，騰訊雲正式成為 MariaDB 基金會白金會員，這是基金會最高級別會員。意味騰訊雲在開源領域的步伐正在不斷深入，從 IaaS 的開源進入到 PaaS 的開源。在騰訊內部，一直有一個數據庫內核團隊，在 MySQL 和 MariaDB 基礎上之上做出改進優化，騰訊雲完成了主備節點鎖拆分、動態調整各種級別複製參數，以及 binlog 寫優化等；發現並解決了死結問題引起的innodb 600S 當機問題、記憶隔離引起的暫停問題以及字元串問題等影響資料庫穩定的問題。未來，騰訊雲還將投入更多精力到內核研發上，並會合併之前的一些內部穩定使用功能發佈開源版本。

### 資料來源：

* MariaDB \| Open Source Database \(RDBMS\) for the Enterprise [https://mariadb.com/](https://mariadb.com/)
* 維基百科 MariaDB [https://zh.wikipedia.org/wiki/MariaDB](https://zh.wikipedia.org/wiki/MariaDB)
* MariaDB 10新版大躍進 [https://www.ithome.com.tw/news/86622](https://www.ithome.com.tw/news/86622)
* MariaDB的介紹 [http://www.w3ii.com/zh-TW/mariadb/mariadb\_introduction.html](http://www.w3ii.com/zh-TW/mariadb/mariadb_introduction.html)
* MariaDB 基金會發布 MariaDB 10 的通用版 [https://ifun01.com/8V8ZFD4.html](https://ifun01.com/8V8ZFD4.html)
* 百度百科 MariaDB [https://baike.baidu.com/item/MariaDB\#reference-\[1\]-2521908-wrap](https://baike.baidu.com/item/MariaDB#reference-[1]-2521908-wrap)
* Google棄甲骨文MySQL，將大規模導入MariaDB [https://blog.pumo.com.tw/archives/630](https://blog.pumo.com.tw/archives/630)
* 騰訊雲正式成為MariaDB基金會白金會員 [http://sina.com.hk/news/article/20170619/0/5/2/%E9%A8%B0%E8%A8%8A%E9%9B%B2%E6%AD%A3%E5%BC%8F%E6%88%90%E7%82%BAMariaDB%E5%9F%BA%E9%87%91%E6%9C%83%E7%99%BD%E9%87%91%E6%9C%83%E5%93%A1-7571666.html](http://sina.com.hk/news/article/20170619/0/5/2/騰訊雲正式成為MariaDB基金會白金會員-7571666.html)



