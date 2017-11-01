**監控**

**OpenNMS**

Ø組織介紹

OpenNMS是一個免費的開源企業級網絡監控和網路管理平台。它是由用戶和開發人員社區以及OpenNMS集團開發和支持的，提供商業服務、培訓和支持。目標是使OpenNMS成為FCAPS網絡管理模型的所有方面的真正分佈式，可擴展的管理應用平台，同時保持100％的免費和開放源代碼。目前的重點是放在故障和性能管理。與該項目相關的所有代碼均可在Affero通用公共許可證下獲得。



Ø軟體介紹

OpenNMS是一個企業級基於Java/XML的分布式網絡和系統監控管理平台。它能夠顯示你網絡中各中終端和伺服器的狀態和配置，為你方便地管理網絡提供有效信息。



u故障管理\(Fault Management\)：在OpenNMS中，有三種不同且互相獨立的方式來發現故障：

服務定期查詢（周期性檢查服務運行情況）

收到自動發送的通知消息（如SNMP trap）

性能數據的閾值檢查

u性能管理\(Performance Management\)：在OpenNMS中是通過稱之為數據收集器提供的數據收集接口來定期收集性能數據，目前的實現中，包括諸如SNMP，JMX，HTTP及NSClient，對於收集的性能數據可以用於顯示性能圖表，閾值檢查，TopN分析等。

u計費功能：OpenNMS隻提供瞭對於網絡的使用情況的數據、系統資源諸如帶寬、CPU、磁盤空間等的使用情況。

u配置管理：OpenNMS提供瞭資產管理，另外還可以通過UI開啟/關閉設備接口，也隻僅限於這些功能。

u安全管理：提供瞭對於SNMPv3的支持，另外還提供瞭基於用戶的訪問控制及LDAP安全模型。



Ø應用

uOpenNMS是在1999年發布的，旨在為大型企業級用戶提供事件管理，服務監控和性能測量。使企業用戶受益的主要特點包括外部腳本、向通話系統工程師發送警報、擴展Java本機通知策略API、請求跟蹤\(RT\)集成、高級警報、IPv4和IPv6網路可達性超過\(ICMP\)、測試狀態和節點庫存信息。企業服務或是「風格」網路提供預置事件，通知，數據收集，工作流和附加報告等功能。



uOpenNMS的手機套件，預設是透過HTTP、TCP 8980埠的管道與系統相連接，或者也可以視需求，而改用SSL加密傳輸的資料。在手機開啟OpenNMS的管理介面，可以從Alarms的分頁查看條列的訊息，或者是切換到Nodes的畫面，根據特定裝置，查找與之相關的所有記錄，使用上算是相當容易。

如果管理者是透過瀏覽器連接OpenNMS的網頁介面，則除了收集連網裝置的狀態之外，也能進一步連接到設備進行操作。對於能透過文字介面的Telnet、SSH，及RSH從遠端登入的裝置來說，可以將連線所需的帳號、密碼先行設定於OpenNMS，日後就可以直接從網管系統的網頁介面直接開啟連線。而除了網管軟體最常使用的SNMP之外，OpenNMS也能透過WMI收集Windows主機的相關資訊。







資料來源：

[http://www.wenwenti.info/article/780163](http://www.wenwenti.info/article/780163)

[http://www.ifuun.com/a2017773630947/](http://www.ifuun.com/a2017773630947/)

[https://translate.google.com.tw/translate?hl=zh-TW&sl=en&u=https://en.wikipedia.org/wiki/OpenNMS&prev=search](https://translate.google.com.tw/translate?hl=zh-TW&sl=en&u=https://en.wikipedia.org/wiki/OpenNMS&prev=search)

[https://read01.com/QagjGG.html](https://read01.com/QagjGG.html)

[https://www.ithome.com.tw/tech/92231](https://www.ithome.com.tw/tech/92231)
