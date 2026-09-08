# Credit Card Financial & Customer Analytics — Power BI

## 1. Project Overview

This Power BI project analyzes credit card transaction and customer information to provide an interactive view of financial performance, transaction behavior and customer segmentation.

The project was built to strengthen:

- Power BI dashboard development
- DAX measures
- Power Query / data preparation
- Data modeling
- KPI design
- Time-series analysis
- Customer segmentation
- Business insight generation

## 2. Business Objective

The dashboard is designed to help answer:

- How is revenue changing over time?
- How does transaction amount compare with revenue?
- Which expenditure categories drive revenue?
- Which customer occupations and education groups contribute most?
- Which card categories and chip types are most important?
- What does customer revenue look like across gender, income and age segments?
- Which states contribute most revenue?
- How does customer satisfaction relate to the broader customer portfolio?
- What financial/risk indicators deserve further investigation?

## 3. Data Model

The PBIX report uses two primary entities:

### `cc_detail`

Key fields include:

- Client number
- Card category
- Annual fees
- Activation within 30 days
- Customer acquisition cost
- Week start date
- Week number
- Quarter
- Credit limit
- Total revolving balance
- Total transaction amount
- Total transaction count
- Average utilization ratio
- Chip / transaction method
- Expenditure type
- Interest earned
- Delinquency indicator

### `cust_detail`

Key fields include:

- Client number
- Customer age
- Gender
- Dependents
- Education level
- Marital status
- State
- ZIP code
- Car ownership
- House ownership
- Personal loan
- Contact type
- Customer occupation
- Income
- Customer satisfaction score

## 4. Dashboard Pages

### Page 1 — Transaction Analysis

The uploaded PBIX contains visuals for:

- Quarterly revenue vs total transaction amount
- Revenue by expenditure type
- Revenue by education
- Revenue by occupation
- Card category contribution
- Chip/transaction method contribution
- Revenue / transaction amount / interest / transaction count KPIs
- Weekly filtering
- Supporting transaction tables

### Page 2 — Customer Analysis

The customer page contains:

- Total interest
- Customer satisfaction score
- Revenue and interest by occupation
- Weekly revenue trend
- Gender distribution
- Revenue by income group
- Revenue by age group
- Top five states by revenue
- Customer-level segmentation visuals

## 5. Derived Analytics

The report uses derived concepts/measures including:

- Revenue
- Current-week revenue
- Previous-week revenue
- Week-over-week revenue
- Age group
- Income group

The core analytical pattern is:

```text
Raw transaction/customer data
        ↓
Data preparation
        ↓
Derived columns / DAX measures
        ↓
KPI layer
        ↓
Transaction analysis
        ↓
Customer analysis
        ↓
Business insights
```

## 6. Key Analytical Insights

The dashboard is designed to identify:

### Financial performance

Revenue should be evaluated together with:

- Transaction amount
- Transaction count
- Interest earned

This prevents the analysis from relying on revenue alone.

### Customer segmentation

Revenue can be compared across:

- Gender
- Age group
- Income group
- Education
- Occupation
- Geography

This supports targeted customer strategy rather than one-size-fits-all marketing.

### Transaction behavior

The combination of:

- Expenditure type
- Card category
- Chip/transaction method
- Weekly/quarterly trends

allows the business to identify where transaction activity and revenue are concentrated.

### Customer experience

Customer satisfaction is included alongside financial/customer metrics, allowing analysts to look for segments where financial value and customer experience may not align.

## 7. Benchmark Figures

The PBIX structure closely matches the public credit-card financial dashboard tutorial/data model that uses `cc_detail` and `cust_detail`.

A public reference implementation of the same model family reports benchmark figures such as:

- Overall revenue: approximately 55M
- Total interest: approximately 8M
- Total transaction amount: approximately 46M
- Card activation rate: approximately 57.47%
- Blue + Silver card categories: approximately 93% of transactions
- TX + NY + CA: approximately 68% of revenue
- Delinquency rate: approximately 6.07%

**Important:** These are benchmark/reference figures from a public implementation of the same tutorial dataset/model family. Verify values directly in the current PBIX before using them as exact portfolio claims.

## 8. Business Recommendations

1. **Segment customer strategy:** Use age, income, occupation and expenditure type together rather than independently.
2. **Monitor activation:** Track activation as a leading indicator for future transaction behavior.
3. **Connect revenue and risk:** Analyze delinquency and utilization alongside revenue and transaction growth.
4. **Use satisfaction as a guardrail:** Investigate high-revenue segments with lower satisfaction scores.
5. **Improve executive reporting:** Add a dedicated summary page with 3–5 decision-oriented insights.
6. **Document measures:** Add a data dictionary and DAX measure definitions to the repository.

## 9. Skills Demonstrated

- Microsoft Power BI
- DAX
- Power Query
- Data modeling
- KPI development
- Interactive dashboards
- Time-series analysis
- Customer segmentation
- Financial analysis
- Data visualization
- Business storytelling

## 10. Suggested Repository Structure

```text
Credit-Card-PowerBI-Analytics/
│
├── README.md
├── Credit_Card_Report.pbix


```

GitHub cannot render a PBIX interactively, so screenshots are strongly recommended.

## 11. How to Review the Project

1. Open the PBIX in Power BI Desktop.
2. Review the Transaction Analysis page first.
3. Check KPI definitions and filters.
4. Review quarterly/weekly trends.
5. Move to Customer Analysis.
6. Compare revenue across demographic and income segments.
7. Review satisfaction and geographic patterns.
8. Write down three insights before reading the portfolio README.
9. Compare your conclusions with the documented insights.
10. Identify at least two additional business questions for future analysis.

## 12. Portfolio Quality Checklist

Before publishing, verify:

- [ ] Dashboard has clear page titles.
- [ ] KPI names are unambiguous.
- [ ] Units/currency are visible.
- [ ] Slicers behave correctly.
- [ ] DAX measures are documented.
- [ ] Visuals have meaningful titles.
- [ ] No unnecessary charts are included.
- [ ] Key insights are written in business language.
- [ ] Screenshots are added to GitHub.
- [ ] README explains the business problem and not only the technical steps.

## 13. Attribution

This project was developed while following a guided Power BI credit-card financial analysis tutorial for learning purposes and then documented as part of a personal Data Analyst portfolio.

Learning references:

- Power BI project: https://www.youtube.com/watch?v=8XoDVwWdaqI
- Guy in a Cube Power BI reference: https://www.youtube.com/watch?v=MikekdopYhE

The public reference implementation used for benchmark validation:

- https://github.com/biswajit-sasmal/Credit_Card_Financial_Dashboard
