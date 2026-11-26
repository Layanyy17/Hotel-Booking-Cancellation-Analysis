# Hotel Booking Cancellation Analysis

**Excel Data Analytics Portfolio Project** · Data Cleaning · Data Quality · PivotTables · Interactive Dashboards · Business Insights

An end-to-end Excel analysis of hotel booking behavior, cancellation patterns, and **estimated booking-value exposure** across **119,390 reservations** (arrival years 2015–2017). The workbook includes **18 worksheets**, including the cleaned dataset, audit and cleaning documentation, supporting analyses, and two interactive dashboards.

> **Interpretation:** Estimated canceled booking value represents the booked value associated with canceled reservations. It is **not confirmed revenue loss**. No reporting currency is asserted.

## Dashboard previews

Screenshots are included in the project upload package and will appear here after the `assets/` images are added to this repository.

**Overview dashboard** — booking volumes, cancellation performance, hotel comparisons, deposit type, market segments, and booking lead time.

**Risk Deep Dive dashboard** — lead-time risk, deposit type × market segment, monthly risk, and estimated canceled value by hotel.

Both dashboards include dropdown filters for **hotel**, **arrival year**, **market segment**, and **deposit type**. Category-comparison charts intentionally exclude their own category filter in some views to preserve meaningful comparisons. When *All Years* is selected, the seasonal risk view uses **2016**, the complete calendar year in this dataset.

## Key performance indicators

| Metric | Result |
| --- | ---: |
| Total reservations | **119,390** |
| Canceled reservations | **44,224** |
| Overall cancellation rate | **37.04%** |
| Average lead time | **104.0 days** |
| Estimated canceled booking value | **16,727,237** (currency unspecified) |

## Findings

### Hotel comparison

| Hotel | Bookings | Canceled | Cancellation rate |
| --- | ---: | ---: | ---: |
| City Hotel | 79,330 | 33,102 | **41.73%** |
| Resort Hotel | 40,060 | 11,122 | **27.76%** |

### Deposit categories

The **Non Refund** category had **14,494 canceled bookings out of 14,587** (**99.36%**). This unusual relationship warrants further investigation of booking, deposit, and cancellation processes; it should not be interpreted as proof of causation.

### Lead-time risk

Across the full dataset, reservations made **360+ days before arrival** had a **67.15%** cancellation rate. In **2015** the rate was **96.24%**, but the sample contained only **266 bookings** (**256 canceled**). Sample sizes are essential context for unusually high rates.

### Booking-value concentration

**Online TA** accounted for approximately **10,227,646** in estimated canceled booking value across both hotels. This is a useful starting point for investigating exposure, not a measured financial loss.

### Seasonality

For the full year **2016**, **October** had a **40.53%** cancellation rate (**2,514 / 6,203**), versus **24.78%** in **January** (**557 / 2,248**). The arrival-year coverage for 2015 and 2017 is partial and should be considered when comparing years.

## Workflow

1. **Data audit:** Inspect missing and unusual values, zero-night stays, possible duplicates, lead-time anomalies, and deposit patterns.
2. **Cleaning documentation:** Record checks and handling decisions in `Audit` and `cleaning Log`. Exact matching records were flagged rather than automatically deleted because a unique booking ID was not available.
3. **PivotTable analysis:** Review cancellation rates, hotel differences, market segments, deposit categories, booking lead time, and seasonal trends.
4. **Interactive dashboard development:** Build KPI cards, charts, and four dropdown filters, supported by a dedicated `Dashboard Engine` worksheet.
5. **Business interpretation:** Document evidence, implications, and recommended follow-up investigations in `Business Insights`.

## Formulas and definitions

```text
Cancellation rate = Canceled bookings / Total bookings
Estimated booking value = ADR × (weekend nights + week nights)
Estimated canceled booking value =
    Sum of estimated booking value where is_canceled = 1
```

The project does not model actual refunds, rebookings, payments, operating costs, or realized revenue losses.

## Workbook guide

The Excel workbook includes **18 sheets**. Important sheets include:

| Area | Worksheets |
| --- | --- |
| Data and quality | `raw Data`, `clean data`, `Audit`, `cleaning Log`, `Duplicate Check` |
| Core analysis | `Cancellation Overiew`, `Hotel Comparison`, `Market Segment`, `Deposit Analysis`, `Lead Time Analysis` |
| Extended analysis | `Revenue Risk Analysis`, `Revenue by Segment`, `Canecllation  Drivers Analysis`, `Monthly&Seasonal Analysis` |
| Presentation | `Business Insights`, `Dashboard Engine`, `Risk Deep Dive`, ` Dashboard` |

*Original sheet names, including spacing and spelling, are preserved from the workbook.*

## How to use

1. Open `hotel_bookings_Analysis.xlsx` in **desktop Microsoft Excel** once the workbook has been uploaded.
2. Start with the **Dashboard** tab for the overall view.
3. Explore **Risk Deep Dive** and use the dropdown filters.
4. Open **Business Insights** to see findings, evidence, implications, and next investigations.
5. Review **Audit** and **cleaning Log** for data-quality documentation.

**Compatibility:** The project is intended for desktop Excel because it contains charts, PivotTables, and formula-driven dashboard interactions. GitHub's in-browser file preview is not an interactive Excel dashboard.

## Limitations and publication notes

- The data covers only the supplied snapshot of bookings; the dashboards do not use a live booking feed.
- Large cancellation percentages may relate to small samples.
- `Non Refund` is a dataset label, and correlations are **not evidence of causation**.
- Monetary results have **no asserted currency** and are **not confirmed revenue losses**.
- Verify the original dataset's licensing and redistribution terms before publicly uploading raw booking records. If redistribution is restricted, publish the dashboard previews and analysis instead.

---

**Project:** Hotel Booking Cancellation Analysis · **Tools:** Microsoft Excel, PivotTables, formulas, data cleaning, and dashboard design.
