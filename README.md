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

The fish catch data across 1997 to 2023 were obtained through the International Council for the Exploration of the Seas (ICES). The datasets include information on the country responsible, catch region, species name, and number of landings in tonnes. The data is split across three different time periods (1903-1949, 1950-2010, 2006-2023).

Data source: [ICES CIEM](https://www.ices.dk/data/dataset-collections/Pages/Fish-catch-and-stock-assessment.aspx)

**Northeast Atlantic Sea Surface Temperature Data**

The sea surface temperature that spans Portugal's coast was obtained through the European Environment Agency which has maximum and minimum sea surface temperatures for the Northeast Atlantic Ocean. For this simplicity, I've only chosen to use maximum surface temperature as an independent variable.

Data source: [European Environment Agency](https://www.eea.europa.eu/en/analysis/indicators/european-sea-surface-temperature?activeAccordion=309c5ef9-de09-4759-bc02-802370dfa366)

**Annual Fish Price Data**

Annual fish price data (euros/kg) from 2011 to 2024 was obtained from Statistics Portugal's Annual Fishery Statistics Report. I manually scrolled through each pdf document and recorded the annual fish price stated for that year's report. The reports seemingly start reporting this number from 2011 onwards.  

Data source: [Statistics Portugal's](https://www.ine.pt/xportal/xmain?xpid=INE&xpgid=ine_pesquisa&frm_accao=PESQUISAR&frm_show_page_num=1&frm_modo_pesquisa=PESQUISA_SIMPLES&frm_texto=Anu%C3%A1rio+estat%C3%ADstico+de+Portugal&frm_modo_texto=MODO_TEXTO_ALL&frm_data_ini=&frm_data_fim=&frm_tema=QUALQUER_TEMA&frm_area=o_ine_area_Publicacoes&xlang=en) Annual Fishery Statistics Report

Example PDF: [Portugal Fishery Statistics 2023](https://www.ine.pt/ngt_server/attachfileu.jsp?look_parentBoui=669999694&att_display=n&att_download=y)

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