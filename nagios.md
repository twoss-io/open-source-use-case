# **監控**

## **Nagios**

![](/assets/nagios.png)

### 典範案例

* [台中榮民總醫院 — 致力引進開源軟體](//use-case/vghtc.md)

### 組織介紹

Nagios 是一個監視系統運行狀態和網路訊息的系統，它檢測主機和服務，當異常發生和解除時能提醒使用者。它是根據 GPLv2 開發的開源軟體，可免費獲得及使用。Nagios 原名為 NetSaint，由 Ethan Galstad 開發並維護至今。可運行在 Linux/Unix 平台之上，同時提供一個可選用的瀏覽器 WEB 介面以方便系統管理人員查看網路狀態，各種系統問題，以及日誌等。

### 軟體介紹

Nagios 是外掛式的結構，本身沒有任何監控功能，所有的監控都是通過外掛進行的，因此是高度模組化和富於彈性的。Nagios 監控的對象可分為兩類：主機和服務。主機通常指的是實體主機，如伺服器、路由器、工作站和印表機等，這裡的主機也可以是虛擬設備，如 xen 虛擬出的 Linux 系統；而服務通常指某個特定的功能，如提供 http 服務的 httpd 處理過程等。而為了管理上的方便，主機和服務還可以分別被規劃為主機組和服務組等。

Nagios 不監控任何具體數值指標（如作業系統上的處理過程個數），它僅用四種抽象屬性對被監控對象的狀態進行描述：OK、WARNING, CRITICAL, UNKNOWN。於是，管理員只需要對某種被監控對象的 WARNING 和 CRITICAL 狀態的門檻值進行關注和定義即可。

Nagios的監控對象有哪些：

* 本機的運行狀態
* 本機的服務的運行狀態
* 遠端主機
* 遠端主機上的服務
* 監控網路服務（SMTP, POP3, HTTP, PING等）
* 監控主機資源（處理器負荷、磁碟利用率等）

系統特點：

* 監控主機資源和網路服務
* 允許使用者通過設計實現簡單的插件來監控自己特定的服務
* 當被監控對象出現問題時，會及時通知管理人員
* 事先定義事件處理程序，當對象出現問題時自動調用對應的處理程序
* 通過 web 頁面來監視對象狀態，警告提示和日誌文件

### 應用

Nagios 是一款用於監控 IT 基礎架構和查看當前狀態、歷史日誌和基本報告的開源軟體工具。Nagios 使用者可以監控系統指標、網路協議、應用程序、伺服器、網路基礎架構和接收故障警報。Nagios 提供三種類型的網路管理工具，Nagios XL, Nagios 日誌伺服器和Nagios 網路分析器。其中 Nagios XL 最適合網路監控。Nagios XL 提供企業級網路監控，為使用者提供頻寬報告、網路心跳監控、自定義 URL、電子郵件報告和遠程機器監控。升級的企業版提供依據 Web 的伺服器控制台訪問，業務流程監控，記錄審核和自動化刪除功能。

Nagios 是在 OpenStack 部署中廣泛使用的，用於監控雲平台各種服務的開源工具，另外，它的擴展性良好，很容易加入自行開發的監控項目，為使用者提供了很大的便利性和靈活性。

來自 2011 年 DZone 的數據顯示，該網站的企業級開發使用者中，43% 都使用過 Nagios, Zabbix 或者 Ichinga。此外 Nagios 是最受歡迎的監控工具之一，甚至占據了 29% 的市場佔率。

### 資料來源：

* The Industry Standard In IT Infrastructure Monitoring [https://www.nagios.org/](https://www.nagios.org/)
* nagios簡介，nagios及其查件的安裝
  http://blog.51cto.com/cuanlf/1403379
* 維基百科Nagios [https://zh.wikipedia.org/zh-tw/Nagios](https://zh.wikipedia.org/zh-tw/Nagios)
* nagios監控伺服器的搭建 [https://kknews.cc/zh-tw/other/3jq6n3.html](https://kknews.cc/zh-tw/other/3jq6n3.html)
* OpenStack企業雲平台監控實踐 http://www.csdn.net/article/1970-01-01/2823636
* 誰會是 Zabbix 和 Nagios 的繼任者？ http://blog.oneapm.com/apm-tech/633.html
* 2017 年最佳開源網路監控工具 https://www.oschina.net/translate/best-open-source-network-monitoring-tools-2017
* NAGIOS 百度百科 [https://baike.baidu.com/item/Nagios](https://baike.baidu.com/item/Nagios)



