# Benchmarking Research Impact Across Countries and Fields at Scale

Standard bibliometric measures -- raw citation counts and average Field Citation Ratios -- are poorly suited for cross-country and cross-field comparison. Citation counts ignore field norms; average FCR collapses across vastly different publication volumes. Without field-sensitive measures, research landscape assessments produce a distorted picture: funders miss high-impact targets, institutions fail to recognize their own relative strengths, and potential partners go unidentified because volume-based rankings bury the contributors that matter most. This project develops and validates an Impact-Weighted Research Output metric that balances field-normalized citation impact with log-transformed publication volume, then applies it to benchmark country-level performance, map international collaboration networks, and compare research contributions across disciplines using the Dimensions COVID-19 public dataset via Google BigQuery.

## Key Findings

- China edges the US on field-normalized impact (FCR 7.27 vs. 6.37) despite less than half the publication volume
- US and UK betweenness centrality (0.09 and 0.07 vs. network mean 0.006) identifies them as structural brokers -- connectors across otherwise disconnected research communities, not just prolific producers
- Volume and field-level impact are orthogonal -- Math/Physical Sciences and Philosophy/Religious Studies lead on FCR despite modest output
- Social Sciences impact cannot be reliably assessed in this dataset -- FOR classification codes fragment the field across subcategories, making it effectively invisible as a coherent unit

## Tech Stack

- **Languages:** Python | R | SQL
- **Tools:** Google BigQuery | Jupyter
- **Packages:** `dplyr`, `gt`, `ggplot2`, `plotly`, `igraph`, `viridis`, `cowplot`, `gridExtra`
- **Data:** `covid-19-dimensions-ai.data.publications` -- freely accessible via Google BigQuery sandbox

## Full Analysis

For narrative, figures, study design, and methodology see the [portfolio page](https://kchoover14.github.io/Bibliometrics-COVID19-Research/).
