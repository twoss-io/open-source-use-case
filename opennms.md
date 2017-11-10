# **監控**

## **OpenNMS**

![](/assets/opennms.png)

### 典範案例

* [內政部營建署著手打造 SDS 架構](/use-case/di-zhi-teng-yun-wang-yun-yong-duo-tao-kai-yuan-ruan-ti/ying-jian-shu-zhu-shou-da-zao-sds-jia-gou.md)

### 組織介紹

OpenNMS 是一個免費的開源企業級網路監控和網路管理平台。它是由用戶和開發人員社群以及 OpenNMS 集團開發和支持的，提供商業服務、培訓和支持。目標是使 OpenNMS 成為 FCAPS 網路管理模型的所有方面的真正分佈式，可擴展的管理應用平台，同時保持 100% 的免費和開放原始碼。目前的重點是放在故障和性能管理。與該項目相關的所有原始碼均可在 Affero 通用公共許可證下獲得。

### 軟體介紹

OpenNMS 是一個企業級基於 Java/XML 的分布式網路和系統監控管理平台。它能夠顯示網路中各終端和伺服器的狀態和配置，方便地管理網路提供有效信息。

* 故障管理 \(Fault Management\)：在 OpenNMS 中，有三種不同且互相獨立的方式來發現故障：服務定期查詢（周期性檢查服務運行情況）、收到自動發送的通知消息（如 SNMP trap）、性能數據的門檻值檢查。
* 性能管理 \(Performance Management\)：在 OpenNMS 中是通過稱之為數據收集器提供的數據收集介面來定期收集性能數據，目前的實現中，包括諸如 SNMP, JMX, HTTP 及 NSClient，對於收集的性能數據可以用於顯示性能圖表，門檻值檢查，TopN 分析等。
* 計費功能：OpenNMS 提供了對於網路的使用情況的數據、系統資源諸如頻寬、CPU、磁碟空間等的使用情況。
* 配置管理：OpenNMS 提供資產管理，另外還可以通過 UI 開啟／關閉設備介面，也僅限於這些功能。
* 安全管理：提供對於 SNMPv3 的支持，另外還提供用戶的存取控制及 LDAP 安全模型。

### 應用

OpenNMS 是在 1999 年發布的，旨在為大型企業級用戶提供事件管理，服務監控和性能測量。使企業用戶受益的主要特點包括外部腳本、向通話系統工程師發送警報、擴展 Java 本機通知策略 API、請求追蹤 \(RT\) 集成、高級警報、IPv4 和 IPv6 網路可達性超過\(ICMP\)、測試狀態和節點庫存信息。企業服務或是「風格」網路提供預置事件，通知，數據收集，工作流程和附加報告等功能。

OpenNMS 的手機套件，預設是透過 HTTP、TCP 8980 埠的管道與系統相連接，或者也可以視需求，而改用 SSL 加密傳輸的資料。在手機開啟 OpenNMS 的管理介面，可以從 Alarms 的分頁查看條列的訊息，或者是切換到 Nodes 的畫面，根據特定裝置，查找與之相關的所有記錄，使用上算是相當容易。

如果管理者是透過瀏覽器連接 OpenNMS 的網頁介面，則除了收集連網裝置的狀態之外，也能進一步連接到設備進行操作。對於能透過文字介面的 Telnet、SSH，及 RSH 從遠端登入的裝置來說，可以將連線所需的帳號、密碼先行設定於 OpenNMS，日後就可以直接從網管系統的網頁介面直接開啟連線。而除了網管軟體最常使用的 SNMP 之外，OpenNMS 也能透過 WMI 收集 Windows 主機的相關資訊。

### 資料來源：

* OpenNMS [https://www.opennms.org/en](https://www.opennms.org/en)
* OpenNMS架構介紹 [http://www.wenwenti.info/article/780163](http://www.wenwenti.info/article/780163)
* 2017 年最佳開源網路監控工具 [http://www.ifuun.com/a2017773630947/](http://www.ifuun.com/a2017773630947/)
* 維基百科OpenNMS [https://en.wikipedia.org/wiki/OpenNMS](https://en.wikipedia.org/wiki/OpenNMS)
* 開源還是商用？十大雲運維監控工具橫評 [https://read01.com/QagjGG.html](https://read01.com/QagjGG.html)
* 10套讓你作好網管的iPhone軟體 [https://www.ithome.com.tw/tech/92231](https://www.ithome.com.tw/tech/92231)



