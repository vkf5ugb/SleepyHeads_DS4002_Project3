# SleepyHeads_DS4002_Project3
Quinn Glovier (leader), Adam Cook, Victoria Feist
## Contents of Repository 
This repository contains all the source code and data necessary to use a common R package (forecast) to predict the projection of greenhouse gas emissions per capita in the U.S. over the next 11 years.
- SRC Folder
  * Contains annotated R code file
- Data File Folder
  * Contains method of accessing orginal csv (Original Data) and cleaned/downloaded data (cleaned_data).
- Figures Folder
  * Contains 4 figures and 1 table of project results
- LICENSE.md
  * Statement of MIT License
- README.md
  * Explains contents of repository and process of project execution

## SRC
#### Necessary Packages

```{r}
#Installing and loading necessary packages
library(forecast)
library(tseries)
library(tidyverse)
library(ggplot2)
library(dplyr)
library(tidyr)
```


#### Usage of Code
- Download the original csv file from the Our World in Data source. Alternatively, download the cleaned dataset in the Data folder.
- Open the code file in R and ensure your working directory is the folder that contains the data
- Install necessary packages
- If using the original csv file, follow the entirety of the code file to properly clean the dataset. If using the pre-cleaned dataset, skip lines 20-30.
- Run all the code in order to prepare the data, create predictions using ARIMA, and visualize/evaluate the results of the prediction confidence intervals


## DATA 
### Original Data
The original dataset before any cleaning: [Original Data](https://ourworldindata.org/co2-and-greenhouse-gas-emissions)

### Final Data

The data after manipulation, ready to be used for analysis: [Cleaned Data](https://drive.google.com/drive/folders/1M6D-41vEOOeMSL6QIo5UEMeCqJCpaDne?usp=sharing)

### Data Dictionary  
| Category                     | Description                                                                           |
| -------------                | -------------                                                                         |
| year                         | Year of observation                                                                   |
| population                   | The population of the U.S.                                                            |
| ghg_per_capita               | Greenhouse gas emissions per capita in tonnes per person                              |
| total_ghg                    |Total greenhouse gas emissions in millions of tonnes.                                  |
| co2_including_luc            | Annual total emissions of CO2 in millions of tonnes.                                  |
| co2_including_luc_per_capita | Annual emissions of CO2 per capita in tonnes per person.                              |
| oil_co2                      | Annual CO2 emissions from oil production measured in millions of tonnes.              |
| oil_co2_per_capita           | Annual CO2 emissions from oil production per capita, measured in tonnes per person.   |
| methane                      | Total methane emissions measured in millions of tonnes.                               |
| methane_per_capita           | Methane emissions per capita measured in tonnes per person.                           |

## FIGURES
Plot showing the current trend in greenhouse gas emissions per capita in the US since 1990.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project3/blob/main/Figures/GHG_Per_Capita.png" title= "GHG Per Capita">

Plot showing the current trend in TOTAL greenhouse gas emissions in the US since 1990.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project3/blob/main/Figures/GHG_Total.png" title= "GHG Total">

Plot showing the predicted trend in greenhouse gas emissions per capita in the US 1990-2030.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project3/blob/main/Figures/GHG_Per_Capita_Pred.png" title= "Predicted GHG Per Capita">

Plot showing the predicted trend in TOTAL greenhouse gas emissions in the US 1990-2030.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project3/blob/main/Figures/GHG_Total_Pred.png" title= "Predicted Total GHG">

Table showing the predicted GHG reduction (per capita and total) in the US by 2030. In agreement with our hypothesis, the US will not meet the GHG reduction goal of 50-52%.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project3/blob/main/Figures/ResultsTable.png" title= "Results of Predictions">

## References
[1] A. Cook, T. Feist, Q. Glovier, “Climate Change Predictions: Milestone 1”, The Sleepyheads, 04-April-2023, [Online]. Available: [Project3_MI1](https://docs.google.com/document/d/1ucUobykuZswk5Unbu6bWKyQ18jEMa1kowxmz9iMyxfo/edit) . [Accessed 04-06-2023].

[2] A. Cook, T. Feist, Q. Glovier, “Climate Change Predictions: Milestone 2”, The Sleepyheads, 08-April-2023, [Online]. Available: [Project3_MI2](https://docs.google.com/document/d/1HQOttT25JbTY2lmzu_LwqskXsB_EEQCIW2ISqyz_0l8/edit). [Accessed 04-13-2023].

[3] H. Ritchie, M. Roser, P. Rosado, “CO2 and Greenhouse Gas Emissions,” Our World in Data, August-2020, [Online]. Available: https://ourworldindata.org/co2-and-greenhouse-gas-emissions. [Accessed 4-13-2023.]

[4] D. Chao, “Performing Time Series Analysis Using ARIMA Model in R,” Analytics Vidhya, 22-November-2021, [Online]. Available: https://www.analyticsvidhya.com/blog/2021/11/performing-time-series-analysis-using-arima-model-in-r/ [Accessed: 04-13-2023].

