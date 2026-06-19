# RECURIA: Retail Demand Forecasting

## Overview

Retail systems exhibit complex demand behavior driven by seasonality, consumer activity, economic conditions, promotions, and special events.

This project evaluates whether RECURIA-derived instability and transition features can provide useful predictive structure for retail demand forecasting.

Rather than focusing solely on sales prediction, this study investigates whether mathematically interpretable representations of instability can characterize demand transitions and event-driven disruptions within retail systems.

---

## Research Question

Can mathematically derived transition features capture changes in retail demand behavior more effectively than conventional forecasting features alone?

The central hypothesis is that demand shifts may be preceded by measurable changes in instability, curvature, and transition dynamics.

---

## Dataset

### Source

Walmart Retail Sales Dataset

### Domain

Retail Demand Forecasting

### Prediction Task

Forecast retail demand and identify periods of demand transition.

### Features

* Weekly Sales
* Store Information
* Department Information
* Holiday Indicators
* Economic Variables
* Seasonal Variables
* Time-Based Features

---

## RECURIA Framework

The framework derives four core mathematical quantities:

### Instability Magnitude

η

Measures the local magnitude of change.

### Oscillatory Transition State

r = η(sinθ + cosθ)

Represents directional transition behavior.

### Curvature

r''

Captures acceleration and structural changes within demand patterns.

### Transition Interaction Term

m = ηrr''

Represents the interaction between instability and curvature during demand transitions.

---

## Methodology

1. Construct baseline forecasting models.
2. Generate RECURIA-derived features.
3. Train models using conventional and RECURIA feature sets.
4. Evaluate performance on held-out data.
5. Compare predictive behavior and generalization.

---

## Baseline Models

* Logistic Regression
* Random Forest
* XGBoost

---

## Results

| Model   | Baseline F1 | RECURIA F1 |
| ------- | ----------: | ---------: |
| XGBoost |      0.8509 |     0.8509 |

### Interpretation

Performance remained comparable to strong machine learning baselines.

The primary objective of this study was to evaluate whether a common mathematical representation of instability can generalize to economic and retail demand systems.

---

## Key Findings

* Retail demand exhibits measurable transition behavior.
* RECURIA-derived features remained stable across varying sales conditions.
* Results support further investigation of interpretable transition-oriented feature engineering in demand forecasting.

---

## Repository Structure

```text
src/
notebooks/
results/
data/
```

---

## Research Significance

Retail demand systems represent complex adaptive environments influenced by consumer behavior, seasonal effects, promotions, and economic conditions.

This study contributes to a broader investigation into whether instability and transition dynamics can be represented through a common mathematical framework across unrelated domains.

---

## Related RECURIA Studies

* Clinical Deterioration Prediction
* Multiple Sclerosis Conversion Prediction
* Autoimmune Disorder Classification
* Solar Activity Prediction
* Groundwater Stress Forecasting
* Bike-Sharing Demand Forecasting
* Residential Energy Forecasting

---

## Author

**Ishmaelina Okorley**

Independent researcher exploring mathematically interpretable representations of instability, transition dynamics, and complex system behavior.

---

## License

Released under the MIT License.
