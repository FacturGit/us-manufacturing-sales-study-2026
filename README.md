# U.S. Manufacturing Sales Study 2026: Quotes, Purchase Orders and Prospecting Activity

Twelve months (November 2025 to October 2026) of outbound prospecting for U.S. manufacturers and industrial suppliers, run by Factur: **1,271 quotes, 268 purchase orders and $127.3M quoted**, broken down by state, region, industry, quote size and prospecting channel, plus the underlying activity (439,358 calls, 621,119 emails).

- Full report (43 pages, free): https://data.facturmfg.com/reports/us-manufacturing-industry-analysis-2026.html
- Key findings: https://data.facturmfg.com/reports/findings.html
- Statistics roundup: https://data.facturmfg.com/reports/manufacturing-sales-statistics-2026.html
- PDF: `us-manufacturing-sales-study-2026.pdf` (included)

## Files

All CSVs are in `data/`. The full report is `us-manufacturing-sales-study-2026.pdf`; machine-readable metadata is in `dataset-metadata.json`.

| File | Rows | What it holds |
|---|---|---|
| `quotes-po-by-state-2026.csv` | 50 states and territories | Quotes, value, purchase orders and quote-to-PO rate by state (includes a few non-U.S. buyers, e.g. Ontario) |
| `quotes-po-by-region-2026.csv` | 4 Census regions | The same by region |
| `quotes-po-by-industry-2026.csv` | 24 industries | The same by buyer industry (industries with 6+ quotes) |
| `quote-sizes-2026.csv` | 6 bands | Quotes and conversion by quote size |
| `prospecting-channels-2026.csv` | 7 channels | Leads worked, quotes and POs by the channel that sourced them |
| `prospecting-activity-2026.csv` | 10 activities | Calls, emails, voicemails, bounces, meetings |
| `sms-activity-2026.csv` | SMS activity | Texts sent and replies, from the report's SMS section |
| `quotes-po-by-segment-2026.csv` | 5 segments | Quotes, purchase orders and quote-to-PO rate by Factur client segment (machining, fabrication, equipment, plastics and rubber, construction trades). Aggregates of Factur clients' prospecting results, at least 5 clients per segment; not part of the 43-page report |

## Columns

- `quotes`: quotes (RFQ responses) issued in the 12 months
- `quotes_change_pct`: change against the previous 12 months, in percent
- `quote_amount_usd`, `po_amount_usd`: total value in U.S. dollars (rounded as in the report)
- `purchase_orders`: purchase orders received
- `quote_to_po_pct`: purchase orders as a percent of quotes
- `po_change_pct`: change in purchase orders against the previous 12 months
- `leads_worked`, `worked_to_quote_pct` (channels): accounts worked, and quotes as a percent of them
- `share_of_quotes_pct`, `share_of_value_pct` (quote sizes): share of all quotes and of all quoted value
- `nov2025_oct2026`, `change_pct` (activity): count for the period and change against the year before

Empty cells mean the figure was not recorded or does not apply.

## Method

Figures come from Factur's own CRM and prospecting records for its manufacturing clients. A quote counts once, in the state and industry of the buying account. 614 quotes have no industry on the account and appear only in totals. Amounts are as quoted, not as invoiced.

## License and citation

Data and report: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (see `LICENSE`). Please cite as (also in `CITATION.cff`):

> Factur (2026). *U.S. Manufacturing Sales Study 2026: Quotes, Purchase Orders and Prospecting Activity.* https://data.facturmfg.com/reports/us-manufacturing-industry-analysis-2026.html

Factur runs outbound prospecting for manufacturers: https://facturmfg.com
