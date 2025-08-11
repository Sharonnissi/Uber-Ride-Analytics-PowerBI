# Uber Ride Analytics 2024 — Power BI Dashboard

I built this Power BI dashboard to explore patterns in **ride bookings and revenue** using a 2024 Uber dataset. It has attributes like booking status, vehicle type, payment method, ride distance, ratings, and cancellation reasons (customer and driver). I wasn’t just trying to visualize trends, but to understand what’s **really driving revenue and ride success** across payment channels and vehicle categories.

---

### Executive Summary

This project tells the story of how ride outcomes are shaped by **payment behavior, vehicle type, and cancellation friction**, it is not just raw demand.

Some key takeaways:

- **UPI leads revenue share**, with **Cash** a strong second; wallets and cards round out the mix, suggesting that **low-friction payments** boost conversion.
- **Auto / Go Mini / Go Sedan** carry most of the revenue load; premium categories contribute less volume but help with **average revenue per ride**.
- Monthly revenue is **stable within a narrow band**, peaking early in the year—pointing to consistent demand while **operational bottlenecks** limit upside.
- **Top cancellation reasons** (wrong address, driver not moving, change of plans) are actionable via **address validation, driver nudges, and ETA transparency**.
- **Ratings are steady** (customers ≈ 4.4, drivers ≈ 4.2) across vehicle types, indicating generally reliable service quality.

Overall, the data shows that successful growth strategy depends on removing **payment & pickup friction**, keeping **high-throughput vehicle types** available, and tackling **cancellation root causes**, not just putting more cars on the road.

---

## Key Business Questions Answered

1. **Which vehicle types contribute the most to revenue and volume?**  
2. **Which payment methods drive the largest share of revenue?**  
3. **How does revenue evolve across the year (and how do we make the trend readable)?**  
4. **What are the top cancellation reasons (customer vs. driver) and how big are they?**  
5. **Are customers and drivers consistently satisfied across vehicle types?**

---

## Visualizations & Insights

### 1) Which vehicle types generate the most revenue?

> **Auto, Go Mini, and Go Sedan** lead revenue, reflecting high availability and broad price–distance fit. Premium categories (e.g., **Uber XL**, **Premier Sedan**) add to **average revenue per ride** despite smaller share.

---

### 2) Which payment methods drive revenue?

> **UPI** contributes the largest share, followed by **Cash**. **Uber Wallet**, **Credit Card**, and **Debit Card** split the remainder. Frictionless payments appear to **unlock higher conversion** and reduce checkout drop-off.

---

### 3) How does revenue trend across the year?

> To avoid a spiky daily line, the dashboard uses **monthly bins** (and an optional **moving average**) for a cleaner, executive-friendly view. Revenue stays **remarkably consistent** within the year, with a modest peak early on.

---

### 4) Why do cancellations happen?

> **Customers:** wrong address, driver not moving, and change of plans dominate.  
> **Drivers:** capacity/personal issues and customer-related concerns are common.  
> These are **actionable**—address validation UX, driver routing nudges, and clearer pre-pickup comms can **reduce cancellation leakage**.

---

### 5) Are riders and drivers satisfied?

> **Customer ratings ~4.4** and **driver ratings ~4.2** are stable across vehicle types. Sedans tend to score slightly higher with customers; drivers report consistent satisfaction in higher-capacity categories.

---

## Conclusion

This wasn’t just about charts, it was about connecting **revenue outcomes** to **operational levers**.

**These insights can help:**
- **Payments & Growth** drive adoption of **low-friction channels** (UPI/wallets).
- **Ops & Product** cut cancellations with **address validation**, **driver movement nudges**, and **ETA clarity**.
- **Supply** keeps high-throughput vehicle types (Auto/Go Mini/Go Sedan) well covered by **time and area**.
- **CX/Quality** monitors vehicle-type deltas in ratings to preempt **experience gaps**.

---

## Tools Used
- Power BI Desktop  
- DAX (revenue, rates, moving average, MoM%)  
- Power Query (type casting, Trim/Clean, reason standardization, calendar helpers)  
- Visuals: Cards, Donut, Clustered Bar/Column, Line (with MA), Grouped Bars

---

## Dataset
Uber Ride Analytics 2024 (demo dataset with one calendar year of daily bookings).  
https://www.kaggle.com/datasets/yashdevladdha/uber-ride-analytics-dashboard?select=ncr_ride_bookings.csv



