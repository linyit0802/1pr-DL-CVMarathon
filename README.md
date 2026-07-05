# 1pr-DL-CVMarathon

> **狀態：已完結的歷史學習專案（archived）**
> 2020 年（commit 期間 2020-09 ～ 2020-12）完成的百日馬拉松線上課程作業集，內容為 Cupoy 風格的機器學習／深度學習課綱（Day 1 從 MSE/MAE 起步，Day 100 以 Transfer Learning 收尾）。純 Jupyter Notebook 作業存檔，無程式庫、無部署，不再更新。

## 內容地圖

共 93 本 notebook，依主題分五段（天數有缺號，屬正常——部分作業未上傳或課程本身跳號）：

| 階段 | 範圍 | 主題 | 檔名樣式 |
|------|------|------|----------|
| 機器學習基礎與特徵工程 | Day 001–050 | MSE/MAE、EDA、特徵處理、相關係數/L1 特徵篩選、Kaggle 鐵達尼、Lasso/Ridge、超參數搜尋、Blending、Stacking | `Day_0XX_HW.ipynb` |
| 非監督式學習 | Day 054–063 | K-Means（輪廓分析）、階層式分群、PCA、t-SNE | `Day_0XX_HW.ipynb` |
| 深度學習入門 | Day 064–075 | NN Playground 練習、Keras 入門（Dataset / Sequential / Functional API）、MNIST MLP、損失函數、Activation、Gradient Descent、Back Propagation | Day 66 起改為 `DayXX-主題_HW.ipynb` |
| 深度學習訓練技巧 | Day 076–091 | Optimizer、Learning Curve、EarlyStopping、自訂 Callback、CIFAR-10、色彩直方圖（cv2）、傳統 CV 特徵分類 | `Day0XX_HW.ipynb` |
| CNN 與遷移學習 | Day 093–105 | CNN 架構、卷積/池化/Padding、Transfer Learning（ResNet）、ConvNetJS、VGG16 預訓練模型 | `DayXX-主題_HW.ipynb` |

缺號：Day 045、048、051–053、067（底線版）、087、092、096–099、101–103。

檔名有兩套並存的命名慣例（`Day_001_HW` 底線補零式與 `Day66-Keras_Introduction_HW` 連字號主題式），為當年課程原始檔名，保留原樣。

## 技術棧（依 notebook 內容）

- Python / Jupyter Notebook
- NumPy、Pandas、Matplotlib
- scikit-learn
- Keras（TensorFlow 1.x/2.x 時代的 `from keras...` 舊式 import）
- OpenCV（cv2，僅少數 CV 作業）

⚠️ 這些 notebook 以 2020 年的套件版本撰寫（如 `keras.utils.multi_gpu_model`，新版 Keras 已移除）。若要重跑，需自建舊版環境，直接在現代環境執行大多會失敗——但作為存檔專案，通常沒有重跑的必要。

## 專案結構

```
1pr-DL-CVMarathon/
├── Day_001_HW.ipynb ~ Day_066_HW.ipynb   # ML 基礎、特徵工程、非監督式學習
├── Day66-*.ipynb ~ Day75-*.ipynb          # Keras 入門
├── Day076_HW.ipynb ~ Day091_*.ipynb       # DL 訓練技巧、CV 入門
├── Day93-*.ipynb ~ Day105-*.ipynb         # CNN 與遷移學習
├── .gitignore
├── CLAUDE.md
└── README.md
```
