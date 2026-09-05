# Factors Associated with Wages of U.S. Working-Age Civilians

An ECO 521 econometrics project from Spring 2022 examining wage associations and potential labor-force selection bias with the March 2021 IPUMS Current Population Survey Annual Social and Economic Supplement.

## Research design

The analysis:

- restricts the sample to civilians ages 16–64 and constructs hourly wage from annual wage income, weeks worked, and usual weekly hours;
- creates demographic, geographic, education, disability, and family variables;
- screens selected continuous variables using interquartile-range rules;
- estimates a two-step Heckman selection model, with labor-force participation modeled by probit and log hourly wage modeled conditionally on employment.

The raw extract contains 163,543 observations. After filtering and model-specific exclusions, the reported selection model uses 46,247 observations: 43,766 observed wage outcomes and 2,481 censored outcomes. The inverse Mills term is statistically significant in the reported model, providing evidence that a simple wage regression on the observed working sample would be affected by selection.

The estimates are descriptive associations from observational survey data; they are not causal effects.

## Repository contents

- `cps_March_2021.Rmd` — data preparation, visualization, and model estimation
- `final.pdf` — final paper

## Data access and citation

The microdata were obtained from [IPUMS CPS](https://cps.ipums.org/). IPUMS requires citation and does not permit redistribution of CPS extracts without permission.

## Author

Kai Li.
