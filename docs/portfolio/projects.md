# 程式設計專案

---

## 醫檢資料 ETL 流程
- **類型**：資料工程（Data Engineering）
- **內容**：將半結構化 JSON 醫檢資料轉換為乾淨、結構化的資料與階層式文字輸出
- **流程**：資料展開 → 清洗與正規化 → 群組與層級重組 → 輸出
- **延伸**：可選擇性整合 LLM，將結構化結果轉為可讀摘要文字
- **技術**：Python、pandas、FastAPI、MongoDB（pymongo）、LLM API（可 mock）
- **GitHub**：https://github.com/okami518/medical_examination_ETL

---

## 波士頓房價預測 (Kaggle 競賽)
- **類型**：回歸問題（Regression）
- **內容**：以 Boston Housing 資料集預測房價中位數（medv），並參與課程 Kaggle 競賽
- **方法**：結合 Ridge Regression、SVR 與 XGBoost，透過加權 voting 進行集成
- **重點**：自行切分 validation set，以 RMSE 作為模型選擇依據
- **技術**：Python、pandas、scikit-learn、xgboost
- **GitHub**：https://github.com/okami518/Boston-Housing-Competition

---

## 公共工程金質獎建築類廠商清單產生器
- **類型**：文件自動化 / 資料處理
- **內容**：解析公共工程金質獎得獎名單 PDF，自動篩選建築類優良營造廠
- **輸出**：產生 `.txt` 清單，支援低碳與綠建築評分作業
- **重點**：降低人工整理名單的時間成本
- **技術**：Python、pdfplumber、tkinter
- **GitHub**：https://github.com/okami518/construction_enterprise_list_generator

---

## stanCode Python Practice Projects
- **類型**：課程專案 / 基礎能力訓練
- **內容**：涵蓋 Python 基礎語法、資料結構、OOP 與簡易資料視覺化
- **實作**：遊戲（Breakout）、資料視覺化、字串與影像處理、小型演算法題
- **目的**：培養程式結構設計與問題拆解能力
- **技術**：Python、campy、tkinter
- **GitHub**：https://github.com/okami518/stanCode_Projects