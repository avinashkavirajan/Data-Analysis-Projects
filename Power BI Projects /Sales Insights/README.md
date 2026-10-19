# Sales Insights Dashboard (Power BI)

An interactive Power BI dashboard that gives a hardware company's sales team a quick view of performance, built from the company's MySQL sales database.

![Sales Insights dashboard](dashboard.png)

## The problem
Sales data sat in a MySQL database. Getting answers such as "who are our biggest customers?" or "is revenue going up?" meant querying the database each time.

## What I built
- **ETL:** extracted the sales data from MySQL and cleaned it in Power Query.
- **Data model:** related the sales transactions to customers, products and dates.
- **Dashboard:** revenue, sales quantity and revenue trend, plus the top 5 customers and top 5 products, with filters for drilling in.

## What the data showed
- **Total revenue of 984.87M across 2M units sold** (2017–2020).
- **Revenue is concentrated:** Delhi NCR brings in about 53% of revenue, and the top customer (Electricalsara Stores) about 42%. That is a dependency risk worth flagging to the business.
- **Data quality gap:** the largest "product" in the top 5 is **(Blank)**, about 48% of revenue, meaning many transactions have no product code. Fixing this at the source would be the first recommendation before using product-level figures.
- **Revenue trend** peaks in early 2018 and declines towards 2020.

## Tools
Power BI · MySQL · SQL · Power Query

## Files
| File | What it is |
|---|---|
| `db_dump.pbix` | The Power BI report (open in Power BI Desktop) |
| `db_dump.sql` | MySQL database dump used as the data source |
| `dashboard.png` | Screenshot of the dashboard |

---
Portfolio: [nashkavirajan.wixsite.com/avinash-kavirajan](https://nashkavirajan.wixsite.com/avinash-kavirajan)
