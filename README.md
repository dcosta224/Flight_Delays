# Flight Delay Prediction

**UC Berkeley MIDS W261 Final Project**

Predicting flight delays using machine learning on 5 years of US domestic flight data (2015-2019).

---

## Quick Links

| Section | Notebook | Description |
|---------|----------|-------------|
| **📊 Final Report** | [`Team_2_2_Final_Notebook.ipynb`](Team_2_2_Final_Notebook.ipynb) | Complete project writeup with EDA, methodology, and results |

---

## Project Structure

### Data Ingestion
| Notebook | Description |
|----------|-------------|
| [`Ingestion/Custom_Join_Pipeline.ipynb`](Ingestion/Custom_Join_Pipeline.ipynb) | Kriging-based spatial interpolation for flight-weather joins |

### Feature Engineering
| Notebook | Description |
|----------|-------------|
| [`Feature Engineering/Feature_Engineering_p2.ipynb`](Feature%20Engineering/Feature_Engineering_p2.ipynb) | Core feature engineering (lag features, rolling aggregates) |
| [`Feature Engineering/Graph Features.ipynb`](Feature%20Engineering/Graph%20Features.ipynb) | Graph-based features (PageRank, centrality, airport connectivity) |
| [`Feature Engineering/NN_Feature_Eng_p3.ipynb`](Feature%20Engineering/NN_Feature_Eng_p3.ipynb) | Neural network-specific features (cyclic encoding, weather deltas) |

### Models
| Notebook | Description |
|----------|-------------|
| [`Models/2_Stage_Classifier.ipynb`](Models/2_Stage_Classifier.ipynb) | Two-stage XGBoost pipeline with quantile regression |
| [`Models/NN_MLP_Pipeline.ipynb`](Models/NN_MLP_Pipeline.ipynb) | ResFiLM-MLP neural network architecture |
| [`Models/NN_MLP_CV.ipynb`](Models/NN_MLP_CV.ipynb) | Cross-validation and hyperparameter tuning |

---

## Key Results

| Model | F2 Score | Notes |
|-------|----------|-------|
| Two-Stage XGBoost | **0.621** | Best overall performance |
| ResFiLM-MLP | 0.58 | Neural network |
| XGBoost Regressor | 0.54 | Baseline |

---

## Authors

- Daniel Costa
- Team 2-2 Members
