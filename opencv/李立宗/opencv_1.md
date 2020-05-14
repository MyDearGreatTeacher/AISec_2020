# 1.2 影像處理基本操作
```
!wget https://raw.githubusercontent.com/MyDearGreatTeacher/AISec_2020/master/opencv/data/lena.bmp
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
```
