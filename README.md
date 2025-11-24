# Bellabeat Case Study


# Introduction 

The Bellabeat Case Study is a capstone project for the Google Data Analytics Professional Certificate on Coursera. In this project, I will follow the data analysis process: ask, prepare, process, analyze, share and act to analyze the data.

# Scenario
A junior data analyst working on the marketing analyst team at Bellabeat, a high-tech manufacturer of health-focused
products for women. Bellabeat is a successful small company, but they have the potential to become a larger player in the
global smart device market. Urška Sršen, cofounder and Chief Creative Officer of Bellabeat, believes that analyzing smart
device fitness data could help unlock new growth opportunities for the company. You have been asked to focus on one of
Bellabeat’s products and analyze smart device data to gain insight into how consumers are using their smart devices. The
insights you discover will then help guide marketing strategy for the company. You will present your analysis to the Bellabeat
executive team along with your high-level recommendations for Bellabeat’s marketing strategy.

# Business Task
Analyze smart device usage trends to uncover opportunities for Bellabeat’s growth and recommend ways to enhance their marketing strategy.

# 1. Ask
1. What are some trends in smart device usage?
2. How could these trends apply to Bellabeat customers?
3. How could these trends help influence Bellabeat marketing strategy?

# Data
Data Source: [Bellabeat](https://www.kaggle.com/datasets/sawandikirby/bellabeat-case-study-fitbit-data/data)

# 2. Prepare
On Kaggle Notebooks,
18 tables from 4.12.16-5.12.16 were imported.

Activity would be the focus of my analysis and finding trends for target market would be the goal.

# Data Exploration
started with looking at column names and data types
<img width="725" height="776" alt="Screenshot 2025-11-23 at 12 18 38 AM" src="https://github.com/user-attachments/assets/4f0d8345-fea5-4361-a90d-b50baca80bae" />

<img width="794" height="662" alt="Screenshot 2025-11-23 at 12 16 21 AM" src="https://github.com/user-attachments/assets/a686f837-5411-495e-ab61-c0c99a796a48" />


<img width="727" height="393" alt="Screenshot 2025-11-23 at 12 16 34 AM" src="https://github.com/user-attachments/assets/cab2c0cd-4938-49c6-a591-57e18cecdf83" />

# Checking unique ids and counted 33 with only 31 active daily

<img width="643" height="755" alt="Screenshot 2025-11-23 at 12 17 28 AM" src="https://github.com/user-attachments/assets/d90af374-d42e-460f-9c96-8fc62eb74c70" />

# 3. Process

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
The analysis question is
What are some trends in smart device usage?

we grouped each id into sections based on activity to gain insights.

<img width="675" height="500" alt="Screenshot 2025-11-23 at 12 40 25 AM" src="https://github.com/user-attachments/assets/02c0371f-df88-4ad8-86f9-04db68ab58b7" />

<img width="697" height="263" alt="Screenshot 2025-11-23 at 12 45 17 AM" src="https://github.com/user-attachments/assets/70afe22e-15df-4a45-b5af-bda262a4d87f" />

we then looked at correlation between activity level in minutes and calories,percentage of activity in minutes, average steps per day, correlation between steps and calories burned.

# 5. Share
# Correlation between steps and calories burned

<img width="694" height="480" alt="Screenshot 2025-11-23 at 12 46 04 AM" src="https://github.com/user-attachments/assets/5082903c-5015-4bc0-8e73-8bbcfb2f3ebd" />

we can see the average active person walked around 10k steps and burned 2k calories 

while the very active people were over 10k steps but were not the majority of users.

# Average steps per day

<img width="712" height="470" alt="Screenshot 2025-11-23 at 12 46 16 AM" src="https://github.com/user-attachments/assets/6943aa62-705c-405b-b585-d346ad5acea3" />

we can see that the days Tuesday, Wednesday and Saturday were the day people were most active. While thursday was the day with the least activity.

# Percentage of activity in minutes

<img width="705" height="396" alt="Screenshot 2025-11-23 at 12 46 25 AM" src="https://github.com/user-attachments/assets/fbecd846-6c62-4fca-bbba-03faae827bc8" />

we can see that most the activity was caegorized as light activity. meaning, most of the customers are using the device for more casual workouts.

# Correlation between activity level in minutes and calories

<img width="760" height="560" alt="Screenshot 2025-11-23 at 12 46 36 AM" src="https://github.com/user-attachments/assets/122841b4-0fce-4138-a92b-bf0f3ebb73ce" />

we can see most of the users even with high activity were under 3500 calories even with high minutes of activity.

# 6. ACT

Recommendations

• Target customers that want to steadly achieve 2500 calories burned not pro athletes.

• Advertise on days right before high activity like, Monday and Friday.

• Most customers walk 10k steps or less so you can market to customers that want to strive to hit that goal.

• Most activity was light activity reinforcing our idea of targeting normal people who enjoy casual workouts, like simple walks outside for 30 minutes a day.

• Most activity was less than 300 minutes meaning our clients workout on average for 30 minutes a day.

• A large percentage of time while customers wore the device was being sedentary, or not moving very much, potentialy sleeping or while working in an office.


# Conclusion
Trends show to target customers that want to hit 2500 calories burned and do light workouts for less than 30 minutes per day
These trends show who Bellabeats main group of customers are.
These trends help influence Bellabeat marketing strategy, by defining who the target market is.
