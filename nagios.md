**監控**

**Nagios**

Ø組織介紹

Nagios是一個監視系統運行狀態和網絡信息的系統，它檢測主機和服務，當異常發生和解除時能提醒用戶。它是基於GPLv2開發的開源軟體，可免費獲得及使用。Nagios原名為NetSaint，由Ethan Galstad開發並維護至今。可運行在Linux/Unix平台之上，同時提供一個可選的基於瀏覽器的WEB界面以方便系統管理人員查看網絡狀態，各種系統問題，以及日誌等等。



Ø軟體介紹

Nagios是插件式的結構，本身沒有任何監控功能，所有的監控都是通過插件進行的，因此是高度模塊化和富於彈性的。Nagios監控的對象可分為兩類：主機和服務。主機通常指的是物理主機，如伺服器、路由器、工作站和印表機等，這裡的主機也可以是虛擬設備，如xen虛擬出的Linux系統；而服務通常指某個特定的功能，如提供http服務的httpd進程等。而為了管理上的方便，主機和服務還可以分別被規劃為主機組和服務組等。



Nagios不監控任何具體數值指標（如作業系統上的進程個數），它僅用四種抽象屬性對被監控對象的狀態進行描述：OK、WARNING, CRITICAL UNKNOWN。於是，管理員只需要對某種被監控對象的WARNING和CRITICAL狀態的閾值進行關注和定義即可。

Nagios的監控對象有哪些：

u本機的運行狀態

u本機的服務的運行狀態

u遠程主機

u遠程主機上的服務

u監控網絡服務（SMTP、POP3、HTTP、PING等）

u監控主機資源（處理器負荷、磁碟利用率等）



系統特點：

u監控主機資源和網絡服務

u允許用戶通過設計實現簡單的插件來監控自己特定的服務

u當被監控對象出現問題時，會及時通知管理人員

u事先定義事件處理程序，當對象出現問題時自動調用對應的處理程序

u通過web頁面來監視對象狀態，警告提示和日誌文件

Ø應用

Nagios是一款用於監控IT基礎架構和查看當前狀態、歷史日誌和基本報告的開源軟體工具。Nagios用戶可以監控系統指標，網路協議，應用程序，伺服器，網路基礎架構和接收故障警報。Nagios提供三種類型的網路管理工具，Nagios XL，Nagios日誌伺服器和Nagios網路分析器。其中Nagios XL最適合網路監控。Nagios XL提供企業級網路監控，為用戶提供頻寬報告，網路心跳監控，自定義URL，電子郵件報告和遠程機器監控。升級的企業版提供基於Web的伺服器控制台訪問，業務流程監控，記錄審核和自動化刪除功能。



Nagios是在OpenStack部署中廣泛使用的，用於監控雲平台各種服務的開源工具，另外，它的擴展性良好，很容易加入自行開發的監控項目，為用戶提供了很大的便利性和靈活性。

來自2011年DZone的數據顯示，該網站的企業級開發用戶中，43%都使用過Nagios, Zabbix或者Ichinga。此外Nagios是最受歡迎的監控工具之一，甚至占據了29%的市場份額。



資料來源：

[https://read01.com/PMdnzg.html](https://read01.com/PMdnzg.html)

[https://translate.google.com.tw/translate?hl=zh-TW&sl=zh-CN&u=https://zh.wikipedia.org/zh-tw/Nagios&prev=search](https://translate.google.com.tw/translate?hl=zh-TW&sl=zh-CN&u=https://zh.wikipedia.org/zh-tw/Nagios&prev=search)

[https://read01.com/zh-tw/PMdnzg.html\#.WeW6mFtL-M8](https://read01.com/zh-tw/PMdnzg.html#.WeW6mFtL-M8)

[https://kknews.cc/zh-tw/other/3jq6n3.html](https://kknews.cc/zh-tw/other/3jq6n3.html)

[https://read01.com/5MNJ0z.html](https://read01.com/5MNJ0z.html)

[https://kknews.cc/zh-tw/tech/38bgy3.html](https://kknews.cc/zh-tw/tech/38bgy3.html)

[https://ddnews.me/tech/u5bynlwk.html](https://ddnews.me/tech/u5bynlwk.html)

[https://baike.baidu.com/item/Nagios](https://baike.baidu.com/item/Nagios)

