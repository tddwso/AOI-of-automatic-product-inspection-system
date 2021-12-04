# AOI-of-automatic-product-inspection-system

預計完成目標:
建立一套自動化檢測產品設備，主控電腦端接收測試硬體(樹莓派)的螢幕資訊，藉由讀取螢幕資訊對測試硬體及測試機構發出執行命令，以達到無需人員作業即可完成產品檢測。
![image](https://github.com/tddwso/AOI-of-automatic-product-inspection-system/blob/main/%E6%9E%B6%E6%A7%8B%E5%9C%96.png)

使用環境:
Visual Studio 2019

樹莓派4 

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
