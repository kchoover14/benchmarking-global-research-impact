## Executive Summary

**Problem:** Standard bibliometric measures -- raw citation counts and average Field Citation Ratios -- are poorly suited for cross-country comparison. Citation counts ignore field norms while average FCR is skewed by outliers and collapses across vastly different publication volumes. Without field-sensitive measures, research landscape assessments produce a distorted picture -- funders miss high-impact targets, institutions fail to recognize their own relative strengths, and potential partners go unidentified because volume-based rankings bury the contributors that matter most.

**Approach:** Using publication metadata from the Dimensions COVID-19 dataset via Google BigQuery, I developed a novel Impact-Weighted Research Output metric that iteratively tested and validated four candidate measures before selecting one optimized for cross-country stability. The metric balances field-normalized citation impact with log-transformed publication volume, then was applied to three analyses: country-level benchmarking, international collaboration network mapping, and field-level impact comparison.

**Insights:** High publication volume and high research impact do not correlate predictably -- the countries and fields that publish most are not necessarily those generating the most influential work. Closing that gap requires metrics that account for both field norms and output scale simultaneously, moving beyond single-dimension measures toward composite frameworks that reflect how influence actually distributes. Network centrality reveals a complementary dimension that output metrics miss entirely, distinguishing connectors from producers. Both findings depend critically on how fields are classified -- the system used to categorize research shapes which contributions are visible and which are structurally obscured, making classification quality inseparable from the validity of any landscape assessment.

**Significance:** Research landscape assessments -- whether for funding allocation, partnership development, or institutional benchmarking -- rest on the metrics used to build them. Standard measures systematically favor high-volume producers and render high-impact low-volume contributors invisible. Classification systems compound this problem by fragmenting disciplines unevenly, making some fields effectively unmeasurable. Metric quality is not a methodological footnote -- it determines whose contributions count.

**Key Findings**

- The US leads in raw publication volume (327,428) but China edges it on the composite metric, reflecting a higher average FCR (7.27 vs. 6.37)
- US and UK betweenness centrality (0.09 and 0.07 vs. network mean 0.006) identifies them as structural brokers -- connectors across otherwise disconnected research communities, not just prolific producers
- No field achieved both high volume and high impact; Math and Physical Sciences and Philosophy and Religious Studies had the highest FCR despite modest output
- Social Sciences impact cannot be reliably assessed in this dataset -- FOR classification codes fragment the field across subcategories, making it effectively invisible as a coherent unit
