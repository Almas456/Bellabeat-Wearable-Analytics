## **Project Name:** Bellabeat Wearable Analytics

### **Project Overview**

This project is an end-to-end analysis of wearable-device data, inspired by Fitbit usage, designed to uncover behavioral trends and generate actionable product and marketing insights for Bellabeat. The analysis leverages day-level activity, sleep, and heart rate metrics to understand user engagement, identify patterns, and segment users into actionable personas. Insights from this study are intended to guide marketing strategies, personalized product recommendations, and retention campaigns across Bellabeat’s product line — **Leaf, Time, Spring, and Membership**.

### **Objective**

The primary goal is to analyze wearable-device usage data to:

1. Understand daily and hourly activity and sleep patterns.
2. Segment users into meaningful personas based on behavior.
3. Identify opportunities for targeted marketing, engagement nudges, and product upsells.
4. Provide a reproducible analysis pipeline that can be directly applied to real Fitbit data.

### **Data & Methodology**

**1. Data:** Synthetic dataset modeled on Fitbit public data (30 users × 90days).

**2. Key fields:** user\_id, date, total\_steps, very\_active\_min, lightly\_active\_min, sedentary\_min, sleep\_min, avg\_hr, calories, active\_flag.

**Processing Steps:**

1. Timestamp parsing and duplicate removal
2. Definition of active/inactive days
3. Aggregation of per-user statistics
4. Feature scaling and normalization
5. **K-means clustering (k=3)** to identify user personas
6. Correlation analysis between activity and sleep
7. Hourly activity profile creation to identify peak engagement windows
8. Retention proxy analysis (percent of users active per day)

**Tools & Libraries:** Python, pandas, numpy, scikit-learn, matplotlib, Jupyter Notebook

### **Key Findings**

**Activity Peaks:** Users are most active in the morning (06–09) and evening (17–20).
**Sleep & Activity Correlation:** Daily activity positively correlates with sleep duration (Pearson r ≈ 0.225).
**User Personas (k=3):**

  1. **Less Active (13 users):** avg\_steps ≈ 2,599; avg\_sleep ≈ 419 min
  2. **Moderate (13 users):** avg\_steps ≈ 4,307; avg\_sleep ≈ 428 min
  3. **Highly Active (4 users):** avg\_steps ≈ 6,712; avg\_sleep ≈ 435 min
**Engagement Trends:** Simulated retention curves indicate drop-offs after 1–3 weeks, highlighting opportunities for targeted nudges and challenges.

### **Business & Product Recommendations**

**1. Bellabeat Time:** Target moderate and highly active users with time-of-day ads (morning/evening) and premium workout suggestions.
**2. Bellabeat Leaf:** Promote sleep-focused features for less active users (“sleep better by moving more”).
**3. Bellabeat Spring:** Use lunchtime and meal-time reminders for hydration and wellness nudges.
**4. Membership & Retention Campaigns:** Introduce 7–21 day onboarding nudges, in-app challenges, and weekend events to sustain engagement.

### **Reproducibility & Next Steps**

1. Replace the sample CSV with actual Fitbit CSVs (dailyActivity.csv, sleepDay.csv, minuteActivity.csv).
2. Re-run the Jupyter notebook to generate real metrics and visuals.
3. Export results into **visuals/** and slide decks for executive presentation.
4. Track KPIs like CTR, trial-to-paid conversion, and 14/30-day retention lift.

### **Key Takeaways**

1.Wearable usage data can directly inform marketing timing and personalization strategies.
2.Persona-based segmentation enables tailored product messaging and upsell opportunities.
3.Activity-sleep correlation provides a foundation for wellness-oriented campaigns.
4.Mid-term engagement monitoring highlights the importance of timely nudges to improve retention.
