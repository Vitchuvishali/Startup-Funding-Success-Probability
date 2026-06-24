# Startup Funding Success Probability

**Domain:** Statistics + Probability + Data Analytics + Startup Intelligence  
**Difficulty:** Beginner → Intermediate  
**Industry Focus:** Venture Capital / Startup Ecosystem / Investment Analytics / Business Intelligence

---

## 1. Problem Statement

Thousands of startups launch every year, but only a small percentage secure funding and scale successfully. Investors and startup accelerators often ask:

- Which factors influence startup funding success?
- Do experienced founders receive more funding?
- Does industry sector matter?
- Are startups from specific cities or regions more successful?
- Can statistical patterns estimate success probability?

As a Data Analyst working for a startup accelerator program, this project investigates startup funding data to identify statistical indicators associated with funding success, using probability and statistical analysis instead of relying solely on intuition.

---

## 2. Dataset Description

- **Dataset:** Recently Funded Startups In India 2026
- **Total Records:** 101 startups
- **Source:** Indian startup funding dataset (real-world style, 2026 scenario)
- **Format:** CSV

| Column | Description |
|---|---|
| `Name` | Startup name |
| `Website` | Official startup website |
| `Industry` | Sector(s) the startup operates in |
| `City` | City of operation (Bengaluru, Mumbai, Delhi NCR, etc.) |
| `Country` | Country of operation (India) |
| `Funding Amount (USD)` | Capital raised in USD |
| `Funding Type` | Funding stage (Pre-Seed, Seed, Series A–E, Growth Equity, Pre-IPO) |
| `Founder Experience (Years)` | Years of experience of the founding team |
| `Team Size` | Number of employees |
| `Revenue (USD)` | Annual revenue in USD ($0 for pre-revenue startups) |
| `Last Funding Date` | Month/Year of most recent funding round |

---

## 3. Statistical Methods

- **Data Cleaning:** Missing value handling, duplicate removal, currency string parsing (`$1,000,000` → numeric)
- **Descriptive Statistics:** Mean, Median, Standard Deviation, Quartiles, Percentiles
- **Probability Analysis:** Conditional probability by Industry, City, Funding Type, Founder Experience
- **Relationship Analysis:** Correlation matrix, heatmaps, scatter plots, bar charts, box plots
- **Hypothesis Testing:**
  - T-Test — High vs Low funding groups
  - Chi-Square Test — Industry vs Funding Type independence
  - ANOVA — Funding differences across top industries
- **Startup Segmentation:** High Growth, Revenue Driven, Early Stage, High Risk (based on funding quartiles)

---

## 4. Probability Findings

- **Overall funding success rate:** 90.1% of startups have a recorded funding amount
- **AI sector startups funding probability:** 50.0% receive above-average funding
- **Top funded industry:** Real Estate & PropTech — 100% above-average funding probability
- **Most active funding stage:** Series E — 14.9% of all deals
- **Top cities by deal volume:** Delhi NCR, Mumbai, Kolkata — 8.9% of deals each
- **Top city by average funding:** Noida — avg $5,186,000 per deal
- **Founders with 5+ years experience:** 90.5% funding success rate
- **Founders with <5 years experience:** 92.0% funding success rate
- **Probability of raising above-average funding:** ~23–24% across experience groups

**Hypothesis Testing Results:**

| Test | Hypothesis | Result |
|---|---|---|
| T-Test | H₀: No difference between high vs low funding groups | Reject H₀ — Significant difference ✅ |
| Chi-Square | H₀: Industry and Funding Type are independent | Reject H₀ — They are related ✅ |
| ANOVA | H₀: Mean funding equal across industries | Reject H₀ — Industries differ significantly ✅ |

**Business Interpretation:** Funding outcomes show measurable statistical patterns — industry sector, city, and funding stage are stronger predictors of funding success than founder experience alone in this dataset.

---

## 5. Visual Insights

| Chart | Description |
|---|---|
| `images/funding_by_industry.png` | Average funding amount by industry (top 10) |
| `images/funding_by_city.png` | Average funding amount by city |
| `images/funding_type_distribution.png` | Distribution of funding stages |
| `images/funding_distribution.png` | Overall funding amount histogram |
| `images/correlation_heatmap.png` | Correlation — Funding Amount, Founder Exp, Team Size, Revenue |
| `images/top10_funded_startups.png` | Top 10 highest funded startups |
| `images/founder_exp_vs_funding.png` | Scatter — Founder Experience vs Funding Amount |
| `images/team_size_vs_funding.png` | Scatter — Team Size vs Funding Amount |
| `images/boxplot_industry.png` | Funding spread across top 5 industries |
| `images/segment_distribution.png` | Startup segment breakdown (pie chart) |
| `images/segment_avg_funding.png` | Average funding per segment |
| `images/segment_industry_heatmap.png` | Segment vs Industry heatmap |
| `images/segment_boxplot.png` | Funding distribution per segment |
| `images/segment_by_country.png` | Segment distribution by city |

---

## 6. Recommendations

1. **Factors contributing most to funding success:**
   Industry sector, city location, and funding stage are the strongest predictors. Real Estate & PropTech and AI sectors show the highest funding probabilities.

2. **Industries attracting more investment:**
   Real Estate & PropTech (100%), AI & B2B SaaS (50%), and CleanTech sectors attract the highest above-average funding in 2026.

3. **Do experienced founders have an advantage?**
   In this dataset, founders with 5+ years experience show a 90.5% funding success rate vs 92.0% for less experienced founders — experience alone is not a decisive factor; idea and sector matter more.

4. **High potential startup segments:**
   The **High Growth** segment (top 25% by funding) shows the strongest investor interest and highest average deal sizes. Revenue Driven startups show the best path to sustainable scaling.

5. **Recommendations for investors:**
   - Prioritize Real Estate, AI, and CleanTech sectors in 2026
   - Focus on Noida and Ahmedabad — highest average deal values
   - Target Series B–E stage deals for optimal risk-return balance
   - High Growth and Revenue Driven segments offer best ROI potential
   - Avoid over-indexing on founder experience alone — sector fit matters more

---

## 7. Future Scope

- Build a machine learning classification model (Logistic Regression / Random Forest) to predict funding success probability
- Incorporate growth rate, market size, and product stage data for richer analysis
- Expand dataset across 2022–2026 for multi-year trend analysis
- Add NLP-based investor sentiment analysis from news and press releases
- Build an interactive dashboard (Streamlit / Power BI) for real-time funding probability scoring

---

## Project Structure

```
Startup_Funding_Success_Probability/
├── data/
│   └── Recently Funded Startups In India 2026 (with City, Founder Experience, Team Size, Revenue).csv
├── notebook/
│   └── analysis.ipynb
├── images/
│   └── (all generated charts)
├── reports/
├── src/
│   ├── data_loader.py
│   ├── visualizations.py
│   └── probability.py
├── README.md
└── requirements.txt
```

## How to Run

```bash
git clone <your-repo-url>
cd Startup_Funding_Success_Probability
pip install -r requirements.txt
jupyter notebook notebook/analysis.ipynb
```
NAME : VISHALI V 
IV-YEAR BE.CSE
ADHTIPARASAKTHI COLLEGE OF ENGINEERING

