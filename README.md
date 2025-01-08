# 🌋Global Volcanic Activity🌋

Analyzing global volcanic activity, geological characteristics, and historical eruption patterns.

## Overview

This project focuses on creating an interactive platform to provide insights into global volcanic activity, geological characteristics, and historical eruption patterns. By leveraging historical data, the goal is to explore relationships between volcanic attributes such as the Volcanic Explosivity Index (VEI), eruption type, and their resulting consequences, including fatalities and economic damages. 

The dataset includes comprehensive information about volcanoes, such as their locations, types, activity statuses, VEI, and other related attributes. The project involves data cleaning, geospatial mapping, and visualization to highlight trends and potential threats posed by volcanic activity worldwide.

## Table of Contents

- [Usage Guide](#usage-guide)
- [Visualizations](#visualizations)
- [Technologies Used](#technologies-used)
- [References](#references)
- [Ethical Considerations](#ethical-considerations)
- [Credits](#credits)
- [License](#license)


## Usage Guide

### Data Usage Description

The data was downloaded from the sources listed in the [Data Sources](#data-sources) section and saved in the `data` directory. Two TSV files, `locations.csv` and `event.csv`, were converted to CSV format and then combined using PostgreSQL.

- **Location CSV**: Contains latitude and longitude information for all volcanoes.  
- **Event CSV**: Lists all active volcanoes.  
- **Combined CSV**: A left join of the `event.csv` onto the `location.csv`, resulting in a dataset with all volcano locations and an indication of active volcanoes.

### 1. Glone the Repo

To run this project locally, follow these steps:

**Clone the repository**:

   ```bash
   git clone https://github.com/AidanDavid/GlobalVolcanicActivity.git
   cd GlobalVolcanicActivity
   ```

### 2. Running the Analysis

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the relevant notebook file and execute the cells step by step to analyze and visualize the volcanic data.

## Visualizations

The project includes a range of interactive and static visualizations:

- **Geospatial maps**: Visualizing volcano locations and activity statuses.
- **Time series plots**: Tracking volcanic activity trends over time.
- **Bar charts**: Analyzing average total damage and deaths by volcano type, ranking of recorded eruptions by countries, Number of Eruptions per VEI
- **Pie charts**: percentage of Tsunami and Earthquake events

Visualizations are generated using Python libraries and stored in the `images` directory.

## Technologies Used

- **Python**: For data analysis and visualization.  
- **Pandas**: For data manipulation and aggregation.  
- **Matplotlib & Plotly**: For static and interactive visualizations.  
- **PostgreSQL**: Database for storing and managing volcanic data.  
- **Leaflet.js**: For geospatial mapping (loaded via CDN).  
  - JavaScript: [v1.9.4](https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.min.js)  
  - CSS: [v1.9.4](https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.min.css)  
- 🚨 **PapaParse**: For CSV parsing (loaded via CDN).  
  - JavaScript: [v5.4.1](https://cdnjs.cloudflare.com/ajax/libs/PapaParse/5.4.1/papaparse.min.js)  
- 🚨 **Cartopy**: Used for geographical data processing.  


## References

### Data Sources
- **NGDC Hazard Events Database**: National Geography Data Center(NGDC), Event-specific volcanic data, including fatalities and damages.
- **NGDC Location Search**: [NGDC Volcano Location Search](https://www.ngdc.noaa.gov/hazel/view/hazards/volcano/loc-search/).
- **NGDC Event Search**: [NGDC Volcano Event Search](https://www.ngdc.noaa.gov/hazel/view/hazards/volcano/event-search/).

### Reference for Verifying the Data Sources
- **Smithsonian Institution Global Volcanism Program**: ([Comprehensive historical and geological volcanic data.](https://volcano.si.edu/)). This data was used to verify the accuracy and reliability of the data sources, ensuring that the latitude and longitude coordinates match those provided on the website.

### Code References
- **Cartopy for Geospatial Mapping**: [Foundations of Cartopy](https://foundations.projectpythia.org/core/cartopy/cartopy.html)
- **Cartopy Feature Interface (borders and coastline)**: [Cartopy Documentation](https://scitools.org.uk/cartopy/docs/latest/matplotlib/feature_interface.html)
- **Colormap in Matplotlib**: [Matplotlib Colormaps](https://matplotlib.org/stable/users/explain/colors/colormaps.html)
- **Colorbar Configuration in Matplotlib**: [Matplotlib Colorbar](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.colorbar.html)
- **Projection for World Map**: [Cartopy Projections](https://scitools.org.uk/cartopy/docs/latest/reference/projections.html)

## Ethical Considerations

This project aims to use data responsibly by relying only on public and trusted sources like the Smithsonian Institution and NOAA. No personal or private data has been used, ensuring everyone's privacy. We are aware that historical data might be biased, especially for less studied regions, so we checked multiple sources to reduce this. The project shares volcanic activity trends in a clear and honest way, avoiding exaggeration, to help people understand the information accurately and make informed choices.


## Credits

This project was independently developed by the following developers:

**Yiheng Sun**:

- **Github**: [@Sait0uAsuka](https://github.com/Sait0uAsuka)

**Aidan David**:

- **Github**: [@AidanDavid](https://github.com/AidanDavid)

**Lucas Hejmo Jones**:

- **Github**: [@LucasHejmo](https://github.com/LucasHejmo)

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
