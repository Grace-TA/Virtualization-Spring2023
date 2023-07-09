# Lab7: Google VM應用 - AI最經典火紅的應用之人臉偵測(Face Detection)實作

## 101 準備工作: 

![image](https://github.com/Grace-TA/Virtualization-Spring2023/assets/89304181/cdff9261-44e0-48c4-8916-f979007369f1)

## Lab 7-1: 虛擬人臉數據取得

讓我們下載2張自選的虛擬人造臉 (VF04.jpg, VF05.jpg), 並且上傳到我們的Google Drive, 並且用以上的指令來顯示出來.

Reference web site: https://thispersondoesnotexist.com/

![image](https://github.com/Grace-TA/Virtualization-Spring2023/assets/89304181/07a9a7b5-c228-4061-b992-b2b4536c1be5)

![image](https://github.com/Grace-TA/Virtualization-Spring2023/assets/89304181/ffc8cd29-5e6f-4b52-96b8-493a9e2cc966)


## Lab 7-2 OpenCV電腦視覺入門

![image](https://github.com/Grace-TA/Virtualization-Spring2023/assets/89304181/086c6e76-a841-4bd8-b757-58e991a51e14)

```python
img = np.zeros((256, 256, 3), np.uint8) #np.zeros建立0矩陣
img.fill(200)
cv2.line(img, (0, 0), (255, 255), (255, 0, 255), 5)
cv2.line(img, (255, 0), (0, 255), (255, 0, 255), 5)

cv2.putText(img, ('Grace, 2023'), (10, 200), cv2.FONT_HERSHEY_SIMPLEX,
    1, (255, 0, 0), 2, cv2.LINE_AA)
# 顯示圖片
cv2_imshow(img)

```

## Lab 7-3 人臉辨識實際應用

### Using Open CV

![image](https://github.com/Grace-TA/Virtualization-Spring2023/assets/89304181/e4073f85-9a93-4d70-8a92-207c979f1b3e)

```python
#316 練習.找一張圖片有10個以上人臉,並偵測人臉數量
image = cv2.imread('face_mask_test3.jpg')
haar = cv2.CascadeClassifier('haarcascade_frontalface_default.xml') #載入分類器
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)#圖片轉灰階
faces = haar.detectMultiScale(gray) #偵測人臉
for (x,y,w,h) in faces:
    cv2.rectangle(image,(x,y),(x+w,y+h),(0,255,0),2) #畫矩形框 可改框的顏色/線條粗細

#文字 cv2.putText(影像, 文字, 座標, 字型, 大小, 顏色, 線條寬度, 線條種類)
cv2.putText(image, ('Grace: Open CV, 2023.07.09'), (10, 50), cv2.FONT_HERSHEY_SIMPLEX,
    1, (0, 0, 255), 2, cv2.LINE_AA)

plt.figure(figsize=(12,10)) #設定顯示尺寸
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB)) #BGR to RGB
print('找到臉的數量:',len(faces))

```

### Using Deep Learning (i.e., AI Model)

![image](https://github.com/Grace-TA/Virtualization-Spring2023/assets/89304181/7ba5fff3-5dce-4511-8788-1c6b7601ca24)

```python
#322 Commented out IPython magic to ensure Python compatibility.

import cv2
import face_recognition
# %matplotlib inline
import matplotlib.pyplot as plt
image = face_recognition.load_image_file('face_mask_test3.jpg') #92
faces = face_recognition.face_locations(image,model='cnn')
print("找到臉的數量=",len(faces))
for (top, right, bottom, left) in faces: #畫矩形框 可改框的顏色/線條粗細
    cv2.rectangle(image, (left, top), (right, bottom), (0, 255, 0), 2)

#文字 cv2.putText(影像, 文字, 座標, 字型, 大小, 顏色, 線條寬度, 線條種類)
cv2.putText(image, ('Grace: Deep Learning, 2023.07.09'), (10, 50), cv2.FONT_HERSHEY_SIMPLEX,
    1, (255, 0, 0), 2, cv2.LINE_AA)

plt.figure(figsize=(12,10))
#plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.imshow(image)

```
