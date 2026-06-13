# Experience Curve Analysis - Heliotronics Case Study

Business analytics case study - Advanced Data-Driven Decision Making,
GSEM, University of Geneva (Prof. Marcel Paulssen)

## Project Overview

This case study analyzes the experience curve of Heliotronics, a photovoltaic panel manufacturer, to estimate how manufacturing costs decrease as cumulative production increases.

The objective is to evaluate whether production costs follow an experience curve pattern and to use the estimated relationship to support a competitive pricing recommendation for a solar panel tender.

## Business Context

Heliotronics is a photovoltaic panel manufacturer considering a business opportunity related to a solar installation project in Switzerland. The company needs to estimate future production costs before submitting a competitive bid.

The key business question is:

**What should be the competitive bid price based on expected cost reductions from accumulated production experience?**

## Analytical Approach

The analysis is based on the experience curve model:

```text
Y = A X^b
```

where:

* `Y` is the average manufacturing cost
* `X` is cumulative production
* `A` is the estimated cost of the first unit
* `b` is the experience parameter

Because the relationship between production cost and cumulative production is nonlinear, a log-log transformation was applied:

```text
log(Y) = log(A) + b log(X)
```

This transformation allows the experience curve to be estimated using linear regression.

## Main Steps

The project includes the following steps:

1. Visual inspection of the relationship between cumulative production and manufacturing cost
2. Log-log transformation of the experience curve model
3. Linear regression estimation
4. Interpretation of the experience parameter
5. Estimation of the learning rate
6. Forecasting future manufacturing costs
7. Confidence interval analysis
8. Pricing recommendation

## Key Findings
The analysis supports the experience curve hypothesis: manufacturing cost
decreases as cumulative production increases.

- Strong fit: R-squared ≈ 0.95
- Learning rate ≈ 10% (cost drops ~10% each time cumulative output doubles)
- Forecasted average cost ≈ $697 per panel, with a 95% confidence interval of
  roughly $606–$802

## Files
- `experience_curve.R` — R script (transform, regression, forecast, CI)
- `experience_curve.html` — rendered output with plots and regression results
- `presentation.pdf` — case study presentation

## Tools
R — ggplot2, base stats (lm, confint)

## Authors
Group project (3 members): Zahra Ghafghazi, Giovanni Carta, Sophia Ropelewski.
Work was divided across the analysis and reviewed jointly by the team.
