#
```
OpenCV + TensorFlow 深度學習與電腦視覺實戰
出版商:清華大學
出版日期:2019-02-01
```
```
第1章　電腦視覺與深度學習
1.1　電腦視覺與深度學習的關係
1.2　電腦視覺學習的基礎與研究方向


第2章　Python的安裝與使用
2.1　Python基本安裝和用法
2.2　TensorFlow類庫的下載與安裝（基於CPU模式）
2.3　TensorFlow類庫的下載與安裝（基於GPU模式）
2.4　OpenCV類庫的下載與安裝
2.5　Python常用類庫中的threading


第3章　Python資料處理及視覺化
3.1　從小例子起步——NumPy的初步使用
3.2　圖形化資料處理——Matplotlib包的使用
3.3　深度學習理論方法——相似度計算
3.4　資料的統計學視覺化展示
3.5　Python資料分析與視覺化實戰——某地降水的關係處理


第4章　深度學習的理論基礎——機器學習
4.1　機器學習基本分類
4.2　機器學習基本演算法
4.3　演算法的理論基礎
4.4　回歸演算法
4.5　機器學習的其他演算法——決策樹


第5章　電腦視覺處理庫OpenCV
5.1　認識OpenCV
5.2　OpenCV基本的圖片讀取
5.3　OpenCV的卷積核處理


第6章　OpenCV影像處理實戰
6.1　圖片的自由縮放以及邊緣裁剪
6.2　使用OpenCV擴大圖像資料庫


第7章　Let's play TensorFlow
7.1　TensorFlow遊樂場
7.2　Hello TensorFlow

第8章　Hello TensorFlow，從0到1
8.1　TensorFlow的安裝
8.2　TensorFlow常量、變數和資料類型
8.3　TensorFlow矩陣計算
8.4　Hello TensorFlow


第9章　TensorFlow重要演算法基礎
9.1　BP神經網路簡介
9.2　BP神經網路兩個基礎演算法詳解
9.3　TensorFlow實戰——房屋價格的計算
9.4　回饋神經網路反向傳播演算法介紹


第10章　TensorFlow資料的生成與讀取
10.1　TensorFlow的佇列
10.2　CSV文件的創建與讀取
10.3　TensorFlow文件的創建與讀取


第11章　卷積神經網路的原理
11.1　卷積運算基本概念
11.2　卷積神經網路的結構詳解
11.3　TensorFlow實現LeNet實例


第12章　卷積神經網路公式的推導與應用
12.1　回饋神經網路演算法
12.2　使用卷積神經網路分辨CIFAR-10資料集


第13章　貓狗大戰——實戰AlexNet圖像識別
13.1　AlexNet簡介
13.2　實戰貓狗大戰——AlexNet模型


```
# Python資料處理及視覺化
```
import numpy as np
data = np.mat([[1,200,105,3,False],[2,165,80,2,False],
              [3,184.5,120,2,False],[4,116,70.8,1,False],[5,270,150,4,True]])
row = 0
for line in data:
    row += 1
print( row	)
print( data.size	)
```
```


```

# TensorFlow資料的生成與讀取
```
import tensorflow as tf

with tf.Session() as sess:
    q = tf.FIFOQueue(3, "float")
    init = q.enqueue_many(([0.1, 0.2, 0.3],))
    init2 = q.dequeue()
    init3 = q.enqueue(1.)

    sess.run(init)
    sess.run(init2)
    sess.run(init3)

    quelen = sess.run(q.size())
    for i in range(quelen):
        print(sess.run(q.dequeue()))
```
