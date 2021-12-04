# AOI-of-automatic-product-inspection-system
背景介紹:
建立一套自動化檢測產品設備，主控電腦端接收測試硬體(樹莓派)的螢幕資訊，藉由讀取螢幕資訊對測試硬體及測試機構發出執行命令，以達到無需人員作業即可完成產品檢測。
![Uploading image.png…]()


image

預計完成目標:
以卷積神經網絡(Convolutional Neural Network)學習分辨OK及NG品。 運用Transfer Learning(遷移式學習)，將他人訓練好的(pre-trained model)參數複製過來，當作我們模型參數， 使用的模型: VGG16，VGG 是英國牛津大學 Visual Geometry Group 的縮寫，主要貢獻是使用更多的隱藏層，大量的圖片訓練，提高準確率至90%。

資料集:
Train Data : 360

使用環境:
Python 3.8

TensorFlow 2.3.1

訓練和測試結果
最佳模型訓練準確度100%

image

ROC曲線 (Receiver operating characteristic curve) & AUC (Area Under Curve)

ROC曲線會以對角線為基準，曲線下的面積(AUC)來判別ROC曲線的鑑別力，AUC數值的範圍從0到1，數值愈大，代表模型的鑑別力越好。

image

實際測試結果(產品分類編號['走紗': 0, '油汙': 1, 'OK': 2]

image

使用Streamlit App展示成果
image

Streamlit 是一個開源Python函式庫，可以快速製作Data App。

實作影片(以下圖片為Youtube影片連結)

APP操作方法:

1.開啟資料夾選取想要測試的影像

2.APP執行影像辨識

3.顯示辨識結果 IMAGE ALT TEXT HERE
