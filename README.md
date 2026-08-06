## Power Bi dashboard.


<img width="1307" height="702" alt="Screenshot 2025-07-17 200610" src="https://github.com/user-attachments/assets/5c98f6b5-f72a-43ce-b06c-22af381c5b32" />
<img width="1356" height="765" alt="Screenshot 2025-07-17 200552" src="https://github.com/user-attachments/assets/301726f0-aea7-4c0e-83f5-322bfa5a330b" />
<img width="1292" height="697" alt="Screenshot 2025-07-17 200624" src="https://github.com/user-attachments/assets/1c3521ee-2945-48f5-8e7d-b95e7365e613" />


Bank Client & Risk Analysis Dashboard
Problem Statement

Every loan a bank gives out carries risk. Before approving one, the bank needs to know: is this client likely to repay? This project explores client and banking data to understand deposit, saving, and lending behavior — and to surface patterns that could support smarter lending decisions.

What I Did

I cleaned and explored a multi-table banking dataset (clients, relationships, advisors, gender, and time period tables linked by client ID), then built a Power BI dashboard so the numbers are easy to act on.

Data cleaning highlights: handled missing/duplicate values, added an Engagement Days column , grouped clients into Income Bands, and derived Processing Fees from each client's fee tier.

Dashboard: four pages — Home, Loan Analysis, Deposit Analysis, and Summary — built on KPIs like Total Clients, Total Loan, Total Deposit, and Credit Card Balance, using DAX (SUM, SUMX, DISTINCTCOUNT, SWITCH, DATEDIFF).



Key Insights
1. Deposits and savings move together. Clients who deposit more also tend to hold higher savings balances — likely the same financially engaged customers doing both.
2. Age and income drive accumulation. Older and higher-earning clients carry larger savings, superannuation, and credit/loan balances — consistent with having more time and income to build assets.
3. Property ownership is a weak signal. It barely correlates with banking balances, suggesting it's shaped by outside factors like the real estate market or inheritance, not banking behavior.
4. Business banking is its own segment. Business lending overlaps a bit with personal loans but not with deposits — pointing to business clients as a distinct group from typical personal-banking customers.
Why It Matters

A bank could use this dashboard to spot high-exposure clients, identify which segments hold the most deposits or loans, and see that private banks in this dataset attract more clients — a useful signal for growth strategy. Adding repayment history next would move this from descriptive insight toward real credit-risk prediction.

Tools

Python (pandas) · Power BI (DAX)
