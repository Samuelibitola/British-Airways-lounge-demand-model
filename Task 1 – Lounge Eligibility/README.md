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

## 🧩 Example Answer

**Great work!**  
Take a look at the example answer below to see how a member of the **Data Science team at British Airways** might approach this task.  

This example demonstrates how to **group flights** and apply **logical eligibility percentages** across lounge tiers.  
Your final output may look different — what matters most is that your assumptions are **clearly structured, data-driven, and well-reasoned.**

---

### ✈️ Example Lookup Table (Simplified)

| Flight Group              | Route Type | Time of Day  | Region        | Tier 1 (Concorde Room) | Tier 2 (First Lounge) | Tier 3 (Club Lounge) |
|----------------------------|-------------|---------------|----------------|-------------------------|------------------------|----------------------|
| Long-Haul, North America   | Long-haul   | Evening       | North America  | 5 %                     | 15 %                   | 40 %                 |
| Long-Haul, Asia-Pacific    | Long-haul   | Mid-day       | Asia-Pacific   | 4 %                     | 12 %                   | 35 %                 |
| Short-Haul, Europe (AM)    | Short-haul  | Early Morning | Europe         | 1 %                     | 6 %                    | 20 %                 |
| Short-Haul, Europe (PM)    | Short-haul  | Evening       | Europe         | 0.5 %                   | 5 %                    | 18 %                 |
| Middle East & Africa       | Long-haul   | Mixed         | MEA            | 3 %                     | 10 %                   | 30 %                 |

---

### 🧾 Example Justification

**How flights were grouped:**  
Flights were categorized by *route type*, *region*, and *time of day* to capture major behavioral and capacity differences.  
Long-haul evening flights often include a higher proportion of premium passengers compared to short-haul morning flights.

**Why these groupings make sense:**  
Passenger composition and lounge demand vary significantly across route types and regions — for example, business travelers dominate early-morning European flights, while leisure travelers dominate evening long-haul departures.

**Assumptions made:**  
- Long-haul flights have a higher percentage of premium and status passengers.  
- Tier 1 (Concorde Room) represents only the highest fare-paying or elite travelers.  
- Tier 3 (Club Lounge) has broader access for Business Class and mid-tier loyalty members.  

**Scalability:**  
This model can be updated dynamically by adjusting the eligibility percentages and applying the lookup table to future schedules without needing individual flight details.

---

📈 *This example highlights logical reasoning and structure — your version should reflect your own thought process, dataset interpretation, and modeling choices.*

---

## 📄 Notes
This task is part of the **British Airways – Data Analytics Virtual Experience Program** on [Forage](https://www.theforage.com/).  
Content and scenarios are for educational and portfolio purposes only.
