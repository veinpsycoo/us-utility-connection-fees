# U.S. Utility Connection Fee Database

Official water, sewer, electric and gas **connection fees** for U.S. cities: tap fees, impact fees, capacity charges, meter sets, main-extension and permit charges, each linked to the utility document it came from.

Maintained by [Utility Cost Guide](https://utilitycostguide.com/). Browse it, with plain-English explanations per city, at **[utilitycostguide.com/fee-database](https://utilitycostguide.com/fee-database/)**.

| | |
|---|---|
| Records | 1,794 |
| Cities / jurisdictions | 124 |
| States | 35 |
| Utilities | 203 |
| Verified against the source document | 1,588 (the other 206 are flagged `needs_review`) |
| Last verification pass | 24–26 September 2026 |

Rows by service: water 961, sewer 565, general 147, electric 74, stormwater 22, gas 16, reclaimed 9.
Most common fee categories: impact 384, capacity 287, tap 214, connection 203, meter 136.

## Files

- [`data/utility-connection-fees.csv`](data/utility-connection-fees.csv)
- [`data/utility-connection-fees.json`](data/utility-connection-fees.json)

The live copies are updated when a utility changes its schedule:
`https://utilitycostguide.com/data/utility-connection-fees.csv` and `.json`.

## Key fields

| Field | Meaning |
|---|---|
| `jurisdiction_name`, `state_code` | City or county the fee applies to |
| `provider_name` | Utility that charges the fee |
| `service` | water, sewer, electric, gas, stormwater, reclaimed, general |
| `fee_category` | impact, capacity, tap, connection, meter, permit, … |
| `meter_size`, `customer_class` | What the amount is keyed to |
| `amount`, `amount_max`, `basis`, `formula_text` | The charge and how it is calculated |
| `effective_date`, `fiscal_year` | When the amount took effect |
| `source_url`, `source_title`, `source_org` | Official document the figure comes from |
| `verified_date`, `verification_status` | When we last checked it against the source |

The full field dictionary and methodology: [fee database](https://utilitycostguide.com/fee-database/) · [methodology](https://utilitycostguide.com/methodology/) · [sources and data policy](https://utilitycostguide.com/sources-data-policy/).

## Caveats

Fees are not always flat charges: many depend on meter size, lot size or fixture units, and utilities revise them, often on 1 July, 1 October or 1 January. Confirm the amount for a specific property with the utility before you budget. For an estimate of the total, including private work such as the service line, use the free [utility connection cost calculator](https://utilitycostguide.com/utility-connection-cost-calculator/).

## License and citation

Data: [CC BY 4.0](LICENSE). Please credit **Utility Cost Guide** with a link to https://utilitycostguide.com/fee-database/, and cite the original utility document for any specific fee.

> Utility Cost Guide, *U.S. Utility Connection Fee Database*, accessed <date>, https://utilitycostguide.com/fee-database/

Found an outdated fee? Email corrections@utilitycostguide.com with the source link.
