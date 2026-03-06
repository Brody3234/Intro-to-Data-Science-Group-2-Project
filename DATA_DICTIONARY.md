# Data dictionary

This project merges multiple public datasets at the **state** level to model **housing prices (Zillow ZHVI)** and **rent (Zillow ZORI)** over time.

## Dataset abbreviations
- **ZHVI**: Zillow Home Value Index (median home values), typically reported monthly, by geography.
- **ZORI**: Zillow Observed Rent Index (median rent), typically reported monthly, by geography.
- **FRED mortgage rate**: Freddie Mac Primary Mortgage Market Survey / FRED 30-year fixed-rate mortgage average in the U.S. (weekly/monthly)
- **Building permits**: Census building permits for residential construction.
- **Population**: Census annual population estimates.
- **Housing characteristics**: ACS 5-year housing / vacancy / household characteristics (e.g., median household income, rental vacancy rate, owner-occupied share).

## Key columns (merged feature layer)
| Column | Description | Units/notes |
|---|---|---|
| `state` | U.S. state/territory name (merge key). | string |
| `date` | Observation date (monthly aligned). | YYYY-MM-DD |
| `zhvi` | Zillow Home Value Index (median home value). | dollars |
| `zori` | Zillow Observed Rent Index (median asking rent). | dollars |
| `mortgage_rate_30y` | 30-year fixed-rate mortgage average. | percent |
| `building_permits` | Residential building permits issued. | count (monthly) |
| `population` | State population estimate. | persons |
| `median_income` | Median household income. | dollars |
| `rental_vacancy_rate` | Rental vacancy rate. | percent |
| `owner_occupied_share` | Share of housing units that are owner occupied. | percent |
| `unemployment_rate` | State unemployment rate (if included). | percent |
| `gdp_per_capita` | State GDP per capita (if included). | dollars |

### Feature engineering notes
- **Per-capita** metrics (e.g., permits per capita) were created as needed to normalize by state population.
- Rolling windows (e.g., 3-month rolling mean) were used for smoothing time series where appropriate.
- Columns were one-hot encoded or dropped to avoid leakage in modeling as needed (documented in the notebook).
