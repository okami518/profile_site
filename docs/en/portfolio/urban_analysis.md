# Urban_Portfolio

---

## Taiwan Air Quality Spatial Interpolation
- **Description**：This project visualizes the spatial distribution of AQI across Taiwan using point-based monitoring data.
AQI values from monitoring stations were joined with station locations and interpolated using Inverse Distance Weighting (IDW).
The raster result was clipped by air quality management zones to focus on meaningful analysis regions.
- **Workflow**：
1. Imported air quality monitoring station locations (vector)
2. Joined daily AQI values by station name
3. Applied IDW interpolation to generate continuous AQI surface
4. Clipped raster by air quality management zones
- **Tools**：QGIS
- **Data Source**：https://data.moenv.gov.tw/dataset

![Taiwan Air Quality Spatial Interpolation](/profile_site/assets/images/taiwan_aqi_idw.png)

---

## Spatial Interpolation of Ultraviolet Index (UVI)
- **Description**：This project applies spatial interpolation techniques to ultraviolet index (UVI) monitoring data in Taiwan. By using the Inverse Distance Weighting (IDW) method, discrete station-based UVI observations are transformed into a continuous spatial surface to visualize ultraviolet exposure patterns at a specific time.
- **Workflow**：
1. Imported UVI monitoring station locations (vector)
2. Joined UVI values by station name
3. Applied IDW interpolation to generate continuous UVI surface
4. Clipped raster by county outline
- **Tools**：QGIS
- **Data Source**：https://data.moenv.gov.tw/dataset、https://whgis-nlsc.moi.gov.tw/Opendata/Files.aspx

![Spatial Interpolation of Ultraviolet Index](/profile_site/assets/images/uv.png)

---