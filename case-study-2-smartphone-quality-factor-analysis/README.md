# Smartphone Quality Perceptions — Factor Analysis

Business analytics case study — Advanced Data-Driven Decision Making,
GSEM, University of Geneva (Prof. Marcel Paulssen)

## Project Overview

This case study analyzes customer perceptions of smartphone quality using exploratory factor analysis.

The objective is to identify the main latent dimensions underlying perceived smartphone quality and to examine how these dimensions relate to important business outcomes such as willingness to pay and repurchase intention.

## Business Context

Perceived quality is an important driver of competitive advantage, customer behavior, and long-term business performance. However, smartphone quality is multidimensional and cannot be fully understood through a single satisfaction score.

The case focuses on understanding how customers evaluate smartphone quality across multiple perception items and how these quality dimensions can support better product management and marketing decisions.

## Dataset

The analysis is based on survey data from smartphone customers.

The dataset includes:

* 979 smartphone customers
* 33 quality perception items
* Outcome variables related to willingness to pay and repurchase intention

## Analytical Approach

The project applies exploratory factor analysis to uncover the latent structure behind customer quality perceptions.

The analysis includes:

1. Correlation analysis between quality perception items
2. Factorability assessment
3. Kaiser-Meyer-Olkin test
4. Bartlett’s test of sphericity
5. Selection of the number of factors
6. Comparison of alternative factor solutions
7. Factor rotation and interpretation
8. Item refinement
9. Interpretation of quality dimensions
10. Business implications for smartphone quality management

## Key Methods

* Exploratory Factor Analysis
* Principal Axis Factoring
* Promax rotation
* KMO measure of sampling adequacy
* Bartlett’s test
* Scree plot
* Parallel analysis
* Factor loading interpretation
* Regression analysis for business outcomes

## Main Findings
The analysis supports a multidimensional view of smartphone quality.

- Retained an 8-factor solution (30 items) mapping cleanly onto established quality
  dimensions (Garvin 1988; Brucks et al. 2000), explaining ~74% of shared variance
- All factors internally consistent (Cronbach's alpha > 0.85)
- Ease of Use and Performance were the strongest drivers of both willingness to pay
  and repurchase intention
- Repurchase drivers differ by brand: Apple → serviceability, Samsung → durability,
  LG → material quality
  
## Files
- `factor_analysis.Rmd` — R Markdown source (full analysis)
- `factor_analysis.html` — rendered output with tables and plots
- `presentation.pdf` — case study presentation

## Authors
Group project (3 members): Zahra Ghafghazi, Giovanni Carta, Sophia Ropelewski.
Work was divided across the analysis and reviewed jointly by the team

## Tools
R — psych (fa, principal, KMO, Bartlett), base stats (lm), ggplot2.
