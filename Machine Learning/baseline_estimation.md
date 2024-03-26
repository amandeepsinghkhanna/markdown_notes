# Baseline estiamtion for sales in Consumer Packaged Goods (CPG) industry

ACNielsen and Information Resources (IRI) are leading market research firms that collect and track data on various CPG products. This data includes product attributes and detailed information on consumer purchasing behavior. This information allows manufacturers and retailers to develop highly detailed models to measure the effectiveness of promotions and other marketing tactics like advertising, price changes, and public relations [1].

A key element of all these models is establishing a baseline sales level. This represents the expected sales in the absence of a specific marketing tactic, like a price promotion. By comparing actual sales to this baseline, marketers can determine the effectiveness of their campaigns. Baseline sales are simply the counterfactual of sales activity in the hypothetical case of no promotions for a period of time [1].

The estimation of baseline sales is either done at a aggregated (chain/market-level) or at a disaggregated (store-level) data. There are two models that are considered to be the industry and academic standard, they are:

1. Scan Pro
2. Promotion Scan

Both these models were developed on the ACNielson and IRI datasets. They are log-linear models that provide the estimate of baseline sales and sales response as a function of retialer promotional tactics such as price discounts, feature ads, and displays.

*Todo - Read about Phantom spikes.*

## Validating if sales baseline is accurate

The four ways to check if the estimated baselines are accurate:

**1. No correlation with promotional activity**

A valid baseline estimation model should eliminate correlation between the presence of promotional activity and baseline estimates. There should be no structural difference in the baseline between promoted and non-promoted weeks i.e., in other words,  phantom spikes should not appear.

**2. Minimal week-to-week volatility**

The baseline estimates are expected to be steady in the weeks immediately before and after a promotional activity. The change in baseline estimates should have a gradual drift.

**3. No structural basis in the deviations**

The baseline estaimates should not be consistently over-estimated or under-estimated over continous periods of time. 

**4. Minimal error in non-promotional weeks** 

Baseline estimates for the weeks without any promotional activity should be close to the actual sales.

## References

1. [Kurt Jetta, A model to improve the estimation of baseline retail sales, Journal of CENTRUM, 2011](https://deliverypdf.ssrn.com/delivery.php?ID=465084070078097076026070067079114069120073069085030094102095079026125069069030002071042006097007012027110068105003114123066010104032014085018084068116082117021122030029075052101030019127088021086093083107085030126123126121089099101065123086013019111126&EXT=pdf&INDEX=TRUE)
2. [Ahmed Khaled, The difference between baseline & regular sales, LinkedIn Blog, 24th June 2020](https://www.linkedin.com/pulse/difference-between-baseline-regular-sales-ahmed-khaled/)
3. [Telus agriculture & consumer goods blog, 26th September 2019 ](https://www.telus.com/agcg/blog-resources/ways-to-test-cpg-sales-baselines)