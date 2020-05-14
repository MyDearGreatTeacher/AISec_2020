# 1.2 影像處理基本操作
```
!wget https://raw.githubusercontent.com/MyDearGreatTeacher/AISec_2020/master/opencv/data/lena.bmp
```

```
OpenCV之imread,imwrite,imshow

```
```
# -*- coding: utf-8 -*-

import cv2
lena=cv2.imread("lena.bmp")
#lena=cv2.imread("Lenna.jpg")==>error
print(lena)
```

```
type(lena)
```
```
Python 與 OpenCV 基本讀取、顯示與儲存圖片教學
2017/11/24
https://blog.gtwang.org/programming/opencv-basic-image-read-and-write-tutorial/


圖檔格式
OpenCV 的 cv2.imread 在讀取圖片時，可以在第二個參數指定圖片的格式，可用的選項有三種：

cv2.IMREAD_COLOR
此為預設值，這種格式會讀取 RGB 三個 channels 的彩色圖片，而忽略透明度的 channel。
cv2.IMREAD_GRAYSCALE
以灰階的格式來讀取圖片。
cv2.IMREAD_UNCHANGED
讀取圖片中所有的 channels，包含透明度的 channel。
```
```
https://medium.com/@yanweiliu/python%E5%BD%B1%E5%83%8F%E8%BE%A8%E8%AD%98%E7%AD%86%E8%A8%98-%E4%B8%89-open-cv%E6%93%8D%E4%BD%9C%E7%AD%86%E8%A8%98-1eab0b95339c

# 以灰階的方式讀取圖檔
img_gray = cv2.imread('image.jpg', cv2.IMREAD_GRAYSCALE)
#cv2.IMREAD_COLOR     為預設值
#cv2.IMREAD_GRAYSCALE 以灰階的格式來讀取圖片。 
#cv2.IMREAD_UNCHANGED 讀取圖片中所有的 channels，包含透明度的 channel。

```
