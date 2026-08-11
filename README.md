# Public EV Charging Datasets Review and Explorer

This repository reviews and visualizes public EV charging datasets. It hosts two standalone HTML explorers that give researchers a quick entry point for comparing station-level charging demand patterns and session-level charging behavior without redistributing the original raw data.

本仓库用于整理、回顾和可视化公开电动汽车充电数据集。我们不重新分发原始数据，而是提供原始数据链接，并通过两个独立 HTML 页面帮助研究者快速比较不同数据集的地理覆盖、站点/区域级充电需求模式，以及 session 级字段可用性。

## Interactive views

- [EV Charging Dataset Explorer](interactive_dataset_explorer.html): station/site/zone-level geographic and temporal profiles, including map view, weekly aggregate, 24-hour profile, weekday/weekend split, and behavior labels.
- [EV Charging Session Dataset Explorer](session_dataset_explorer.html): session-level dataset comparison, including availability of user IDs, charger IDs, start/end times, duration, energy, price, weather, termination fields, and sample rows.

## 中文说明

- [充电站点与负荷可视化](interactive_dataset_explorer.html)：展示具有可用地理坐标的数据集，包括地图位置、周聚合曲线、24 小时 profile、工作日/周末差异，以及充电行为模式标签。
- [充电 session 数据集可视化](session_dataset_explorer.html)：比较 session 级数据集的字段可用性，包括用户 ID、充电桩/站点 ID、开始/结束时间、充电时长、能量、价格、天气、结束原因和示例记录。

Public website links:

- [Station and Load Explorer](https://chogaliu.github.io/Public-EV-Charging-Datasets-Review-and-Explorer/interactive_dataset_explorer.html)
- [Session Dataset Explorer](https://chogaliu.github.io/Public-EV-Charging-Datasets-Review-and-Explorer/session_dataset_explorer.html)

公开网页链接：

- [充电站点与负荷可视化](https://chogaliu.github.io/Public-EV-Charging-Datasets-Review-and-Explorer/interactive_dataset_explorer.html)
- [充电 session 数据集可视化](https://chogaliu.github.io/Public-EV-Charging-Datasets-Review-and-Explorer/session_dataset_explorer.html)

## Data source links

The raw datasets are not included in this repository. Please use the original sources and follow their licenses/citation requirements.

| Dataset | Main use in explorer | Location / scope | Original source |
|---|---|---|---|
| CHARGED | Station-level hourly panels | Amsterdam, Shenzhen, Los Angeles, Melbourne, Sao Paulo, Johannesburg | [GitHub: IntelligentSystemsLab/CHARGED](https://github.com/IntelligentSystemsLab/CHARGED) |
| UrbanEV | Zone-level charging volume benchmark | Shenzhen, China | [GitHub: SoYoOo/UrbanEV](https://github.com/SoYoOo/UrbanEV) |
| Palo Alto ChargePoint | Station-level and session-level records | Palo Alto, California, United States | [City of Palo Alto open data](https://data.paloalto.gov/dataviews/257812/electric-vehicle-charging-station-usage-july-2011-dec-2020/) |
| Boulder EV charging | Station-level and session-level records | Boulder, Colorado, United States | [City of Boulder ArcGIS FeatureServer](https://services.arcgis.com/ePKBjXrBZ2vEEgWd/arcgis/rest/services/Electric_Vehicle_Charging_Station_Data/FeatureServer) |
| ACN-Data static | Session-level time-series summaries | Caltech / JPL / Silicon Valley, United States | [ACN-Data project page](https://ev.caltech.edu/dataset.html) |
| Perth and Kinross ChargePlace Scotland | Station-level and session-level records | Perth and Kinross, Scotland, United Kingdom | [ArcGIS item](https://www.arcgis.com/sharing/rest/content/items/ca6cae3df2624832a2eaf678f2eabee8) |
| Jiaxing high-resolution transactions | Session-level records | Jiaxing, Zhejiang, China | [Figshare dataset](https://figshare.com/articles/dataset/A_High-resolution_Electric_Vehicle_Charging_Transaction_Dataset_with_Multidimensional_Features_in_China/28182251) |
| Korea multi-faceted transactions | Session-level records | South Korea, exact city anonymized | [Figshare dataset](https://figshare.com/articles/dataset/A_dataset_for_multi-faceted_analysis_of_electric_vehicle_charging_transactions/22495141) |
| Risvollan apartment charging | Session-level residential charging records | Trondheim, Norway | [Mendeley Data](https://data.mendeley.com/datasets/jbks2rcwyj/3) |

## Notes

- The HTML files are self-contained snapshots generated from local preprocessing scripts.
- The station/load explorer excludes datasets without usable geographic coordinates.
- CHARGED data are released as harmonized hourly panels rather than raw sessions.
- Risvollan represents residential apartment charging, which is behaviorally different from public or workplace charging networks.

## 说明

- 本仓库中的 HTML 文件是基于本地预处理脚本生成的自包含快照。
- 站点/负荷可视化页面只保留具有可用地理坐标的数据集。
- CHARGED 发布的是城市级、站点级的小时面板数据，而不是原始 session 记录。
- Risvollan 是住宅公寓场景的充电数据，其行为模式与公共充电站或办公场景可能不同。

## Citation

If this explorer helps your work, please cite the original datasets used in your analysis. This repository is an index and visualization aid, not the authoritative data source.

如果该整理与可视化工具对你的研究有帮助，请引用你实际使用的原始数据集。这个仓库只是索引与可视化入口，不是原始数据的权威来源。
