## Marketplace Growth & Monetization Analysis

**Project Overview**

This project explores user behavior, monetization, marketing efficiency, and product performance for a growing e-commerce marketplace.

The analysis covers the full user lifecycle — from acquisition and activation to retention, monetization, and experimentation — with a focus on identifying growth opportunities and evaluating business performance.

**Key areas of analysis:**

- Funnel and retention analysis
- Unit economics (ARPU, ARPPU, CAC, LTV)
- Marketing channel performance
- User segmentation
- Product metrics and monetization
- A/B testing and statistical evaluation

---

**Dataset Description**

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

**Tools & Technologies**

`Python` `Pandas` `NumPy` `SciPy` `Statsmodels` `Matplotlib` `Seaborn`




