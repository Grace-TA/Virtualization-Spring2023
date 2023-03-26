# Lab 2-4 什麼是Google Colab? 該如何使用?

## A. What Is Google Colab?

Google Colab 是一個基於雲端的編程環境，讓您可以在線上撰寫、運行、儲存和分享程式碼。Colab 可以支援多種程式語言，特別是 Python。它使用 Jupyter Notebook 作為基礎，允許用戶在網頁瀏覽器中編輯和運行代碼。

Colab 提供了一個簡單、直觀的使用者介面，讓開發者能夠快速開始編程，並進行各種數據分析和機器學習任務。此外，它還免費提供了有限的 GPU 和 TPU 資源，使開發者能夠在高性能硬體上訓練模型。

這個工具非常適合學生、教師、研究人員和開發者，它能夠提高協作效率，讓您與他人共享程式碼、數據和結果。Google Colab 已成為許多人學習和開發機器學習和數據科學項目的理想選擇。

## B. Virtual Machine vs. Google Colab ?

Google Colab 是一個基於雲端的編程環境，它運行在一個虛擬機器（Virtual Machine, 簡稱 VM）上。虛擬機器是一種模擬計算機硬體系統的軟體，它可以在實體硬體之上運行多個獨立的操作系統和應用程序。在這種情況下，Google Colab 就是運行在 Google Cloud Platform 的虛擬機器上的一個應用。

當您在 Google Colab 上創建一個新的 Notebook 時，Google 會為您分配一個虛擬機器。這個虛擬機器具有一定的計算資源（例如 CPU、RAM 和 GPU/TPU），用於執行您的代碼和計算。您可以在這個虛擬機器上安裝額外的軟體和函式庫，但需要注意，虛擬機器在一段時間後會自動斷開，並在您重新連接時重置。

所以，簡單來說，Google Colab 是一個在虛擬機器上運行的雲端編程環境。您可以利用 Google 提供的虛擬機器資源來執行代碼、訓練機器學習模型和分析數據。虛擬機器使得 Google Colab 能夠在網絡瀏覽器中提供一個快速、靈活且易於使用的編程環境。

## C. 一起來建立本課程的第一個雲端VM (Cloud-based Virtual Machine)

### C1. 如何確認Ubuntu版本?
![image](https://user-images.githubusercontent.com/55008636/226156685-9fdddbaf-ff0f-406e-8026-b899c19f5c03.png)

### C2. 如何確認Google VM的CPU, RAM, HD?
![image](https://user-images.githubusercontent.com/55008636/226156704-da274016-6feb-45df-97c6-2cfdf15a2fcd.png)

### C3. 如何確認GPU Resources in Google VM?
![image](https://user-images.githubusercontent.com/55008636/226156710-766671ac-4a80-4a88-8282-8a3957314666.png)

NVIDIA -  has paired 16 GB GDDR6 memory with the Tesla T4?


### C4. 如何由Notebook模式進入終端機模式(Terminal Mode)?
![image](https://user-images.githubusercontent.com/55008636/226156716-a9ca7407-cfd1-4ef4-a1af-9ddfd7564613.png)
