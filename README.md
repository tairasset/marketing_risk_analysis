# Marketing Risk & Resilience Simulation Lab

A coursework notebook for exploring how spending assumptions, performance anomalies, and social posts affect a marketing risk assessment.

## Walkthrough

1. Use sample advertising data to examine spending, sales, and return on investment (ROI).
2. Simulate 10,000 campaign scenarios and summarize the ROI distribution, tail risk, and share of loss scenarios.
3. Flag unusual observations using Isolation Forest and review their features.
4. Score fictional social posts and aggregate them into a Brand Risk Index.
5. Export the analysis tables to Excel. A [dashboard file](./marketing_week6.pbix) is included in the original repository.

## Run with synthetic data

Open [the notebook](./marketing_risk_simulation_%281%29%20%281%29.ipynb) in Jupyter using a Python 3 kernel. Run the setup cell to install the dependencies, then run the remaining cells in order. Leave `advertising.csv` out of the working directory to use the built-in synthetic data. Leave `OPENROUTER_API_KEY` unset to score posts with local rules. After dependencies are installed, this workflow uses local computation.

If you want to try the optional OpenRouter route, set `OPENROUTER_API_KEY` in the environment before starting Jupyter. This mode sends the fictional post text to OpenRouter. Keep credentials in the environment.

## Scope

The campaign simulator uses fitted spend parameters and illustrative revenue assumptions. The sensitivity chart uses fixed example impacts. Use the outputs to inspect how the methods work and how their assumptions affect the results.
