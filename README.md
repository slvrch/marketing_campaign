# marketing_campaign

## Background Business

A retail company invests heavily in digital marketing campaigns across multiple marketing channels, campaign types, customer segments, and campaign duration to drive customer acquisition and sales growth.

During the latest marketing period, the company generated **29T in total revenue** with an **average ROI of 246.70**, demonstrating that its marketing investments delivered measurable business value.

However, these high-level KPIs only indicate what the business achieved—not why certain campaigns performed better than others, where customers dropped off throughout the marketing funnel, or which marketing strategies consistently generated stronger business outcomes.


## Business Problem

Although the company has achieved strong overall marketing performance, management lacks visibility into the key drivers behind campaign success. As marketing campaigns become increasingly complex, relying solely on aggregate KPIs makes it difficult to identify which strategies should be prioritized to maximize marketing ROI.

## Business Questions
- How did campaign revenue and acquisition cost change over time?
- Where are the bottlenecks in the customer journey?
- Which campaign types perform best across different campaign durations?
- Which campaign types increase or reduce ROI across customer segments?
- Which multi-channel combinations deliver the highest ROI?
- Does higher customer engagement lead to better campaign performance?

## Objective of Analysis

To support data-driven marketing decisions, this project develops an interactive dashboard that evaluates campaign performance, identifies optimization opportunities across customer journey, campaign strategies, customer segments, and marketing channels, and provides actionable insights to improve marketing effectiveness.

## Data Understanding

### Dataset Overview

- Dataset: Synthetic Digital Marketing Campaign Dataset
- Period: July 2024 - 24 June 2025
- Business Domain: Marketing Analytics
- Total Records: 55.555 campaign records
- Granularity: Each row represents the performance of a single marketing campaign, including campaign characteristics, target audience, marketing channels, customer engagement, and business performance metrics.

### Data Categories

| Category             | Variables                                     | Business Purpose                     |
| -------------------- | --------------------------------------------- | ------------------------------------ |
| Campaign Information | Campaign_ID, Campaign_Type, Campaign_Duration | Identify campaign characteristics    |
| Customer Information | Customer_Segment, Audience_Type, Language     | Analyze audience behavior            |
| Marketing Channels   | Channel_Used, Channel_Count                   | Evaluate multi-channel strategies    |
| Funnel Metrics       | Impressions, Clicks, Leads, Conversions       | Measure customer journey performance |
| Financial Metrics    | Revenue, Acquisition_Cost, ROI                | Evaluate marketing profitability     |
| Engagement Metrics   | CTR, Engagement_Score, Engagement_Level       | Assess customer interaction          |


### Data Quality

- Missing values: None detected
- Duplicate records: None detected
- Data types validated
- Multi-channel combinations standardized

### Feature Engineering

| New Feature             | Purpose                               |
| ----------------------- | ------------------------------------- |
| Campaign Duration Group | Compare campaign duration performance |
| Channel Count           | Measure number of marketing channels  |
| Engagement Level        | Categorize customer engagement        |
| Funnel Table            | Transform funnel metrics into stage-level structure          |

### Mapping Data to Business Questions

| Business Question | Main Variables                                       |
| ----------------- | ---------------------------------------------------- |
| Q1                | Revenue, Acquisition Cost, Date                      |
| Q2                | Impressions, Clicks, Leads, Conversions              |
| Q3                | Campaign Type, Campaign Duration Group, ROI          |
| Q4                | Customer Segment, Campaign Type, ROI                 |
| Q5                | Channel Combination, ROI                             |
| Q6                | Engagement Level, CTR, Revenue, ROI, Conversion Rate |


### Data Limitations

- The dataset is synthetic and designed for analytical practice rather than representing a real company's marketing performance
- Business interpretations should therefore be considered illustrative
- June 2025 contains data only through 24 June 2025, making it a partial reporting period

## Analytics

<img width="873" height="473" alt="image" src="https://github.com/user-attachments/assets/7ca2ebee-26a5-43d0-8015-dfc71bd13510" />

Insight:
- Campaign performance remained stable from July 2024 to June 2025, indicating consistent marketing execution throughout the reporting period
- Revenue and acquisition cost followed similar trends, suggesting that marketing investment remained proportional to campaign performance without unusual spending fluctuations
- The decline observed in June 2025 should not be interpreted as a deterioration in campaign performance because the dataset contains only partial-month records (through 24 June 2025)

