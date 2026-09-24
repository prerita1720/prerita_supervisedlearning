# 🏠 Real Estate House Price Prediction

Supervised Learning & Regression project — built as a Junior Data Scientist exercise for a real estate
analytics firm. The goal is to design, implement, analyze, and evaluate multiple supervised learning
models that predict house prices, and to explain **why** certain models perform better than others.

## 📁 Repository Structure

```
.
├── House_Price_Prediction_Project.ipynb   # Main deliverable: full analysis, code, plots, results
├── RealEstate_HousePrice_Dataset_4200.xlsx # Dataset (4,200 rows)
├── docs/
│   └── Theory_Concepts.pdf                # Part A theory answers (definitions/concepts)
├── requirements.txt                       # Python dependencies
└── README.md
```

## 📊 Dataset

`RealEstate_HousePrice_Dataset_4200.xlsx` — 4,200 rows, 12 columns:

| Column | Description |
|---|---|
| `house_id` | Unique identifier (dropped before modeling) |
| `area_sqft` | House area in square feet |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `location_score` | Numeric location desirability score |
| `age_years` | Age of the property (years) |
| `distance_city_km` | Distance from city center (km) |
| `lot_size_sqft` | Lot size in square feet |
| `has_garage` | 1 if the property has a garage, else 0 |
| `has_pool` | 1 if the property has a pool, else 0 |
| `renovation_years_ago` | Years since last renovation |
| `house_price_inr` | **Target variable** — house price (INR) |

## 🧠 What's Inside the Notebook

| Part | Contents |
|---|---|
| A | Conceptual theory Q&A (supervised learning, regression vs. classification, simple linear regression, assumptions, bias–variance, overfitting/underfitting) |
| B | Dataset exploration, correlation heatmap, feature/target scatter plots, train/test split |
| C | Simple Linear Regression (`area_sqft` → price), regression line plot, assumption validation (residuals, Q-Q plot) |
| D | Model evaluation metrics: MSE, MAE, RMSE, R², Adjusted R² — with interpretation |
| E | Multiple Linear Regression (core features + all features), comparison vs. Simple LR |
| F | Polynomial Regression (degree 1/2/3/8), visual & numerical comparison, overfitting/underfitting analysis |
| G | Gradient Descent from scratch — Batch, Stochastic (SGD), and Mini-Batch — with convergence comparison |
| H | Bias–variance diagnostics across all models (train vs. test RMSE gap analysis) |
| I | Final summary report: best model, effect of gradient descent, overfitting/underfitting evidence, business interpretation |

## 🏆 Key Result

**Multiple Linear Regression (using all available features)** was the best-performing model —
highest test R² / Adjusted R², lowest test RMSE/MAE, and the smallest train–test gap, indicating
strong generalization and a good bias–variance balance. Full metrics, plots and reasoning are in
the notebook (Parts D, E, and H).

## ▶️ How to Run

1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch Jupyter and open the notebook:
   ```bash
   jupyter notebook House_Price_Prediction_Project.ipynb
   ```
4. Run all cells (**Kernel → Restart & Run All**) — the notebook runs end-to-end with no manual steps,
   loading the dataset directly from the repository root.

## 🎥 Video Walkthrough

A 5–10 minute recorded walkthrough (face + screen) explaining the concepts and implementation is
required per the submission guidelines. Add your video link here once recorded:

> **Video:** _[add your Google Drive / YouTube unlisted link here]_

## 📄 Theory Document

See [`docs/Theory_Concepts.pdf`](docs/Theory_Concepts.pdf) for the written answers to Part A's
conceptual questions.

---
*Built as part of a supervised learning / regression coursework project. "Quality is our Motto."*
