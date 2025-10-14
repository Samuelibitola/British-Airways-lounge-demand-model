# Task 1 Justification – Lounge Eligibility Modeling

## 🧠 Background
Lounge access is a key part of the premium travel experience, and understanding lounge demand is crucial for **British Airways (BA)** to maintain high service standards while optimizing space and resources.

As BA prepares for future operations at **Heathrow Terminal 3**, it’s essential to anticipate lounge demand across various customer groups, each linked to different loyalty tiers and cabin classes.

---

## 🎯 Purpose
BA’s future flight schedules and fleet plans are dynamic, so the goal is to build a **flexible and scalable modeling approach** that forecasts how many passengers are eligible for lounge access on a typical day.

To support this, I created a **lookup framework** that allows planners to estimate lounge-eligibility percentages across different flight groupings. This tool enables forecasting even when exact aircraft or schedule details are not yet finalized.

---

## 🔍 Understanding Lounge Eligibility
Before modeling lounge demand, it’s important to understand **who is typically eligible** for lounge access.  
Eligibility is primarily determined by:
- **Travel class** (First, Business, Premium Economy, Economy)  
- **Customer-loyalty tier** (Gold, Silver, Bronze, Blue)  
- **Partner-airline status** (e.g., Oneworld Sapphire, Emerald)

Each tier supports a different group of travelers, and lounge-capacity planning depends on forecasting how many eligible passengers fall into each of these categories.

In practice, planners estimate the **proportion of passengers** eligible for each lounge tier using broad, reusable categories that can apply to future schedules.

---

## 🧮 Creating Eligibility Assumptions
Once the lounge tiers are defined, the next step is to **estimate the percentage of customers eligible** for each tier across the flight schedule.

Because BA is planning for the future, the model needs to remain **flexible** and **high-level**, rather than tied to specific aircraft types or flight numbers.

### 🗂 Example Groupings
Flights can be logically grouped by:
- **Time of Day:** Early morning, mid-day, evening departures  
- **Type of Route:** Short-haul vs long-haul  
- **Region or Destination Group:** Europe, North America, Asia, etc.  

These groupings allow the model to apply consistent assumptions across various schedules and seasons.

---

## 🧾 Eligibility Tiers
Each group of passengers is assigned an estimated eligibility proportion for one of the following tiers:

| Tier | Lounge Type | Description |
|------|--------------|-------------|
| **Tier 1** | Concorde Room | Exclusive access for First-Class and top-tier elites |
| **Tier 2** | First Lounge | For premium customers and mid-tier elites |
| **Tier 3** | Club Lounge | For Business-Class and frequent travelers |

There is no single correct method—what matters most is that **assumptions are logical, justifiable, and easy to apply** to future schedules.

---

## 📊 Applying Assumptions to a Flight Schedule
After exploring lounge eligibility and setting assumptions, the next step is to **apply the model to a real-world flight schedule**.

### 🧾 Instructions
1. **Download and review** the sample flight-schedule dataset.  
2. **Assign each flight** to one of the defined categories (e.g., by time of day, route type, or destination region).  
3. **Apply the estimated eligibility percentages** for each category to calculate how many passengers are likely to use each lounge.

> ⚠️ **Note:** The dataset contains many flights—you only need to analyze a **representative sample** (for example, flights from one time window or region). The goal is to **test your assumptions**, not cover every record.

### 🧱 Example Table Structure

| Time of Day | Route Type | Region | Total Passengers | Tier 1 % | Tier 2 % | Tier 3 % | Tier 1 Users | Tier 2 Users | Tier 3 Users |
|--------------|------------|---------|------------------|-----------|-----------|-----------|---------------|---------------|---------------|
| Morning | Short-haul | Europe | 1,200 | 2 % | 10 % | 18 % | 24 | 120 | 216 |
| Evening | Long-haul | North America | 950 | 5 % | 15 % | 25 % | 48 | 143 | 238 |

This structure provides a **reusable, generalized lookup table** that can be adapted to any future flight schedule.

> 🔹 While there is currently **no Concorde Room at Terminal 3**, the **Tier 1 estimates** can represent passengers who would qualify for that level of service. This helps inform whether a Tier 1 lounge might be needed in the future—treated purely as a **hypothetical scenario**, not a confirmed development.

---

## ⚙️ Methodology Summary
The modeling framework focuses on:
- **Grouping flights** logically by route, region, and time  
- **Applying eligibility assumptions** for each group  
- **Estimating passenger proportions** for Tiers 1–3  

This structured approach gives the **Airport Planning Team** a reusable model for testing future scenarios and planning lounge capacity efficiently.

---

## 📈 Outcome
This model enables British Airways to:
- Forecast total lounge users for each tier  
- Identify **peak-demand windows**  
- Prioritize **future investment decisions** in lounge infrastructure  

---

## 💡 Impact
This framework transforms raw airline data into **strategic insights**, allowing British Airways to maintain its premium standards while efficiently managing lounge resources and passenger experience.
