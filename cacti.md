# **監控**

## **Cacti**

![](/assets/cacti.jpg)

### 典範案例

* [台中榮民總醫院致力引進開源軟體](//use-case/vghtc.md)
* [內政部營建署著手打造 SDS 架構](/use-case/di-zhi-teng-yun-wang-yun-yong-duo-tao-kai-yuan-ruan-ti/ying-jian-shu-zhu-shou-da-zao-sds-jia-gou.md)

### 組織介紹

Cacti 是一個針對數據中心的網路層、平台層、數據層以及業務層全流程進行監控的運維管理平台。它也是根據 RRDTool 開源項目的一個前端展示平台。2001 年發布了它的第一個版本。

### 軟體介紹

Cacti 是一款開源的網路監控和繪圖工具。它通過 snmpget 來獲取數據，使用 RRDtool 繪畫圖形，並提供了非常強大的數據和使用者管理功能，可以指定每一個使用者能查看樹狀結構、主機以及任何一張圖，還可以與 LDAP 結合進行使用者驗證，同時也能自己增加模板。

Cacti 允許使用者以預定的邊界輪詢服務並繪製所得數據。它通常用於繪製例如 CPU 負載和網路寬頻利用率的度量的時間序列數據。常見的用法是通過簡單網路管理協議 \(SNMP\) 輪詢網路交換機或路由器接口來監控網路流量。Cacti 還包括使用者管理工具，支援添加使用者，並按需給他們的賦予某些區域的訪問權限。

Cacti 三層架構：數據展現層、數據存儲層、數據採集層，其具體如下：

* 數據採集層：通過 SNMP 或自定義腳本進行數據采集。
* 數據存儲層：通過 cacti 模板等數據存放至 MySQL中。
* 數據展現層：通過 WEB 方式呈現出來。

### 應用

#### Cacti Plugins

Cacti 豐富的 Plugins 套件，將許多網路管理上常用及好用的軟體整合至 Cacti 系統中，除了有效減輕管理人員所需管理伺服器數量，整合化的頁面也簡化了管理者分析問題時的工作，不再需要同時登入多台主機查閱相關歷史資料。

舉例來說，我們可以讓 Cacti 兼當 syslog Server（安裝 Pluginssyslog 套件），當設備出現異常時不用一台一台登入網路設備查看日誌記錄，假設在 Cacti 偵測資訊裡發現到某一台設備 CPU 出現異常，管理者只需要在同個 web 頁面中點至 syslog 頁面查詢該設備的log 資訊即可。

此外管理者可以利用 Weathermap 套件，依企業或單位的網路架構，繪製出符合使用者實際環境的總體流量資訊圖，而 Weathermap透過 Java script 的語法，只要將滑鼠移至架構圖中任一電路上，即帶出該電路的歷史流量統計圖。除了上述兩個套件外，想要偵測多台主機的運作情形，可以使用監視程式套件、想要進行 netflow 統計分析，可以使用 flowview 套件、針對組織內大量使用者的 mac address 管理，可以使用 MacTrack 套件以及想要由 Cacti 提供警報功能時，則可以使用 Thold 套件。

#### Cacti Graph Templates

雖然 Cacti 在安裝完成後提供部份廠牌設備的模板（如：Cisco、Linux），但是如果需要偵測其他廠牌設備的 CPU, Memory, session 時，可以利用自行定義模板的方式，產生所需要偵測的數據資料。當 Cacti 取回數據資料後，即可如一般流量統計計錄流程數量。

### 資料來源

* Cacti® - The Complete RRDTool-based Graphing Solution. [https://www.cacti.net/](https://www.cacti.net/)
* [https://baike.baidu.com/item/Cacti/10496138](https://baike.baidu.com/item/Cacti/10496138)
* [http://www.itread01.com/content/1506965891.html](http://www.itread01.com/content/1506965891.html)
* [http://www.ringline.com.tw/zh-tw/article\_info.php?id=44](http://www.ringline.com.tw/zh-tw/article_info.php?id=44)
* [https://yq.aliyun.com/articles/117712](https://yq.aliyun.com/articles/117712)
* [https://en.wikipedia.org/wiki/Cacti\_\(software\)](https://en.wikipedia.org/wiki/Cacti_%28software%29)



