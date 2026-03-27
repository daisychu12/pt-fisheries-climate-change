# Climate Change Impacts on Portugal's Fishing Industry

This repo contains data and analysis for a capstone project analyzing whether climate change is impacting Portugal's fishing industry. 

## Project Summary
Using fish catch, ocean surface temperature, and fish price data, I examined whether there is a relationship between fish landings and temperature. I found that impact of landings and vulnerability to climate change is species dependent, but 4 out of the 5 species studied show a significant relationship with rising maximum sea temperatures. 


## Project Question
- How does ocean temperature impact the number of fish landings in Portugal?
- How does ocean temperature and number of fish landings affect the national fish price?

## Project Rationale
**The problem I'm trying to address:**
Decades of overfishing have led many fisheries to collapse across the globe. For Portugal, on top of the economic strain due to drop in fish species populations, species like sardine have started to be observed moving towards cooler waters due to climate change.

**Audience of interest:** 
Portugal's policymakers, marine scientists, and data scientists.

**Why does the answer to this question matter?** 
If climate change is already impacting fish landings numbers, stricter monitoring of catches in Portugal's Marine Protected Area Network in the Azores is needed. This call for more frequency and transparency in monitoring can protect the marine species people love to eat while restoring overfished marine ecosystems.


## Data Sources
**Fish Landings Datasets**

Data source:

**Northeast Atlantic Sea Surface Temperature Data**

Data source:

**Annual Fish Price Data**

Data source:
Example PDF:

## Process
- Clean fish landings datasets
- Filter fish landing datasets to Portugal landings only
- Merge fish landing datasets across years
- Filter to data from 1997-2023
- Merge fish landing datasets with ocean temperature dataset
- Merge ocean temperature dataset with fish price dataset
- Conduct exploratory data analysis
- Plot and run correlation analysis on:
  - the top 5 landed species with ocean temperature, temperature and fish price, total landings and fish price
- Run polynomial regression analysis on:
  - the top 5 landed species with ocean temperature, temperature and fish price, total landings and fish price


## Repository Structure
```
pt-fisheries-climate-change/
├── analysis/              # All code and scripts
│   └── README.md          # Communication folder overview
├── data/                  # All datasets and related files
│   ├── archive/           # Unnecessary or old data
│   ├── metadata/          # Data documentation
│   ├── processed_data/    # Cleaned datasets
│   ├── raw_data/          # Original, untouched data
│   └── README.md          # Data folder overview
├── outputs/               # Slides, reports, presentations
│   └── README.md          # Scripts folder overview
└── README.md              # Project overview
```

## Contact Information
- Daisy Chu
- daisychu@berkeley.edu
- [LinkedIn](www.linkedin.com/in/daisy-chu)