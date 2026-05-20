## Marketplace Growth & Monetization Analysis

### Project Overview

This project analyzes the performance of a growing e-commerce marketplace.

The marketplace is in a strong growth phase and already generates stable revenue through a 5% commission on each sale. However, product decisions were previously based mostly on reports and intuition, without systematic product analytics.

As the business scaled, it became important to better understand:
- user behavior
- marketing efficiency
- revenue drivers
- product category performance

This project provides a full analysis of the user journey from acquisition to monetization, including an A/B test evaluation and business insights.

### Key Business Question

How can we improve growth quality and profitability while scaling user acquisition?

### Project Goals
- Analyze user behavior across the full funnel
- Evaluate monetization and unit economics
- Measure marketing efficiency and ROI
- Segment users and identify growth opportunities
- Analyze product categories and revenue drivers
- Evaluate A/B test results
- Generate business insights and recommendations

---

### Data Description

The project uses marketplace datasets:

`pa_marketplace_users.csv`
- `user_id` — Unique user identifier
- `registration_date` — User registration date
- `age` — User age
- `gender` — User gender
- `region` — User region
- `acq_channel` — Acquisition channel
- `buyer_segment` — Buyer segment
- `cohort_week` — Acquisition cohort week
- `cohort_month` — Acquisition cohort month


`pa_marketplace_events.csv`
- `event_id` — Unique event identifier
- `user_id` — User identifier
- `event_date` — Event date
- `event_type` — Event type
- `os` — Operating system
- `device` — Device type
- `product_name` — Product name related to the event (if applicable)
- `event_week` — Event week
- `event_month` — Event month


`pa_marketplace_orders.csv`
- `order_id` — Unique order identifier
- `user_id` — Identifier of the user who placed the order
- `order_date` — Order date and time
- `product_name` — Product name
- `quantity` — Number of product units in the order
- `unit_price` — Price per unit
- `total_price` — Total order amount
- `category_name` — Product category
- `order_week` — Order week
- `order_month` — Order month


`pa_marketplace_campaign_costs.csv`
- `acq_channel` — Acquisition channel
- `spend_month` — Month when the marketing budget was spent
- `budget` — Marketing budget spent on the acquisition channel during the specified month


`Event Types`
- `page_view` — User opened any page of the website or app
- `product_view` — Product page view
- `product_click` — Click on a product
- `add_to_cart` — Product added to cart
- `remove_from_cart` — Product removed from cart
- `search` — Search action on the platform
- `filter_apply` — Applying filters (price, brand, category, etc.)
- `checkout_start` — Start of checkout process
- `checkout_complete` — Checkout completion (does not guarantee payment)
- `user_login` — User login
- `user_logout` — User logout
- `wishlist_add` — Product added to wishlist
- `category_view` — Product category page view
- `banner_click` — Click on an advertising banner
- `promo_view` — Promotional offer or campaign view

---

### Project Structure
**1. Data loading and preprocessing**
**2. Key metrics overview**
- Monetization efficiency
- User activity and engagement
- Unit economics and marketing analysis
**3. Product performance and key risks**
**4. Insights, growth opportunities and user segmentation**
- Acquisition channel analysis
- User segmentation by type
  - New vs returning users
  - Purchase frequency analysis
- Device-based segmentation
- Regional analysis
- Funnel analysis
- Product category analysis
- Key analytical insights
**5. Experiment preparation and results analysis**
- Experiment audience analysis
- Event funnel comparison
- A/B test metrics analysis
- Final experiment conclusions

---

### Key Findings
- The marketplace shows strong user growth, but revenue growth is slowing in the second half of the year
- ARPPU and AOV remain stable, but ARPU drops due to a lower share of paying users
- Funnel conversion decreases from ~43% to ~24%, reducing overall monetization efficiency
- CAC increases over time, making user acquisition less cost-effective
- `TikTok` is the highest-volume but least efficient marketing channel (negative ROI)
- Affiliate, SEO, and Social Media channels show strong and stable profitability
- Main bottleneck is funnel conversion and user quality, not product monetization per buyer

### Conclusions

The marketplace is growing in size but losing efficiency.

**Main problem:**

User acquisition is scaling faster than monetization quality.

**Key issue areas:**
- weak funnel conversion
- inefficient marketing channels
- declining user quality in high-volume sources

### Recommendations
- Reduce or optimize TikTok spend (low ROI channel)
- Increase investment in high-performing channels (Affiliate, SEO, Social)
- Improve checkout and payment conversion
- Focus on retention and repeat purchases
- Optimize funnel before scaling marketing budget
- Validate A/B test long-term impact before scaling

---

### Tools & Technologies

`Python` `Pandas` `NumPy` `SciPy` `Statsmodels` `Matplotlib` `Seaborn`




