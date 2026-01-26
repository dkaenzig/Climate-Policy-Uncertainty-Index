# Climate Policy Uncertainty and Sentiment Dataset

## Overview
This repository provides data on the U.S. **climate policy uncertainty** index, a news-based measure designed to capture uncertainty about the future direction of climate policy in the United States.

### Construction
The index is constructed by applying automated text-search methods to the full text of major U.S. newspapers, following the broader literature on news-based measures of policy uncertainty. Specifically, we identify articles that jointly discuss climate change, policy, and uncertainty-related concepts, using carefully curated dictionaries for each component. Dictionaries are constructed in broad and narrow versions to balance coverage and precision; the narrow version serves as our baseline. The index is based on coverage in the *New York Times*, *Wall Street Journal*, *Washington Post*, and *Los Angeles Times*.

The index exhibits pronounced spikes around major climate policy events, including international climate agreements, congressional debates over climate legislation, regulatory actions and reversals, and presidential elections associated with shifts in climate policy direction. 

In addition to the headline CPU Index, we also provide measures of **climate policy news** intensity and **climate policy sentiment**. The data is intended to support research on the macroeconomic, financial, and firm-level effects of climate policy uncertainty.

### Instrument and Shock Series

We also introduce an event-based **instrument** designed to identify exogenous shocks to climate policy uncertainty. The instrument is constructed from major climate policy events that generate sharp changes in uncertainty. Event intensity is measured using newspaper coverage and is explicitly purged of the first moment of climate policy (policy stringency), isolating variation that reflects uncertainty rather than anticipated policy tightening or loosening. 

This instrument is used to construct a monthly series of **climate policy uncertainty shocks**, which can also be used for macroeconomic and firm-level analysis.

### Reference

The methodology and results are described in detail in:

Gavriilidis, Känzig, Raghavan, and Stock (2026). ["The Macroeconomic Effects of Climate Policy Uncertainty"](https://dkaenzig.github.io/diegokaenzig.com/Papers/gkrs_cpu.pdf). Working Paper. 

## Files

| File | Description |
|------|-------------|
| `cpu.dta` | Stata dataset |
| `cpu.xlsx` | Excel dataset |

## Variables

### Constructed Indices

| Variable | Description |
|----------|-------------|
| `cpu_index_narrow` | News-based climate policy uncertainty index using narrow dictionary concepts |
| `cpu_index_broad` | News-based climate policy uncertainty index using broad dictionary concepts |
| `cpnews_index_narrow` | Climate policy news index using narrow dictionary concepts |
| `cpnews_index_broad` | Climate policy news index using broad dictionary concepts |
| `cpsent_index` | News-based climate policy sentiment index |


### Instrument and Shock

| Variable | Description |
|----------|-------------|
| `cpu_instrument` | Event-based climate policy uncertainty instrument |
| `cpu_shock` | Climate policy uncertainty shock series |
