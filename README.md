# Description & Project Workflow Overview​

Horizon Financial Group is facing a serious risk crunch: their personal loan default rate has hit roughly 25% (1 in 4 loans), which is over double their healthy corporate target of 12%. This project analyzes a dataset of over 600 historical loans across 2024 and 2025 to figure out exactly why borrowers are crashing out. By exploring the relationships between borrower demographics, debt levels, and credit history, this analysis provides concrete, data-backed thresholds to help the underwriting team filter out high-risk applicants before the money leaves the bank.



# Project Workflow

- **Data Integration & Cleaning:** Merged the borrower profile dataset (demographics, income, credit scores) with the loan application dataset (amounts, interest rates, status) on a unique identifier. Cleaned missing values and verified data types.

- **Feature Engineering:** Created structured bins/ranges for continuous variables (such as credit score brackets and Debt-to-Income ratios) to make the data digestible for business analysis.

- **Exploratory Data Analysis (EDA) & Segmentation:** Grouped the data by specific borrower traits to calculate exact default rates per bucket (e.g., analyzing default percentages among lower credit tiers).

- **Correlation Analysis:** Ran a global correlation matrix across all numeric metrics to identify the strongest linear relationships and predictors of loan default status.

- **Data Visualization:** Built visual assets, including sorted bar charts and density scatter plots to clearly map out the "risk cliffs" where defaults drastically spike.

Through comprehensive exploratory data analysis, correlation testing, and data visualization, this project successfully identified the root causes behind Horizon Financial Group’s elevated 26.78% default rate and delivered actionable risk mitigation rules.



# Key Discoveries & Data Insights

- **The Ultimate Risk Factor (Credit Score):** Credit score proved to be the strongest negative predictor of default. Borrowers in the lowest bracket (520–599) experienced a staggering 49.14% default rate, meaning nearly half of these loans failed.
![Credit Score vs Default Rate](<images/Credit Score.png>)
- **The Income Strain Breakeven (DTI):** A borrower's Debt-to-Income ratio has a direct positive relationship with loan failure. Once an applicant's DTI crosses the 50% threshold, the default rate jumps to 32.83%.
![Credit Score vs Default Rate](<images/DTI vs Default Status.png>)
- **The Wedding Loan Bias (Loan Purpose):** Categorical analysis revealed that loan intent heavily influences repayment behavior. Wedding loans carry the highest risk profile with a 32.1% default rate, whereas necessity-driven Medical loans sat at the bottom at 20.6%. Interestingly, the average loan amount did not differ significantly between paid ($22,012.75) and defaulted ($22,570.55) loans, proving that loan size is not a major risk driver.
![Credit Score vs Default Rate](<images/Loan Purpose.png>)

- **Job Tenancy Impact (Employment Length):** Short-term job tenure heavily correlates with higher risk. Borrowers with less than 2 years of employment had a 32.29% default rate, compared to just 22.32% for those with 2+ years of stability.



# Measurable Business Impact

By applying the data-driven underwriting thresholds established in this project, Horizon Financial Group can systematically eliminate high-risk segments from their pipeline.
Implementing a hard cutoff at minimum 600 credit score and a maximum 50% DTI, alongside stricter manual underwriting for short-tenure employees (< 2 years) and luxury/experiential loan purposes (Weddings), is projected to drastically compress the company's overall default rate back toward its corporate target of 12%, protecting capital reserves without sacrificing high-quality loan growth.
