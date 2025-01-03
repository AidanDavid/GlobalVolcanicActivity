# Global Volcanic Activity

Analyzing global volcanic activity, geological characteristics, and historical eruption patterns.

## Overview

This project focuses on creating an interactive platform to provide insights into global volcanic activity, geological characteristics, and historical eruption patterns. By leveraging historical data, the goal is to explore relationships between volcanic attributes such as the Volcanic Explosivity Index (VEI), eruption type, and their resulting consequences, including fatalities and economic damages. 

The dataset includes comprehensive information about volcanoes, such as their locations, types, activity statuses, VEI, and other related attributes. The project involves data cleaning, geospatial mapping, and visualization to highlight trends and potential threats posed by volcanic activity worldwide.

## Table of Contents

- [Data Resources](#data-resources)
- [Usage Guide](#usage-guide)
- [Visualizations](#visualizations)
- [Technologies Used](#technologies-used)
- [Credits](#credits)
- [License](#license)

## Data Resources

The data used in this project is sourced from reliable volcanic and geological records, including:

- **Smithsonian Institution Global Volcanism Program**: Comprehensive historical and geological volcanic data.
- **NOAA Hazard Events Database**: Event-specific volcanic data, including fatalities and damages.
- **NGDC Location Search**: [NGDC Volcano Location Search](https://www.ngdc.noaa.gov/hazel/view/hazards/volcano/loc-search/).
- **NGDC Event Search**: [NGDC Volcano Event Search](https://www.ngdc.noaa.gov/hazel/view/hazards/volcano/event-search/).

## Usage Guide

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
- **Bar charts**: Analyzing average total damage and deaths by volcano type.
- **Scatter plots**: Identifying relationships between VEI and other factors.

Visualizations are generated using Python libraries and stored in the `output/visualizations` directory.

## Technologies Used

- **Python**: For data analysis and visualization.
- **Pandas**: For data manipulation and aggregation.
- **Matplotlib & Plotly**: For static and interactive visualizations.
- **Cartopy**: For geographical data processing.
- **PostgreSQL**: Database for storing and managing volcanic data.
- **Leaflet.js**: For geospatial mapping.

## Credits

This project was independently developed by the following developers:

**Yiheng Sun**:

- **Github**: [@Sait0uAsuka](https://github.com/Sait0uAsuka)

<br><br />

**Aidan David**:

- **Github**: [@AidanDavid](https://github.com/AidanDavid)

<br><br />

**Lucas Hejmo Jones**:

- **Github**: [@LucasHejmo](https://github.com/LucasHejmo)

<br><br />

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
