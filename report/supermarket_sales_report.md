#  Supermarket Sales 分析報告

##  資料來源
- 使用 [Supermarket Sales Dataset](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales)
- 共包含銷售日期、商品種類、客戶資訊、付款方式等多維度欄位

---

##  分析目標

1. 探索資料中的城市、性別、商品線等對銷售的影響
2. 建立預測模型，判斷顧客是否為高價值會員（HighValueMember）

---

##  特徵工程與變數轉換

- 日期轉換為 datetime 格式，擷取 Hour、Day
- 對類別欄位進行 one-hot encoding
- 建立衍生欄位：
  - `HighValueMember`：根據 Sales銷售金額 是否大於中位數標記高價值顧客

---

##  特徵選擇方法比較

| 方法          | 機制說明                                 | 結果                             |
|---------------|------------------------------------------|----------------------------------|
| SelectKBest   | 根據 F-score 排序，選出前 k 個變數        | `Quantity`, `Unit price`, `Gender_Male` |
| RFECV         | 用交叉驗證反覆遞迴移除變數                | 選出 13 個變數                  |
| Logistic coef | 根據邏輯回歸的係數大小                    | 前三名為 `Quantity`, `Unit price`, `Gender_Male` |

---

##  建模：Logistic Regression 模型

###  精簡模型結果
- Accuracy：0.78
- Precision（高價值顧客）：0.62
- Recall：0.50
- F1-score：0.55

---
