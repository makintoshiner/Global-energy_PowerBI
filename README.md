# Global-energy_PowerBI

**My Portfolio Visualization Project in Power BI**

![Dashboard Screenshot](https://github.com/user-attachments/assets/9e0807f8-cb9f-4910-8f68-ec333eab4b2f)  
*[Add additional screenshots of key visuals if available]*

---

## Project Overview

This project aims to analyze global power plant data to identify key regions of electricity generation, examine fuel sources, and assess overall generation capacity across countries, regions, and continents. The dataset contains information on approximately **35,000 power plants** worldwide, including precise coordinates, names, nominal capacity, fuel type, and other characteristics. The goal is to evaluate the potential for power generation globally and determine which countries have the highest capacities and which fuel types are used.

---

## Dataset and Data Preparation

The **Global_power_plant_database** dataset includes the following fields:

- **country (text):** 3-character country code according to ISO 3166-1 alpha-3.  
- **country_long (text):** Full country name.  
- **name (text):** Name or title of the power plant (generally in Romanized form).  
- **capacity_mw (number):** Electrical generating capacity in megawatts.  
- **latitude (number):** Geolocation (latitude) in decimal degrees (WGS84).  
- **longitude (number):** Geolocation (longitude) in decimal degrees (WGS84).  
- **primary_fuel (text):** Primary energy source used.  
- **owner (text):** Majority shareholder or owner of the power plant.  
- **source (text):** Data source (organization, report, or document).  

Additionally, the project uses a **world_population** table, which provides data on population, area, capital, cintinent and other demographic indicators for different countries.  

Before analysis, data cleaning and formatting were performed: columns with incomplete or missing values were removed, and numeric values were properly formatted. 

---

## Data Model and Relationships

To enhance the analysis, two tables were joined:  
1. **global_power_plant_database**  
2. **world_population**

A relationship was established (based on country fields) to enable filtering and comparison of power plant capacity alongside population and other country-level indicators.

[Data Model Screenshot](https://github.com/user-attachments/assets/8694b401-658b-44ff-b24a-19c0bbc1cd7b)

---

## Key Metrics

Based on the data, the following key metrics were calculated (dynamically adjusted based on applied filters):

- **Total Capacity** – the overall generating capacity.  
- **Count of Stations** – the number of power plants.  
- **Average Capacity** – the average capacity.

---

## Technologies Used

- **BigQuery:** Data preparation and cleaning.  
- **Power BI:** Dashboard and visualization development.  
- **DAX Functions:** Calculation of key performance indicators.

---

## Visualization Tools

The project features an interactive dashboard that:
- **Displays** the distribution of generating capacity by country.  
- **Allows** filtering by fuel type and region.  
- **Includes** a table with details on the most powerful stations and key metrics.  
- **Provides** a button to reset all filters.

---

## Link

You can view the live Power BI dashboard here:  
[View Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYmFmNjRjOTctMGJkZC00OTQyLTlhOTYtYjdkNDEwYzViMTFjIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

---

*Feel free to explore the project and leave feedback or suggestions for improvement!*
