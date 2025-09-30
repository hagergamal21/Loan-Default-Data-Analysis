# Loan Default Dashboard  

📊 **Dashboard Link**:  
[View on Power BI](https://app.powerbi.com/groups/aea97e13-2a76-4be4-985e-69593914219b/reports/61d810f9-9246-449a-b0ed-e75376d9eacc/77202c15de02ed887440?experience=power-bi)

📂 **Dataset Link**: [Download from Google Drive](https://drive.google.com/file/d/1LxdlX7Yh6IrifvobCMpdk9i0jH-raSqF/view?usp=sharing)  


---

## Problem Statement  

This dashboard analyzes loan performance between 2013–2018, focusing on borrower demographics, credit scores, income levels, and employment types.  

The goal is to identify high-risk borrower groups, understand default trends across years, and highlight stable lending segments. This helps financial institutions improve their risk management strategies, lending policies, and predictive modeling for defaults.  

---

## Key Questions Addressed  

- Which borrower groups contribute most to loan defaults?  
- How do credit scores and income levels impact loan stability?  
- What are the year-over-year (YOY) trends in loan growth and default rates?  
- Which segments are stable and profitable for lenders?  

---

## Steps Followed  

1. Data was ingested into Power BI Desktop from Dataflows (Dataflow Gen1 used as data source).  
2. Preprocessing in Power Query (column transformations, cleaning).  
3. Data model with measures and calculated columns (credit score bins, YOY changes, borrower categories).  
4. DAX measures created for Loan Growth YOY %, Default Rate YOY %, risk segmentation.  
5. Visualizations built with cards, line charts, bar/column charts, demographic slicers.  
6. Filters added for employment type, marital status, education, age group.  
7. Report published to Power BI Service with automated refresh using On-premises Data Gateway.  

---

## Insights & Visuals  

### [1] Loan Overview  
![Loan Default & Overview](images/Loan%20Default%20%26%20Overview.png)

- **Loan Purpose**: Home loans dominate (~6.5B), followed by business, education, and auto.  
- **Employment Risk**: Highest defaults among unemployed (3.39%) vs lowest for full-time employees (2.36%).  
- **Age Groups**: Borrowing is fairly even across adults, middle-aged, and seniors (~127K loans each). Teens borrow slightly less (~126K).  
- **Default Trends**: Defaults peaked in 2015–2016 (~11.7%), dipped in 2017, and rose again in 2018 (~11.6%).  

---

### [2] Borrower Demographics  
![Applicant Demographics & Financial Profile](images/Applicant%20Demographics%20%26%20Financial%20Profile.png)

- **Credit Scores**: Low-credit borrowers still take large loans (~128K median), creating high-risk exposure.  
- **Marital Status**: Loan amounts are consistent across single, married, and divorced (~123K–128K).  
- **Credit Bins**: Medium & high credit groups dominate (~4.5–4.6B loan volume). Very low/low groups contribute less but carry higher risk.  
- **Education**: Bachelor’s & high school grads lead (~64K loans each). PhD borrowers (~63.5K) are fewer but notable.  
- **Dependents & Mortgages**: Limited influence (~3.1B each).  

---

### [3] Financial Risk Metrics  
![Financial Risk Matrics](images/Financial%20Risk%20Matrics.png)

- **YOY Loan Growth**: +1.3% in 2015, +1.7% in 2018; dips in 2014 (–1.5%) & 2017 (–1.0%).  
- **YOY Default Change**: Spike in 2015 (+2.7%), sharp drop in 2017 (–2.8%), rebound in 2018 (+1.9%).  
- **Income & Employment**: High-income borrowers dominate with ~21.7B loans. Loan volume is balanced across employment (~5.4B each). Income stability is a stronger predictor than job type.  

---

## Key Insights  

- **Risk Hotspots**: Unemployed, self-employed, and part-time workers.  
- **Stable Borrowers**: Full-time employees & high-income groups.  
- **Economic Sensitivity**: Defaults vary YOY, influenced by external economic conditions.  
- **Credit Paradox**: Low-credit borrowers still access large loans.  

---

## Recommendations  

- **Tighten Screening** for unemployed and low-credit borrowers.  
- **Risk-Based Pricing**: Adjust interest rates/collateral for high-risk groups.  
- **Portfolio Diversification**: Spread exposure across jobs & incomes.  
- **Early Intervention**: Proactive support during downturns.  
- **Data-Driven Lending**: Use demographics & credit segmentation for predictive modeling.  
