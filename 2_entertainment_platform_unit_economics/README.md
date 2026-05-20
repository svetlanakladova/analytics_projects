## Procrastinate Pro+ Marketing & Unit Economics Analysis

### Project Overview

This project analyzes the performance of a digital entertainment platform after the launch of a new sports content category and changes in the marketing strategy.

The objective of the analysis is to identify the reasons behind revenue stagnation despite continuous audience growth and increasing user activity.

The study focuses on user acquisition efficiency, engagement, monetization, and marketing profitability during the first 28 days after acquisition.

### Metrics Tree

Below is the metrics tree used in this analysis to structure hypotheses and investigate revenue stagnation.

<img width="1788" height="880" alt="metrics_tree" src="https://github.com/user-attachments/assets/ae682f8d-9839-4b94-a61b-153b40a82ea9" />



### Key Business Question

Why is revenue stagnating despite growing user activity and audience size?

### Project Objectives

- Analyze unit economics in the first 28 days after acquisition
- Identify reasons for revenue stagnation
- Evaluate marketing channel performance
- Compare CAC, LTV, and ROI across channels
- Identify profitable and unprofitable acquisition sources
- Provide recommendations to the marketing team


---

### Dataset Description

The project uses datasets:

`ppro_visits.csv` — information about user sessions in the application (users registered from April 1, 2024 to November 30, 2024):
- `user_id` — unique user identifier
- `region` — user country
- `device` — user device category
- `channel` — marketing acquisition channel
- `session_start` — session start date and time
- `session_end` — session end date and time


`ppro_orders.csv` — information about purchases:
- `user_id` — unique identifier of the user who made the purchase
- `event_dt` — purchase date and time
- `revenue` — revenue from the purchase


`ppro_costs.csv` — information about marketing expenses:
- `dt` — date
- `channel` — marketing acquisition channel
- `costs` — marketing cost for the channel on that day

---

### Project Steps
1. Data loading and preprocessing
2. Cohort preparation for analysis
3. User engagement analysis
4. Unit economics analysis (CAC, LTV, ROI)
5. Channel-level performance comparison
6. Payback period analysis
7. Conclusions and recommendations

---

### Key Findings
- User base increased significantly after the launch of sports content
  - DAU grew from ~350 to ~900
  - MAU grew from ~9,000 to ~14,000
- Engagement increased slightly
  - Stickiness grew from 5.3% to 6.2%
  - New users are not significantly more engaged than old users
- Marketing efficiency decreased over time
  - CAC increased in several channels (especially `TipTop` and `FaceBoom`)
  - LTV peaked mid-year and then declined
- ROI issues
  - Most cohorts show negative ROI starting from June
  - Marketing does not pay back within the target 28-day period
- Channel differences:
  - `FaceBoom`: fast purchases but very low retention and negative ROI
  - `TipTop`: loyal users but too expensive to acquire
  - `RocketSuperAds`: best balance of cost and profitability
  - `MediaTornado`: stable and low-cost channel with moderate performance

### Conclusions

The increase in users did not lead to proportional revenue growth.

**Main reasons:**
- Weak user engagement after acquisition
- High acquisition costs in key channels
- Low long-term value from some fast-conversion users
- Declining profitability of major marketing sources

**Recommendations:**
- Reduce spending on `FaceBoom` due to negative ROI
- Limit budget for `TipTop` in the short term (high CAC problem)
- Increase investment in:
  - `RocketSuperAds`
  - `MediaTornado`
- Monitor CAC growth in all major channels
- Improve retention and engagement strategies for new users
- Focus on increasing LTV, not only user acquisition

---

### Tools & Technologies

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn`





