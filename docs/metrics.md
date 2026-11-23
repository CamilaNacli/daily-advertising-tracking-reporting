# Metrics

[← Back to README](../README.md)

All amounts are in USD. When a denominator is zero, the spreadsheet and the dashboard show **N/A** instead of an error or a misleading zero.

## Inputs (one row per campaign per day)

| Field | Meaning |
| --- | --- |
| Date, Product, Campaign | When and what was advertised |
| Ad Spend | Amount spent on ads that day |
| Gross Revenue | Revenue from all sales before any adjustment |
| Refunds | Amount refunded to customers |
| Chargebacks ◆ | Amount reversed through card disputes — recorded separately from refunds |
| Clicks | Ad clicks |
| Hops | Tracked visits to the sales page |
| OFI | Order-form impressions (visitors who reached the order form) |
| Sales / Upsell Sales | Front-end orders / additional upsell orders |

## Calculated metrics

| Metric | Formula | N/A when |
| --- | --- | --- |
| Net Revenue | Gross Revenue − Refunds − Chargebacks | — |
| Profit After Ad Spend | Net Revenue − Ad Spend | — |
| ROI (after ad spend) | Profit After Ad Spend ÷ Ad Spend | Ad Spend = 0 |
| Upsell Rate | Upsell Sales ÷ Sales | Sales = 0 |
| Order Form Conversion | Sales ÷ OFI | OFI = 0 |
| Landing Page CTR | Hops ÷ Clicks | Clicks = 0 |
| CPC | Ad Spend ÷ Clicks | Clicks = 0 |
| CPA | Ad Spend ÷ Sales | Sales = 0 |
| Hops per Sale | Hops ÷ Sales | Sales = 0 |
| Hops per OFI | Hops ÷ OFI | OFI = 0 |
| AOV | Gross Revenue ÷ Sales | Sales = 0 |

## Period totals

For a month, week, weekday, campaign or any filtered period, the inputs are **summed first** and the ratios are calculated on the totals. For example, monthly ROI = total profit after ad spend ÷ total ad spend for the month. Averaging daily ROIs would give days with small budgets the same weight as days with large ones.

## Why refunds and chargebacks are separate

A chargeback and a refund can look alike in a revenue report. Keeping them in two columns makes each one visible, lets the dashboard show each as a share of gross revenue, and avoids deducting the same adjustment twice.

◆ marks additions made for this demo.
