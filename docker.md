**虛擬化**

**Docker**

Ø組織介紹

Docker是一個開源專案，誕生於2013年初，最初是dotCloud公司內部的一個業餘專案。它基於Google公司推出的Go語言實作。專案後來加入了Linux基金會，遵從了Apache 2.0協議，原始碼在GitHub上進行維護。基於容器技術，對其進一步的封裝，讓使用者更容易操作、快速建立Container、搭建一個開發環境、部署程式碼進行測試。Docker提供應用程式在獨立的container中執行，透過Docker Engine來進行管理。



Docker自開源後受到廣泛的關注和討論，以至於dotCloud公司後來都改名為Docker Inc。Redhat已經在其RHEL6.5中集中支援Docker；Google也在其PaaS產品中廣泛應用。



Ø軟體介紹

Docker專案的目標是實作輕量級的作業系統虛擬化解決方案。包含了三個主要部份：

uDocker映像檔：Docker映像檔是一個唯讀的環境模板，裡面包含了Container內的所有程式\(包括應用程式、相關函式庫、設定檔\)，用來建立Docker容器。舉例來說，一個網頁的執行環境映像檔內會有ubuntu OS、Apache網站伺服器、MySQL資料庫等。

uDocker容器：容器是根據映像檔建立的實例。映像檔是唯讀的，而容器則是是映像檔的可寫層。容器是一個簡易版的Linux環境應用程式並可在其中運行程式。一個映像檔可以建立多個容器，每個容器都是相互隔離的。

uDocker註冊伺服器：Docker註冊伺服器上有許多倉庫，倉庫內存放許多映像檔供人使用。註冊伺服器分為公開和私有，最大的公開註冊伺服器是Docker Hub，存放了大量的映像檔供使用者下載使用；使用者也可以在local網路上建立一個私有註冊伺服器。



Ø應用

u英國政府的軟體開發流程逐漸擁抱雲端技術及DevOps，並且開始尋找小型供應商，避免與大型IT廠商簽訂長期契約。近日Docker企業版已被英國政府認證，納入政府雲計畫G-Cloud 9中。Docker表示，G-Cloud 9是英國政府所推出的雲端計畫，目的是在公布門推動使用雲端服務。在Docker被納入G-Cloud 9之後，公部門可自行選擇適合的容器解決方案，「免除冗長、競標的採購流程。」

u甲骨文的Oracle資料庫、Oracle Linux、Java以及中介軟體都登上Docker Store後，近日甲骨文自家的中介軟體解決方案Oracle Coherence也登上了Docker Store。而目前甲骨文已經讓Oracle Coherence可在Docker Swarm上執行，在叢集開始執行時，開發者可提前輸入一份紀錄各容器IP位址的清單，「使用者也可以替Docker容器指派一個固定IP。」



資料來源：

[http://www.runpc.com.tw/content/content.aspx?id=109895](http://www.runpc.com.tw/content/content.aspx?id=109895)

[https://philipzheng.gitbooks.io/docker\_practice/content/introduction/what.html](https://philipzheng.gitbooks.io/docker_practice/content/introduction/what.html)

[https://www.ithome.com.tw/news/114818](https://www.ithome.com.tw/news/114818)



