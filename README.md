# DER-Minimum-Demand-Dashboard
Power BI project analysing Distributed Energy Resources (DER), minimum demand risk, and rooftop solar adoption in Western Australia using AEMO data.

## Table of Contents
- [Project Overview](#project-Overview)
- [Objectives](#objectives)
- [Goal](#goal)
- [Dataset Overview](#dataset-overview)
- [ Data Preparation](#data-preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Key Insights](#key-insights)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)

## Project Overview
Western Australia is experiencing one of the fastest Distributed Energy Resource (DER) transitions globally, driven primarily by rapid rooftop solar adoption. While this supports decarbonisation goals, it is also creating operational challenges for the electricity network, including record-low minimum demand during midday and steep demand ramping in the evening. This Power BI project analyzes how DER growth is reshaping system demand patterns and identifies where DER adoption is concentrated geographically. The dashboard provides a system-level and customer-level view to support decision-making around grid reliability, storage investment, and demand flexibility.

## Objectives
The main objectives of this project were:

1. **To analyze the impact of rooftop solar generation on operational demand patterns**
2. **To quantify minimum demand risk and evening ramping requirements**
3. **To evaluate the scale and distribution of DER adoption across Western Australia**
4. **To identify imbalances between rooftop solar capacity and battery storage adoption**
5. **To provide actionable insights to support grid planning and energy transition strategies**

## Project Goal
The goal of the dashboard is to create a decision-support tool that helps stakeholders understand how increasing DER penetration affects electricity demand, network reliability, and operational planning. By combining system demand data with DER installation data, the dashboard highlights the operational risks associated with rapid solar growth and the need for storage and flexibility solutions.

## Dataset Overview
The analysis uses publicly available datasets from the Australian Energy Market Operator (AEMO):

Operational Demand Data (2022–2023)
Half-hourly operational demand values representing system load after distributed solar generation is accounted for.

Distributed PV (DPV) Generation Data (2022–2023)
Half-hourly rooftop solar generation estimates used to calculate gross system demand.

DER Register (Aggregated by Postcode)
The DER Register dataset represents a snapshot of aggregated Distributed Energy Resource (DER) installations by postcode as at July 2024, reflecting the cumulative number of installations and installed capacity of rooftop solar and battery systems in Western Australia at the time of reporting.

## Data Cleaning and Preparation
1. Data preparation was conducted in Power Query and involved:

2. Cleaning and standardizing timestamp formats

3. Appending 2022 and 2023 operational demand datasets

4. Appending distributed PV generation datasets

5. Merging demand and PV datasets to calculate Gross Demand

6. Creating derived metrics such as minimum demand, solar penetration share, and evening ramp rate

7. Cleaning the DER Register dataset by filtering invalid or unknown postcodes

8. Converting installed capacity units for consistency and aggregation

## Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand how rooftop solar affects daily demand patterns and how DER adoption varies geographically. The analysis included:

- Duck Curve visualization comparing gross demand and net demand

- Minimum demand trend analysis across the study period

- Identification of solar adoption hotspots by postcode

- Comparison of solar and battery installation counts and capacities

- KPI analysis summarizing DER penetration and system demand metrics

## Key Insights
Based on the analysis of the reporting period examined, several key insights were identified:

- Minimum operational demand fell to 595 MW, indicating increasing system stress during midday periods

- Rooftop solar supplied up to 76% of total demand, demonstrating significant DER penetration

- Evening ramp rates reached 564 MW per hour, highlighting operational challenges in balancing supply

- Western Australia recorded approximately 483,000 DER connections as at the period of reporting

- Installed rooftop solar capacity reached 1.93 GW, while battery capacity remained extremely low at 6.7 MW

- Solar installations represent 99.7% of DER systems, confirming a significant imbalance between generation and storage

- DER adoption is geographically concentrated in specific postcode clusters, suggesting localized network pressure

## Recommendations
Based on the analysis, the following actions are recommended:

- Increase investment in distributed and utility-scale battery storage to balance solar generation

- Implement demand-response programs to reduce evening ramping pressure

- Prioritize network upgrades in DER adoption hotspots

- Support policy and incentive programs that accelerate battery adoption alongside rooftop solar installations

- Develop DER orchestration strategies to better manage distributed generation resources

## Conclusion
The DER & Minimum Demand Dashboard demonstrates that while rooftop solar adoption is accelerating Western Australia’s transition toward renewable energy, the imbalance between generation and storage is creating new operational challenges for the electricity grid. Strategic investment in storage technologies, demand flexibility programs, and targeted network planning will be essential to ensure system reliability as DER penetration continues to grow
  
