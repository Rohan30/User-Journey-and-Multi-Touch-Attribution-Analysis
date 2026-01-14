# 📊 User Journey & Multi-Touch Attribution Analysis

## 📌 Project Overview
This project analyzes multi-touch customer journeys to understand how users interact with multiple marketing channels before converting, and how conversion probability and channel contribution vary across different attribution models.

The dataset consists of 10,000+ user interactions from 2,847 unique users across six marketing channels:

- 📍 Direct Traffic
- 🖥️ Display Ads
- 📧 Email
- 🔗 Referral
- 🔍 Search Ads
- 📱 Social Media

User journeys range from single-touch interactions to complex paths with up to 12 touchpoints, enabling an in-depth study of journey complexity and conversion behavior.

---

## 🎯 Objectives
- 🎯 Analyze user journey complexity and identify the optimal number of touchpoints for conversion
- 📈 Study conversion behavior across journey depth and channel position
- 🔄 Compare heuristic and data-driven attribution models
- 💡 Generate actionable insights for campaign optimization and budget allocation

---

## 🔎 Exploratory Data Analysis (EDA)

### 🔁 Conversion vs Non-Conversion Split
Users are initially segmented into converted and non-converted groups to establish baseline conversion behavior before deeper journey analysis.

### 📊 Distribution of User Journey Lengths
- Most users experience journeys with 1–6 touchpoints
- Very few users undergo long and complex journeys beyond 7 touchpoints
- Users with longer journeys show a higher likelihood of eventual conversion, although such journeys are rare

This indicates that while complex journeys can convert effectively, they are inefficient from a scalability and marketing ROI perspective.

### 📉 Journey Depth & Conversion Behavior
- Conversions increase sharply as touchpoints rise from 1 to 4
- Beyond 4 touchpoints, total conversions decline due to fewer users continuing the journey
- Conversion rates steadily increase until around 6 touchpoints, after which they plateau
- Journeys beyond 7–8 touchpoints approach 100% conversion, driven by a small, highly committed user group

Marketing efforts should focus on maximizing conversions within 4–5 touchpoints, as additional touchpoints yield diminishing returns.

### 📍 Conversion Rates by Touchpoint Position Across Channels
- Conversion rates vary across channels during early and mid-journey touchpoints
- From the 8th touchpoint onward, conversion rates plateau close to 100% across all channels
- Channel placement is critical early in the journey but less influential in long journeys

This highlights the importance of strategic channel sequencing to maximize early and mid-funnel effectiveness.

### 📦 Interaction Volume by Channel
- 📍 Direct Traffic has the highest interaction volume
- 🔍 Search Ads have the lowest interaction volume
- High interaction volume does not directly translate into conversion contribution

This emphasizes the need for attribution modeling beyond raw interaction counts.

---

## 🧠 Attribution Modeling

### 🧩 Attribution Models Used
- 🥇 First-Touch Attribution
- 🥈 Last-Touch Attribution
- 🔗 Markov (Data-Driven) Attribution

Each model is evaluated using:
- 📊 Conversion Rate
- 🧮 Attribution Score

---

## 📐 Understanding the Metrics

### 📈 Conversion Rate
- Measures the probability that a user converts after interacting with a channel
- Reflects traffic quality and channel effectiveness
- Useful for campaign and messaging optimization

### 🧮 Attribution Score
- Measures the share of total conversion credit assigned to a channel
- Reflects overall channel importance in the conversion process
- Useful for budget allocation and strategic planning

---

## 📊 Results & Insights

### 📉 Conversion Rates Across Attribution Models
- First-Touch Attribution highlights acquisition effectiveness
  - Display Ads and Direct Traffic perform strongly at the beginning of journeys
- Last-Touch Attribution highlights closing effectiveness
  - Referral and Display Ads excel near conversion
- Markov Attribution provides a balanced, data-driven estimate
  - Conversion rates are more stable across channels
  - Reflects the contribution of channels across the entire journey

Relying on a single attribution model can be misleading. Data-driven attribution provides a more holistic view of marketing performance.

### 🧮 Attribution Scores Across Models
- First-Touch Attribution over-credits acquisition-focused channels
- Last-Touch Attribution over-credits closing-focused channels
- Markov Attribution distributes credit more evenly by accounting for inter-channel dependencies

Conversions are driven by a combination of channels, not a single dominant source.

---

## 🏁 Key Conclusions
- Optimal user conversion typically occurs within 4–5 touchpoints
- Long and complex journeys convert well but are inefficient and rare
- Marketing channels play different roles at different journey stages
- Markov attribution offers the most reliable estimate of true channel contribution
- Data-driven attribution is best suited for budget allocation and strategic decisions

---

## 🛠️ Tech Stack
- Python
- pandas
- numpy
- matplotlib
- seaborn

---
