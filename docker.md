# **虛擬化**

## **Docker**

![](/assets/Docker.png)

### 典範案例

* [經濟部中央地質調查所 — 地質騰雲網運用多套開源軟體](/use-case/di-zhi-teng-yun-wang-yun-yong-duo-tao-kai-yuan-ruan-ti.md)

### 組織介紹

Docker 是一個開源專案，誕生於 2013 年初，最初是 dotCloud 公司內部的一個業餘專案。它根據 Google 公司推出的 Go 語言實作。專案後來加入了 Linux 基金會，遵守了 Apache 2.0 協議，原始碼在 GitHub 上進行維護。依據容器技術，對其進一步的封裝，讓使用者更容易操作、快速建立 Container、搭建一個開發環境、部署程式碼進行測試。Docker 提供應用程式在獨立的容器中執行，透過 Docker Engine 來進行管理。

Docker 自開源後受到廣泛的關注和討論，以至於 dotCloud 公司後來都改名為 Docker Inc。Redhat 已經在其 RHEL6.5 中集中支援Docker；Google 也在其 PaaS 產品中廣泛應用。

### 軟體介紹

Docker 專案的目標是實作輕量級的作業系統虛擬化解決方案。包含了三個主要部份：

* Docker 映像檔：Docker 映像檔是一個唯讀的環境模板，裡面包含了 Container 內的所有程式\(包括應用程式、相關函式庫、設定檔\)，用來建立 Docker 容器。舉例來說，一個網頁的執行環境映像檔內會有 ubuntu OS、Apache 網站伺服器、MySQL 資料庫等。
* Docker 容器：容器是根據映像檔建立的實例。映像檔是唯讀的，而容器則是是映像檔的可寫層。容器是一個簡易版的Linux環境應用程式並可在其中運行程式。一個映像檔可以建立多個容器，每個容器都是相互隔離的。
* Docker 註冊伺服器：Docker 註冊伺服器上有許多倉庫，倉庫內存放許多映像檔供人使用。註冊伺服器分為公開和私有，最大的公開註冊伺服器是 Docker Hub，存放了大量的映像檔供使用者下載使用；使用者也可以在 local 網路上建立一個私有註冊伺服器。

### 應用

* 英國政府的軟體開發流程逐漸擁抱雲端技術及 DevOps，並且開始尋找小型供應商，避免與大型 IT 廠商簽訂長期契約。近日Docker 企業版已被英國政府認證，納入政府雲計畫 G-Cloud 9 中。Docker 表示，G-Cloud 9 是英國政府所推出的雲端計畫，目的是在公布門推動使用雲端服務。在 Docker 被納入 G-Cloud 9 之後，公部門可自行選擇適合的容器解決方案，「免除冗長、競標的採購流程。」
* 甲骨文的 Oracle 資料庫、Oracle Linux、Java 以及中介軟體都登上 Docker Store 後，近日甲骨文自家的中介軟體解決方案Oracle Coherence 也登上了 Docker Store。而目前甲骨文已經讓 Oracle Coherence 可在 Docker Swarm 上執行，在叢集開始執行時，開發者可提前輸入一份紀錄各容器 IP 位址的清單，「使用者也可以替 Docker 容器指派一個固定 IP。」

### 資料來源：

* Docker - Build, Ship, and Run Any App, Anywhere [https://www.docker.com/](https://www.docker.com/)
* Docker介紹與入門使用 [http://www.runpc.com.tw/content/content.aspx?id=109895](http://www.runpc.com.tw/content/content.aspx?id=109895)
* 什麼是 Docker [https://philipzheng.gitbooks.io/docker\_practice/content/introduction/what.html](https://philipzheng.gitbooks.io/docker_practice/content/introduction/what.html)
* Container雙周報第36期：Docker企業版納入英國政府雲計畫，公部門可線上採購容器解決方案 [https://www.ithome.com.tw/news/114818](https://www.ithome.com.tw/news/114818)



