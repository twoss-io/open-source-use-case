# **虛擬化**

## **OpenStack**

![](/assets/OpenStack.png)

### 典範案例

* [經濟部水利署—水利雲受推崇開源軟體扮演幕後功臣](/shui-li-yun-shou-tui-chong-kai-yuan-ruan-ti-ban-yan-mu-hou-gong-chen.md)
* [台中榮民總醫院致力引進開源軟體](//use-case/vghtc.md)
* [財政部關務署導入 LibreOffice 有成](/cai-zheng-bu-guan-wu-shu-dao-ru-libreoffice-you-cheng.md)

### 組織介紹

美國國家航空暨太空總署和Rackspace合作研發的雲端運算軟體，以Apache授權條款，是一個自由軟體和開放原始碼計畫，來打造基礎設施即服務。

2012年OpenStack基金會成立，目標是在全球範圍內服務開發者、用戶及整個生態系統，為其提供共享資源，擴大OpenStack公有雲與私有雲的成長，從而幫助技術廠商選擇平台，助力開發者開發出最佳的雲軟體。

### 軟體介紹

OpenStack項目分為核心服務和共享服務兩大類，核心服務包括計算、存儲和網絡，核心服務之外其他構件則稱為共享服務。並可以提供虛擬機器的方式，對外提供運算資源以便彈性擴充或調度。

* Nova：透過配置及管理使用任何Hypervisor的虛擬機器，提供隨需運算資源。
* Swift：提供了彈性可伸縮、高可用的分布式對象存儲服務，適合存儲大規模非結構化數據。
* Glance：提供可開機磁碟映像的登錄，以及儲存與擷取這些映像的服務。
* Horizon：提供簡易Web介面和管理，控制台為系統管理員和使用者提供圖形化介面，以供存取、配置及自動化雲端資源。可擴充設計更易與協力廠商產品和服務搭配使用。
* Cinder：提供Block資料存取，將持續區塊存取裝置對應至OpenStack運算執行個體，提供區塊儲存設備服務功能，並支援多種儲存解決方案。
* Keystone：提供身分驗證機制，提供集中式使用者目錄，並將其對應至使用者可存取的OpenStack服務。本模組可做為跨雲端作業系統的通用驗證機制，並可與現有的後端目錄服務進行整合。
* Neutron：提供網路管理功能，提供插入式、可擴充、由API驅動的系統，用以管理網路和IP位址。插件式架構可讓使用者充分善用其基本市售工具，或是支援廠商的進階網路服務。
* Trove：主要負責銜接與簡化實際資料庫的使用，提供OpenStack各個服務一個具延展性且可靠的雲端資料庫服務。
* Sahara：提供海量資料運算佈署功能。
* Ceilometer：提供計量與監控功能，提供在OpenStack雲端內收集使用狀況和效能評量的通用基礎架構。
* Heat：以模板為基礎的架構來描述雲端的應用，讓使用者可以設定一個雲端應用模板，來串連建立所需的OpenStack服務資源，而不必分別去建立設定。

### 應用

OpenStack的優勢在於能以開放式軟體架構，供企業作為私有雲環境建置之用，並且提供給公有雲服務業者使用，藉此整合以OpenStack建置的私有雲與雲端私有代管環境，也有一些企業用這套平臺，來支撐關鍵業務應用系統的運作。

OpenStack多半用於軟體測試與開發、網站代管與前導式的IT專案。超過60％的用戶，將OpenStack用於軟體開發、測試、品質保證、持續整合；其次，是以此提供基礎架構服務，占51%；接著，是用於資料庫系統\(35%\)、網站服務與電子商務\(34%\)、網路功能虛擬化\(30%\)、儲存／備份／歸檔\(29%\)；再接下來，才是大數據分析\(26%\)、業務應用系統\(22%\)。用戶產業類別，科技業以20%位居榜首，其次為製造業\(15%\)、零售／餐旅業\(11%\)。

### 資料來源：

* OpenStack is open source software for creating private and public clouds. [https://www.openstack.org/](https://www.openstack.org/)
* 聯通成OpenStack基金會黃金會員，三大運營商齊了 [https://read01.com/zh-tw/exnK02.html\#.WeQth1uCyM8](https://read01.com/zh-tw/exnK02.html#.WeQth1uCyM8)
* OpenStack如何打破“應用牆” [http://www.sites-help.com/aliyun/aliyunqi/1507683483\_zh.html](http://www.sites-help.com/aliyun/aliyunqi/1507683483_zh.html)
* OpenStack 介紹技術 [https://kairen.gitbooks.io/openstack-liberty/content/conceptions/index.html](https://kairen.gitbooks.io/openstack-liberty/content/conceptions/index.html)
* 尋找OpenStack成長新動能 [https://www.ithome.com.tw/news/112032](https://www.ithome.com.tw/news/112032)



