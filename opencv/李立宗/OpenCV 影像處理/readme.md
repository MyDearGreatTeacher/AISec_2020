#  ch1
```
讀取影像  cv2.imread() 來讀取影像,該函數支援各種靜態影像

cv2.imwrite(filename, imgl, params))

namedWindow()

cv2.waitKey()

destroyWindow函數   vs  destroyAIIWindows()
http://www.1zlab.com/wiki/python-opencv-tutorial/opencv-destroy-window/
```
```
https://blog.gtwang.org/programming/opencv-basic-image-read-and-write-tutorial/

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
```
import cv2

lena=cv2.imread("lenacolor.png")
cv2.imshow("demo", lena )

cv2.waitKey()
cv2.destroyWindow("demo")
```
```
import cv2

lena=cv2.imread("lena.bmp")
cv2.imshow("demo1", lena )
cv2.imshow("demo2", lena )

cv2.waitKey()
cv2.destroyAllWindows()
```
