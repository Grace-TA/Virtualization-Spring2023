# Lab9: Ubuntu VM -  作業系統層虛擬化的Docker

<a name="000"/>

## 目錄(Table of Contents)

[Lab 9-1 What Is Docker? 請您介紹一下什麼是Docker?](#111)

[Lab 9-2 How To Install Docker on Ubuntu?](#222)

[Lab 9-3 什麼是Docker 映像檔（image）? 容器（container）?倉庫（repository）? Docker初體驗](#333)

[Lab 9-4 進入Docker Image的世界: Ubuntu, and Install nano and python3](#444)

[Lab 9-5 進入Docker Image的世界: Python3](#555)

[Lab 9-6 最後, 來試試建立自己的Docker Image. Let’s go!!](#666)

[return to content](#000) 
---
<a name="111"/>

## Lab 9-1 What Is Docker? 請您介紹一下什麼是Docker, 您會如何簡要的介紹? 請您找一張您認為最適合的圖與說明

> 在同一台伺服器上的容器實體共享同一個系統核心，因此在運行上不會存在實體與主機操作系統爭奪RAM的問題發生，從而能夠保證實體的效能。

![image](https://user-images.githubusercontent.com/89304181/178129234-02b77097-283d-46fa-9595-026d8926900e.png)

[return to content](#000) 
---
<a name="222"/>

## Lab 9-2 How To Install Docker on Ubuntu?

### A. Run Docker Image (i.e., hello-world)

![image](https://user-images.githubusercontent.com/89304181/178129300-ee1fe766-5d6b-492c-bddf-d558f9f60344.png)

### B. 在沒有 sudo 的情況下運行 Docker 命令

![image](https://user-images.githubusercontent.com/89304181/178129420-d09042b3-2b82-4773-b528-a0600663e320.png)

### C. 執行多次docker run之後的結果
 
![image](https://user-images.githubusercontent.com/89304181/178129425-4200ccdd-1b63-4e9a-b23c-6f67a0512b07.png)

[return to content](#000) 
---
<a name="333"/>

## Lab 9-3 什麼是Docker 映像檔（image）? 容器（container）?倉庫（repository）? Docker初體驗

### A. 如何查詢目前全部使用的docker image?

![image](https://user-images.githubusercontent.com/89304181/178131057-ba0cfe1e-4729-4cb9-8e83-7b29533d6b69.png)

### B. 和VM比較一下, Docker到底有多"省"? 如何得知”使用中”的container & dock image的Size (Virtual XX)?

![image](https://user-images.githubusercontent.com/89304181/178131061-b8905cdf-aa26-40e7-84c0-ada0aecdf9d2.png)

### C. 如何刪除docker image?

![image](https://user-images.githubusercontent.com/89304181/178131064-febcc5d9-c0f2-4df3-a617-54cdb758cfe4.png)

### D. 如何刪除多個docker image?

![image](https://user-images.githubusercontent.com/89304181/178131066-bd80c374-4c30-4dd6-8939-e89a31e682da.png)

[return to content](#000) 
---
<a name="444"/>

## Lab 9-4 進入Docker Image的世界: Ubuntu, and Install nano and python3

### 1. Shell Programming的Table 9X9

<img width="686" alt="image" src="https://user-images.githubusercontent.com/89304181/178130897-dc0479de-2c50-421a-b8e7-a4d9a0514932.png">

### 2. 對齊的九九乘法表Python程式

<img width="692" alt="image" src="https://user-images.githubusercontent.com/89304181/178130905-fabd40e3-9f2e-4018-9623-672d071615ff.png">

[return to content](#000) 
---
<a name="555"/>

## Lab 9-5 進入Docker Image的世界: Python3

<img width="698" alt="image" src="https://user-images.githubusercontent.com/89304181/178130924-df774ba8-5013-4270-9835-46873346f87b.png">

[return to content](#000) 
---
<a name="666"/>

## Lab 9-6 最後, 來試試建立自己的Docker Image. Let’s go!!

````
# 1. docker commit :从容器创建一个新的镜像
## https://www.runoob.com/docker/docker-commit-command.html

## 1.1 確認由python image file所生成的container ID (e.g., bec73142fed7)

ta@ubuntu:~$ docker ps -a

## 1.2 用我們有table99.py的Container, 建立一個新的Dokcer Image作為後續開發或測試的基礎)

ta@ubuntu:~$ docker commit bec73142fed7 py99

## 1.3 確認一下, 是否有看到py99?

# 2. 試用一下py99 docker image, 看看效果如何?

````

<img width="703" alt="image" src="https://user-images.githubusercontent.com/89304181/178130865-12edf6ac-1bf0-43e8-8962-15269392d7fb.png">

[return to content](#000) 



