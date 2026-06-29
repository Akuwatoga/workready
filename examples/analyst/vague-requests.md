# Vague Analyst Requests

Use these examples to test `/analyst-intake`.

Each request is intentionally ambiguous. A good intake should clarify business context, requester, decision owner, metric definition, data source, deliverable, timeline, and risk.

## 1. Retention Drop

Raw request:

> Can you look into why retention dropped last week?

Hidden ambiguity:

- Which retention metric: D1, D7, D30, weekly active retention, paid retention?
- Which cohort: new users, active users, paid users, region, channel?
- What baseline: previous week, same weekday, rolling average, same campaign period?
- Who will use the answer?

Good output:

- metric definition questions
- cohort/time-window questions
- likely data sources
- first-pass analysis plan
- confirmation message before pulling data

## 2. Campaign Performance

Raw request:

> Help me analyze this campaign and see whether it worked.

Hidden ambiguity:

- What does "worked" mean: conversion, revenue, retention, CAC, ROI, activation?
- Which campaign, date range, target group, and control group?
- Is the request for a quick readout or a formal review?

Good output:

- success metric list
- comparison method
- data-source map
- assumptions and risks

## 3. GMV Abnormality

Raw request:

> Check whether GMV is abnormal this week.

Hidden ambiguity:

- Which GMV definition?
- Gross or net? Includes refunds/cancellations?
- Compared with what baseline?
- Is this for all business or one category/channel/region?

Good output:

- metric definition risk
- anomaly baseline options
- data quality checks
- escalation path if abnormality is real

## 4. Sales Dashboard

Raw request:

> Make a dashboard for the sales team.

Hidden ambiguity:

- Who in sales uses it?
- What decision does it support?
- Which KPIs matter?
- Refresh frequency?
- Source of truth?
- Is this exploratory or production dashboard?

Good output:

- stakeholder map
- dashboard requirement questions
- metric owner list
- deliverable scope

## 5. Churn Reason

Raw request:

> Can you analyze why customers are churning?

Hidden ambiguity:

- Which customers?
- What counts as churn?
- What time period?
- Is this descriptive, predictive, or recommendation-oriented?
- Are there qualitative sources like tickets or interviews?

Good output:

- churn definition questions
- segmentation plan
- data-source and qualitative-source map
- likely limitations

## 6. Conversion Funnel

Raw request:

> 最近转化率不太对，你看一下。

Hidden ambiguity:

- Which conversion rate?
- Which funnel step?
- Which platform/channel/user segment?
- What changed recently?
- Who owns the funnel events?

Good output:

- funnel definition
- event tracking questions
- segment and time-window plan
- confirmation message in Chinese

## 7. User Growth

Raw request:

> 帮我看看这个月用户增长怎么样。

Hidden ambiguity:

- New users, active users, paid users, retained users?
- Compared with last month, target, forecast, or same period last year?
- Is the goal reporting, diagnosis, or recommendation?

Good output:

- growth metric matrix
- comparison baseline
- deliverable recommendation

## 8. Product Feature Impact

Raw request:

> We launched the new feature. Can you tell if it improved engagement?

Hidden ambiguity:

- Which engagement metric?
- What launch date and exposure population?
- Is there a control group or staged rollout?
- What confounders exist?

Good output:

- experiment/causal caveats
- exposure definition
- metric owner and event tracking
- analysis method options

## 9. Data Discrepancy

Raw request:

> The dashboard number does not match the finance report. Can you check?

Hidden ambiguity:

- Which dashboard, which finance report, which metric?
- Is the difference caused by timing, filters, definition, ETL, or manual adjustment?
- Who owns each source?

Good output:

- reconciliation plan
- source-of-truth questions
- owner map
- risk of reporting wrong number

## 10. Executive Update

Raw request:

> The VP wants a quick update on business health tomorrow.

Hidden ambiguity:

- Which business area?
- Which metrics define health?
- Is this a slide, email, dashboard, or talking points?
- What decisions might the VP make?
- What level of confidence is needed?

Good output:

- executive question framing
- metric shortlist
- data readiness risk
- timeline and checkpoint
- manager confirmation message

