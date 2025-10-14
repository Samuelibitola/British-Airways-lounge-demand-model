# ✈️ Task 1 – Modeling Lounge Eligibility at Heathrow Terminal 3

## 🧭 Overview
This task helps **British Airways** plan for **future lounge demand** at **Heathrow Terminal 3** using strategic data modeling.  
The goal is to analyze passenger data to determine who qualifies for lounge access so planners can forecast lounge usage and make capacity decisions.

---

## 🎯 Learning Outcomes
- Understand how airline data and modeling support **capacity planning**.  
- Learn how **customer segmentation** drives lounge-demand assumptions.  
- Build a **reusable lookup table** that predicts lounge eligibility across future flight schedules.

---

## 🧩 What Was Done
1. **Reviewed Lounge Eligibility Criteria**  
   - Ticket class (First, Business, Premium Economy, Economy)  
   - Executive Club status (Gold, Silver, Bronze, Blue)  
   - Partner-airline membership (e.g., Oneworld tiers)  

2. **Grouped Customers by Eligibility**  
   Passenger groupings were defined to estimate lounge usage and identify key drivers of demand.

3. **Created Lookup Table**  
   A reusable lookup table maps cabin class and frequent-flyer tier to lounge-access eligibility.

4. **Provided Justification**  
   Explained the logic behind the eligibility mapping and how it can be applied to future flying schedules for scenario testing and forecasting.

---

## 🗂 Example Lookup Table

| Cabin Class | Frequent Flyer Tier | Lounge Eligible | Notes |
|--------------|--------------------|----------------|--------|
| First | Any | ✅ Yes | All First-Class passengers |
| Business | Any | ✅ Yes | Access included |
| Premium Economy | Gold / Silver | ✅ Yes | Tier-based access |
| Economy | Gold | ✅ Yes | Elite-status benefit |
| Economy | Silver | ❌ No | Access only via partner rules |
| Economy | Blue | ❌ No | Not eligible |

---

## 🧠 Deliverables
- `lounge_lookup_table.xlsx` – Reusable eligibility mapping  
- `task1_justification.md` – Written rationale and modeling explanation  

---

## 💼 Skills Demonstrated
- Data modeling & segmentation  
- Analytical reasoning for capacity forecasting  
- Excel / Python data manipulation  

---

## 📄 Notes
This task is part of the **British Airways – Data Analytics Virtual Experience Program** on [Forage](https://www.theforage.com/).  
Content and scenarios are for educational and portfolio purposes only.
