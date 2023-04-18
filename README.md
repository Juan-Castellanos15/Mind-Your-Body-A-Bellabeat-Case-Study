<h1 align="center"><img src="https://bellabeat.com/wp-content/uploads/2022/10/Leaf-Urban-Rose-Gold-Bellabeat-2.jpg" alt="Bellabeat Sleep" width="45" height="37.5">  Mind Your Body  <img src="https://bellabeat.com/wp-content/uploads/2022/10/Leaf-Urban-Rose-Gold-Bellabeat-2.jpg" alt="Bellabeat Sleep" width="45" height="37.5"></h1> 
<h3 align="center">How Bellabeat Helps Users Optimize Physical Activity and Sleep</h3>
<div align="center"><img src="https://i.giphy.com/media/26BRq9PYFLeJl3WLu/giphy.webp" alt="Bellabeat Fit" width="270" height="250"> <img src="https://news.mit.edu/sites/default/files/styles/news_article__image_gallery/public/images/202009/MIT-Sleep-Positions-01-ani_0.gif?itok=OyNbfmyA" alt="Bellabeat Sleep" width="270" height="250"></div>
<hr style="border: none; height: 3px; background-color: #d2b48c;">

## Table of Contents 
[<img src="https://cdn-icons-png.flaticon.com/512/1436/1436664.png" alt="intro" width="30" height="30"> Introduction](#introduction) 
[<img src="https://cdn-icons-png.flaticon.com/512/3782/3782284.png" alt="intro" width="30" height="30"> Ask Phase](#ask) 
[<img src="https://cdn-icons-png.flaticon.com/512/2644/2644445.png" alt="intro" width="30" height="30"> Prepare Phase](#prepare) 
[<img src="https://cdn-icons-png.flaticon.com/512/2974/2974322.png" alt="intro" width="30" height="30"> Process Phase](#process) 
[<img src="https://cdn-icons-png.flaticon.com/512/6471/6471650.png" alt="intro" width="30" height="30">  Analyze and Share Phase](#analyze--share) 
[<img src="https://cdn-icons-png.flaticon.com/512/9196/9196093.png" alt="intro" width="30" height="30"> Act Phase](#act)
<hr style="border: none; height: 3px; background-color: #d2b48c;">

##  [<img src="https://cdn-icons-png.flaticon.com/512/1436/1436664.png" alt="intro" width="40" height="40"> Introduction](#introduction) 

Bellabeat is a successful high-tech company that specializes in health-focused smart products for women. While the company offers a range of smart devices, **the goal of this analysis was to help Bellabeat develop effective marketing strategies** to promote their fitness tracker app based on the insights obtained from analyzing user data. The analysis focused on the correlation between physical activity and sleep patterns, with additional emphasis on the importance of daily step count and its correlation with calories burned. Based on the insights obtained, marketing strategies were proposed, including personalized recommendations, gamification, emphasizing the benefits of tracking daily step count, promoting weight loss, and highlighting the app's ability to optimize workouts and achieve fitness goals faster. The goal of these strategies is to increase user engagement, drive sales, and promote the app as a tool to help users improve their health and well-being.

According to the co-founder and Chief Creative Officer of Bellabeat, analyzing data from smart devices has the potential to uncover new opportunities for the company's growth. **As a data analyst, I have been assigned the responsibility of conducting an analysis of smart device data to gain insights into consumer usage patterns.** Specifically, for this project, I will be analyzing data from a non-Bellabeat device, the Fitbit.

## [<img src="https://cdn-icons-png.flaticon.com/512/3782/3782284.png" alt="intro" width="40" height="40"> Ask Phase](#ask) 

### 2.1 Scope of Work
Before commencing the analysis process, it was crucial to establish a clear scope of work that ensures alignment with business goals, adherence to expected timelines, and production of reliable and actionable results. Consequently, the following deliverables summarize the expected outcomes of this analysis: 

* A clear summary of the business task
* A description of all data sources used
* Documentation of any cleaning or manipulation of data
* A summary of the analysis
* Supporting visualizations and key findings
* Top high-level content recommendations based on the analysis </div>

### 2.2 Business Task
To ensure a successful outcome in the process of analyzing data and extracting valuable insights, the following business objectives are to be prioritized:

* Identify key trends in smart device usage.
* Evaluate how these trends relate to Bellabeat's target audience.
* Determine how these trends can inform and influence Bellabeat's marketing strategy. </div>

### 2.3 Stakeholder / Target Audience
    
* Urška Sršen: Bellabeat’s cofounder and Chief Creative Officer 
* Sando Mur: Mathematician and Bellabeat’s cofounder; key member of the Bellabeat executive team 
* Bellabeat marketing analytics team: A team of data analysts responsible for collecting, analyzing, and reporting data that helps guide Bellabeat’s marketing strategy. </div>

### 2.4 Product Focused
As previously stated, the primary product that will be the focus of this analysis is the Bellabeat app. The app offers users health data pertaining to their activity, sleep, stress, menstrual cycle, and mindfulness habits, enabling them to gain a better understanding of their current habits and make informed decisions about their health. </div>

## [<img src="https://cdn-icons-png.flaticon.com/512/2644/2644445.png" alt="intro" width="40" height="40"> Prepare Phase](#prepare) 
### 3.1 Data Used
The "FitBit Fitness Tracker Data" dataset is available on Kaggle under the CC0 Public Domain license, and was made accessible through the user, Mobius. This dataset contains personal fitness tracker data collected from thirty eligible Fitbit users who consented to the submission of minute-level output for physical activity, heart rate, and sleep monitoring. The dataset was generated through a distributed survey via Amazon Mechanical Turk between March 12, 2016 and May 12, 2016.

### 3.2 Data Usage Rights</div>
To ensure my rights to use this data and upon further investigation of the CC0 Public Domain license, it has been confirmed that the individual who shared this dataset has waived all rights to the work worldwide under copyright law. This means that the data can be freely copied, modified, distributed, or used for commercial purposes, without requiring any permission.

### 3.2 Data Breakdown
There are a total of 18 datasets available in CSV file format. The majority of the datasets are structured in a long format, with a few containing over 2,483,658 observations. However, there are a few exceptions that are presented in a wide format with approximately 62 attributes. The table below provides a summary of each dataset and its characteristics:

| Dataset Name | Structure Type | Description | Column Names | 
| :---  | :--- | :--- | :--- |
| dailyActivity_merged | Long Format | 15 Columns & 941 Rows |  Id, ActivityDate, TotalSteps, TotalDistance, TrackerDistance, LoggedActivitiesDistance, VeryActiveDistance, ModeratelyActiveDistance, LightActiveDistance, SedentaryActiveDistance, VeryActiveMinutes, FairlyActiveMinutes, LightlyActiveMinutes, SedentaryMinutes, Calories |
|dailyCalories_merged | Long Format | 3 Columns & 941 Rows | Id, ActivityDay, Calories |
| dailyIntensities_merged | Long Format | 9 Columns & 941 Rows | Id, ActivityDay, SedentaryMinutes, LightlyActiveMinutes, FairlyActiveMinutes, VeryActiveMinutes, SedentaryActiveDistance, LightActiveDistance, ModeratelyActiveDistance, VeryActiveDistance |
| dailySteps_merged | Long Format | 3 Columns & 941 Rows | Id, ActivityDay, StepTotal |
| heartrate_seconds_merged | Long Format | 3 Columns & 2,483,658 Rows | Id, Time, Value |
| hourlyCalories_merged | Long Format | 3 Columns & 22,100 Rows | Id, ActivityHour, Calories |
| hourlyIntensities_merged | Long Format | 4 Columns & 22,100 Rows | Id, ActivityHour, TotalIntensity, AverageIntensity |
| hourlySteps_merged | Long Format | 3 Columns & 22,100 Rows | Id, ActivityHour, StepTotal |
| minuteCaloriesNarrow_merged | Long Format | 3 Columns & 1,325,580 Rows | Id, ActivityMinute, Calories |
| minuteCaloriesWide_merged | Wide Format | 62 Columns & 21,646 Rows | Id, ActivityHour, Calories00 to Calories59 |
| minuteIntensitiesNarrow_merged | Long Format | 3 Columns & 1,325,580 Rows | Id, ActivityMinute, Intensity |
| minuteIntensitiesWide_merged | Wide Format | 62 Columns & 21,646 Rows | Id, ActivityHour, Intensity00 to Intensity59 |
| minuteMETsNarrow_merged | Long Format | 3 Columns & 1,325,580 Rows | Id, ActivityMinute, METs |
| minuteSleep_merged | Long Format | 4 Columns & 188,522 Rows | Id, date, value, LogId | 
| minuteStepsNarrow_merged | Long Format | 3 Columns & 1,325,580 Rows | Id, ActivityMinute, Steps | 
| minuteStepsWide_merged | Wide Format | 62 Columns & 21,646 Rows | Id, ActivityHour, Steps00 to Steps59 |
| sleepDay_merged | Long Format | 5 Columns & 414 Rows | Id, SleepDay, TotalSleepRecords, TotalMinutesAsleep, TotalTimeInBed |
| weightLogInfo_merged | Long Format | 8 Columns & 68 Rows | Id, Date, WeightKg, WeightPounds, Fat, BMI, IsManualReport, LogId |

### 3.3 Data Credibility & Integrity
When analyzing the used data, it is essential to consider its strengths and limitations. The data was obtained from a third party, Kaggle/Mobius, and while it appears to be accurate, the original source (Amazon) cannot be verified, thus making it potentially unreliable. 

Moreover, the data is limited in scope, covering only the months from March to May, and therefore may not be as comprehensive as desired for gathering meaningful insights. The data is also outdated, being taken 7 years ago, and may not accurately reflect current technology and smart device adoption. 

Additionally, the sample size is biased and does not represent the overall population, although it is still acceptable for the purpose of this case study. Despite these limitations, the data still provides valuable insights into the topic under investigation.

## [<img src="https://cdn-icons-png.flaticon.com/512/2974/2974322.png" alt="intro" width="40" height="40"> Process Phase](#process) 
 This phase is a critical component of data analytics, as it establishes the foundation for subsequent analysis. By ensuring that the data is clean, complete, and consistent, accurate and reliable insights can be achieved to facilitate decision-making.
 
###  4.1 Moving Forward Strategy
At this stage of the analysis, I considered which tools would be best suited for performing the analysis moving forward. After careful consideration, I decided to use R for the following reasons:

* Spreadsheets: For this particular case, spreadsheets were not the ideal method for cleaning the data, as some of the datasets contained large amounts of rows that could not be opened without losing data.
* SQL: Working with SQL presented some challenges, although not insurmountable. The main drawback was the formatting of the Date & Time column in the datasets. Unfortunately, BigQuery did not recognize the original format of this column, so the only way to upload the datasets was by writing a query that specified the format of each column. Additionally, it is important to note that uploading tables via a query may not work with a BigQuery Sandbox account.
* R: After considering the other options, R appeared to be the most suitable tool for this project. It allowed for easy upload of the datasets and provided a range of visualization options that helped to further explain the analysis.


### 4.2 Uploading Datasets
Prior to uploading any datasets in R, I needed to determine which libraries would be used throughout the analysis. However, if an additional library was needed at any point, I simply downloaded and included it with the other libraries in my code. 

The following libraries were used: 
~~~ r
library(tidyverse)
library(readr)
library(dplyr)
library(lubridate)
library(hms)
library(janitor)
library(ggplot2)
library(cowplot)
library(scales)
library(ggpubr)
~~~
After downloading the aforementioned libraries, the next step was to upload the datasets that would be used in the analysis. Keeping in mind the business task at hand and the insights that could inform potential recommendations for the Bellabeat app, I focused on the following datasets:
    
* dailyActivity
* sleepDay
* hourlyCalories
* hourlySteps
* hourlyIntensities
* heartrate_seconds 
~~~ r
daily_activity <- read.csv(file= "../input/fitbit/Fitabase Data 4.12.16-5.12.16/dailyActivity_merged.csv")
daily_sleep <- read.csv(file= "../input/fitbit/Fitabase Data 4.12.16-5.12.16/sleepDay_merged.csv")
hourly_calories <- read.csv(file= "../input/fitbit/Fitabase Data 4.12.16-5.12.16/hourlyCalories_merged.csv")
hourly_steps <- read.csv(file= "../input/fitbit/Fitabase Data 4.12.16-5.12.16/hourlySteps_merged.csv")
hourly_intensities <- read.csv(file= "../input/fitbit/Fitabase Data 4.12.16-5.12.16/hourlyIntensities_merged.csv")
heart_rate_sec <- read.csv(file= "../input/fitbit/Fitabase Data 4.12.16-5.12.16/heartrate_seconds_merged.csv")
~~~
### 4.3 Cleaning & Formatting Data
Upon uploading the datasets and reviewing the structure of each, the next step was to check for data integrity and begin the process of cleaning the data.

#### Consistency
To ensure uniformity of the data and accurate comparisons and analyses, I will begin by transforming the column names to a more consistent and clean style. </div>

~~~ r
daily_activity <- clean_names(daily_activity)
daily_sleep <- clean_names(daily_sleep)
heart_rate_sec <- clean_names(heart_rate_sec)  
hourly_calories <- clean_names(hourly_calories)
hourly_steps <- clean_names(hourly_steps)
hourly_intensities <- clean_names(hourly_intensities)
~~~

To further ensure consistency across all datasets, I wanted to confirm that all ID numbers were of a consistent length. If I found any inconsistencies, I would investigate whether it was due to an incorrect entry or whether the users' IDs were indeed of different lengths.
~~~ r
id_length1<- daily_activity %>%
  group_by(id) %>% 
  reframe(id_len = nchar(id)) %>% 
  distinct(id, id_len) 
id_length1

id_length2<- daily_sleep %>%
  group_by(id) %>% 
  reframe(id_len = nchar(id)) %>% 
  distinct(id, id_len)  
id_length2

id_length3<- hourly_calories %>%
  group_by(id) %>% 
  reframe(id_len = nchar(id)) %>% 
  distinct(id, id_len)  
 id_length3

id_length4<- hourly_steps %>%
  group_by(id) %>% 
  reframe(id_len = nchar(id)) %>% 
  distinct(id, id_len)  
id_length4

id_length5<- hourly_intensities %>%
  group_by(id) %>% 
  reframe(id_len = nchar(id)) %>% 
  distinct(id, id_len) 
id_length5

id_length6<- heart_rate_sec %>%
  group_by(id) %>% 
  reframe(id_len = nchar(id)) %>% 
  distinct(id, id_len)
id_length6
~~~
It was found that the length of the user IDs was consistent across all datasets, but not the number of unique users. After analyzing the results, it was found that most datasets had 33 unique users except for daily_sleep, which had 24 unique users, and heart_rate_sec, which had 14 unique users. This discrepancy will be taken into consideration during the analysis phase.

#### Correct Columns Data Type
As observed in the previous steps, many of the datasets contained a column with a date and/or time in an incorrect data type, such as &lt;chr&gt;. To facilitate the analysis and improve its effectiveness, I opted to split the date and time into separate columns, where possible, and corrected their data types to &lt;date&gt; and &lt;time&gt;, respectively.

~~~ r
# Since time was not provided, this only corrects the date column data type
daily_activity <- daily_activity %>% 
  mutate(activity_date = mdy(activity_date)) %>% 
  mutate(activity_date = as.Date(activity_date)) %>% 
  rename(date = activity_date)

daily_sleep <- daily_sleep %>% 
  mutate(sleep_day = mdy_hms(sleep_day)) %>% 
  mutate(sleep_day = as.Date(sleep_day)) %>% 
  rename(date = sleep_day)

# Separates date and time into different columns and corrects columns data type
hourly_calories <- hourly_calories %>% 
  mutate(activity_hour = mdy_hms(activity_hour)) %>% 
  separate(activity_hour,into=c("date", "time"), sep=" ") %>% 
  mutate(date=as.Date(date), time=as_hms(time))

hourly_steps <- hourly_steps %>% 
  mutate(activity_hour = mdy_hms(activity_hour)) %>% 
  separate(activity_hour,into=c("date", "time"), sep=" ") %>% 
  mutate(date=as.Date(date), time=as_hms(time))

hourly_intensities <- hourly_intensities %>% 
  mutate(activity_hour = mdy_hms(activity_hour)) %>% 
  separate(activity_hour,into=c("date", "time"), sep=" ") %>% 
  mutate(date=as.Date(date), time=as_hms(time))

heart_rate_sec <- heart_rate_sec %>% 
  mutate(time = mdy_hms(time)) %>% 
  separate(time,into=c("date", "time"), sep=" ") %>% 
  mutate(date=as.Date(date), time=as_hms(time))
~~~
#### Duplicates Check & Removal
Removing duplicates from data is important as it can significantly impact the accuracy and reliability of the results. Duplicate records can lead to skewed results, bias, and inaccurate conclusions to be drawn. 

For this step, I opted for two slightly different approaches to check for duplicates, depending on the type of dataset:

1. Datasets with a limited number of columns: This first approach involves checking the entire row and finding duplicated rows within the dataset. 
~~~r
sum(duplicated(heart_rate_sec))

sum(duplicated(hourly_calories))

sum(duplicated(hourly_intensities))

sum(duplicated(hourly_steps))
~~~
2. Datasets with multiple columns: The second approach aims to detect duplicates by combining the id and date columns rather than examining the entire row. By merging the id-date observations, the approach is designed to identify any duplicates in the dataset based on this criteria. The rationale behind this strategy is to prevent the possibility of having different observations values for the same user and date, thereby ensuring the accuracy and reliability of the analysis.
~~~r 
dup_entries_count1 <- daily_activity %>%
  mutate(combined = paste(id, as.character(date), sep = "_")) %>%
  filter(duplicated(combined)) %>% 
  nrow()
dup_entries_count1
 
dup_entries_count2 <- daily_sleep %>%
  mutate(combined = paste(id, as.character(date), sep = "_")) %>%
  filter(duplicated(combined)) %>% 
  nrow()
dup_entries_count2
~~~
Based on my previous analysis, I was able to determine that the daily_sleep data frame had three duplicates that need to be removed
~~~r
daily_sleep <- daily_sleep %>%
  distinct() 

# Double checks that daily_sleep no longer has duplicates
dup_entries_count3 <- daily_sleep %>%
  mutate(combined = paste(id, as.character(date), sep = "_")) %>%
  filter(duplicated(combined)) %>% 
  nrow()
dup_entries_count3
~~~
#### Finding Missing & N/A Values
Missing values can have a negative impact on data analysis, often skewing the results. However, when I first observed all eighteen datasets, I noticed that one of them contained a column with many missing values. Therefore, before blindly removing entire rows due to NA or missing observations, I wanted to double-check whether any of the datasets being used for this analysis were incomplete. 
~~~r
missing_values1 <- daily_activity %>%
  mutate_if(is.Date, as.character) %>% #This code line is required to perform the next function
  summarize_all(~sum(is.na(.) | . == ""))
missing_values1 

missing_values2 <- daily_sleep %>%
  mutate_if(is.Date, as.character) %>% #This code line is required to perform the next function
  summarize_all(~sum(is.na(.) | . == ""))
missing_values2

missing_values3 <- hourly_calories %>%
  mutate_if(is.Date, as.character) %>% #This code line is required to perform the next function
  summarize_all(~sum(is.na(.) | . == ""))
missing_values3

missing_values4 <- hourly_steps %>%
  mutate_if(is.Date, as.character) %>% #This code line is required to perform the next function
  summarize_all(~sum(is.na(.) | . == ""))
missing_values4

missing_values5 <- hourly_intensities %>%
  mutate_if(is.Date, as.character) %>% #This code line is required to perform the next function
  summarize_all(~sum(is.na(.) | . == ""))
missing_values5

missing_values6 <- heart_rate_sec %>%
  mutate_if(is.Date, as.character) %>% #This code line is required to perform the next function
  summarize_all(~sum(is.na(.) | . == ""))
missing_values6
~~~

## [<img src="https://cdn-icons-png.flaticon.com/512/6471/6471650.png" alt="intro" width="30" height="30">  Analyze and Share Phase](#analyze--share) 

The aim of the analyze phase is to gain a deeper understanding of the data and draw actionable insights that can help Bellabeat make informed decisions based on the data.I will proceed with performing various analyses and modeling techniques on the data in order to extract insights, patterns, and relationships that can inform decision-making. 

### 5.1 User Category
To begin my analysis of the cleaned data, I decided to first understand the users and their categorization in a more comprehensive manner. It's important to note that the aim of categorization is not to generalize or stereotype individuals but rather to identify patterns and differences across various groups. Given that demographic area, gender, age, or occupation cannot be used to categorize users based on the available data, I concluded that activity levels would be the most appropriate variable for this purpose.

During my extensive research on activity levels, I came across an article that defined different activity levels and provided a framework for categorizing users based on their daily step count. The article outlined the following levels of activity based on the total number of steps per day, which I used for my analysis:

* Sedentary: less than 5,000 steps per day
* Lightly active: 5,000 to 7,499 steps per day
* Fairly active: 7,500 to 9,999 steps per day
* Very active: more than 10,000 steps per day
* Note that the step goal of 10,000 is the recommended daily step target for healthy adults

This data was gathered from the website "10,000 Steps" (https://www.10000steps.org.au/articles/healthy-lifestyles/counting-steps/).

For this particular analysis, I will be using the daily_activity dataset, which comprises 33 distinct users. I will generate a data frame that includes the activity level category, standard deviation, and lower standard deviation limit for each user, providing a comprehensive understanding of their activity levels based on their daily step count. 
~~~r
user_type <- daily_activity %>% 
  group_by(id) %>% 
  summarise(avg_steps=mean(total_steps), sd=sd(total_steps), lower_sd=mean(total_steps)-sd(total_steps)) %>% 
  mutate(user_type = case_when(
    avg_steps < 5000 ~ "sedentary",
    avg_steps >= 5000 & avg_steps < 7500 ~ "lightly active", 
    avg_steps >= 7500 & avg_steps < 10000 ~ "fairly active", 
    avg_steps >= 10000 ~ "very active"
  )) %>% 
  arrange(avg_steps)
head(user_type)
~~~

![User Activity Level Category Plot](User Activity Level Category Plot2.png)



