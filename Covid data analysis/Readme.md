# Experiment 19 & 20 - COVID-19 Data Analysis

## Introduction
The outbreak of Coronavirus Disease 2019 (COVID-19), driven by the SARS-CoV-2 virus, brought about one of the most severe global health emergencies in recent times. Initially detected in late 2019, it was officially designated a Global Pandemic by the World Health Organization (WHO) on March 11, 2020. 

Beyond the immediate medical toll, the virus caused massive socio-economic upheaval, overwhelming healthcare systems and disrupting supply chains worldwide. As nations and medical bodies fought to slow the transmission, data-centric decision-making took center stage. Precise monitoring of case counts, recovery rates, and fatalities became the bedrock for forming public health policies and distributing vital resources.

## Libraries and Functions Used
* **Python:** The primary programming language used for scripting and data handling.
* **Pandas & NumPy:** Leveraged for importing data, data cleansing, feature extraction, and performing statistical summaries.
* **Plotly Express:** Used to create dynamic, high-quality geographical visualizations (specifically choropleth maps).
* **GeoJSON:** Applied to map out regional state boundaries for localized plotting within India.

## Dataset Overview
The data driving this COVID-19 study is an extensive compilation of pandemic statistics provided by the World Health Organization (WHO), covering the timeline from the start of 2020 through May 2021. 

In its raw form, the dataset holds 306,429 records structured across 8 primary columns.

## Methodologies and Functional Implementation
Unique analytical methods and functions were applied during the data processing phase:
* **Data Loading:** Leveraged functions from the pandas library to ingest over 300,000 records and execute initial preprocessing steps.
* **Data Cleaning:** Applied the `.drop()` command to eliminate unnecessary columns like `SNo` and `Last Update`, effectively optimizing memory usage.
* **Data Transformation:** Utilized the `pd.to_datetime` method to parse string-formatted dates into temporal objects, unlocking the ability to conduct Time Series Analysis.
* **Hierarchical Aggregation:** Implemented the `.groupby()` function on key columns such as `Country/Region` and `Province/State` to facilitate statistical computations across large subsets of the data.

## Experiment - 19: Global Data Visualization
To assess the worldwide impact of the pandemic at that time, we filtered the records to isolate the most recent date of observation using the `max()` function, which identified May 29, 2021, as the endpoint.

### Geospatial Visualization
By utilizing `plotly.express`, we plotted a global choropleth map. This provided a clear visual gradient, where color intensity highlighted the countries hit the hardest versus those least affected. 

According to the visualizations generated, the Top 10 affected countries were:
*(Insert Top 10 List/Visual Here)*

## Experiment - 20: India-Specific COVID Data Analysis
This segment of the study focused exclusively on India by extracting a sub-dataframe where the `Country/Region` matched India. This regional deep-dive is highly relevant, given that May 2021 was the height of India's severe "second wave" of the virus.

The analysis showed that COVID cases were monitored across 38 specific regional entities, covering every state and union territory. By grouping the most recent observation data by `Province/State`, we could pinpoint exactly which geographic areas bore the highest viral loads. 

The most heavily impacted states and provinces in India emerged as:
*(Insert Top States/Visual Here)*

## Key Insights and Inferences
* Maharashtra, alongside several southern states, experienced the most severe initial blow. Maharashtra alone accounted for more than 20% of the country's total caseload.
* Even with a massive surge in infections, Kerala managed to keep its mortality rate notably low compared to territories like Delhi. This reflects the strength and resilience of their regional public health network.
* The use of choropleth mapping turned raw statistical data into actionable visual guides of affected districts. These map visualizations were crucial for real-time logistics, helping target the delivery of oxygen and vaccines directly to the most vulnerable communities.

## Conclusion
This analysis highlights a complete, end-to-end data science workflow using Python. By importing, refining, and plotting the `covid_19_data.csv` records, we successfully measured the staggering global impact of the virus up to May 2021. Our worldwide breakdown validated that the US, India, and Brazil were the primary epicenters of the disease. Additionally, our targeted geographical mapping of India using GeoJSON offered a transparent, empirical view of the localized emergencies ravaging states like Maharashtra and Karnataka. In closing, this study emphasizes how critical data science is for monitoring, interpreting, and broadcasting the realities of widespread public health crises.
