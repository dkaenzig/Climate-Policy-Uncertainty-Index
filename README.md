# Climate Policy Uncertainty and Sentiment Dataset

## Overview
This dataset provides **monthly indices of climate policy uncertainty and sentiment**, together with the instrument and shock-series for climate policy uncertainty. For details on the construction of these indices, see [Gavriilidis, Känzig, Raghavan, and Stock, 2026](https://dkaenzig.github.io/diegokaenzig.com/Papers/gkrs_cpu.pdf). 

## Files
| File | Description |
|------|-------------|
| `cpu.dta` | Stata dataset containing all variables |
| `cpu.xlsx` | Excel version of the dataset (dates formatted as `YYYY'M'MM`) |

## Variables

### Time Variable

| Variable | Description |
|----------|-------------|
| `date` | Month-year variable |

### Constructed Indices

| Variable | Description |
|----------|-------------|
| `cpu_index_narrow` | News-based climate policy uncertainty index using narrow dictionary concepts |
| `cpu_index_broad` | News-based climate policy uncertainty index using broad dictionary concepts |
| `cpnews_index_narrow` | Climate policy news index using narrow dictionary concepts |
| `cpnews_index_broad` | Climate policy news index using broad dictionary concepts |
| `cpsent_index` | News-based climate policy sentiment index |

### Shock and Instrument

| Variable | Description |
|----------|-------------|
| `cpu_instrument` | Event-based climate policy uncertainty instrument |
| `cpu_shock` | Climate policy uncertainty shock-series |
