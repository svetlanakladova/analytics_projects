## SollmaFin A/B Test & Product Analytics

### Project Overview

SollmaFin is a fintech app for investing in stocks, ETFs, currencies, and crypto. It is mainly used by beginner investors in Latin America (Brazil, Mexico, Colombia, Argentina).

The main problem in the product was that many users invest in risky assets without fully understanding them. This often leads to losses and users stop using the app after their first deposit.

To solve this, the product team introduced a new onboarding flow. It explains how financial assets work and shows the risks in a simple way.

This project analyzes user behavior and A/B test results to understand whether educational onboarding improves long-term user activity and monetization.

### Key Business Question
Does educational onboarding help users become more active and valuable, without reducing first deposit conversion?

**A/B Test Design**
- Users: New users (June 2 – June 15, 2025)
- Groups: Control vs Test (random split)
- Control: Standard onboarding
- Test: New onboarding with education about assets and risks
- Observation period: 7 days after registration

**Metrics**
- Main metric: Average total deposit per user
- Safety metric: Registration → First deposit conversion
- Support metrics:
  - First → Second deposit conversion
  - Average deposit per paying user
  - Deposit distribution (25th, 50th, 75th percentiles)

---

### Contents

**1. Historical Data Preparation**
- Data Loading and Preprocessing
  
**2. Exploratory Data Analysis**
- New User Analysis
- Event Funnel Analysis
- Impact of Asset Risk Level on Second Deposit Conversion
- Historical Monetization Metric Analysis

**3. A/B Test Analysis**
- Experiment Audience Analysis
- Event Funnel Comparison
- Impact of the New Feature on Second Deposit Conversion by Asset Risk Level
- A/B Test Metrics Analysis

**4. Paying User Deposit Analysis**
- Changes in Deposit Amounts per Paying User

**5. Conclusions**
- Final Conclusions

---

### Final Summary

The new onboarding does not change the main conversion rate, but it improves user quality after the first deposit.

**Main results:**
- First deposit: no negative impact
- Second deposit: clear improvement
- Paying users: higher deposits
- Low-intent users: slightly lower activity

**Recommendation:**

Use a mixed onboarding strategy:
- Keep educational onboarding for users interested in risky assets
- Use simpler onboarding for beginners
- Continue tracking long-term user behavior

---

### Dataset Description

The project uses two datasets:
`Historical Dataset` — contains user activity data for new users acquired between April 1 and June 1, 2025.
`A/B Test Dataset` — contains experiment data for users registered between June 2 and June 15, 2025.

**Main Dataset Features:**
- `user_id` — unique user identifier
- `country_code` — user country (BR, MX, AR, CO)
- `platform` — mobile or web
- `first_ts` — timestamp of the user's first appearance in the system
- `first_dt` — date of the user's first appearance (without time)
- `event_ts` — event timestamp
- `event_name` — user action inside the platform
- `amount` — deposit amount
- `asset` — purchased financial asset
- `risk_level` — asset risk category (low / medium / high)
  
The `/datasets/pa_sollmafin_abt.csv` dataset also includes two additional fields:
- `ab_test` —  A/B experiment name
- `group` — A/B experiment group

---

### Tools & Technologies

`Python` `Pandas` `NumPy` `SciPy` `Matplotlib` `Statsmodels`
