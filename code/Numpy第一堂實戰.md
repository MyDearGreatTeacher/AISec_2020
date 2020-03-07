# Numpy實戰
```

```
# 確認Google Colab上的套件使用版本
```
import pandas as pd
print("pandas version: %s" % pd.__version__)

import matplotlib
print("matplotlib version: %s" % matplotlib.__version__)

import numpy as np
print("numpy version: %s" % np.__version__)

import sklearn
print("scikit-learn version: %s" % sklearn.__version__)

import tensorflow as tf
print("tensorflow version: %s" % tf.__version__)

import torch
print("PyTorch version: %s" %torch.__version__)
print("2020年3月PyTorch version最新版本 是1.4 請參閱https://pytorch.org/")
```
## NUMPY

### NUMPY ndarray(N-Dimensional Arrays)
### NUMPY ndarray(N-Dimensional Arrays)重要屬性
```
shape
dimension
```
```
import numpy as np
ar2=np.array([[0,3,5],[2,8,7]])
# ar2.shape
ar2.ndim
```
### ndarray資料型態(dtype)與型態轉換(astype)
```
ar=np.array([2,4,6,8]); 
ar.dtype
```
### 下列程式執行後的結果為何?
```
f_ar = np.array([13,-3,8.88])
f_ar

intf_ar=f_ar.astype(int)
intf_ar
```
## 建立array(陣列)的方式與實作
```
1.使用Python內建的array()建立陣列
2.使用numpy提供的創建函數建立陣列
3.直接生成使用genfromtxt()方法建立陣列
```

### 下列程式執行後的結果為何?
```
import numpy as np
np.array([range(i, i + 3) for i in [2, 4, 6]])
```
