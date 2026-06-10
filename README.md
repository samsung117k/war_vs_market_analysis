# War vs Market Analysis

## Overview
In this project, I analyzed the relationship between major war periods and U.S. stock market returns using statistical hypothesis testing. 
The analysis is structured in two parts, progressing from a broad overview to a more precise event-driven approach.

## Tools Used
- Python(Pandas, Matplotlib, Seaborn, scipy) for analysis and visualization
- Yahoo Finance(Python Library) for data sourcing

## Dataset
- Source: Yahoo Finance
- NASDAQ Composite Index and S&P 500 Index
- Data range: 50 years of daily closing prices

## Part 1: NASDAQ vs War Analysis
Compared average daily NASDAQ returns during four major war periods against the 
50-year historical average using a two-tailed z-test.

**Wars Analyzed:** Gulf War, Iraq War, Afghanistan War, Russia-Ukraine War

**Result:** All four wars failed to reject the null hypothesis, suggesting that war periods as a whole did not produce statistically significant differences in NASDAQ returns. 
This was attributed to long war durations, overlapping macroeconomic events, and markets pricing in conflict before official declarations.

## Part 2: S&P 500 vs War Uncertainty Analysis
Rather than analyzing entire war periods, Part 2 focused on specific moments of uncertainty and resolution, 
measuring S&P 500 returns over the 14 trading days following each key event. The data analyzed using left-tailed z-test for uncertainty begin and right-tailed z-test for uncertainty resolved.

**Key Findings:**
- p-value for uncertainty begin: 0.0089
- p-value for uncertainty resolve: 0.0066
- Both results rejected the null hypothesis at the 0.05 significance level

**Conclusion:** Markets do not react to war itself, but to the shock and uncertainty caused by the information embedded within wars. 
The start of uncertainty is associated with a significant market decline, and the resolution of uncertainty is associated with a significant recovery.

## Limitations
- Iraq War period overlaps with dot-com bubble collapse and accounting scandals.
- Russia-Ukraine War impact is difficult to isolate due to Fed rate hike cycle.
- Sample size of four wars makes it difficult to generalize the results.
