# Financial-Based Company Valuation Using Integrated AHP-DEA Method

## Overview
This project evaluates the financial performance of selected Malaysian banking companies using a **hybrid Multi-Criteria Decision-Making (MCDM) approach** that integrates the **Analytic Hierarchy Process (AHP)** and **Data Envelopment Analysis (DEA)**. The aim is to rank companies based on financial metrics and identify efficient performers over the 2018–2024 period.

---

## Motivation
Financial valuation is essential for investors, fund managers, and analysts. Traditional approaches may not consider multiple criteria simultaneously. This project applies a **systematic, quantitative methodology** by combining expert judgment and efficiency analysis to provide actionable insights for decision-making.

---

## Scope
- Focused on **Malaysian banking companies** listed on Bursa Malaysia:  
  - RHB Bank Berhad  
  - Hong Leong Bank Berhad  
  - CIMB Group Holdings Berhad  
  - Public Bank Berhad  
  - Malayan Banking Berhad  
- **Time frame:** 2018–2024  
- **Metrics used:** Detailed in Appendix Table 1.1  
- **Expert input:** Weights obtained from 10 experts including Portfolio Managers, Fund Managers, Managing Directors, and Investment Analysts  
- **Tools:** RStudio and Excel for modeling and analysis  

*Appendix: Table 1.1 – Financial Metrics*  
```markdown


| Criteria                     | Definition                                                      | Subcriteria           | Definition & Formula                                |
| ---------------------------- | --------------------------------------------------------------- | --------------------- | --------------------------------------------------- |
| C1 Valuation Ratios          | Assess stock price relative to earnings, revenue, or book value | P/E Ratio             | Price per earnings, indicates over/undervaluation   |
|                              |                                                                 | P/B Ratio             | Price per book value, indicates over/undervaluation |
|                              |                                                                 | EV/EBITDA             | Enterprise value relative to operating earnings     |
| C2 Profitability Ratios      | Company’s ability to generate profit                            | Net Profit Margin     | % revenue remaining as profit                       |
|                              |                                                                 | ROA                   | Profit generated per asset                          |
|                              |                                                                 | ROE                   | Profit generated per equity                         |
| C3 Liquidity Ratios          | Ability to meet short-term obligations                          | Current Ratio         | Current assets ÷ current liabilities                |
| C4 Cash Flow Analysis        | Evaluate cash inflows/outflows                                  | Free Cash Flow        | Cash available after capital expenditures           |
| C5 Operational Efficiency    | Resource utilization effectiveness                              | Gross Margin          | % revenue retained after production costs           |
|                              |                                                                 | Operating Margin      | % revenue remaining after operating expenses        |
| C6 Debt Metrics              | Company leverage & debt management                              | Debt-to-Equity        | Total debt ÷ shareholder equity                     |
|                              |                                                                 | Interest Coverage     | EBIT ÷ interest expenses                            |
| C7 Revenue & Earnings Growth | Financial expansion over time                                   | Revenue Growth Rate   | % increase in sales                                 |
|                              |                                                                 | EPS Growth            | % increase in earnings per share                    |
| C8 Dividend Metrics          | Evaluate dividends                                              | Dividend Yield        | % of price returned as dividends                    |
|                              |                                                                 | Dividend Payout Ratio | % of net income distributed as dividends            |
```
---

## Technologies / Tools Used
- **RStudio** – computational modeling and analysis  
- **Excel** – data preprocessing and visualization  
- **Libraries / Packages:** `dplyr`, `tidyverse`, `deaR`, `ggplot2`  
- **Methodologies:** AHP for weight determination, DEA for efficiency evaluation  

---

## Methodology
1. **Data Collection:** Gathered financial statements of selected banks (2018–2024).  
2. **Financial Metric Selection:** Metrics defined in Table 1.1.  
3. **Weight Assignment using AHP:** Experts performed pairwise comparisons; consistency validation ensured reliable weights.  
4. **DEA Analysis:** Weighted DEA-VRS model calculated efficiency scores and rankings.  
5. **Integration:** Combined AHP weights with DEA for final company rankings.  
6. **Visualization:** Plots and tables generated for comparative analysis.  

---

## Results / Key Findings
- **Efficiency Scores & Rankings:** DMU2 consistently performed best; DMU3 underperformed.  
- **Correlation with Stock Performance:** DEA efficiency showed moderate correlation with stock price growth, highlighting intrinsic financial quality beyond market fluctuations.  

---

## References

Saaty, T. L. (1980). The Analytic Hierarchy Process.

Charnes, A., Cooper, W. W., & Rhodes, E. (1978). Measuring the efficiency of decision-making units.

Aljuhaishi and Kadhim (2023); Eghbali Amooghin et al. (2023)
