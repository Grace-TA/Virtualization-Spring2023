# Lab 2-4 [參考] 請加入一台Android的Virtual Machine

## 什麼是Android? (Source: wiki)
> Android（讀音：英：['ændrɔɪd]，美：[ˈænˌdrɔɪd]），中文使用者多以非官方名稱「安卓」稱之，[[註 1]](https://zh.wikipedia.org/wiki/Android#cite_note-14)是一個基於[Linux核心](https://zh.wikipedia.org/wiki/Linux%E6%A0%B8%E5%BF%83)與其他[開源軟體](https://zh.wikipedia.org/wiki/%E5%BC%80%E6%BA%90%E8%BD%AF%E4%BB%B6)的[開放原始碼](https://zh.wikipedia.org/wiki/%E9%96%8B%E6%94%BE%E5%8E%9F%E5%A7%8B%E7%A2%BC)的[行動作業系統](https://zh.wikipedia.org/wiki/%E8%A1%8C%E5%8B%95%E4%BD%9C%E6%A5%AD%E7%B3%BB%E7%B5%B1)，由[Google](https://zh.wikipedia.org/wiki/Google)成立的[開放手機聯盟](https://zh.wikipedia.org/wiki/%E9%96%8B%E6%94%BE%E6%89%8B%E6%A9%9F%E8%81%AF%E7%9B%9F)持續領導與開發。**
Android Inc.**於2003年10月**由[安迪·魯賓](https://zh.wikipedia.org/wiki/%E5%AE%89%E8%BF%AA%C2%B7%E9%B2%81%E5%AE%BE)、[利奇·米納爾](https://zh.wikipedia.org/wiki/%E5%88%A9%E5%A5%87%C2%B7%E7%B1%B3%E7%B4%8D%E7%88%BE)、尼克·席爾斯、克里斯·懷特在[加州](https://zh.wikipedia.org/wiki/%E5%8A%A0%E5%B7%9E)[帕羅奧圖](https://zh.wikipedia.org/wiki/%E5%B8%95%E7%BE%85%E5%A5%A7%E5%9C%96)建立。Android最初由[安迪·魯賓](https://zh.wikipedia.org/wiki/%E5%AE%89%E8%BF%AA%C2%B7%E9%B2%81%E5%AE%BE)等人開發製作[[14]](https://zh.wikipedia.org/wiki/Android#cite_note-15)，最初開發這個系統的早期方向是建立一個[數位相機](https://zh.wikipedia.org/wiki/%E6%95%B8%E4%BD%8D%E7%9B%B8%E6%A9%9F)的先進作業系統，但是後來發現相機市場規模不夠大，加上智慧型手機發展趨勢快速成長，於是Android成為一款面向智慧型手機的作業系統。**於2005年7月11日**Android Inc.被[美國](https://zh.wikipedia.org/wiki/%E7%BE%8E%E5%9C%8B)科技企業Google收購[[15]](https://zh.wikipedia.org/wiki/Android#cite_note-gba-16)[[16]](https://zh.wikipedia.org/wiki/Android#cite_note-hh-17)。

## 安裝方式: [Ref](https://blog.csdn.net/qq_29667985/article/details/106299924)

### 1: 使用vmware虚拟磁盘文件（.vmdk文件）
> 我們為 VMware Player/Plus/Workstation 提供開源 (Linux/Unix) 虛擬機 (VMDK)，我們為您安裝並製作可隨時使用的 VMware 映像。從這裡您可以下載 VMDK 映像並將其附加到您的 VMware 並使用它。
> 我們提供了 32 位和 64 位架構的圖像，您可以免費下載這兩種架構。目前我們計劃為您提供 30 多個 Linux/Unix 發行版. 如果我們從列表中缺少任何流行的發行版，您也可以向我們發送建議。
> 您可以查看有關 VMDK 映像憑據（用戶名和密碼）的常見問題解答。在這裡，您可以按照指南如何將 VMDK 映像附加/配置到 VMware。我們不會在操作系統中安裝“VMware Tools”或添加任何類型的東西，請閱讀我們的隱私政策。
> VMware player是和VirtualBox一樣的虛擬化產品。它由 VMware 公司免費供個人使用。 VMware Player 可以運行現有的虛擬設備並創建自己的虛擬機（需要安裝操作系統才能正常運行）。

https://www.osboxes.org/vmware-images/

### 2: 使用光盘镜像文件安装（.iso文件）

> 這是一個將 Android Open Source Project 移植到 x86 平台的項目，以前稱為“patch hosting for android x86 support”。 
> 最初的計劃是為開源社區的 android x86 支持託管不同的補丁。 

https://www.android-x86.org/

## 過程與結果 (login by TA Account: ta2021.vnu@gmail.com)

### 我的新Android的VM #1 (i.e., Android9)

<img width="509" alt="image" src="https://user-images.githubusercontent.com/89304181/160241023-d42d0e27-3cff-4dcc-adb6-3a2bbf9f834e.png">

### Play Store

![image](https://user-images.githubusercontent.com/89304181/160241044-a43eead9-8775-4672-b6f0-8d2488e94588.png)

### Check Network & Communication

![image](https://user-images.githubusercontent.com/89304181/160243771-43901134-8802-4074-83e9-c8c0f8748647.png)


### 我的新Android的VM #2 (i.e., [LineageOS](https://zh.wikipedia.org/wiki/LineageOS))
LineageOS（也稱Lineage OS、Lineage OS Android Distribution）是一個面向智慧型手機和平板電腦的自由、免費、開放原始碼的Android系統分支。它是深受歡迎的客製化ROM CyanogenMod的繼任者。它在2016年12月Cyanogen公司突然宣布停止開發並關閉專案基礎設施後復刻而生

<img width="335" alt="image" src="https://user-images.githubusercontent.com/89304181/160243429-088b2e6d-1ceb-488c-b3f3-2e1c7e5a5c63.png">

<img width="575" alt="image" src="https://user-images.githubusercontent.com/89304181/160243635-c449b80b-e2e4-4d77-85d9-46768d030cbf.png">



