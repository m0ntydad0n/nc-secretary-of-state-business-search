# North Carolina Secretary of State Business Search API

Unofficial API-style NC Secretary of State business entity lookup powered by Apify.

Run the Actor:

https://apify.com/monty15/north-carolina-sos-business-search

## Bulk NC business entity lookup

This Apify Actor bulk-searches North Carolina Secretary of State Business Registration records by company/entity name and exports structured dataset rows for CSV, Excel, JSON, and API workflows.

Use it for:

- NC Secretary of State business search
- North Carolina business entity search API workflows
- NC SOS business lookup
- NC registered agent lookup
- North Carolina company status verification
- Bulk NC business lookup from a spreadsheet
- CSV enrichment for North Carolina companies
- NC annual report phone number extraction

## What data can it return?

- Entity legal name
- SOS ID
- Entity status
- Business type
- Formation date
- Prior names
- Registered agent
- Principal office address
- Company officials
- Filing metadata
- Latest annual-report date
- Public principal office phone number when present in annual-report PDFs
- Official NC SOS source URL

## Example input

```json
{
  "searchTerms": ["Red Hat Inc", "Lowe's Companies Inc"],
  "maxResultsPerSearch": 1,
  "includeProfiles": true,
  "includeFilings": false,
  "includePhones": true
}
```

## Example workflow

1. Put your North Carolina company names into `searchTerms`.
2. Run the Actor on Apify.
3. Export the dataset as CSV, Excel, JSON, or JSONL.
4. Join the official-source fields back to your spreadsheet or pipeline.

## Run it on Apify

https://apify.com/monty15/north-carolina-sos-business-search

The hosted Actor page includes the full README, input schema, output schema, pricing, and limitations.

## Notes

This is an unofficial workflow for public NC Secretary of State records. It is not affiliated with or endorsed by the North Carolina Secretary of State. It does not identify beneficial owners, infer private phone ownership, or provide legal/compliance advice.
