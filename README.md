# Financial Performance Analysis — Power BI

An interactive Power BI dashboard that analyses sales and profitability across five business segments, from top-line gross sales down to segment- and product-level profit.

width="100%" alt="Financial Performance Analysis dashboard"


---

## Business question

Which segments and products drive gross sales and profit, and which parts of the business are underperforming?

## Key insights

- **$127.93M** in gross sales analysed across **5 business segments** (Government, Small Business, Enterprise, Midmarket, Channel Partners).
- **Government** and **Small Business** are the highest-performing segments.
- **Channel Partners** is the weakest segment at **3.2%** contribution, which supports a review of segment focus.

## Dataset

| Item | Detail |
|---|---|
| Source | [Microsoft Power BI Financial Sample](https://learn.microsoft.com/en-us/power-bi/create-reports/sample-financial-download) (public sample data) |
| Period | 2013 – 2014 |
| Grain | One row per sale (segment × product × date) |
| Main fields | Segment, Product, Units Sold, Manufacturing Price, Sale Price, Gross Sales, Sales, Profit, Date |

## Approach

1. **Load** – imported the Excel data into Power BI Desktop.
2. **Clean & transform (Power Query)** – set correct data types, built the date fields (Year, Quarter, Month, Day) and prepared the table for reporting.
3. **Model** – used the date hierarchy so every visual can be filtered by period through a single date slicer.
4. **Visualise** – built the report page below.

| Visual | What it answers |
|---|---|
| Date slicer | Filters the whole page by period |
| Gauge – Gross Sales and Profit | Total gross sales against range |
| Donut – Units Sold by Segment | Volume mix by segment |
| Funnel – Sale Price by Segment | Segment contribution ranking |
| Treemap – Manufacturing Price by Segment and Year | Cost base by segment over time |
| Line – Gross Sales trend | How sales build over time |
| Waterfall – Profit by Segment and Product | Which segment/product combinations add or reduce profit |
| Multi-row cards | Year / quarter / month drill-down of sales |

## Repository contents

```
financial-performance-powerbi/
├── README.md
├── Financial Performance Analysis.pbix    # Power BI file
├── Financial Performance Analysis.pdf     # PDF export for quick viewing
└── Financial Performance Excel.xlsx       # source data (exported from the .pbix)
```

## How to view

- **No Power BI?** Open [Financial Performance Analysis.pdf](Financial%20Performance%20Analysis.pdf).
- **Want the data?** Download [Financial Performance Excel.xlsx](Financial%20Performance%20Excel.xlsx).
- **With Power BI Desktop** (free, Windows): download [Financial Performance Analysis.pbix](Financial%20Performance%20Analysis.pbix) and open it — the data loads with it.


## Tools

Power BI Desktop · Power Query · Microsoft Excel

---

**Surya V Vakade** — SAP FICO · Finance & Analytics
[LinkedIn](https://www.linkedin.com/in/surya-vv) · [GitHub](https://github.com/suryavakade-1745)
