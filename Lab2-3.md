# Lab 2-3 請加入一台Win11 Professional的Virtual Machine

## A. 簡介一下Windows 11以及安裝後的體驗
> Windows 11是微軟於2021年推出的Windows NT系列作業系統，為Windows 10的後繼者。正式版本於2021年10月5日發行[7][8]，並開放給符合條件的Windows 10裝置透過Windows Update免費升級。[9][10][11] Windows 11對於受到已取消的Windows 10X影響的Windows shell進行主要更改，包括重新設計的開始功能表、工作列上單獨的「小工具」面板取代「動態磚」、從工作列建立以群組能最小化和恢復的編排視窗，以及從Xbox Series X/S繼承的新遊戲技術，例如相容硬體上的Auto HDR和DirectStorage。Internet Explorer被基於Blink排版引擎的Microsoft Edge取代，而Edge的IE模式保留了IE的核心，Microsoft Teams則被整合至Windows shell中。微軟還宣布計劃讓通過Microsoft Store發布的軟體提供更大的靈活性。 與Windows 10相比，微軟提高了硬體需求，且僅支援使用英特爾酷睿第8代或更新的處理器（少數的第7代處理器例外）、AMD Zen+或更新的處理器及高通驍龍850或更新的處理器的裝置。Windows 11專為UEFI安全開機和信賴平台模組（TPM） 2.0支援而構建。此外，Windows 11不再支援32位元x86架構或使用BIOS韌體的系統。Windows 11自發布後收到褒貶不一的評價；關於該操作系統預發行的報導集中在其更嚴格的硬體需求上，討論這些需求是否合法地旨在提高Windows的安全性，還是將使用者追加銷售到更新裝置的策略，以及與這些變化相關的電子垃圾。發行後，Windows 11因其改進的視覺設計、視窗管理和更加注重安全性而獲得正面評價，但因其使用者介面方面的回歸和修改而受到批評。 Source: https://zh.wikipedia.org/wiki/Windows_11

## B. 請自由截取3張有關於Windows 11的安裝過程, 並更新於GitHub.


### 1. 硬體配置

![image](https://user-images.githubusercontent.com/89304181/158962820-8c174ce9-27f2-43d4-adda-1dfcdc755b2c.png)


### 2. 選擇Windows 11 Professional 

![image](https://user-images.githubusercontent.com/89304181/158962985-9d9debcc-0927-496f-9686-d83b114fd32a.png)

### 3. 完成安裝後的登入畫面

A. 用Outlook e-mail帳號設定 (e.g., Grace TA) by HP i7 NB

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/158963063-c3961a76-690c-4ba5-97b0-fc4c1ab3aa95.png" 
      width="50%" height="50%">
    </div>

B. 用Offline Account (e.g., grace2022) by HP i5 NB


<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/158963605-8632d889-69ae-4350-801b-9d0f1573fd77.png" 
      width="50%" height="50%">
    </div>

### 4. 安裝中文環境

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/158963605-8632d889-69ae-4350-801b-9d0f1573fd77.png" 
      width="50%" height="50%">
    </div>
    
<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/158963765-63c6c1eb-2bce-4ad7-ba53-c7e3bb3c309f.png" 
      width="50%" height="50%">
    </div>
    
### 5. 讓Windows 11 VM 與 Windows 10 主機可以相互PING到對方

* Windows 11 VM IP: 192.168.85.152

* Windows 10 主機: 192.168.90.6

![image](https://user-images.githubusercontent.com/89304181/158964137-ff27b56b-edd4-49f0-ae62-c9600c53c1aa.png)


> Note: Windows 11 VM的公用網路Firewall關閉後, 應該就可以相互Ping到對方了. (Windows10主機 vs. Windows 11 VM)

![image](https://user-images.githubusercontent.com/89304181/159145341-060fd87c-cc55-479c-ad43-5662def77dd9.png)
