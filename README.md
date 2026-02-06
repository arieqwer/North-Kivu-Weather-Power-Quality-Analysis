
# High-frequency evidence on the associations between meteorological variability and power quality in North Kivu’s healthcare facilities

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18510525.svg)](https://doi.org/10.5281/zenodo.18510525)

This repository contains the code and data supporting the findings of the study **"High-frequency evidence on the associations between meteorological variability and power quality in North Kivu’s healthcare facilities"**

## Abstract
Reliable electricity is essential for healthcare delivery, particularly in resource-constrained settings vulnerable to weather extremes. This study investigates the associations between temperature, precipitation, and power quality, specifically local temperature extremes and precipitation anomalies, on power quality and reliability (PQR) in 24 healthcare facilities across North Kivu, Democratic Republic of the Congo (DRC). Using high-frequency sensor data and satellite-derived climate indices from May 2022 to October 2024, we assessed relationships between meteorological conditions (dry and wet extremes, heatwaves) and key PQR metrics: daily power source uptime, within-nominal voltage time, and within-nominal frequency time. Regression models incorporating monthly fixed effects revealed that small-scale hydroelectric systems, especially those with poor maintenance, were particularly sensitive to droughts and wet extremes, showing significant declines in voltage and within-nominal frequency time. Conversely, generator-based and utility-scale hydro facilities exhibited greater resilience, though not without vulnerability under extreme wet conditions. Hospital facilities consistently maintained higher power reliability than non-hospital facilities due to superior infrastructure and management practices. Our findings highlight the need for targeted infrastructure investment, preventive maintenance, and diversified hybrid power solutions to ensure robust healthcare service delivery under increasing weather variability.


## Repository Structure

```text
├── data/
│   ├── north_kivu_spi_daily.csv         # Daily SPI 1 and 3 and dryness status for each selected Aire de Sante
│   ├── Td_allAS_heatwave.csv.csv        # Td and heatwave status for all AS
│   ├── Td_selectedAS_heatwave.csv.csv   # Td and heatwave status for selected AS
│   ├── Tw_allAS_heatwave.csv.csv        # Tw and heatwave status for all AS
│   ├── Tw_selectedAS_heatwave.csv.csv   # Tw and heatwave status for selected AS
├── notebooks/
│   ├── SPI_calculation.ipynb            # Scripts to calculate SPI 1 and 3
│   ├── Td&heatwave_calculation.ipynb    # Scripts to extract Td from ERA5 via GEE and determine heatwave status base on Td
│   └── Tw&heatwave_calculation.ipynb    # Scripts to extract Tw from ERA5 via GEE and determine heatwave status base on Tw
├── figures/                        # Output figures used in the manuscript
├── requirements.txt                # Python dependencies
└── README.md                       # Project documentation
