# Data-Driven Crime Analysis: Optimizing LAPD Resource Allocation (2020-2023) | Python Data Science Project

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
- Temporal Trends: The Midday Peak
    - Peak Activity: Crime incidents follow a clear daily cycle, peaking at 12:00 PM with 13,663 recorded crimes.
    - Lowest Activity: The lowest frequency of crime occurs at 5:00 AM, recording only 3,171 incidents when overall public activity is minimal.
    - Time Blocks: Crime is most frequent during the afternoon and evening periods, while midnight to early morning shows the lowest frequency reflecting reduced public activity during those hours..

- Geographic Hotspots
    - High-Volume Areas: Crime is not evenly distributed; the Central division reports the highest number of incidents, followed by the Southwest and 77th Street divisions. These areas likely experience higher crime rates due to increased population density, commercial activity, and urban congestion.
    - Nighttime Risks: Between 10:00 PM and 3:59 AM, the Central division remains the area with the largest frequency of "night crimes".

- Victim Demographics & Crime Categories
    - Target Age Group: Victims aged 26–34 are the most affected demographic, accounting for 47,470 recorded incidents.
    - Prevalent Crimes: "Theft of Identity" is the most commonly reported crime in Los Angeles, followed by simple battery and burglary from vehicles.

## Recommendations
- Shift to Midday Patrols
Given that crime peaks at midday, the LAPD should consider re-allocating patrol units from early morning shifts to high-density commercial zones during the 11:00 AM – 2:00 PM window.

- Specialized Identity Theft Task Force
With Theft of Identity being the #1 reported crime, resource investment should be directed toward digital forensic units and public awareness campaigns specifically targeting the 26–34 age demographic.

- Central Division "Night-Watch" Initiative
Because the Central division is a significant hotspot for nighttime crime, city planners should prioritize increased street lighting and "night-watch" community policing in this specific sector.

## Conclusion
Crime data analysis provides valuable insights into the behavioral and spatial patterns of criminal activity. 
The findings from this project highlight opportunities for more strategic law enforcement deployment, enabling the LAPD to respond more effectively to crime trends across Los Angeles.
Future work could include predictive modeling and machine learning approaches to forecast crime hotspots and further enhance proactive policing strategies.

## Limitations 
- No coordinate points: The dataset provides street addresses and Area Names but lacks precise coordinate points. This prevents the creation of "hotspot map" that identify specific street corners or blocks where crime is concentrated.
- Missing Values: Several columns, such as "Weapon Desc", contain a high frequency of "NaN" (Not a Number) values. This limits the ability to perform a detailed analysis of the severity or methods of various crimes.

## About Me
I am Oladejo Olasunkanmi, a Data Scientist with a background in Remote Sensing and Geographic Information Systems (GIS) and over three years of experience analyzing geospatial and spatial datasets across multiple domains. I specialize in transforming complex datasets into actionable insights that support data-driven decision-making for governments and organizations.

My work focuses on data analysis, spatial analytics, and data visualization to uncover patterns, trends, and opportunities hidden in data. I leverage tools such as Python, SQL, GIS technologies, and statistical analysis to build analytical solutions that improve operational efficiency and strategic planning.

I am passionate about using data science and geospatial intelligence to solve real-world problems and support smarter, evidence-based decisions.

I am open to Data Scientist, Geospatial Data Scientist, and Data Analyst opportunities where I can apply data-driven solutions to complex problems.



### Keywords
Data Science, Python, Pandas, Data Visualization, GIS, Crime Analysis, Exploratory Data Analysis, Geospatial Analytics
