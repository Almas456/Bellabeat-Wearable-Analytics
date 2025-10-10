# Bellabeat: A Data-Driven Analysis of Activity and Sleep Patterns

## 1. Introduction

This report presents a data-driven analysis of user activity and sleep patterns using data from the public Fitbit dataset. The goal is to identify key trends and provide actionable insights that can inform the marketing and product strategies for Bellabeat, a wellness technology company.

The analysis was performed in Google Sheets for data cleaning, exploration, and visualization. Findings highlight opportunities for Bellabeat to encourage more consistent physical activity, reduce sedentary time, and promote healthier sleep habits.

## 2. Data & Methods

**Dataset:** Fitbit Fitness Tracker Data (2016)
**Link:** [https://www.kaggle.com/datasets/arashnic/fitbit](https://www.kaggle.com/datasets/arashnic/fitbit)

**Sample size:**
- ~33 unique users
- ~940 daily activity records
- ~400 sleep records

**Files analyzed:**
- `dailyActivity_merged.csv` (steps, sedentary minutes, calories)
- `sleepDay_merged.csv` (total minutes asleep, time in bed)
- `dailySteps_merged.csv` (validation of steps data)

**Data cleaning steps:**
- Removed duplicates
- Converted date formats (e.g., “MM/DD/YYYY hh:mm:ss” → “MM/DD/YYYY”)
- Merged activity and sleep data by Id + Date
- Handled missing values (replaced with 0 when appropriate)

**Tools used:** Google Sheets for formulas, pivot tables, and visualizations.

## 3. Key Findings

### Finding 1: Users fall short of the 10,000-step benchmark

- **Average steps/day:** ≈ 7,600, which is below the recommended 10,000.
- The histogram shows a sharp drop-off above 10,000 steps.
- Images/DistributionofDailySteps.png


**Interpretation:** Most users are moderately active or inactive, leaving room for Bellabeat to encourage higher daily movement.

### Finding 2: Sedentary time dominates the day

- **Average sedentary minutes/day:** ≈ 991 minutes (~16.5 hours).
- This is ~70% of a day spent inactive.

**Interpretation:** Bellabeat has an opportunity to motivate micro-movements and reduce long sedentary periods.

### Finding 3: Sleep duration is below recommended levels

- **Average sleep:** 5–7 hours/day, compared to the recommended 7–8 hours.


**Interpretation:** Sleep improvement is as important as activity for wellness. Bellabeat should emphasize both.

### Finding 4: Activity and sleep show weak correlation

- Scatter plots show that higher steps or active minutes don’t necessarily lead to longer sleep.
- Images/ActiveMinutevsSleep.png
- Images/StepsvsSleep.png


**Interpretation:** Activity alone is not enough for holistic wellness. Sleep must be addressed independently.

### Finding 5: Weekday vs weekend differences

- Average steps are slightly higher on weekends.
- Images/WeekdayandAVERAGEofTotalSteps.png


**Interpretation:** Users are more active when free from work routines. Mid-week activity drops sharply.

## 4. Recommendations

### 1. Promote Weekday Micro-Challenges

- **Focus:** Engage users between Wednesday and Friday, when activity declines.
- **Example actions:**
    - Launch “Hump Day Hustle” or “Friday Finish Strong” challenges.
    - Push notifications during work hours (e.g., 2 PM walk/stretch reminders).
    - Integrate Bellabeat devices with productivity apps for desk reminders.

### 2. Gamify the 10,000-Step Goal

- **Focus:** Turn 10,000 steps into a fun and rewarding experience.
- **Example actions:**
    - Daily badges, streaks, or virtual rewards for users crossing 10k steps.
    - Social sharing of progress inside the Bellabeat app to build community.

### 3. Launch Sleep Coaching Campaigns

- **Focus:** Address the sleep deficit directly.
- **Example actions:**
    - Bedtime reminders, relaxing sounds, and “sleep hygiene tips.”
    - Personalized sleep reports inside the app.
    - Marketing message: “Wellness = activity + rest.”

### 4. Implement Sedentary Alerts

- **Focus:** Tackle the high sedentary time.
- **Example actions:**
    - Device nudges if users remain sedentary >60 minutes.
    - Marketing theme: “Little moves matter.”

## 5. Conclusion

This analysis shows that while Bellabeat users are moderately active, they fall short of step benchmarks, spend excessive time sedentary, and sleep less than recommended. Importantly, physical activity does not automatically improve sleep, underscoring the need for a holistic wellness strategy.

By implementing weekday challenges, gamifying activity, introducing sleep campaigns, and sending sedentary alerts, Bellabeat can strengthen user engagement and position itself as a brand that supports complete wellness — activity + rest.
