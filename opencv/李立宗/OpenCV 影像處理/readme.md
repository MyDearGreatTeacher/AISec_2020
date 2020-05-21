#  ch1
```
讀取影像  cv2.imread() 來讀取影像,該函數支援各種靜態影像

```
```
# -*- coding: utf-8 -*-

import cv2
lena=cv2.imread("lena.bmp")
print(lena)
type(lena)
lena.shape
```
```
import cv2

lena=cv2.imread("lena.bmp")
cv2.namedWindow("lesson")

cv2.imshow("lesson", lena )
```
```
import cv2

lena=cv2.imread("lena.bmp")
cv2.imshow("demo", lena )

key=cv2.waitKey()
if key==ord('a'):
    cv2.imshow("PressA",lena)
elif key==ord('b'):
    cv2.imshow("PressB",lena)
```
```
import cv2
lena=cv2.imread("lena.bmp")
cv2.imshow("demo", lena )
key=cv2.waitKey()
if key!=-1:
    print("觸發按鍵")
```
