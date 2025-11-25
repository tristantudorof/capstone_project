# Bellabeat Case Study


# Introduction 

This case study is part of the Google Data Analytics Professional Certificate. Following the six-step analysis process—Ask, Prepare, Process, Analyze, Share, and Act—I analyzed smart device fitness data to uncover user behavior trends and recommend marketing strategies for Bellabeat, a health-focused manufacturer of smart wellness devices.

# Scenario
Bellabeat is a successful small company, but they may have the potential to become a larger player in the
global smart device market. Urška Sršen, cofounder and Chief Creative Officer of Bellabeat, believes that analyzing smart
device fitness data could help unlock new growth opportunities for the company. I have been asked to focus on one of
Bellabeat’s products and analyze smart device data to gain insight into how consumers are using their smart devices. The
insights I discover will then help guide marketing strategy for the company. 

I will present my analysis to the Bellabeat executive team along with high-level recommendations for Bellabeat’s marketing strategy.

# Business Task
Analyze smart device usage trends and identify opportunities for Bellabeat to improve marketing strategy and grow its user base.

# 1. Ask
1. What are some trends in smart device usage?
2. How could these trends apply to Bellabeat customers?
3. How could these trends help influence Bellabeat marketing strategy?

# 2. Prepare
Dataset:
FitBit Fitness Tracker Data (Kaggle): [Bellabeat](https://www.kaggle.com/datasets/sawandikirby/bellabeat-case-study-fitbit-data/data)

On Kaggle Notebooks,
18 tables from 4/12/16 – 5/12/16, were imported.


Primary focus areas:
✔ Activity behavior
✔ Steps
✔ Calories
✔ Daily usage patterns

Imported and explored in Kaggle Notebooks.

# Exploration included:

Reviewing data types, column names and the number of unique users.

Checking number of unique users: 33 total, 31 active daily
This is important becouse it shows how many people out of the 33 actually used the device daily, delivering us consistent data on the full time period. 
We will be using the 31 active daily users for our analysis and identifying and grouping them from their unique id.

# Looking at column names and data types

<img width="725" height="776" alt="Screenshot 2025-11-23 at 12 18 38 AM" src="https://github.com/user-attachments/assets/4f0d8345-fea5-4361-a90d-b50baca80bae" />

<img width="794" height="662" alt="Screenshot 2025-11-23 at 12 16 21 AM" src="https://github.com/user-attachments/assets/a686f837-5411-495e-ab61-c0c99a796a48" />


<img width="727" height="393" alt="Screenshot 2025-11-23 at 12 16 34 AM" src="https://github.com/user-attachments/assets/cab2c0cd-4938-49c6-a591-57e18cecdf83" />

# Checking unique ids and counted 33 total with only 31 active daily for the full time period.

This issue will be addressed later on.

<img width="643" height="755" alt="Screenshot 2025-11-23 at 12 17 28 AM" src="https://github.com/user-attachments/assets/d90af374-d42e-460f-9c96-8fc62eb74c70" />



# 3. Process


Data Cleaning Steps

Standardized Column Names

Converted to lowercase + snake_case

I did this to make querys easier later in the analysis inculding any case senstive issues that could come up, and to improve readability of the code.

Added derived columns:

activity_date

day_of_week

n_day_of_week

Adding derived columns helps group the raw data we need into useful data to make analysis, grouping, and reporting much easier.

• Checked for missing values

• Removed duplicates

• Validated data consistency and user counts

Missing data and duplicates can interfier with our analysis, causing inacurate results, so i checked and cleaned the data to ensure the data quality.

Validating the data conssistency and user count was super important to understand how many users actualy wore the device every day. If someone wore the device for one day out of 30, and worked out at a very high level or possibly not have even worn the device during our time period, it could mess up our analysis and give us wrong insights.

# Data Cleaning

Before analysis, the dataset was cleaned by,
1. Creating and renaming columns.
   making all names lowercase and snake case.
   adding columns activity_date, day_of_week, and n_day_of_week
3. Checking for null values
4. Checking for duplicates

<img width="787" height="582" alt="Screenshot 2025-11-23 at 12 33 23 AM" src="https://github.com/user-attachments/assets/e46f5816-5762-4680-9a8d-29fb4e8c1237" />

<img width="629" height="132" alt="Screenshot 2025-11-23 at 12 33 38 AM" src="https://github.com/user-attachments/assets/cd74b84c-57ac-4137-ba32-48d706c0c2c4" />
<img width="334" height="632" alt="Screenshot 2025-11-23 at 12 33 55 AM" src="https://github.com/user-attachments/assets/acb7305e-ef08-470e-a3e8-3b91c0bc26d6" />

# 4. Analyze
The central question:

What trends exist in smart device usage?

To find trends in the data, it was important to see how people were using the device. Then from that we could find trends on what the majority of people were doing. That data could give us powerful insights on target market and simply how the majority of people a using the device and what they're using it for.

To explore this, I grouped users by activity levels and analyzed relationships among calories, steps, and activity minutes.

<img width="675" height="500" alt="Screenshot 2025-11-23 at 12 40 25 AM" src="https://github.com/user-attachments/assets/02c0371f-df88-4ad8-86f9-04db68ab58b7" />

<img width="697" height="263" alt="Screenshot 2025-11-23 at 12 45 17 AM" src="https://github.com/user-attachments/assets/70afe22e-15df-4a45-b5af-bda262a4d87f" />

I then looked at correlation between activity level in minutes and calories,percentage of activity in minutes, average steps per day, correlation between steps and calories burned.

This data could give us imporatant insights on goals, how long people were active for, and what the majority of activity looked like, to find trends.

# 5. Share

# 1. Steps vs. Calories Burned

The average active user walked ~10,000 steps and burned ~2,000 calories.

"Very active" users exceeded 12k steps but represented a small portion of the dataset.

<img width="777" height="593" alt="Screenshot 2025-11-25 at 4 00 15 PM" src="https://github.com/user-attachments/assets/61364842-f548-418d-83fb-4bbc69ea726f" />

We can see the average active person walked around 10k steps and burned 2k calories. 

While the very active people were over 12k steps but were not the majority of users.


# 2. Average Steps by Day

Most active days: Tuesday, Wednesday, Saturday

Least active day: Thursday

This suggests weekly behavioral patterns that marketing can leverage.

<img width="712" height="470" alt="Screenshot 2025-11-23 at 12 46 16 AM" src="https://github.com/user-attachments/assets/6943aa62-705c-405b-b585-d346ad5acea3" />

we can see that the days Tuesday, Wednesday and Saturday were the day people were most active. While thursday was the day with the least activity.

# 3. Activity Category Percentages

The majority of logged activity was light activity (e.g., walking).

Most users are casual exercisers, not athletes.

<img width="705" height="396" alt="Screenshot 2025-11-23 at 12 46 25 AM" src="https://github.com/user-attachments/assets/fbecd846-6c62-4fca-bbba-03faae827bc8" />
Sedentary Time

Users spent a significant portion of their day sedentary—likely due to work, commuting, or sleep.

we can see that most the activity was caegorized as light activity. meaning, most of the customers are using the device for more casual workouts.

# 4. Activity Minutes vs. Calories
Even users with high activity minutes typically stayed under 3,500 calories/day.

Suggests moderate-intensity workouts rather than endurance training.

<img width="760" height="560" alt="Screenshot 2025-11-23 at 12 46 36 AM" src="https://github.com/user-attachments/assets/122841b4-0fce-4138-a92b-bf0f3ebb73ce" />

Daily Workout Duration

Most users exercised under 300 minutes per day, averaging ~30 minutes.

# 6. Act — Recommendations

Recommendations

# Target Everyday Wellness Users

Most users aim for manageable goals like burning 2,000–2,500 calories/day—not elite training levels.
Marketing should reflect this.

# Advertise Before High-Activity Days

Activity peaks on Tuesday, Wednesday, and Saturday.
Bellabeat can increase engagement by promoting workouts and features on Monday and Friday.

# Emphasize Step-Based Goals

Most users walk 10k steps or fewer, making campaigns like:
“Reach your 10,000 steps with Bellabeat.”
highly relevant.

# Focus on Light & Moderate Activity

Market to users who prefer:

• Walking

• Light cardio

• Short daily routines

• General wellness habits

# Promote Consistency (30-Minute Workouts)

Daily reminders, streaks, and habit-building features align well with user behavior.

# Sedentary Insights = Opportunity

Highlight:

• Sedentary alerts

• Stress/breathing reminders

• Sleep tracking

These features match how users wear their devices throughout the day and night.


# Conclusion
Trends show to target customers that want to hit 2500 calories burned and do light workouts for less than 30 minutes per day. These trends show who Bellabeats main group of customers are.

The data reveals that most users engage in light to moderate physical activity, with habits centered around walking and short daily routines. 

To maximize growth, Bellabeat should emphasize wellness, achievable goals, and everyday habit-building rather than high-intensity fitness.
