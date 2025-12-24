# Portfolio Risk & Concentration Analysis

## Overview
This notebook demonstrates a **portfolio risk and concentration analysis pipeline** using your current stock positions.  
It calculates **portfolio weights, evaluates position-level risk, identifies concentration exposures**, and provides **visual analytics** to guide informed decision-making.

The notebook emphasizes **reviewer-friendly design**, including enhanced charts, inline screenshots, and clear risk-level tables.

---

## Features
- Calculation of **% of portfolio** for each position  
- Rule-based **risk scoring** per position  
- **Concentration analysis** across sectors and holdings  
- Enhanced visualizations:  
  - **Pie chart** for portfolio allocation (Step 5a)  
  - **Horizontal bar chart** for risk levels (Step 5b)  
- Inline documentation with screenshots  
- Summary insights for **top-risk positions**  

---

## Skills Demonstrated
- Data manipulation with **pandas**  
- Risk-level assignment and **rule-based analysis**  
- Visual analytics using **matplotlib** and **seaborn**  
- Portfolio concentration and sector exposure analysis  
- Notebook documentation with inline screenshots  

---

## Sample Portfolio Positions
| Ticker | Name | Shares | Price | % of Portfolio | Risk Level | Sector |
|--------|------|--------|-------|----------------|------------|--------|
| WBD    | Warner Bros Discovery | 31 | $28.75 | 7.96% | High | Media |
| COHR   | Coherent Corp | 3 | $190.98 | 5.12% | Medium | Tech |
| VSCO   | Victoria's Secret & Co | 5 | $55.28 | 2.47% | Medium | Retail |
| ...    | ...  | ...    | ...   | ...            | ...        | ...    |

---

## Pipeline Steps

1. **Load Portfolio Positions** — Import positions with shares, prices, and tickers.  
2. **Normalize & Calculate % of Portfolio** — Compute each position's weight relative to the total portfolio.  
3. **Concentration Analysis** — Evaluate sector and position concentration.  
4. **Rule-Based Risk Scoring** — Assign Low, Medium, or High risk based on position size, volatility, and sector exposure.  
5. **Visualizations**  
   - **Step 5a:** Portfolio Allocation Pie Chart  
   - **Step 5b:** Position Risk Levels Bar Chart  
6. **Top-Risk Positions & Summary Insights** — Highlight high- and medium-risk positions, provide key summary stats.  
7. **Inline Screenshots & Documentation** — Embed workflow screenshots and enhanced charts for clarity.

---

## Screenshots

### Step 1 — Load Portfolio
<img width="1760" height="529" alt="Step 1" src="https://github.com/user-attachments/assets/1ec00260-547c-4bb4-a034-44eef8da92bb" />

### Step 2 — % of Portfolio Calculated
<img width="1760" height="520" alt="Step 2" src="https://github.com/user-attachments/assets/b7ca5dc9-3718-4962-9650-0071b3bead59" />

### Step 3 — Concentration Analysis
<img width="1760" height="465" alt="Step 3" src="https://github.com/user-attachments/assets/d83e7bbb-11f3-4110-8529-d9f84000bd43" />

### Step 4 — Risk Scoring Applied
<img width="1761" height="479" alt="Step 4" src="https://github.com/user-attachments/assets/b66dab29-9ec9-41d0-a1b2-58ec75015376" />

### Step 5a — Portfolio Allocation Pie Chart
<img width="775" height="667" alt="Step 5a" src="https://github.com/user-attachments/assets/c5c8d31d-5fb4-410a-a8a2-dd835cee445d" />

### Step 5b — Position Risk Levels Bar Chart
<img width="1075" height="684" alt="Step 5b" src="https://github.com/user-attachments/assets/f67f5d7d-936a-492a-a765-ef8a7f3ab5aa" />

### Step 6 — Top-Risk Positions & Summary Insights
<img width="1759" height="631" alt="Step 6" src="https://github.com/user-attachments/assets/fe5ce19c-dbba-46af-9b85-0dc4e40f5b14" />

---

## Key Insights
- Largest positions are clearly highlighted in **pie chart**.  
- High- and medium-risk positions are **flagged** for review.  
- Sector concentration is monitored to prevent overexposure.  
- Portfolio is **diversified**, but top positions drive overall allocation risk.

---

## Suggested Next Steps
1. Re-run periodically to capture portfolio changes.  
2. Integrate **stress-testing or scenario simulations**.  
3. Align position risk with **overall investment objectives**.  
4. Use visuals and tables in **executive reports or presentations**.

---

## Notes
- Fully reproducible and self-contained.  
- Enhanced charts improve **reviewer comprehension**.  
- Inline screenshots document the **entire workflow**.
