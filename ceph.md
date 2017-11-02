# **檔案儲存**

## **Ceph**

![](/assets/1509609660571.jpg)

### 組織介紹

在2004年，Sage Weil開發了一個名叫Ceph的開源項目，並於2006年，基於開源協議開源了Ceph。Weil曾經是「Inktank Storage」公司的創始人。Inktank Storage一直專注於Ceph的研發，直到它被紅帽收購。2012年，Ceph的第一個穩定版本發布了。2014年10月，Ceph的開發團隊發布了Ceph的第七個穩定版本Giant。為了讓Ceph更加成熟與完美，這個項目還在繼續開發中。

### 軟體介紹

它是以RADOS \(Reliable Autonomic Distributed Object Store\)為主要設計方式的分散式儲存平台，因此在水平擴展的能力極為強大。

Ceph以單一架構，同時提供物件、區塊、檔案的儲存，藉由RADOS函式庫中介，程式可直接存取底層叢集，並提供物件儲存閘道、區塊儲存裝置來對應存取，也可搭配元資料伺服器來提供檔案系統服務，而底層則是由多個RADOS節點組成的叢集所構成，可橫向擴充數千個節點，並以此提供PB、甚至EB等級的儲存空間。

* 物件儲存：Ceph的底層是RADO儲存著許許多多的物件，應用程式可以透過LIBRADOS這個API或是透過Ceph提供的RADOSGW\(RADOS Gateway\)網頁介面存取物件。

* 區塊設備：於LIBRADOS之上，RBD \(Distributed Block Device\)提供區塊設備，可以當成系統的一個區塊設備格式化並掛載，也可以提供給QEMU/KVM虛擬機使用。

* 檔案系統：於LIBRADOS之上，CEPH FS提供檔案系統，類似NFS或SAMBA，直接掛載就可以存取。

要使Ceph能夠成為高可靠度、高擴充性的儲存環境，它所採用的RADOS服務是重要基礎。RADOS架構包含了儲存節點和監控器，而其中的儲存節點，又可區分為OSD、檔案系統與硬碟等三大部分。

uMON \(Monitor\)：監控整個cluster的狀態，算是Ceph cluster的中樞，可以有多台來避免單點失效。

uOSD \(Object storage device\)：實際儲存資料，一台主機可以有多個OSD，不建議使用RAID。若發現有其他OSD故障則回報MON。

uMDS \(Metadata server\)：若有使用CEPH FS則必須有此MDS記錄檔案系統Metadata,但目前只支援同時一台Active,因此會造成效能瓶頸。

### 應用

在OpenStack的系統架構下，為了充分支援各式資料儲存應用，而發展了Cinder和Swift套件，分別對應區塊式儲存與物件式儲存，此外，提供運算服務的Nova套件與映像服務的Glance套件，也都需要儲存資料。由於能同時滿足多種儲存環境的需求，採用Ceph的用戶日益增加，尤其是想要運用OpenStack來建構雲環境的服務業者和企業。

包含大型網站、雲服務業者、企業。像是美國財經媒體彭博社，他們以OpenStack建構私有雲IaaS環境：Bloomberg Clustered Private Cloud時，當中搭配了Ceph儲存系統，由250臺以上的運算節點所組成，提供的容量高達PB。

另一個例子是時代華納有線電視公司，他們也是在2014年建置OpenStack的初期，就開始採用Ceph作為區塊式儲存環境，以便搭配OpenStack的Cinder套件來使用，支援虛擬機器的不停機遷移應用，至今他們已經歷4次儲存容量擴展的作業。

### 資料來源：

* Ceph 簡介 [http://godleon.blogspot.tw/2014/10/ceph.html](http://godleon.blogspot.tw/2014/10/ceph.html)
* 一次搞懂Ceph儲存架構與應用形式 [https://www.ithome.com.tw/tech/98860](https://www.ithome.com.tw/tech/98860)
* 理解Ceph：一個開源的分布式存儲平台 [https://read01.com/0z5aGM.html](https://read01.com/0z5aGM.html)
* 超大型儲存應用異軍突起！Ceph有機會翻轉雲服務與企業儲存架構 [https://www.ithome.com.tw/tech/98858](https://www.ithome.com.tw/tech/98858)



