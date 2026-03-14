# Mortgage Calculator

A single-file, client-side mortgage calculator for **15-year fixed** and **2-1 buydown** loan scenarios. No build step, no dependencies beyond Chart.js (loaded from CDN).

## Features

- **15-year fixed** and **2-1 buydown** scenario comparison
- Configurable home price, down payment, interest rate, and start year
- **Discount points** slider — adjusts effective rate and shows upfront cost
- **Extra principal** slider — shows interest savings and accelerated payoff
- **Balance over time** chart with Chart.js
- **Monthly breakdown** tab with full amortization table
  - Toggle between every-month and year-end summary views
  - Highlight rows by high-interest or high-principal months
- Cost breakdown with visual bars (principal, interest, points, buydown subsidy)
- Light/dark mode via `prefers-color-scheme`

## Usage

Open `index.html` directly in a browser — no server required.

```
open index.html
```

## Inputs

| Field | Default | Description |
|---|---|---|
| Home price | $450,000 | Total purchase price |
| Down payment | $90,000 | Upfront cash (20%) |
| Interest rate | 6.75% | Annual rate (base) |
| Start year | 2025 | Loan origination year |
| Discount points | 0 | 1 pt = 0.25% rate reduction, costs 1% of loan |
| Extra principal/mo | $0 | Additional monthly payment toward principal |

## 2-1 Buydown

In the buydown scenario the rate is reduced by 2% in year 1 and 1% in year 2, then reverts to the full rate from year 3 onward. The subsidy value (typically covered by the seller or builder) is shown in the metrics.
