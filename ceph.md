# **檔案儲存**

## **Ceph**

![](/assets/1509609660571.jpg)![](/assets/Ceph.png)

### 典範案例

* [經濟部水利署 — 水利雲受推崇開源軟體扮演幕後功臣](/shui-li-yun-shou-tui-chong-kai-yuan-ruan-ti-ban-yan-mu-hou-gong-chen.md)

### 組織介紹

在 2004 年，Sage Weil 開發了一個名叫 Ceph 的開源項目，並於 2006 年，根據開源協議開源了 Ceph。Weil 曾經是「Inktank Storage」公司的創始人。Inktank Storage 一直專注於 Ceph 的研發，直到它被紅帽收購。2012 年，Ceph 的第一個穩定版本發布了。2014 年 10 月，Ceph 的開發團隊發布了 Ceph 的第七個穩定版本 Giant。為了讓 Ceph 更加成熟與完美，這個項目還在繼續開發中。

### 軟體介紹

它是以 RADOS \(Reliable Autonomic Distributed Object Store\) 為主要設計方式的分散式儲存平台，因此在水平擴展的能力極為強大。Ceph 以單一架構，同時提供物件、區塊、檔案的儲存，藉由 RADOS 函式庫中介，程式可直接存取底層叢集，並提供物件儲存閘道、區塊儲存裝置來對應存取，也可搭配原資料伺服器來提供檔案系統服務，而底層則是由多個 RADOS 節點組成的叢集所構成，可橫向擴充數千個節點，並以此提供 PB、甚至 EB 等級的儲存空間。

* 物件儲存：Ceph 的底層是 RADO 儲存著許多的物件，應用程式可以透過 LIBRADOS 這個 API 或是透過 Ceph 提供的RADOSGW \(RADOS Gateway\) 網頁介面存取物件。

* 區塊設備：於 LIBRADOS 之上，RBD \(Distributed Block Device\) 提供區塊設備，可以當成系統的一個區塊設備格式化並掛載，也可以提供給 QEMU/KVM 虛擬機使用。

* 檔案系統：於 LIBRADOS 之上，Ceph FS 提供檔案系統，類似 NFS 或 SAMBA，直接掛載就可以存取。

要使 Ceph 能夠成為高可靠度、高擴充性的儲存環境，它所採用的 RADOS 服務是重要基礎。RADOS 架構包含了儲存節點和監控器，而其中的儲存節點，又可區分為 OSD、檔案系統與硬碟等三大部分。

* MON \(Monitor\)：監控整個 cluster 的狀態，算是 Ceph cluster 的中樞，可以有多台來避免單點失效。
* OSD \(Object storage device\)：實際儲存資料，一台主機可以有多個 OSD，不建議使用 RAID。若發現有其他 OSD 故障則回報MON。
* MDS \(Metadata server\)：若有使用 Ceph FS 則必須有此 MDS 記錄檔案系統 Metadata，但目前只支援同時一台 Active，因此會造成效能瓶頸。

### 應用

在 OpenStack 的系統架構下，為了充分支援各式資料儲存應用，而發展了 Cinder 和 Swift 套件，分別對應區塊式儲存與物件式儲存，此外，提供運算服務的 Nova 套件與映像服務的Glance套件，也都需要儲存資料。由於能同時滿足多種儲存環境的需求，採用Ceph 的用戶日益增加，尤其是想要運用 OpenStack 來建構雲環境的服務業者和企業。

包含大型網站、雲服務業者、企業。像是美國財經媒體彭博社，他們以 OpenStack 建構私有雲 IaaS 環境：Bloomberg Clustered Private Cloud 時，當中搭配了 Ceph 儲存系統，由 250 臺以上的運算節點所組成，提供的容量高達PB。

另一個例子是時代華納有線電視公司，他們也是在 2014 年建置 OpenStack 的初期，就開始採用 Ceph 作為區塊式儲存環境，以便搭配 OpenStack 的 Cinder 套件來使用，支援虛擬機器的不停機遷移應用，至今他們已經歷 4 次儲存容量擴展的作業。

### 資料來源：

* Ceph Incremental Snapshots with RBD [http://ceph.com/geen-categorie/incremental-snapshots-with-rbd/](http://ceph.com/geen-categorie/incremental-snapshots-with-rbd/)
* Ceph 簡介 [http://godleon.blogspot.tw/2014/10/ceph.html](http://godleon.blogspot.tw/2014/10/ceph.html)
* 一次搞懂Ceph儲存架構與應用形式 [https://www.ithome.com.tw/tech/98860](https://www.ithome.com.tw/tech/98860)
* 理解Ceph：一個開源的分布式存儲平台 [https://read01.com/0z5aGM.html](https://read01.com/0z5aGM.html)
* 超大型儲存應用異軍突起！Ceph有機會翻轉雲服務與企業儲存架構 [https://www.ithome.com.tw/tech/98858](https://www.ithome.com.tw/tech/98858)



