# Data-Driven Crime Analysis: Optimizing LAPD Resource Allocation (2020-2023)

## Project Overview and Problem
This project analyzes criminal behavior patterns in Los Angeles to support the Los Angeles Police Department (LAPD) in effective resource allocation.
This analysis was conducted to uncover actionable insights from historical crime data, helping stakeholders better understand:
- Where crimes occur most frequently
- What types of crimes are most common
- When crimes are more likely to occur
- Patterns that could inform strategic resource deployment

## Objectives
The goal of this analysis is to identify meaningful crime patterns within Los Angeles that can support data-driven policing strategies.

### Key objectives include:
- Identify high-frequency crime categories
- Determine areas with the highest crime rates
- Analyze temporal patterns (time of day, month, etc.)
- Highlight potential hotspots
- Provide data-driven recommendations for resource allocation

## Dataset Overview
- Data Source: DataCamp data archive for capstone project
- Time Period Covered: 2020 – 2023
- Volume: 185,715 rows x 15 columns
- Geography: Los Angeles, Southern California, United States.

## Key Columns in the Dataset
| Column     | Description              |
|------------|--------------------------|
| `'DR_NO'` | Division of Records Number: Official file number made up of a 2-digit year, area ID, and 5 digits. |
| `'Date Rptd'` | Date reported - MM/DD/YYYY. |
| `'DATE OCC'` | Date of occurrence - MM/DD/YYYY. |
| `'TIME OCC'` | In 24-hour military time. |
| `'AREA NAME'` | The 21 Geographic Areas or Patrol Divisions are also given a name designation that references a landmark or the surrounding community that it is responsible for. For example, the 77th Street Division is located at the intersection of South Broadway and 77th Street, serving neighborhoods in South Los Angeles. |
| `'Crm Cd Desc'` | Indicates the crime committed. |
| `'Vict Age'` | Victim's age in years. |
| `'Vict Sex'` | Victim's sex: `F`: Female, `M`: Male, `X`: Unknown. |
| `'Vict Descent'` | Victim's descent:<ul><li>`A` - Other Asian</li><li>`B` - Black</li><li>`C` - Chinese</li><li>`D` - Cambodian</li><li>`F` - Filipino</li><li>`G` - Guamanian</li><li>`H` - Hispanic/Latin/Mexican</li><li>`I` - American Indian/Alaskan Native</li><li>`J` - Japanese</li><li>`K` - Korean</li><li>`L` - Laotian</li><li>`O` - Other</li><li>`P` - Pacific Islander</li><li>`S` - Samoan</li><li>`U` - Hawaiian</li><li>`V` - Vietnamese</li><li>`W` - White</li><li>`X` - Unknown</li><li>`Z` - Asian Indian</li> |
| `'Weapon Desc'` | Description of the weapon used (if applicable). |
| `'Status Desc'` | Crime status. |
| `'LOCATION'` | Street address of the crime. |

![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Data_columns_snapshot.png)

## Tools and Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Cleaning & Preparation
- Converted date columns to datetime format
- Removed duplicate records
- Handled missing values in demographic fields
- Extracted new columns features such as:
  - Hour of crime occurrence
  - Day of week
  - Month
  - Year
  - Age brackets
  - Time periods(Morning, Afternoon, Evening and Mid-night)

## Key Questions & Analysis 
  ### Questions
  1. What is the highest frequency of crimes by hour? 
  2. How does crime victimization vary by age group?
  3. How does crime frequency change throughout the daytime period?
  4. Which Los Angeles divisions experience the highest crime rates?
  5. What are the top 15 crime categories reported?
  6. What are the top 10 types of crimes dominate nighttime hours (10 PM – 3:59 AM)?
  7. Are crimes more common on weekdays or weekends?
  8. Which area + hour combination produces the highest crime counts?
  9. Crime trend: Is crime increasing or decreasing over time?

  ### Analysis
  #### Question 1
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Crime_Frequency_by_Hour_(2020-2023).png)
  
  #### Question 2
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Crime_Victimization_by_Age_Group.png)
  
  #### Question 3
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Crime_Distribution_by_Time_Period_(2020-2023).png)
  
  #### Question 4
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Top10_Crime-Prone_Areas_(2020%20-%202023).png)
  
  #### Question 5
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Top_15_Crimes_reported_(2020%20-%202023).png)
  
  #### Question 6
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Top_Crimes_During_Night_Hours_(10PM_3AM).png)
  
  #### Question 7
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Crime_Counts_by_Day_of_the_Week_(2020-2023).png)
  
  #### Question 8
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Crime_Counts_by_Area_and_Hour.png)
  
  #### Question 9
  ![Image Description](https://github.com/olasunkanmitheCoder/crime_data_analysis_in_Los_Angeles_between_2020_2023/blob/main/Crime_Trend_by_Month_and_Year.png)


## Key Insights 

  