<img width="789" height="386" alt="image" src="https://github.com/user-attachments/assets/be3d2273-410a-48ca-b73c-86fb07008530" />

Insight:
- Only **1.9%** of users completed the entire customer journey
- The most significant customer drop-off occurred between **Impressions and Clicks**, with **91.49%** of users failing to engage
- Customer progression improved after the lead stage, with **55.02%** of leads successfully converting
- The initial engagement stage represents the highest-priority opportunity for funnel optimization


<img width="764" height="423" alt="image" src="https://github.com/user-attachments/assets/4dca798f-ae0d-4c3a-8838-86a10dc0c5fe" />

Insight:
- Medium-duration campaigns generated the highest ROI for SEO, Social Media, and Influencer
- Paid Ads achieved the strongest ROI in **long-duration campaigns**
- Email campaigns delivered their highest ROI in **short-duration campaigns**
- Campaign duration should be optimized based on campaign type rather than applying a single duration across all marketing activities

<img width="790" height="418" alt="image" src="https://github.com/user-attachments/assets/fad141c5-a41c-4127-aaef-361da6761c8c" />

Insight:
- Working Women responded most positively to **Social Media** campaigns, while **Email** campaigns generated the largest negative ROI contribution
- Premium Shoppers achieved the strongest ROI improvement from **Email** campaigns, whereas **Social Media** generated the largest negative ROI contribution
- Tier 2 City Customers benefited most from **Influencer** campaigns, while **Paid Ads** showed the largest negative ROI contribution
- College Students exhibited the weakest overall ROI improvement, with only marginal positive contributions from **Email** and **Paid Ads**, while **Influencer** campaigns generated the largest decline in ROI


<img width="768" height="405" alt="image" src="https://github.com/user-attachments/assets/14f54e7f-bac5-4fd5-b32f-d0fc035d18f1" />


Insight:
- The **Email-WhatsApp-Facebook** achieved the highest average ROI among the Top 10 channel combinations
- Most of the Top 10 highest-performing combinations integrated **three marketing channels**, suggesting that coordinated multi-channel execution was common among the strongest-performing campaigns
- **Email** appeared in **6 of the Top 10** channel combinations, indicating its frequent presence in high-performing marketing strategies


<img width="787" height="189" alt="image" src="https://github.com/user-attachments/assets/5dd07854-3ec9-497e-ae90-782b6e17aee4" />

Insight:
- High-engagement campaigns achieved an average ROI of **421.54**, nearly four times higher than low-engagement campaigns, making engagement one of the strongest indicators of campaign profitability
- Average revenue increased substantially as engagement improved, with high-engagement campaigns generating more than double the revenue of low-engagement campaigns
- Customer engagement was positively associated with CTR, increasing from **5.40%** in low-engagement campaigns to **12.20%** in high-engagement campaigns
- Conversion rate also improved as engagement increased, although the improvement was more moderate than the gains observed in CTR and ROI
- Higher customer engagement was consistently associated with better campaign performance across every key business metric


## Conclusion

Although the company achieved strong overall marketing performance, the analysis demonstrates that campaign success depends on far more than overall revenue and ROI. Customer journey efficiency, campaign duration, customer segmentation, multi-channel marketing strategies, and customer engagement all played important roles in determining campaign effectiveness. These findings suggest that marketing performance can be achieved through strategic campaign optimization rather than increased marketing expenditure alone


## Recommendation

- Improve ad creatives, audience targeting, and call-to-action strategies to reduce early-stage customer drop-off and increase customer engagement, as higher engagement was consistently associated with stronger campaign performance
- Develop segment-specific marketing strategies by aligning campaign types and campaign durations with the characteristics of each customer segment, rather than applying a one-size-fits-all approach
- Prioritize high-performing multi-channel combinations identified in the analysis and validate their effectiveness across different campaign objectives and customer segments through controlled campaign experiments before large-scale implementation
- Establish a continuous marketing performance monitoring process using key KPIs-Revenue, Acquisition Cost, ROI, CTR, and Conversion Rate-to evaluate campaign effectiveness, detect performance deviations, and measure the impact of future optimizations initiatives


## Preview Dashboard

<img width="1275" height="1650" alt="marketing campaign dashboard" src="https://github.com/user-attachments/assets/f1660814-c4e3-4ffe-bde2-c54e24e327ff" />


## Tools
- Excel
- Power BI 
