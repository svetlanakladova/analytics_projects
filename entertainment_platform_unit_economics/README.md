## Procrastinate Pro+ Marketing & Unit Economics Analysis

**Project Overview**

This project analyzes the performance of a digital entertainment platform after the launch of a new sports content category and changes in the marketing strategy.

The objective of the analysis is to identify the reasons behind revenue stagnation despite continuous audience growth and increasing user activity.

The study focuses on user acquisition efficiency, engagement, monetization, and marketing profitability during the first 28 days after acquisition.

**Key areas of analysis:**

- Cohort and retention analysis
- Unit economics (CAC, LTV, ROI)
- Marketing channel performance
- User engagement metrics (DAU, MAU, Stickiness)
- Customer acquisition and payback period analysis
- Product monetization and revenue dynamics


---

**Dataset Description**

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

**Tools & Technologies**

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn`





