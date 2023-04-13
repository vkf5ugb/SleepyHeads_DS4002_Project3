# SleepyHeads_DS4002_Project3
Quinn Glovier (leader), Adam Cook, Victoria Feist
## Contents of Repository 
This repository contains all the source code and data necessary to use a common R package (forecast) to predict the projection of greenhouse gas emissions per capita in the U.S. over the next 11 years.
- SRC Folder
  * Contains annotated R code file
- Data File Folder
  * Contains method of accessing orginal csv (Original Dataset) and cleaned/downloaded data (Cleaned Dataset).
- Figures Folder
  * Contains - figures
- LICENSE.md
  * Statement of MIT License
- README.md
  * Explains contents of repository and process of project execution

## SRC
#### Necessary Packages and Set Seed

```{r}
#Installing and loading necessary packages
#install.packages('tensorflow')
#install.packages('keras')
#install.packages('tfdatasets')
#install_tensorflow()
library(tensorflow)
library(keras)
set.seed(1234)
```


#### Usage of Code
- Download the original csv file from the Our World in Data source. Alternatively, download the cleaned dataset in the Data folder.
- Open the code file in R and ensure your working directory is the folder that contains the data
- Install necessary packages
- If using the original csv file, follow the entirety of the code file to properly clean the dataset. If using the pre-cleaned dataset, skip lines 20-30.
- Run all the code in order to prepare the data, run the predictions, and visualize/evaluate the results


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

## Figures
Bar graph showing the distrubution of images across 3 patient statuses: healthy, pneumonia, covid.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project2/blob/main/Figures/DataDist.jpeg" title= "Data Distribution">

Accuracy and loss fluctuate over the course of image testing.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project2/blob/main/Figures/Accuracy.jpeg" title= "Accuracy">

The model can easily classify normal, healthy lungs as such. However, it can only classify COVID-19 patient lungs correctly ~86% of the time.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project2/blob/main/Figures/CorrectClassifications.jpeg" title= "Correct Classifications">

## References
[1] A. Cook, T. Feist, Q. Glovier, “Climate Change Predictions: Milestone 1”, The Sleepyheads, 04-April-2023, [Online]. Available: [Project3_MI1](https://docs.google.com/document/d/1ucUobykuZswk5Unbu6bWKyQ18jEMa1kowxmz9iMyxfo/edit) . [Accessed 04-06-2023].

[2] A. Cook, T. Feist, Q. Glovier, “Climate Change Predictions: Milestone 2”, The Sleepyheads, 08-April-2023, [Online]. Available: [Project3_MI2](https://docs.google.com/document/d/1HQOttT25JbTY2lmzu_LwqskXsB_EEQCIW2ISqyz_0l8/edit). [Accessed 04-06-2023].
