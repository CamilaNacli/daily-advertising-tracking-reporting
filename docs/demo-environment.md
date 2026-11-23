# Demo environment

[← Back to README](../README.md)

## What is fictional

- **Products and campaigns:** “Product A”, “Product B” and campaign names such as `A-Broad-01` are invented.
- **Figures:** spend, revenue, refunds, chargebacks, clicks and sales were generated for this demo. Prices, rates and the period (Jul–Oct 2026) are illustrative.
- **Result:** monthly ROI close to +30% was set as a target for the fictional dataset. It is not a real result.
- **Currency:** all amounts are in USD.

The demo has no connection to the original spreadsheet, dashboard, ad accounts or sales platform. The dashboard reads only `data/daily-performance.csv` from this repository.

## What the demo keeps from the original

- One row per campaign per day, with the same inputs and the same formulas for profit after ad spend, ROI, upsell rate, order form conversion, landing page CTR, CPC, CPA, hops per sale, hops per OFI and AOV.
- Monthly, day-of-week and per-product summaries.
- Dashboard filters (start date, end date, month, product, campaign), overview indicators, daily spend vs gross revenue chart, monthly and weekday views, and a paginated daily table.

## Demo additions (◆)

| Addition | Why |
| --- | --- |
| **Chargebacks** column | Shows chargeback control as its own line, separate from refunds |
| **Net Revenue** shown on its own | Makes the step from gross revenue to profit explicit |
| **Performance by Calendar Week** | Week-by-week trend, separate from the weekday comparison |
| **By Campaign** tab and **funnel metrics** panel | Quick comparison between campaigns and funnel steps |
| **N/A** for zero denominators | Clear output on days without sales or spend |

## Left out

- An adjusted-AOV metric from the original, because its business rule is not documented.
- Real product, campaign, platform and account names, links, and any real figures.
