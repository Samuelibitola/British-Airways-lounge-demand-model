# ✈️ British Airways Data Science Virtual Experience – Task 1  
### Modeling Lounge Eligibility at Heathrow Terminal 3  

---

## 🧠 Task Overview

**Objective:**  
Help British Airways plan for future **lounge demand** using strategic data modeling.

**Goal:**  
Create a reusable **lookup table** and written justification that British Airways can apply to future flying schedules.  

---

## 💡 What You'll Learn
- How airline data and modeling help BA forecast lounge demand.  
- How to use customer groupings to inform future capacity planning.  
- How to create scalable, logical assumptions for predictive modeling.  

---

## 🧾 Background

Lounge access is a vital part of the premium travel experience.  
Understanding lounge demand helps **British Airways (BA)** maintain high standards while optimizing space and resources.

As BA plans for future operations at **Heathrow Terminal 3**, it’s essential to anticipate demand across different lounge access types — each associated with varying levels of loyalty and travel class.

However, future schedules are unpredictable. This means we need a **flexible, scalable modeling approach** to estimate lounge usage without requiring exact aircraft or flight details.

Your job is to create a **lookup table** BA can use to estimate lounge eligibility percentages across different flight groupings — allowing the business to forecast demand and make informed investment decisions.

---

## 🔍 Understanding Lounge Eligibility

Lounge access depends on **customer loyalty status** and **travel class**, with each tier representing a different level of exclusivity and amenities.

Eligibility is typically determined by:
- **Travel class** – First, Business, Premium Economy, Economy.  
- **Loyalty status** – Gold, Silver, Bronze, Blue.  
- **Partner status** – e.g., Oneworld Sapphire, Emerald.  

Each tier supports a different group of travelers, so lounge capacity planning relies on forecasting how many passengers fall into each tier.

---

## ⚙️ Creating Eligibility Assumptions

Since BA is planning far into the future, your model should rely on **high-level groupings** — not specific flight numbers or aircraft types.  

Common groupings include:
- **Time of day:** Early morning, mid-day, evening.  
- **Route type:** Short-haul vs. long-haul.  
- **Region or destination group:** Europe, North America, Asia, etc.

You’ll estimate what proportion of passengers in each group are likely to be eligible for:

| Tier | Lounge Type        |
|------|--------------------|
| Tier 1 | Concorde Room      |
| Tier 2 | First Lounge        |
| Tier 3 | Club Lounge         |

There’s no single “correct” approach — what matters most is that your assumptions are **logical, justifiable, and scalable**.

---

## 🧮 Applying Assumptions to a Flight Schedule

Now, apply your model to a real-world flight schedule.

**Instructions:**
1. Download and review the dataset:  
   📂 `British Airways Summer Schedule Dataset - Forage Data Science Task 1 (1).xlsx`
2. Assign each flight to one of your defined categories (e.g., time of day, route type, region).
3. Apply your eligibility percentages to calculate the number of passengers likely to use each lounge.

> 💡 *Note:* While there’s currently no Concorde Room at Terminal 3, Tier 1 estimates represent a **potential premium segment** for future strategic planning.

Focus on applying your assumptions **per category**, not per flight.  
Your output should be a **reusable lookup table** that can easily scale to future schedules.

---

## 📂 Dataset

**File Name:** `British Airways Summer Schedule Dataset - Forage Data Science Task 1 (1).xlsx`  
This dataset represents a **sample summer flight schedule** used for modeling lounge eligibility.  
It includes departure times, routes, and destination details.


