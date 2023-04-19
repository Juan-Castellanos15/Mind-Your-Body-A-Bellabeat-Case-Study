<h1 align="center"><img src="https://cdn-icons-png.flaticon.com/512/3048/3048398.png" alt="Bellabeat Sleep" width="55" height="55">  Mind Your Body  <img src="https://cdn-icons-png.flaticon.com/512/3048/3048398.png" alt="Bellabeat Sleep" width="55" height="55"></h1>

<h2 align="center">How Bellabeat Helps Users Optimize Physical Activity and Sleep</h2>

<div align="center"><img src="https://i.giphy.com/media/26BRq9PYFLeJl3WLu/giphy.webp" alt="Bellabeat Fit" width="270" height="250"> <img src="https://news.mit.edu/sites/default/files/styles/news_article__image_gallery/public/images/202009/MIT-Sleep-Positions-01-ani_0.gif?itok=OyNbfmyA" alt="Bellabeat Sleep" width="270" height="250"></div>
<hr style="border: none; height: 3px; background-color: #d2b48c;">

## Table of Contents 

<img src="https://cdn-icons-png.flaticon.com/512/1436/1436664.png" alt="introduction" width="30" height="30"> [1. Introduction](#introduction) 

<img src="https://cdn-icons-png.flaticon.com/512/3782/3782284.png" alt="ask" width="30" height="30"> [2. Ask Phase](#ask)
 
<img src="https://cdn-icons-png.flaticon.com/512/2644/2644445.png" alt="prepare" width="30" height="30"> [3. Prepare Phase](#prepare) 

<img src="https://cdn-icons-png.flaticon.com/512/2974/2974322.png" alt="process" width="30" height="30"> [4. Process Phase](#process)
 
<img src="https://cdn-icons-png.flaticon.com/512/6471/6471650.png" alt="analyze--share" width="30" height="30">  [5. Analyze and Share Phase](#analyze--share) 

<img src="https://cdn-icons-png.flaticon.com/512/9196/9196093.png" alt="act" width="30" height="30"> [6. Act Phase](#act)

<hr style="border: none; height: 3px; background-color: #d2b48c;">

##  <img src="https://cdn-icons-png.flaticon.com/512/1436/1436664.png" alt="introduction" width="40" height="40"> [1. Introduction](#introduction) 

Bellabeat is a successful high-tech company that specializes in health-focused smart products for women. While the company offers a range of smart devices, **the goal of this analysis was to help Bellabeat develop effective marketing strategies** to promote their fitness tracker app based on the insights obtained from analyzing user data. The analysis focused on the correlation between physical activity and sleep patterns, with additional emphasis on the importance of daily step count and its correlation with calories burned. Based on the insights obtained, marketing strategies were proposed, including personalized recommendations, gamification, emphasizing the benefits of tracking daily step count, promoting weight loss, and highlighting the app's ability to optimize workouts and achieve fitness goals faster. The goal of these strategies is to increase user engagement, drive sales, and promote the app as a tool to help users improve their health and well-being.

According to the co-founder and Chief Creative Officer of Bellabeat, analyzing data from smart devices has the potential to uncover new opportunities for the company's growth. **As a data analyst, I have been assigned the responsibility of conducting an analysis of smart device data to gain insights into consumer usage patterns.** Specifically, for this project, I will be analyzing data from a non-Bellabeat device, the Fitbit.

## <img src="https://cdn-icons-png.flaticon.com/512/3782/3782284.png" alt="ask" width="40" height="40"> [2. Ask Phase](#ask) 

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

## <img src="https://cdn-icons-png.flaticon.com/512/2644/2644445.png" alt="prepare" width="40" height="40"> [3. Prepare Phase](#prepare) 
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

## <img src="https://cdn-icons-png.flaticon.com/512/2974/2974322.png" alt="process" width="40" height="40"> [4. Process Phase](#process) 
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

## <img src="https://cdn-icons-png.flaticon.com/512/6471/6471650.png" alt="analyze--share" width="40" height="40">  [5. Analyze and Share Phase](#analyze--share) 

The aim of the analyze phase is to gain a deeper understanding of the data and draw actionable insights that can help Bellabeat make informed decisions based on the data.I will proceed with performing various analyses and modeling techniques on the data in order to extract insights, patterns, and relationships that can inform decision-making. 

### 5.1 User Category
To begin my analysis of the cleaned data, I decided to first understand the users and their categorization in a more comprehensive manner. It's important to note that the aim of categorization is not to generalize or stereotype individuals but rather to identify patterns and differences across various groups. Given that demographic area, gender, age, or occupation cannot be used to categorize users based on the available data, I concluded that activity levels would be the most appropriate variable for this purpose.

During my extensive research on activity levels, I came across an article that defined different activity levels and provided a framework for categorizing users based on their daily step count. The article outlined the following levels of activity based on the total number of steps per day, which I used for my analysis:

* Sedentary: less than 5,000 steps per day
* Lightly active: 5,000 to 7,499 steps per day
* Fairly active: 7,500 to 9,999 steps per day
* Very active: more than 10,000 steps per day
* Note that the step goal of 10,000 is the recommended daily step target for healthy adults

This data was gathered from the source [10,000 Steps](https://www.10000steps.org.au/articles/healthy-lifestyles/counting-steps/).

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
<img src="https://user-images.githubusercontent.com/130716302/232902956-930a76c4-8322-4e1c-a6de-849a79892f0c.png" alt="User Activity Level Category" width="300">

The user_type data frame obtained above provides valuable insights regarding the users' step count. Based on this data, the following conclusions can be drawn:
    
- Some users have negative values when subtracting one standard deviation from their average step count. Typically, these negative values belong to sedentary users, whose average daily step count is very low and whose daily step count is highly dispersed throughout the week, resulting in a high standard deviation. In reality, it's impossible for a user to have negative step counts. Therefore, "sedentary" and "lightly active" users should aim to increase their average daily step count and be more consistent throughout the week to improve their overall health and wellbeing.
- Although fairly active users are closer to reaching the goal of 10,000 daily steps, it's highly recommended that they include additional walks throughout the day to achieve this goal. Upon evaluating their standard deviation, it is also noted that it is fairly high, which suggests that there is room for consistency. By eventually adding more walks to reach the 10,000 daily steps goal, the standard deviation is likely to decrease, resulting in a more predictable and consistent step count. This will ultimately lead to improved health and wellbeing.
- For the very active users, I would encourage them to keep up the good work and consider including additional walks to maintain a step count above 10,000 for days when they don't work or when they aren't as active as usual.   

To facilitate a better understanding of the user categories, I will create a pie chart that displays their respective population percentages.
~~~r
activity_levels_percentage <- user_type %>%
  group_by(user_type) %>%
  summarize(count = n()) %>%
  mutate(percentage = percent(count / sum(count)))
head(activity_levels_percentage)

ggplot(activity_levels_percentage, mapping=aes(x="", y=percentage, fill=user_type)) +
  geom_bar(stat="identity") +
  coord_polar(theta = "y") +
  theme_minimal() +
  geom_text(aes(label=paste(user_type, "\n", percentage)),
            position = position_stack(vjust=0.5),
            show.legend=FALSE, fontface="bold", size=5) +
  theme(axis.title.x= element_blank(),
        axis.title.y = element_blank(),
        panel.border = element_blank(), 
        panel.grid = element_blank(), 
        axis.ticks = element_blank(),
        axis.text.x = element_blank(),
        plot.title = element_text(hjust=0.5, size=14, face="bold")) +
  guides(fill = FALSE) +
  labs(title = "User Activity Level Category")
~~~
<img src="https://user-images.githubusercontent.com/130716302/232825901-04f96b49-05f8-454b-ad69-4d52419c6e40.png" alt="Activity Category" width="300">

After analyzing the results, it can be concluded that the distribution of users across the various activity level categories is fairly even, with each category representing between 21.2% and 27.3% of the total user population. However, a significant proportion of users fall into the "sedentary" (24.2%), "lightly active" (27.3%) and "fairly active" (27.3%) categories, indicating the need for interventions or strategies to promote physical activity, particularly among sedentary and lightly active individuals.

### 5.2 Combining Datasets
To conduct further in-depth analysis and identify patterns and relationships across the available datasets, I will combine them where feasible. It is important to note that these datasets may contain a different number of unique users (as shown in the cleaning phase) which should be taken into consideration during the analysis.

I will proceed by combining the daily_activity and daily_sleep datasets, resulting in a combined data frame named daily_data, which will include data from 24 unique users. Additionally, I will combine the hourly_steps, hourly_calories, and hourly_intensities datasets to create a new data frame named hourly_data, which will include data from 33 unique users. While it is not ideal to have a reduced number of unique users in the daily_data data frame (24 users), we will proceed with this outcome to facilitate further analysis.
~~~r
daily_data <- left_join(daily_activity, daily_sleep, by = c("id", "date")) %>% 
  drop_na()
head(daily_data)

hourly_data <- hourly_calories %>% 
  left_join(hourly_steps, by = c("id", "date", "time")) %>% 
  left_join(hourly_intensities, by = c("id", "date", "time")) %>% 
  drop_na()
head(hourly_data)
~~~
### 5.3 Fitness Smart Device Usage
In this analysis, I aimed to understand the frequency of users' daily and hourly usage of their fitness smart device. Furthermore, the correlation between daily and hourly usage was explored to provide insights that could be used to improve marketing strategies aimed at promoting physical activity and healthy habits, depending on the obtained results.

First, I will determine the total number of unique days recorded in the daily_data dataframe. Subsequently, I will employ this outcome to derive a percentage value by creating a new dataframe grouped by Id. This newly created dataframe will display the usage number of days and hours per user, alongside their corresponding percentage values.

~~~r
total_days <- daily_data %>% 
  summarise(total_days = n_distinct(date))

user_usage <- daily_data %>%
  group_by(id) %>% 
  reframe(days_used = n_distinct(date), hours_used=round((very_active_minutes+
              fairly_active_minutes+lightly_active_minutes+sedentary_minutes)/60,1)) %>% 
  mutate(days_usage_percentage=round(days_used/total_days$total_days*100), 
        hours_usage_percentage=round(hours_used/24*100)) %>% 
  distinct(id, .keep_all = TRUE)
head(user_usage)
~~~
Finally, to determine if there is a correlation between daily and hourly usage, I will create a scatter plot to assess whether there is a negative, positive, or no correlation.
~~~r
ggplot(user_usage, aes(x=days_usage_percentage, y=hours_usage_percentage)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title = "Days vs Hours Usage", x = "Days Usage", y= "Hours Usage") +
  theme(plot.title = element_text(hjust=0.5))
~~~
<img src="https://user-images.githubusercontent.com/130716302/232828243-8ce58e3b-5328-4712-bd9f-672912663b46.png"  alt="Days vs Hours" width="250">

A fairly flat line of best fit on a scatter plot suggests that there is little to no correlation between the two variables being plotted, in this case daily and hourly usage. It implies that the daily usage of the fitness smart device does not necessarily determine the hourly usage and vice versa.

This suggests that marketing campaigns could promote not only daily usage of fitness smart devices but also the benefits of incorporating physical activity throughout the day. This could involve activities such as taking the stairs instead of the elevator, going for a walk during lunch breaks, doing stretching exercises at a desk, or standing up and moving around every hour. The aim is to increase overall physical activity levels and promote better health by integrating more movement into everyday activities.

Additionally, targeting specific user groups who are more likely to engage in physical activity at certain times of the day could be a more effective approach, which I will explore further in the next steps.

### 5.4 Physical Activity Levels

In this next analysis, I will examine the activity levels of users on a daily and hourly basis. To obtain a broader perspective of the activity levels, I will calculate the average step count from all users and present the findings in a plot to better visualize the patterns.

First, I will obtain the average step count from Sunday to Saturday and organize the data in a dataframe.
~~~r
weekly_active <- daily_data %>% 
  mutate(day_of_week = wday(date, label= TRUE)) %>% 
  group_by(day_of_week) %>% 
  summarise(avg_daily_steps = mean(total_steps))
head(weekly_active)
~~~
Using the weekly_active dataframe mentioned above, I will now visualize the results in a bar graph.
~~~r
daily_steps_plot <- ggplot(weekly_active, mapping=aes(x=day_of_week, y=avg_daily_steps))+ 
  geom_bar(stat="identity", fill="#F8766D")+
  geom_hline(yintercept = mean(weekly_active$avg_daily_steps), color = "black", size=1.2) +
  annotate("text", x=.95, y=mean(weekly_active$avg_daily_steps), 
           label=paste0("Avg:", round(mean(weekly_active$avg_daily_steps), 0)), size=3.3, vjust=-0.5) +
  labs(title="Average User Steps by Day of Week", x="Day of Week", y= "Average User Steps")+
  theme(plot.title = element_text(hjust=0.5))
print(daily_steps_plot)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232834527-e5156852-a5cb-4e7c-8f52-1717b8d4fa75.png" alt="Daily Steps" width="250">

Based on the "daily_steps_plot" bar graph above, the following conclusions can be drawn:

-   The average daily steps from Sunday to Saturday is below the 10,000 step goal. This is consistent with the previous analysis, which showed that nearly 80% of users fall into the sedentary, lightly, and fairly active categories, all of which have step counts that are below the desired goal.
-   It is evident that Sunday has the lowest number of steps compared to the rest of the week. This could suggest that users take Sunday as a day of rest and engage in fewer physical activities. However, as typically people have more free time on Sunday, it could present a perfect opportunity to add extra steps and increase the average step count.
-   It is not clear why there are relatively fewer steps on Wednesday, Thursday, and Friday compared to Monday and Tuesday, which are typical work weekdays.

Next, I will obtain the average step count on hourly basis and organize the data in a dataframe.
~~~r
daily_active <- hourly_data %>% 
  group_by(time) %>% 
  summarise(avg_hourly_steps = mean(step_total))
head(daily_active)
~~~
Using the daily_active dataframe mentioned above, I will now visualize the results in a bar graph.
~~~r
hourly_steps_plot <- ggplot(daily_active, mapping=aes(x=time, y=avg_hourly_steps)) +
  geom_bar(stat="identity", fill="#619CFF")+
  geom_hline(yintercept = mean(daily_active$avg_hourly_steps), color = "black", size=1.2) +
  annotate("text", x=1, y=mean(daily_active$avg_hourly_steps),
           label=paste0("Avg:", round(mean(daily_active$avg_hourly_steps))), 
           size=3.3, vjust=-0.5, hjust=0.4) +
  labs(title="", x="", y="") +
  theme(plot.title = element_text(size=7,hjust=0.5), axis.text.x = element_text(angle=45, hjust=1))
print(hourly_steps_plot)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232835548-69e3059c-24ac-4eeb-894d-d65ca6e339d9.png" alt="Hourly Steps" width="250">

Based on the "hourly_steps_plot" bar graph above, the following conclusions can be drawn:

-   Based on the analysis of the average step count on an hourly basis, it is observed that users tend to be more active between 8am to 8pm.
-   The data shows a peak step count during the hours of 6-7pm. There could be several reasons for this trend. One possibility is that people tend to be more active during the evening hours after finishing their work or daily chores.
-   The evening hours may provide a more convenient time for physical activity as people have more free time to engage in exercise or leisure activities.
-   It is important to note that this is a general trend, and there may be variations among different user groups based on their lifestyles and preferences.

Combining the daily and hourly results, we can conclude that users are more active during the day, but their overall daily activity levels are not meeting the recommended goal. This suggests that marketing campaigns could focus on encouraging users to incorporate more physical activity throughout the day to increase their overall activity levels and promote better health.

### 5.5 Physical Activity Comparisons

#### Daily Step Comparisons

To gain a more comprehensive understanding of activity levels, I will perform a detailed analysis including comparisons of the activities of different user categories.

My first comparison will involve comparing the daily step activity of "very active" users with that of users in other categories such as "sedentary," "lightly active," and "fairly active." For this purpose, I will create two different dataframes, one for very active users and another for users in the remaining categories. It is important to note that very active users are defined as those whose step count exceeds 10,000 steps, as discussed earlier in my analysis.
~~~r
very_active_daily <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps > 10000) %>% 
  select(id) %>%
  inner_join(daily_data, by = "id") %>% 
  mutate(day_of_week = wday(date, label= TRUE)) %>% 
  group_by(day_of_week) %>% 
  summarise(avg_daily_steps = mean(total_steps))
head(very_active_daily)

less_active_daily <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps < 10000) %>% 
  select(id) %>%
  inner_join(daily_data, by = "id") %>% 
  mutate(day_of_week = wday(date, label= TRUE)) %>% 
  group_by(day_of_week) %>% 
  summarise(avg_daily_steps = mean(total_steps))
head(less_active_daily)
~~~
To compare the two different dataframes, I will create a bar graph for each and plot them side by side. This will visually facilitate the identification of significant differences.
~~~r
very_active_daily_plot <- ggplot(very_active_daily, mapping=aes(x=day_of_week, y=avg_daily_steps))+ 
  geom_bar(stat="identity", fill="#F8766D")+
  geom_hline(yintercept = mean(very_active_daily$avg_daily_steps), color = "black", size=1) +
  annotate("text", x=.95, y=mean(very_active_daily$avg_daily_steps), 
           label=paste0("Avg:", round(mean(very_active_daily$avg_daily_steps))), size=2.5, vjust=-0.5, hjust=-1) +
  labs(title="Very Active Daily Average Steps", x="Day of Week", y= "Very Active User Steps")+
  theme(plot.title = element_text(hjust=0.5, size=6), axis.text.x = element_text(angle=45, hjust=1), 
        axis.title = element_text(size=8))+
  ylim(0, 15000)

less_active_daily_plot <- ggplot(less_active_daily, mapping=aes(x=day_of_week, y=avg_daily_steps))+ 
  geom_bar(stat="identity", fill="#F8766D")+
  geom_hline(yintercept = mean(less_active_daily$avg_daily_steps), color = "black", size=1) +
  annotate("text", x=.95, y=mean(less_active_daily$avg_daily_steps), 
           label=paste0("Avg:", round(mean(less_active_daily$avg_daily_steps))), size=2.5, vjust=-0.5, hjust=-1) +
  labs(title="Less Active Daily Average Steps", x="Day of Week", y= "Less Active User Steps")+
  theme(plot.title = element_text(hjust=0.5, size=6), axis.text.x = element_text(angle=45, hjust=1), 
        axis.title = element_text(size=8)) + 
  ylim(0, 15000)

combined_daily_plots <- ggarrange(very_active_daily_plot, less_active_daily_plot, ncol = 2) %>% 
  ggdraw() +
  draw_label("") 
print(combined_daily_plots)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232836331-89a027ab-0e3f-4977-94fa-b67824bb6dcb.png" alt="Daily Steps Comparison" width="350">

Based on the "combined_daily_plots" bar graph above, the following conclusions can be drawn:

-   It is quite apparent that users who are less active should increase their physical activity and incorporate additional steps into their daily routine to enhance their well-being. On average, it is recommended that they walk approximately 2,500 more steps per day.
-   The most noticeable difference between very active and less active users is observed on Saturdays, where very active users take significantly more steps than the average, whereas the same cannot be said for less active users. Although less active users do increase their step count on Saturdays, the increase is not significant enough to narrow the gap with the very active users. Hence, it is recommended that less active users should strive to increase their physical activity levels on weekends, especially on Saturdays, to enhance their overall health and wellbeing.
-   If the less active users were able to match the step count of very active users on Saturdays and Sundays, their average daily step count would dramatically increase to approximately 9,000. This would leave only 1,000 steps to be achieved across five days, with a 200-step increase from Monday to Friday, which seems more attainable.

#### Hourly Step Comparisons

For my second comparison, I will follow a similar analysis process to the one used for the daily step comparison, but this time I will compare the hourly step activity of "very active" users with that of "less active" users. To maintain consistency in my analysis, I will use the same "very active" users identified in the daily dataset and join their IDs to the hourly data. This approach ensures that my analysis remains consistent throughout.
~~~r
very_active_hourly <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps > 10000) %>% 
  select(id) %>%
  inner_join(hourly_data, by = "id") %>% 
  group_by(time) %>% 
  summarise(avg_hourly_steps = mean(step_total))
head(very_active_hourly)

less_active_hourly <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps > 10000) %>% 
  select(id) %>%
  inner_join(hourly_data, by = "id") %>% 
  group_by(time) %>% 
  summarise(avg_hourly_steps = mean(step_total))
head(less_active_hourly)
~~~
As with the previous analysis, I will generate a bar graph for each of the dataframes and display them side by side. This will allow for easier visual identification of any significant differences between the two sets of data. It is important to note that the y and x axis must remain the same to provide an accurate comparison.
~~~r
very_active_hourly_plot <- ggplot(very_active_hourly, mapping=aes(x=time, y=avg_hourly_steps)) +
  geom_bar(stat="identity", fill="#619CFF")+
  geom_hline(yintercept = mean(very_active_hourly$avg_hourly_steps), color = "black", size=1) +
  annotate("text", x=1, y=mean(very_active_hourly$avg_hourly_steps),
           label=paste0("Avg:", round(mean(very_active_hourly$avg_hourly_steps))), size=2.5, vjust=-0.5, hjust=0) +
  labs(title="Very Active Hourly Average Steps", x="Time", y= "Very Active User Steps")+
    theme(plot.title = element_text(hjust=0.5, size=6), axis.text.x = element_text(angle=45, hjust=1), 
        axis.title = element_text(size=8)) +
  scale_y_continuous(limits = c(0, 1400), breaks = seq(0, 1400, by = 200))

less_active_hourly_plot <- ggplot(less_active_hourly, mapping=aes(x=time, y=avg_hourly_steps)) +
  geom_bar(stat="identity", fill="#619CFF")+
  geom_hline(yintercept = mean(less_active_hourly$avg_hourly_steps), color = "black", size=1) +
  annotate("text", x=1, y=mean(less_active_hourly$avg_hourly_steps),
           label=paste0("Avg:", round(mean(less_active_hourly$avg_hourly_steps))), size=2.5, vjust=-0.5, hjust=0.2) +
  labs(title="Less Active Hourly Average Steps", x="Time", y= "Less Active User Steps")+
  theme(plot.title = element_text(hjust=0.5, size=6), axis.text.x = element_text(angle=45, hjust=1), 
        axis.title = element_text(size=8))+
  scale_y_continuous(limits = c(0, 1400), breaks = seq(0, 1400, by = 200))

combined_hourly_plots <- ggarrange(very_active_hourly_plot, less_active_hourly_plot, ncol = 2) %>% 
  ggdraw() +
  draw_label("") 
print(combined_hourly_plots)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232836936-996f19a8-b108-4e12-a409-7ee0b7c5df41.png" alt="Hourly Steps Comparison" width="350">

Based on the "combined_hourly_plots" bar graph above, the following conclusions can be drawn:

-   To rectify previous results, "less active" users should increase their step count throughout the day. The difference in averages seems to be close to 200 steps.
-   The graphs exhibit significant similarities between the hours of 12am to 12pm for both very active and less active users. However, significant differences start to emerge from 1pm onwards. There is a sharp increase in activity for the "very active" users between the hours of 1-3pm, which could be attributed to lunchtime, and evening activities from 4pm to 10pm, which could be attributed to physical activities after work.
-   These results mean that "less active" users may benefit from incorporating physical activity into their lunch breaks and after work hours, in order to increase their overall daily step count and improve their physical health and wellbeing. It is worth noting that this recommendation may vary based on individual work schedules and personal preferences.

### 5.6 Sleep Analysis

Having gained a comprehensive understanding of physical activity, I will shift my focus towards analyzing sleep patterns and insights. Analyzing sleeping patterns is important for several reasons. Firstly, getting adequate sleep is essential for overall health and wellbeing. Understanding sleep patterns can help identify any potential issues, such as insomnia or sleep apnea, which can negatively impact health. Additionally, analyzing sleep patterns can help identify any patterns or habits that may be affecting sleep quality, such as caffeine intake or late-night technology use. Finally, understanding sleep patterns can help individuals optimize their sleep routines, leading to better quality sleep and improved overall health. For the purpose of this analysis and based on the available data, I will only be analyzing the number of hours of sleep and the time it takes for users to fall asleep.

#### Sleep Hours

To commence this analysis, I will create a dataframe that shows the average sleep duration for all users, arranged by day of the week from Sunday to Saturday.
~~~r
asleep_data <- daily_data %>% 
  mutate(day_of_week = wday(date, label= TRUE)) %>% 
  group_by(day_of_week) %>% 
  summarise(avg_sleep_hr = mean(total_minutes_asleep)/60)
head(asleep_data)
~~~
Using the "asleep_data" dataframe above, I will now visualize the results in a bar graph.
~~~r
ggplot(asleep_data, mapping=aes(x=day_of_week, y=avg_sleep_hr))+
  geom_bar(stat="identity", fill="palegreen4")+
  labs(title="Daily Hours of Sleep", x="Day of the Week", y="Asleep Hours")+
  scale_y_continuous(breaks = seq(0, 8, by = 1))+ 
  theme(plot.title = element_text(size=10, hjust=0.5), axis.text.x = element_text(hjust=1))
~~~
<img src="https://user-images.githubusercontent.com/130716302/232837856-91f6392e-6824-4935-9f0a-567707739baf.png" alt="Daily Sleep" width="250">

Based on the bar graph above, the following conclusions can be drawn:

-   Based on the Centers for Disease Control and Prevention (CDC) recommendation of 7 hours or more of sleep per night for adults (source:  [How Much Sleep Do I Need?](https://www.cdc.gov/sleep/about_sleep/how_much_sleep.html)), it appears that the average users in this dataset are getting the recommended amount of sleep, which is 7 hours.
-   While the average sleep hours appear to meet the recommended amount of 7 hours per night, there are some days, namely Tuesday, Thursday, and Friday, where users are falling short of this amount. It is recommended that users aim to increase their sleep hours to improve their overall health and provide sufficient rest for all days of the week.

#### Duration To Fall Asleep

To get a clearer understanding of sleeping patterns, I will analyze the time it takes for users to fall asleep on average. Similar to the steps above, I will create a dataframe that shows the average duration to fall asleep, arranged by day of the week from Sunday to Saturday.
~~~r
falling_asleep_data <- daily_data %>% 
  mutate(day_of_week = wday(date, label= TRUE)) %>% 
  group_by(day_of_week) %>% 
  summarise(avg_falling_sleep = (mean(total_time_in_bed)-mean(total_minutes_asleep))/60)
head(falling_asleep_data)
~~~
Using the "falling_asleep_data" dataframe above, I will now visualize the results in a bar graph.
~~~r
ggplot(falling_asleep_data, mapping=aes(x=day_of_week, y=avg_falling_sleep)) +
  geom_bar(stat="identity", fill="paleturquoise4") +
  geom_hline(yintercept = mean(falling_asleep_data$avg_falling_sleep), color = "black", size=1) +
  annotate("text", x=1, y=mean(falling_asleep_data$avg_falling_sleep),
           label=paste0("Avg:", round(mean(falling_asleep_data$avg_falling_sleep),2), " hr"), 
           size=3, vjust=-0.5, hjust=-1) +
  labs(title="Daily Hours To Fall Asleep", x="Day of the Week", y="Hours To Fall Asleep") +
  scale_y_continuous(breaks = seq(0, 1, by = 0.1)) + 
  theme(plot.title = element_text(size=10, hjust=0.5), axis.text.x = element_text(hjust=1))
~~~
<img src="https://user-images.githubusercontent.com/130716302/232839488-2969e7df-b322-4a44-8638-aca02039e022.png" alt="Daily Fall Asleep" width="250">

Based on the bar graph above, the following conclusions can be drawn:

-   According to the Sleep Foundation study (source:  [How Long Should It Take to Fall Asleep?](https://www.sleepfoundation.org/sleep-faqs/how-long-should-it-take-to-fall-asleep#:~:text=Most%20adults%20with%20healthy%20sleep,sleep%20or%20a%20medical%20condition.html)), it should take an average of 15-20 minutes for an adult to fall asleep on a typical night. However, in this particular case, users are taking an average of 40 minutes (0.66 hours) to fall asleep, which is well beyond the recommended amount.
-   There are various factors that can affect a person's ability to fall asleep quickly or within the recommended timeframe, including disorders, medical conditions, medications, and bedtime routine and environment. However, for the purpose of this analysis, I will focus solely on any physical activity factors that may contribute to a slower ability to fall asleep.

#### Sleep Differences - Very Active vs Less Active Users
In order to delve deeper into the results obtained above, I have decided to perform a separate analysis of "very active" users and "less active" users to potentially gain valuable insights. To accomplish this, I will create two dataframes - one for "very active" users and the other for "less active" users - that display sleep hours and the amount of time it takes to fall asleep for each group.
~~~r
very_active_sleep <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps > 10000) %>% 
  select(id) %>%
  inner_join(daily_data, by = "id") %>% 
  mutate(day_of_week = wday(date, label= TRUE)) %>% 
  group_by(day_of_week) %>% 
  summarise(avg_sleep_hr = mean(total_minutes_asleep)/60, 
            avg_falling_asleep = (mean(total_time_in_bed)-mean(total_minutes_asleep))/60)
head(very_active_sleep)

less_active_sleep <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps < 10000) %>% 
  select(id) %>%
  inner_join(daily_data, by = "id") %>% 
  mutate(day_of_week = wday(date, label= TRUE)) %>% 
  group_by(day_of_week) %>% 
  summarise(avg_sleep_hr = mean(total_minutes_asleep)/60, 
            avg_falling_asleep = (mean(total_time_in_bed)-mean(total_minutes_asleep))/60)
head(less_active_sleep)
~~~
With the use of the previously obtained dataframes, I will now visualize and compare the sleep hours and duration it takes to fall asleep for both very active and less active users.
~~~r
combined_sleep_plots <- ggarrange(
  ggplot(very_active_sleep, mapping=aes(x=day_of_week, y=avg_sleep_hr))+
    geom_bar(stat="identity", fill="palegreen4")+
    geom_hline(yintercept = mean(very_active_sleep$avg_sleep_hr), color = "black", size=1) +
    annotate("text", x=1, y=mean(very_active_sleep$avg_sleep_hr),
             label=paste0("Avg:", round(mean(very_active_sleep$avg_sleep_hr),2)), 
             size=2.5, vjust=-0.5, hjust=-0.8) +
    labs(title="Very Active Sleep Hours", x="Day of the Week", y="Asleep Hours")+
    scale_y_continuous(breaks = seq(0, 8, by = 1))+ 
    theme(plot.title = element_text(size=10, hjust=0.5), axis.text.x = element_text(hjust=1)),
  ggplot(less_active_sleep, mapping=aes(x=day_of_week, y=avg_sleep_hr))+
    geom_bar(stat="identity", fill="palegreen4")+
    geom_hline(yintercept = mean(less_active_sleep$avg_sleep_hr), color = "black", size=1) +
    annotate("text", x=1, y=mean(less_active_sleep$avg_sleep_hr),
             label=paste0("Avg:", round(mean(less_active_sleep$avg_sleep_hr),2)), 
             size=2.5, vjust=-0.5, hjust=0.5) +
    labs(title="Less Active Sleep Hours", x="Day of the Week", y="Asleep Hours")+
    scale_y_continuous(breaks = seq(0, 8, by = 1))+ 
    theme(plot.title = element_text(size=10, hjust=0.5), axis.text.x = element_text(hjust=1)),
  nrow = 2)
print(combined_sleep_plots)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232842704-891b6927-d9ba-41a4-a658-9b87abffbe7e.png" alt="Asleep Comparison" width="350">

~~~r
combined_falling_sleep_plots <- ggarrange(
  ggplot(very_active_sleep, mapping=aes(x=day_of_week, y=avg_falling_asleep)) +
    geom_bar(stat="identity", fill="paleturquoise4") +
    geom_hline(yintercept = mean(very_active_sleep$avg_falling_asleep), color = "black", size=1) +
    annotate("text", x=1, y=mean(very_active_sleep$avg_falling_asleep),
             label=paste0("Avg:", round(mean(very_active_sleep$avg_falling_asleep),2), " hr"), size=3, vjust=-0.5, hjust=-0.2) +
    labs(title="Very Active Falling Asleep Hours", x="Day of the Week", y="Hours To Fall Asleep") +
    scale_y_continuous(breaks = seq(0, 1, by = 0.1)) + 
    theme(plot.title = element_text(size=10, hjust=0.5), axis.text.x = element_text(hjust=1)),
  ggplot(less_active_sleep, mapping=aes(x=day_of_week, y=avg_falling_asleep)) +
    geom_bar(stat="identity", fill="paleturquoise4") +
    geom_hline(yintercept = mean(less_active_sleep$avg_falling_asleep), color = "black", size=1) +
    annotate("text", x=1, y=mean(less_active_sleep$avg_falling_asleep),
             label=paste0("Avg:", round(mean(less_active_sleep$avg_falling_asleep),2), " hr"), size=3, vjust=-0.5, hjust=-1.2) +
    labs(title="Less Active Falling Asleep Hours", x="Day of the Week", y="Hours To Fall Asleep") +
    scale_y_continuous(breaks = seq(0, 1, by = 0.1)) + 
    theme(plot.title = element_text(size=10, hjust=0.5), axis.text.x = element_text(hjust=1)),
  nrow = 2)
print(combined_falling_sleep_plots)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232843195-9c57b60d-a6b8-4d83-a0e0-21d2b9c05dc2.png" alt="Falling Asleep Comparison" width="350">

After analyzing the above graphs, the following conclusions can be drawn:

-   Surprisingly, not every aspect of the "very active" users' lifestyle is beneficial to their well-being. The results indicate that very active users are consistently getting less than the recommended 7 hours of sleep per night, with an average of 6.13 hours on every day of the week except for Sunday, on which they typically get 8 hours.
-   The "less active" users, on average, get more sleep than the "very active" users, with 7.28 hours of sleep per night compared to 6.13 hours for the "very active" users. This observation implies that being very active and engaging in a lot of physical activity during the day, or in the evening, close to bedtime, may have a negative impact on sleep quality or duration.
-   Moreover, the analysis indicates that "very active" users take an average of around 26 minutes longer to fall asleep than "less active" users. This finding suggests that high levels of physical activity may pose a challenge for individuals in falling asleep quickly. The cause could be the physical activity that stimulates their body, making it more challenging for them to relax and unwind before sleep.

#### Further Analysis Support

One suggestion that has yet to be fully confirmed is whether evening physical activity has a negative impact on sleep duration and the time it takes to fall asleep. To investigate this hypothesis, two analyses can be conducted: 1) comparing the heart rate of "very active" users with that of "less active" users to notice eveninig typical rest heart rates, and 2) comparing the evening step activity of both groups.

##### Heart Rate Analysis

For my first analysis, I will use the heart_rate_sec dataset to create two dataframes with hourly heart rates for both "very active" and "less active" users. Next, I will generate a line plot to compare and analyze the heart rates of both caterogies. However, before performing a thorough analysis, it is important to keep in mind that this dataset contains only 14 users as previously discussed. Therfore, I will first check how many "very active" and "less active" users recorded their heart rates and determine whether it makes sense to proceed with this analysis.
~~~r
very_active_heart_rate <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps > 10000) %>% 
  select(id) %>%
  inner_join(heart_rate_sec, by = "id") %>%
  distinct(id)
very_active_heart_rate
~~~
<img src="https://user-images.githubusercontent.com/130716302/232907368-ec72dc9e-bc12-4b7f-9115-50be2b59bcdc.png" alt="Heat Rate" width="300">

Unfortunately, only one "very active" user recorded their heart rate, which is not a reliable representation of the entire "very active" user population. Therefore, I cannot proceed with further analysis using this dataset and method.

##### Evening Steps Comparison

I will now proceed with my second analysis, which involves exploring the evening physical activity data to identify patterns that may impact sleep duration or the time taken to fall asleep. According to an article titled "Evening Hours" on the website incorporated.zone (source: [Evening Hours](https://www.incorporated.zone/evening-hours/)), the evening hours are defined as the period from 6pm to 9pm. However, for this analysis, I will be considering the steps activity data from 6pm to 11pm to allow for a broader time window that includes activity beyond 9pm and encompasses more data points.

Firstly, I will create two dataframes, one for "very active" users and another for "less active" users, displaying the steps recorded from 6pm to 11pm. Then, I will plot them on the same graph in the form of a line graph to compare the results.
~~~r
very_active_evening_steps <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps > 10000) %>% 
  select(id) %>%
  inner_join(hourly_data, by = "id") %>% 
  filter(between(hour(time), 18, 24)) %>% 
  group_by(time) %>% 
  summarise(avg_hourly_steps = mean(step_total))
head(very_active_evening_steps)

less_active_evening_steps <- daily_data %>%
  group_by(id) %>% 
  summarise(avg_daily_steps = mean(total_steps)) %>%
  filter(avg_daily_steps < 10000) %>% 
  select(id) %>%
  inner_join(hourly_data, by = "id") %>% 
  filter(between(hour(time), 18, 24)) %>% 
  group_by(time) %>% 
  summarise(avg_hourly_steps = mean(step_total))
head(less_active_evening_steps)

ggplot() +
  geom_line(data=very_active_evening_steps, aes(x=time, y=avg_hourly_steps, color="Very Active")) +
  geom_line(data=less_active_evening_steps, aes(x=time, y=avg_hourly_steps, color="Less Active")) +
  geom_point(data = very_active_evening_steps, aes(x=time, y=avg_hourly_steps), 
	  size=2.5, shape=21, fill="#FFFFFF", color="red") +
  geom_point(data=less_active_evening_steps, aes(x=time, y=avg_hourly_steps), 
	  size=2.5, shape=21, fill="#FFFFFF", color="blue") +
  labs(title = "Evening Steps", x = "Time", y = "Average Steps") +
  scale_color_manual(values = c("Very Active" = "red", "Less Active" = "blue")) +
  scale_y_continuous(breaks = seq(50, 1400, by = 150)) +
  theme(plot.title = element_text(size = 10, hjust = 0.5), 
	  axis.text.x = element_text(angle = 45, hjust = 1))
~~~
<img src="https://user-images.githubusercontent.com/130716302/232843771-b3efc6fd-12a2-47ed-8ddf-6d76a6b49e2b.png" alt="Evening Steps" width="300">

After analyzing the above graph, the following conclusions can be drawn:

-   Both "very active" and "less active" users wind down their physical activity as bedtime approaches. However, the difference in steps is very distinct, as "very active" users take 2 to 4 times more steps than "less active" users.
-   While this doesn't completely confirm my hypothesis of having high evening activity negatively impacting sleep or falling asleep duration, it does provide some evidence to support the idea. Further investigation with more data is warranted, as this topic could greatly help users.
    

### 5.7 Correlation Analysis

#### Falling Asleep Duration Vs Sleep Duration

For the upcoming analysis, I aim to explore the possibility of discovering a correlation between the duration of falling asleep and the amount of time spent sleeping. Identifying a relationship between these two variables can have several practical implications, including:

-   Assisting individuals in optimizing their sleep habits and enhancing their overall health and well-being.
-   Providing valuable insights to the Bellabeat app for suggesting improvements in sleep, thus opening up opportunities for marketing campaigns.

To establish a correlation between the two variables, I will create a scatter plot with falling asleep duration as the independent variable and sleep time as the dependent variable.
~~~r
sleep_corr1<- daily_data %>% 
  mutate(mins_to_fall_asleep = total_time_in_bed - total_minutes_asleep) %>%
  ggplot(mapping=aes(x=mins_to_fall_asleep/60, y=total_minutes_asleep/60)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title="Hours Asleep vs Hours to Fall Asleep", x="Hours to Fall Asleep", y="Hours Asleep") +
  scale_y_continuous(breaks = seq(0, 14, by = 2)) + 
  scale_x_continuous(breaks = seq(0, 7, by = 1)) +
  theme(panel.background = element_blank(), plot.title = element_text(hjust=0.5, size=14))
print(sleep_corr1)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232845529-c4bccae8-b004-481f-bf28-6b62ea7bcf43.png" alt="Asleep vs Falling Asleep" width="250">

The plot seems to show a positive correlation as the geom_smooth() function, or line of best fit, appears to be on an upward trend. However, the majority of the data points are concentrated within the 0-2 falling asleep hour interval, with a lot of noise outside of this range. Therefore, to confirm this positive correlation assumption, I will plot the same data again, but only with the data points that fall within the 0-2 hours mark.
~~~r
sleep_corr2 <- daily_data %>% 
  mutate(mins_to_fall_asleep = total_time_in_bed - total_minutes_asleep) %>%
  filter(mins_to_fall_asleep < 60*2) %>% 
  ggplot(mapping=aes(x=mins_to_fall_asleep/60, y=total_minutes_asleep/60)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title="Hours Asleep vs Hours to Fall Asleep", x="Hours to Fall Asleep", y="Hours Asleep") +
  scale_y_continuous(breaks = seq(0, 14, by = 2)) + 
  scale_x_continuous(breaks = seq(0, 7, by = 1)) +
  theme(panel.background = element_blank(), plot.title = element_text(hjust=0.5, size=14))
print(sleep_corr2)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232845841-1531c7b8-ae13-4484-9e30-33dc0041eaaf.png" alt="Asleep vs Falling Asleep 2" width="250">

Based on the second plot that includes only the data points in the 0-2 hours mark, it appears that there is no clear relationship or correlation between falling asleep duration and sleep time. While the first plot may have showed a positive correlation, it was heavily influenced by a concentration of data points in the 0-2 hours mark and noise outside of this interval, which may have skewed the results. However, by narrowing the focus to only the data points in the 0-2 hours range, it becomes clear that there is no consistent relationship between the two variables.

#### Daily Steps Vs Falling Asleep Duration

For this analysis, I aim to investigate the possible correlation between daily step count and the time taken to fall asleep. This investigation is essential as it can provide insight into any potential impediments that may hinder an individual's ability to maintain an active lifestyle and obtain quality sleep. To establish a correlation between the two variables, I will create a scatter plot with daily step count as the independent variable and falling asleep duration as the dependent variable.
~~~r
sleep_corr3 <- daily_data %>% 
  mutate(mins_to_fall_asleep = total_time_in_bed - total_minutes_asleep) %>%
  ggplot(mapping=aes(x=total_steps, y=mins_to_fall_asleep/60)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title="Daily Steps vs Duration to Fall Asleep", x="Daily Steps", y="Duration to Fall Asleep") +
  scale_y_continuous(breaks = seq(0, 14, by = 2)) + 
  theme(panel.background = element_blank(), plot.title = element_text(hjust=0.5, size=14))
print(sleep_corr3)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232846731-c4917aa3-8e8f-4b59-93e5-7f7b7341a3d6.png" alt="Steps vs Falling Asleep" width="250">

The analysis revealed that there is no correlation between daily step count and the time it takes to fall asleep. Despite not finding a correlation between these two variables, this analysis offers valuable insights and enhances our understanding of the relationship between physical activity and falling asleep.

#### Daily Steps Vs Asleep Duration

Based on my previous analysis, it only makes sense to investigate a potential correlation between daily step count and sleep duration. This analysis aims to provide valuable insights into the relationship between an active lifestyle and the quality of sleep. To establish a correlation between the two variables, I will create a scatter plot with daily step count as the independent variable and asleep duration as the dependent variable.
~~~r
sleep_corr4 <- daily_data %>% 
  ggplot(mapping=aes(x=total_steps, y=total_minutes_asleep/60)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title = "Sleep Hours vs Total Steps", x = "Daily Steps", y= "Daily Asleep Hours") +
  scale_y_continuous(breaks = seq(0, 16, by = 2)) + 
  theme(plot.title = element_text(hjust=0.5, size=14),axis.text.x = element_text(hjust=0.5))
print(sleep_corr4)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232847273-fab6752a-0395-4184-9f37-2d6c3067797d.png" alt="Steps vs Sleep" width="250">

Once again I found that there is no significant correlation between daily steps and the duration of sleep. While it may be disappointing not to find a relationship between these two variables, the results are still valuable in understanding the relationship between physical activity and sleep quality. The findings suggest that increasing daily steps may not necessarily lead to improved sleep duration, and other factors may have a more significant impact on the duration of sleep.

#### Intensity Activity Vs Asleep Duration

For this analysis, my objective is to investigate the potential correlation between users who participated in high-intensity activities and their duration of sleep. To establish a correlation between these two variables, I will create a scatter plot where the intensity count will be the independent variable, and the asleep duration will be the dependent variable.
~~~r
user_avg_sleep <- daily_data %>% 
  group_by(id) %>% 
  summarise(avg_daily_asleep = mean(total_minutes_asleep/60))

user_avg_intensity <- hourly_data %>% 
  group_by(id) %>% 
  summarise(avg_daily_intensity = mean(total_intensity))

sleep_corr5 <- user_avg_sleep %>% 
  left_join(user_avg_intensity, by = c("id")) %>% 
  ggplot(mapping=aes(x=avg_daily_intensity, y=avg_daily_asleep)) +   
    geom_jitter() +
    geom_smooth(color = "red") + 
    labs(title = "Intensity vs Sleep", x = "Daily Average Itensity", y= "Daily Average Sleep") +
    theme(plot.title = element_text(hjust=0.5, size=14))
print(sleep_corr5)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232851737-e80e412b-dcb8-4f77-bde0-03974eb77ccb.png" alt="Intensity vs Sleep" width="250">

After conducting the analysis, it appears that there is no correlation between the intensity count and sleep duration. In other words, there is no significant statistical relationship between the number of intensity activities and the amount of sleep a person gets. It is worth noting that while this finding provides valuable insights, it should be acknowledged that having more data would lead to more accurate results.

#### Burned Calories Vs Asleep Duration

Another correlation analysis worth exploring is the relationship between the amount of calories burned and the duration of sleep. This can offer another perspective on whether being more active during the day, thus burning more calories, can have an impact on a person's sleep quality. To establish a correlation between these two variables, I will create a scatter plot where the calories burned will be the independent variable, and the asleep duration will be the dependent variable.
~~~r
sleep_corr6 <- daily_data %>% 
  ggplot(mapping=aes(x=calories, y=total_minutes_asleep/60)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title = "Calories Burned vs Sleep Hours", x = "Calories Burned", y= "Daily Asleep Hours") +
  scale_y_continuous(breaks = seq(0,16, by = 2)) + 
  theme(plot.title = element_text(hjust=0.5, size=14))
print(sleep_corr6)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232864365-7f4f355f-8f83-4f99-a80b-7e9828409bfe.png" alt="User Usage" width="250">

The analysis shows that there is no correlation between the calories burned and the duration of sleep. This strengthens the idea that there is no statistical relationship between physical activity and the amount of time a person sleeps.

#### User Activity Category Vs Asleep Duration

To conclude this series of sleep correlation analyses, I will revisit our initial analysis where we classified users into four different activity categories - "very active", "fairly active", "lightly active", and "sedentary" - and examine their correlation with sleep duration. To establish a correlation between these variables, I will create scatter plots with the activity category as the independent variable and sleep duration as the dependent variable.
~~~r
combined_plots_activity <- ggarrange(
  ggplot(daily_data, mapping=aes(x=very_active_minutes/60, y=total_minutes_asleep/60))+   
    geom_jitter() +
    geom_smooth(color = "red") + 
    labs(title = "Very Active vs Sleep", x = "Very Active Hours", y= "Sleep Hours") +
    theme(plot.title=element_text(hjust=0.5, size=11, face="bold"), 
          axis.title.x=element_text(size=9), axis.title.y=element_text(size=9),
          axis.text.x=element_text(size=6), axis.text.y=element_text(size=6)),
  ggplot(daily_data, mapping=aes(x=fairly_active_minutes/60, y=total_minutes_asleep/60))+   
    geom_jitter() +
    geom_smooth(color = "red") + 
    labs(title = "Fairly Active vs Sleep", x = "Fairly Active Hours", y= "") +
    theme(plot.title = element_text(hjust=0.5, size=11, face="bold"), 
          axis.title.x=element_text(size=9), axis.title.y=element_text(size=9),
          axis.text.x=element_text(size=6), axis.text.y=element_text(size=6)),
  ggplot(daily_data, mapping=aes(x=lightly_active_minutes/60, y=total_minutes_asleep/60))+   
    geom_jitter() +
    geom_smooth(color = "red") + 
    labs(title = "Lightly Active vs Sleep", x = "Lightly Active Hours", y= "Sleep Hours") +
    theme(plot.title = element_text(hjust=0.5, size=11, face="bold"), 
          axis.title.x=element_text(size=9), axis.title.y=element_text(size=9),
          axis.text.x=element_text(size=6), axis.text.y=element_text(size=6)),
  ggplot(daily_data, mapping=aes(x=sedentary_minutes/60, y=total_minutes_asleep/60))+   
    geom_jitter() +
    geom_smooth(color = "red") + 
    labs(title = "Sedentary vs Sleep", x = "Sedentary Hours", y= "") +
    theme(plot.title = element_text(hjust=0.5, size=11, face="bold"), 
          axis.title.x=element_text(size=9), axis.title.y=element_text(size=9),
          axis.text.x=element_text(size=6), axis.text.y=element_text(size=6)),
  nrow = 2, ncol = 2)
print(combined_plots_activity)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232852418-f7cad204-a01a-44f7-a1c0-7c53fd2408a8.png" alt="Activity Category vs Sleep" width="350">

Based on the results obtained from the scatter plots, it appears that there is no correlation between sleep duration and activity level for the categories of "Very Active", "Fairly Active", and "Lightly Active". However, for the category of "Sedentary", a negative correlation was observed. A negative correlation means that as the activity level decreases, the sleep duration tends to increase. In other words, individuals who are less active tend to have longer sleep durations than those who are more active, which makes sense as sleeping can be considered a sedentary activity.

It's important to note that correlation does not necessarily imply causation. While we can observe a statistical relationship between these variables, it's difficult to determine the exact cause-and-effect relationship between them. Nonetheless, this analysis provides valuable insights into the relationship between activity level and sleep duration, which can inform future research and interventions aimed at improving sleep health.

#### Daily Steps Vs Calories Burned

Moving our analysis towards calories burnt, I will investigate the possibility of a correlation between daily step count and calories burnt. As losing weight and burning calories are crucial aspects of maintaining and enhancing a healthy lifestyle, this analysis is significant. To establish a correlation between these variables, I will generate a scatter plot in which the daily step count will serve as the independent variable, and the calories burned will be the dependent variable.
~~~r
cal_corr1 <- daily_data %>% 
  ggplot(mapping=aes(x=total_steps, y=calories)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title = "Daily Steps vs Calories", x = "Daily Steps", y= "Calories Burned")+
  scale_x_continuous(breaks = seq(0, 25000, by = 3000)) + 
  theme(panel.background = element_blank(), plot.title = element_text(hjust=0.5, size=14),
        axis.text.x = element_text(angle=45, hjust=1))
print(cal_corr1)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232852802-b168b02f-0ce6-4a37-a056-47922a0bb347.png" alt="Steps vs Calories" width="250">

A positive correlation was found between daily step count and calories burned, which means that as the daily step count increases, so does the number of calories burned. This result suggests that walking more, or being more physically active, can have a direct impact on the number of calories burned, which is a critical factor in weight loss and maintaining a healthy lifestyle.

#### Intensity Vs Calories Burned

In order to strengthen my previous analysis on calories burned, I will now delve deeper into the correlation between physical activities, specifically their intensity, and compare it to the amount of calories burned. To establish a correlation between these variables, I plan to generate a scatter plot where the intensity count will be the independent variable, and the calories burned will be the dependent variable.
~~~r
cal_corr2 <- hourly_data %>% 
  ggplot(mapping=aes(x=average_intensity, y=calories)) +
  geom_jitter() +
  geom_smooth(color = "red") + 
  labs(title = "Intensity vs Calories", x = "Hourly Average Itensity", y= "Hourly Calories Burned") +
  theme(panel.background = element_blank(), plot.title = element_text(hjust=0.5, size=14),
        axis.text.x = element_text(hjust=1))
print(cal_corr2)
~~~
<img src="https://user-images.githubusercontent.com/130716302/232853189-1973a87c-cff3-466b-9b39-d9df2357c134.png" alt="Intensity vs Calories" width="250">

A positive correlation was found between intensity count and calories burned, which means that as the intensity increases, so does the number of calories burned. This result is not surprising as the intensity of physical activity is one of the primary determinants of the number of calories burned. The higher the intensity, the more energy is required to perform the activity, and the more calories are burned. However, it is important to note that while a positive correlation exists, this does not necessarily mean that causation exists.

## <img src="https://cdn-icons-png.flaticon.com/512/9196/9196093.png" alt="act" width="40" height="40"> [6. Act Phase](#act)

Bellabeat has achieved success by catering to the unique health needs of women, identifying a gap in the market for health and wellness products designed specifically for this demographic. The company's products feature innovative technology, stylish devices, and user-friendly apps and interface which combined, monitors activity levels, tracks heartbeat and intensity, and provides all sort of useful data to improve a healthy lifestyle. In addition, Bellabeat has effectively marketed its products through various channels, and by analyzing data such as the analysis we have completed, the company can develop new marketing strategies to build a loyal customer base and establish itself as a leader in the women's health and wellness market.

Based on my analysis, the following marketing strategies are recommended:

### 6.1 Sleep Tracking and Improvement

Getting a good night's sleep is crucial for maintaining physical health. The following are some ways that our app can help users improve their sleep patterns and quality of sleep:

-   **Emphasize the importance of sleep quality and offer notifications:**  The app will emphasize the importance of sleep quality and how it can affect overall health. To help users improve their sleep patterns, the app will send notifications that provide useful tips and reminders.
-   **Provide tips and suggestions for improving sleep habits:**  The app will include a dedicated section that provides tips and suggestions for improving sleep habits. These tips will be categorized by sub-categories to make it easy for users to find what they need.
-   **Highlight the negative impact of sleep deprivation:**  The app will also highlight the negative impact of sleep deprivation on physical performance and overall health. A recommendations section through the app will provide users with information on the importance of sleep and its impact on cognitive function and physical well-being.

### 6.2 Encourage an Active Lifestyle

Regular exercise is essential for maintaining physical and mental health. The following are some ways that the app can help users stay active and achieve their fitness and weight loss goals:

-   **Promote the benefits of physical activity and offer notifications:**  The app will emphasize the benefits of physical activity and encourage users to engage in physical activity throughout the day, while winding down and relaxing as bedtime approaches. The app will send notifications to remind users to move their bodies and stay active.
-   **Track step count and physical activity levels:**  The app will allow users to track their daily, weekly, and monthly step count and monitor their physical activity levels. Users can set daily or weekly goals for their step count or calories burned, and the app will provide progress updates to help them stay motivated and reach the next activty level, from sedentary to very active.
-   **Use correlation between daily step count and calories burned to motivate users:**  The app will use the correlation between daily step count and calories burned to motivate users to stay active and achieve their fitness goals. Users can set target step count or calories burned and track their progress through the app. The app will send notifications to users as they reach their goals and celebrate their achievements.

### 6.3 Personalized Recommendations:

The app can provide users with personalized recommendations and suggestions to help them achieve their fitness and sleep goals. The following are some ways we can achieve this:

-   **Use data from tracking daily step count and calories burned:**  The app will use data collected from tracking daily step count and calories burned to provide personalized recommendations and suggestions to users. These recommendations can be presented in the app's recommendation section and will help users stay motivated and achieve their fitness goals.
-   **Provide personalized recommendations for effective calorie burning:**  The app will highlight its value in helping users achieve their fitness goals and provide personalized recommendations for the types of physical activities and intensity routines that would be most effective for burning calories. These recommendations will be tailored to each user's fitness level, physical ability, and interests.
-   **Offer personalized solutions for sleep disorders:**  For people with sleep disorders or those who struggle to fall asleep, the app can offer personalized solutions to improve sleep quality. Users can opt for an additional pay-in feature that will provide customized solutions.

### 6.4 Achieving Fitness Goals:

The devices and app have several features that can help users achieve their fitness goals. The following are some ways to emphasize the benefits of the Bellatbeat devices and app:

-   **Measure physical activity intensity and calories burned using advanced algorithms:**  The devices and app use advanced algorithms to measure physical activity, intensity, and calories burned accurately. Users can track their progress and make informed decisions about their fitness goals.
-   **Target a wide range of users:**  The devices and app have been designed to cater to a broad range of users, including young and elderly women. Emphasis should be placed on the convenience and ease of use of the devices and app to ensure that everyone can use them without difficulty.

### 6.5 Gamification & Promotions:

The app cann offer several gamification and promotion features to make physical activity more engaging and motivate users to stay active. The following are some ways to achieve this:

-   **Use gamification to engage users:**  The app can use gamification to make physical activity more engaging and motivate users to stay active. This can include challenges, leaderboards, and other interactive features.
-   **Offer rewards and incentives for reaching daily step count goals:**  The app can offer rewards and incentives for reaching weekly or monthly step count goals. Users can earn badges, discounts, or other incentives to encourage them to stay active and achieve their fitness goals.
-   **Use badges and discounts to incentivize users:**  The app can use badges, discounts, or other incentives to encourage users to stay active and achieve their fitness goals. This can help users stay motivated and track their progress.
-   **Offer promotions and referral programs:**  Offer promotions, discounts, or referral programs to incentivize users to purchase and use the devices and app. This can include discounts on purchases, referral bonuses, or other incentives.
-   **Collect customer feedback and reviews:**  Collecting customer feedback and reviews to continually improve the device and app's features and user experience will helps understand the users' needs and make informed decisions about how to improve all product services provided.

<h2 align="center">Let's make data-driven decisions to achieve fitness goals</h2>