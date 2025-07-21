

# Supermarket Sales Tableau Dashboard  視覺化報告

## 1.每日銷售與 7 日移動平均趨勢圖-折線圖

本圖呈現每日超市銷售金額（藍線）與 7 日移動平均（橘線）的變化趨勢。可清楚觀察：
- 銷售數據每日波動明顯
- 透過移動平均線，可看出月初、月底可能有高峰出現
- 可協助行銷或庫存做高峰預測好觀測掌握短期與長期波動情況

![Daily Sales with 7-day Moving Average](../images/daily_sales_with_moving_avg.png)

## 2.城市總銷售額比較-長條圖

此圖表展示三個城市的總銷售表現：

- **Naypyitaw** 銷售總額略高於其他兩城市，表示有穩定的客源
- **Yangon** 為主要商業中心，銷售表現穩定但非最高
- **Mandalay** 表現中等，可視為潛力市場

此分析可作為區域資源配置的參考，幫助行銷團隊精準投放策略。

![City-wise Sales](../images/city_total_sales.png)

## 3.各城市 × 小時銷售-熱力圖

為了觀察不同城市在一日中各時段的銷售表現，製作了【城市 × 小時】的熱力圖：

X 軸：銷售時段（Hour）

Y 軸：城市（City）

色階深淺：表示該城市在該時段的銷售額（越深表示銷售額越高）

- **Mandalay**：銷售集中在晚上 19:00，建議安排晚間推播活動
- **Naypyitaw**：銷售高峰出現在 13:00 及 19:00
- **Yangon**：上午 11:00 與下午 15:00 為高峰時段

📌 此分析有助於：
- 規劃每個城市最佳行銷發送時段（EDM / 廣告）
- 安排人力資源高峰時間

![CityHour Heatmap](../images/city_hour_heatmap.png)

## 4.商品類別 × 會員狀態：會員 vs 非會員購買偏好分析-堆疊長條圖

分析會員（Member）與非會員（Normal）對不同商品類別的購買偏好

此圖為會員（Member）與非會員（Normal）在各類商品的購買行為堆疊圖：

- X 軸：商品類別（Product line）
- Y 軸：銷售額
- 顏色區分：會員 vs 非會員

**觀察重點**：
- 會員偏好「Food and beverages」
- 非會員對「Fashion accessories」與「Electronic accessories」偏好明顯
→ 可為會員設計專屬品類促銷，並對非會員進行導入轉換設計

![productline_membertype](../images/productline_membertype.png)

## 5.顧客性別 × 商品偏好：百分比堆疊分析

分析性別在不同商品上的購買比例差異

本圖展示男性與女性在不同商品線的購買比例差異：

- X 軸：商品類別
- Y 軸：購買佔比（百分比）
- 顏色區分：男性與女性

**重點觀察**：
- 女性偏好「Fashion accessories」、「Sports and travel」
- 男性偏好「Electronic accessories」與「Food and beverages」
→ 可根據性別進行精準商品推薦與行銷策略設計

![gender_productline](../images/gender_productline.png)

## 後續建議：

可針對高銷售時段推出促銷活動（例如 Mandalay 的晚間時段）。

擴大在會員購買力強的類別中提供更多折扣方案。

根據性別偏好優化商品推薦與宣傳策略。

## [🔗 查看完整 Tableau Dashboard](https://public.tableau.com/app/profile/你的網址)
