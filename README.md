# Free delivery on orders over 100 SAR

## Description
Bayt Market is a grocery-delivery app. The experiment decides whether to waive the delivery fee on orders of 100 SAR or more.

## Question and hypothesis
- Decision: Should Bayt Market waive the delivery fee on paid orders of 100 SAR or more?
- Hypothesis: If we waive that fee, then the 7-day order rate will rise by at least 1 percentage point, because the fee is a reason people stop at checkout.

## Design
- Unit of randomization: the user account, one entry each, split 50/50.
- Primary metric and guardrail metrics: 7-day order rate. Guardrails are profit per user, cancellation, and contact with support.
- Sample size and duration: 14,749 users per group, 7 enrollment days, about 35,000 users. The planned week can detect about 0.90 percentage points.

## Results and recommendation
- Main effect and confidence interval: +0.44 percentage points (95% CI -0.20 to +1.08). Profit per user -0.93 SAR (95% CI -1.10 to -0.76).
- Recommendation: Do not launch. The order-rate result is not decisive, and profit per user deteriorated.

## How to run
1. Open the notebook in Google Colab: from the project folder open the file, or in Colab choose File, then Open notebook.
2. Run the cells in order. The data come from a simulation with a fixed seed, so the same results repeat.

## Requirements
Python 3 with numpy, pandas, scipy, statsmodels and matplotlib, all available in Colab.

## Technical documentation
- Section 3: sample size and duration.
- Section 6: trust checks and allocation ratio.
- Section 7: analysis with CUPED and multiple-testing correction.
- Section 9: report and recommendation.

## Repository structure
- project_template.ipynb: the project notebook
- README.md: this file
- one_page_report.md: the one-page report from section 9
- presentation.pptx: the 10-minute presentation

## About the program
This project was carried out as part of the "Experiments, A/B Testing & Causal Inference" program at SDAIA Academy, November 2026.
SDAIA Academy on GitHub: https://github.com/SDAIAAcademy
