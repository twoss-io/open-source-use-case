# 典範案例 {#典範案例}

## 經濟部水利署 — 水利雲受推崇開源軟體扮演幕後功臣

![](/assets/vghtc-2.png)

**經濟部水利署資訊室 何丁武 工程師**

目前為水利雲主要負責人之一，規劃並辦理水利雲雲端環境的建置與維運相關工作；水利雲背後眾多開源軟體及函式庫\(library\)的構建及應用，即由其率先規劃與導入。

由政府做為領頭羊角色，各個部會邁向開源步伐，無需被商用軟體綁架，並能將資訊架構靈活使用，水利雲從IaaS、PaaS與SaaS層，大量使用開源軟體，效能及穩定性更勝商用軟體，軟體技術服務費用也相當低廉，日後亦不需要擔心授權費用問題。

## 政府帶頭使用開源軟體　有助技術發展改革

由經濟部水利署資訊室負責規劃與建置的水利雲，背後是運用OpenStack建置並搭載眾多開源軟體，系統效能極佳，達成開放活化水文資料的目標，是政府單位運用開源軟體的代表案例之一。

經濟部水利署資訊室何丁武工程師指出，水利雲建立後，可提供開放資料、資料交換、應用服務等三大功能，藉由將各相關機關及單位的水利及水資源資料，資料交換至雲端環境，再以雲端運算加以整合並產製標準化格式及開放格式檔案，供民眾或其它政府機關進行跨界加值。水利雲內，開源軟體擔任重要角色，包括IaaS是運用OpenStack；PaaS使用到Hadoop、CKAN、PostgreSQL、Spark、MySQL、ceph⋯等，何丁武表示，導入開源軟體後，資訊架構展現比商業軟體更佳的穩定性、效能、擴充性，也讓我們有信心在日後於水利雲平臺上，可增加更多跨部門整合運用及讓民眾有感的服務。

## 商用軟體效果不如預期 轉向使用開源軟體

水利署掌管台灣所有水庫安全、經營管理、水庫集水區保育治理及水源涵養保護，依據經濟部水利署組織條例第二條規定，負責掌理12大類型的工作事項，包含水利與自來水政策、法規之擬訂及執行事項，水利與自來水事業之調查、規劃及興辦之審議、協調與督導事項，河川流域保育經理之整體調查規劃、治理計畫之擬訂及水土資源經理分工協調事項等等。

當初在配合行政院推動政府雲的政策下，水利署也在2013年起投入水利雲建置工作，除藉此具備儲存各式水文、水情、河川與水庫等巨量資料能力外，更能活化資料加值性與提升水利、水文的分析能力，將資料轉換為更具加值的服務型態。

何丁武說，水利雲剛建置之初，資訊室是使用商用軟體VMware做為IaaS雲端基礎環境，期望藉由商業軟體廠商的技術支援，確保專案可如期完成，也解決資訊室人力不足的問題。只是系統上線之後，資訊室發現水利署雲效能不如預期，亦無法有效管理後台系統串連的NAS設備，反而造成同仁管理上的負擔。為解決此問題，資訊室也曾考慮引進公有雲，只是經過縝密評估之後，在預算有限挹注的情況下，長期使用成本將會超過水利署的負擔能力。此時恰逢專為雲端IaaS打造的OpenStack，其成熟度與穩定度已備受眾多企業用戶肯定，於是資訊室決定在2015年重新添購10台伺服器及相關網路設備，並運用OpenStack搭配Apache Hadoop、ApacheTomcat、Spark、MySQL、ceph、PostgreSQL等開源軟體，打造效能更好、穩定性更佳的新版水利雲後端雲端環境。

## 搭配眾多開源軟體 水利雲既高效又穩定

在經濟部水利署規劃中，水利資料整合雲平臺上線之後，將具備「整合式服務導向目錄、一致的服務存取規格」、「關聯式資料庫平行轉入雲端功能，個人化雲端儲存空間」、「使用資訊室自行開發API操作底層雲端運算及雲端資料庫」、「Step-by-Step雲端資料庫服務發佈」、「雲端效能監控與警示通知報表」、「開放資料流程與雲端環境緊密整合」等功能。此外，水利署各部門也能享有水利雲所提供的雲端應用系統開發環境及多樣雲端服務，達到降低水利署成本支出的目標。

考量到水利署水資源及水利相關資料，分別來自綜合企劃組、保育事業組、河川海岸組、水利行政組、工程事務組、水文技術組、資訊室、防災中心、水源經營組、土地管理組等，又得分別滿足開放資料、資料交換、應用服務等三大功能需求。經水利署資訊室搭配業界現況並多方考量之後，決定先以OpenStack為IaaS，並以ceph優異的軟體定義儲存開源軟體為其儲存層，Apache Hadoop為主要PaaS，搭配MySQL Cluster，收集及儲存來自各單位的多元資料外，並依照不同功能屬性採用相對應的開源軟體，如針對水利署開放資料呈現部分，即以CKAN搭配PostgreSQL、Solr等；有關開放資料存取及查詢部分，則以Apache Olingo打造OData protocol RESTful API進行M2M資料存取與查詢機制，讓資料可有一致性及標準化的查詢介面。

何丁武解釋， 當水利雲的I a a S 架構， 從VMware解決方案轉換成OpenStack之後，前述效能不佳問題立即獲得改善，初次導入的軟體技術服務費用也相當低廉，日後亦不需要擔心授權費用問題，且導入後之應用效能穩定、整體失效率幾近為零，於接受基礎教育訓練後，可以自行有效維運。至於Apache Hadoop搭配MySQL Cluster，則是收集及儲存多元管道資訊的最佳軟體組合，也成功為日後發展大數據應用的最佳工具。除此之外，在擬定資訊策略「標準化」是非常重要的基本工作，舉例來說，水利署各個所轄機關的資料格式及其命名皆不同，包括水位單位、位置坐標、管理單位、圖資格式⋯等，雖然之前就訂有「水資源格式標準」但屬表格式定義，不利M2M資料交換的進行，於 2013 年以XML Schema 訂定「水資源交換標準」，並將檔案格式規範至標準開放格式。何丁武表示，建立水利資料整合雲平臺，並搭配「水資源交換標準」，目的除為了水利資料可在高效且穩定的雲端環境下被廣範地跨界加值應用外，而資料標準化則有助於提供正確的資料，此外該平臺也確保資料傳送的安全性。

## 積極擁抱開源 提升台灣技術能量

水利署「全國水環境改善計畫」為政府前瞻基礎建設計畫中的一環，水利署也已規劃未來將會主要使用開源軟體及函式庫，來建置「全國水環境改善計畫」中的水資源物聯網雲端平臺（水資源物聯網感測基礎雲端作業網絡），讓資訊架構秉持開放、開源的精神，資訊架構也能更靈活。而從學生時代便開始接觸開源軟體的何丁武認為，配合國家整體資訊政策，由公部門帶頭使用開源軟體，藉由政府專案導入的方式，讓有意投入開源領域的軟體產業，將公務機關當做試煉場，在適合的環境，有足夠的機會磨練與訓練人才，透過不斷的創新，讓台灣資訊技術能量提升，帶動軟體技術發展，這將成為正向循環，讓台灣不只是成為開源軟體重要一角，更能引領資訊技術發展，改變世界。

---

* 本文同步刊登於：[https://www.ithome.com.tw/pr/116548](https://www.ithome.com.tw/pr/116548)



