# EV Charging Dataset Explorer

This repository hosts two standalone HTML explorers for public EV charging datasets. The goal is to give researchers a quick visual entry point for comparing station-level charging demand patterns and session-level charging behavior without redistributing the original raw data.

## Interactive views

- [EV Charging Dataset Explorer](interactive_dataset_explorer.html): station/site/zone-level geographic and temporal profiles, including map view, weekly aggregate, 24-hour profile, weekday/weekend split, and behavior labels.
- [EV Charging Session Dataset Explorer](session_dataset_explorer.html): session-level dataset comparison, including availability of user IDs, charger IDs, start/end times, duration, energy, price, weather, termination fields, and sample rows.

If GitHub Pages is enabled for this repository, the public links should be:

- `https://chogaliu.github.io/EV-Charging-Dataset-Explorer/interactive_dataset_explorer.html`
- `https://chogaliu.github.io/EV-Charging-Dataset-Explorer/session_dataset_explorer.html`

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

## Citation

If this explorer helps your work, please cite the original datasets used in your analysis. This repository is an index and visualization aid, not the authoritative data source.
