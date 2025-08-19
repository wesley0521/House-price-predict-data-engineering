# House-price-predict-data-engineering
本專案使用 Kaggle House Prices: Advanced Regression Techniques 數據集，建立一個房價預測系統，涵蓋 數據清理、特徵工程、模型訓練、模型解釋，並使用 XGBoost 與 Stacking Ensemble 提升準確率。

此專案展示了端到端的 Data Engineering 與 Machine Learning Workflow，可應用於房價預測、金融風險建模、甚至醫療數據分析。

🔑 功能特色

數據清理：處理缺失值、刪除高缺失欄位、標準化與編碼。

特徵工程：

建立新特徵 (e.g., TotalBaths, KitchenScore)

PCA 主成分分析

高相關特徵刪除以避免多重共線性

模型訓練與調參：

使用 XGBoost，透過 GridSearchCV 進行超參數調優

模型評估指標：RMSE、MAE

模型解釋：

使用 SHAP (Shapley Values) 解釋模型預測邏輯

瞭解哪些特徵對房價影響最大

模型融合：

使用 Stacking Regressor (XGBoost + RandomForest + Linear Regression) 進一步提升泛化能力

提交結果：生成符合 Kaggle 格式的 submission.csv

⚙️ 使用方法

下載 Kaggle 資料集：
House Prices Dataset

將 train.csv 與 test.csv 放入專案資料夾

執行 Notebook：

jupyter notebook House_price_predict_data_engineering.ipynb


輸出結果會自動生成 submission.csv

📊 成果展示

最佳 XGBoost 模型：

RMSE ≈ 0.118

MAE ≈ 14,792

SHAP 模型解釋：

OverallQual, GrLivArea, YearBuilt 等特徵對房價影響最大

Stacking Ensemble：比單一模型表現更穩定
<img width="790" height="940" alt="image" src="https://github.com/user-attachments/assets/c15e5a2c-f6a8-407f-b421-a18e8d0ed09b" />


🛠 技術棧

Python

數據處理：Pandas, NumPy, Scikit-learn

模型：XGBoost, RandomForest, Linear Regression, Stacking Regressor

可視化：Matplotlib, Seaborn, SHAP

降維：PCA

📌 專案價值

此專案展示了：

端到端數據工程能力（缺失值處理、特徵工程、降維、多重共線性處理）。

AI 模型訓練與部署能力（超參數調優、模型融合）。

可解釋性 AI 能力（SHAP，對醫療/金融應用至關重要）。
