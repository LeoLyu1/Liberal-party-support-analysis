# Liberal Party Support Analysis

Analyzed 2019 Canadian Election Study web survey data to estimate Liberal Party support and examine its association with age, gender, and education. Combined gender-based population weighting with logistic regression in R.

## Approach

- **Data preparation:** Cleaned 37,822 survey responses to obtain an analysis sample of 31,273 observations. Recoded education into five groups, derived age, and created a binary indicator for Liberal vote choice.
- **Proportion estimation:** Weighted gender-specific support proportions using 2021 Census population totals and calculated a 95% confidence interval under the report's assumed stratified sampling framework.
- **Logistic regression:** Modeled Liberal support using age, gender, and education, with a binomial distribution and logit link.
- **Statistical interpretation:** Used coefficient estimates and Wald tests to assess demographic associations while holding the other included variables constant.

## Results

The reported weighted estimate of Liberal support was **28.5%**, with a **95% confidence interval of 27.99%–29.01%** under the analysis assumptions. Education and age were statistically significant predictors; gender was not significant after adjustment for the other variables.

The estimate depends on the assumed sampling design, use of 2021 population totals for 2019, and exclusion of some responses. It is a survey-based estimate, not the official election result.

## Code and Report

- [Full report](liberal_support_report.pdf)
- [Code](liberal_support_analysis.qmd)

**Tools:** R, tidyverse, ggplot2, knitr, and Quarto.


