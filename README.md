# Massachusetts-Loan-Default-Risk
*Contributors:* Kara Liao, Roberto Albornoz, Sai Leela Rahul Pujari, Juncheng (Leo) Zhu, Sarah Dsouza

### Objectives:
Build a Massachusetts loan-level risk view by combining LendingClub 2019 borrower features with local ACS socioeconomic indicators at the ZIP3 level.
Quantify how credit quality (FICO, grade) and capacity-to-repay (DTI, term) drive default probability and pricing.
Test whether community-level conditions (income, age structure) add incremental signal to borrower-level risk.
### Key Findings:
#### Default risk declines monotonically with higher FICO and better grades
<img width="1570" height="971" alt="image" src="https://github.com/user-attachments/assets/7f5303ff-f975-4107-8015-16c7a44fa4a7" />

#### Interest rates are inversely related to FICO and grade, indicating broadly consistent risk-based pricing.
<img width="1778" height="981" alt="image" src="https://github.com/user-attachments/assets/b25c4540-20af-4257-9ddc-9d3e0515e4e0" />

#### High-income areas (yellow-green on the left map — e.g., Greater Boston, MetroWest) tend to exhibit lower delinquency rates (darker green on the right map).
<img width="2922" height="1471" alt="image" src="https://github.com/user-attachments/assets/f78c474a-e397-4de8-b33a-6d7f6495c501" />

#### Higher income groups tend to have higher average FICO scores, with FICO score trends increasing as income rises.
<img width="932" height="583" alt="image" src="https://github.com/user-attachments/assets/b7e589eb-4a0e-4408-9c34-34ca5ccd11c4" />

#### The Massachusetts portfolio skews modestly toward higher-grade (lower-risk) loans, suggesting better borrower quality relative to the U.S. average.
<img width="975" height="506" alt="image" src="https://github.com/user-attachments/assets/d6e105a3-4b42-4403-a93d-054f85667f5c" />

###  Methods:
Data Preparation: Cleaned and standardized LendingClub data. Derived key metrics such as Debt-to-Income (DTI), Revolving Balance, and Employment Length.
Exploratory Data Analysis (EDA): Conducted national-level and Massachusetts-specific EDA through visualizations (violin, heatmap, bar, and correlation plots) to identify relationships between borrower risk factors (FICO, grade, term, purpose) and loan outcomes.
Integration & Mapping: Joined borrower data with ZIP3-level ACS indicators (income, age, and population metrics) to visualize spatial variation in loan delinquency and median income across Massachusetts.
### Recommendations:
Anchor underwriting on FICO and grade, and add term-based PD uplifts to reflect longer exposure.
Incorporate a simple geographic overlay (ZIP3 median income) as a tie-breaker for borderline files and for portfolio concentration limits.
Favor smaller amounts and/or shorter terms for riskier grades, and monitor high-DTI pockets within low-income ZIP3s for early-warning signals.
