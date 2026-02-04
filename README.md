# Summer 2026 Internship Technical Assessment

Hello! This small assessment is designed to evaluate your analytical and coding skills. Please choose one of the two tasks to tackle. We designed a test as a realistic representation of the work - if you like it, you'll do well, and you'll like working with us (hopefully!). Please don't spend more than 3-4 hours on this :) Please keep this test confidential and do not distribute. 

---

## Before You Begin: Logistics Questions

**Please include your answers to the following questions at the beginning of your report:**

1. **Availability**: When can you start the internship?
2. **Short-term visa**: Do you need a US visa for short-term work (summer internship)?
3. **Full-time interest**: Are you able/interested to work full-time after the internship?
4. **Full-time visa**: Would you need visa sponsorship for a full-time role?
5. **Compensation**: What is your expected compensation for this internship?
6. **Anything else**: Is there anything else we should know about you?
7. feedback for us on the tasks / anything else? 

---

## Overview

You are provided with two synthetic datasets:
- **Electricity price data**: Hourly futures and spot prices (1 year)
- **Temperature data**: Daily temperature (10 years)

Choose **one** of the two tasks below (or attempt both if you wish, but completing one well is sufficient).

---

## Data Description

### 1. Electricity Price Data (`electricity_prices.csv`)

| Column | Description |
|--------|-------------|
| `datetime` | Timestamp |
| `futures_price` | Futures price ($/MWh) — known one day ahead |
| `spot_price` | Spot price ($/MWh) — actual settlement price |

This is a **next-day trading** setup: trades are submitted one day ahead based on the futures price, and settle at the spot price.

### 2. Temperature Data (`temperature.csv`)

| Column | Description |
|--------|-------------|
| `date` | Date (YYYY-MM-DD) |
| `temp_c` | Daily average temperature (Celsius) |

Weather affects electricity demand and prices.

---

## Task 1: Electricity Futures Trading Strategy

### Objective
Design and backtest a trading strategy for next-day electricity trading.

### Requirements

1. **Strategy design**: Develop a trading strategy — spread trading, trend following, mean reversion, or any approach you can justify.

2. **Backtest**: Implement and evaluate on out-of-sample data. Report total return, Sharpe ratio, and any other relevant metrics.

3. **Discussion**: Briefly discuss your backtesting setup, limitations, and assumptions.

### Hints
- Weather affects electricity prices
- Consider seasonality and time-of-day patterns
- You can ignore transaction costs 

---

## Task 2: Weather Pattern Analysis & Cold Winter Prediction

### Objective
Analyze temperature patterns and build a model to predict cold winter days.

**We've deliberately left this open-ended** — we want you to creatively curate your own project. Define your own target, choose your own approach, and tell us a compelling story with the data.

### Suggested Direction

1. **Explore**: Has temperature volatility changed over the 10-year period?

2. **Predict**: Build a model to predict cold winter days.
   - **Constraint**: Only use data from 6+ months prior (e.g., predict November using data up to May)
   - **Define your own target** — for example: "days below 0°C in November", "cold spells lasting 5+ days", or something else entirely

3. **Evaluate**: How well does your model work? What are its limitations?

We're excited to see what you come up with!

---

## Deliverables

Please submit the following:

### 1. Report (PDF or Markdown)
- **Maximum 5 pages** (excluding appendix)
- Structure (for example):
  1. Logistics answers (from the questions above)
  2. Executive summary (1 paragraph)
  3. Approach and methodology
  4. Results and evaluation
  5. Limitations and future improvements
  6. **AI tools disclosure**: You are welcome to use any AI tools — we want to understand your workflow 

### 2. Code
- Jupyter notebook (.ipynb) or Python scripts (.py)
- Code should be runnable and well-commented
- Include a brief explanation if necessary of how to run your code

### 3. Appendix (optional)
- Additional visualizations
- Extended analysis
- Any supporting material

---

## Submission

Please submit your report and code to [INSERT EMAIL/LINK].

**Deadline**: [INSERT DEADLINE]

---

## Questions?

If you have clarifying questions about the task, please email [INSERT CONTACT].

Good luck!
