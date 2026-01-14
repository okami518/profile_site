# 都市分析專案

---

## 台灣空氣品質空間插值分析（IDW）
- **描述**：本專題以台灣空氣品質監測站之每日空氣品質指標（AQI）資料為基礎，透過地理資訊系統（GIS）進行空間分析，呈現空氣品質在台灣地區的連續分布情形。
首先將監測站位置資料與 AQI 屬性資料進行欄位連結（Attribute Join），再將資料統一轉換至 TWD97 投影座標系（EPSG:3826），以確保距離計算的正確性。
接著採用反距離加權法（Inverse Distance Weighting, IDW）進行空間插值，產生連續的 AQI 分布 Raster，最後依空氣品質管理區範圍進行裁切（Raster Masking），使分析結果聚焦於具實際管理意義的區域。
- **流程**: 
1. 匯入空氣品質監測站位置資料 (vector)
2. 依測站名稱將每日 AQI 資料與測站位置進行屬性連結
3. 使用 IDW 方法進行空氣品質空間插值，產生連續分布 Raster
4. 依空氣品質管理區範圍裁切插值結果，完成分析圖層
- **工具**：QGIS
- **圖資來源**：https://data.moenv.gov.tw/dataset

![Taiwan Air Quality Spatial Interpolation](/profile_site/assets/images/taiwan_aqi_idw.png)

---

## 台灣空氣品質空間插值分析（IDW）
- **描述**：本作品以臺灣紫外線測站資料為基礎，透過反距離加權法（Inverse Distance Weighting, IDW）進行空間插值分析，將離散測站的紫外線指數（UVI）轉換為連續空間分布圖，以呈現特定時間點下紫外線暴露的空間差異。
- **流程**: 
1. 匯入紫外線測站位置資料 (vector)
2. 依測站名稱將UVI數值與測站位置進行屬性連結
3. 使用 IDW 方法進行UVI空間插值，產生連續分布 Raster
4. 依行政區界區範圍裁切插值結果，完成分析圖層
- **工具**：QGIS
- **圖資來源**：https://data.moenv.gov.tw/dataset、https://whgis-nlsc.moi.gov.tw/Opendata/Files.aspx

![Spatial Interpolation of Ultraviolet Index](/profile_site/assets/images/uv.png)

---