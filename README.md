# ML Fundamentals

Five classic machine-learning problems I worked through while learning supervised and unsupervised methods: regression, classification and clustering, from data cleaning to evaluation. Each folder has the notebook and its dataset.

## Results

| Project | Task | Model | Test result |
|---|---|---|---|
| [Car price](car-price-regression/) | Regression | Linear Regression, Lasso | R² 0.84 (Linear), 0.87 (Lasso) |
| [House price](house-price-regression/) | Regression | Linear Regression | R² 0.58 |
| [Diabetes](diabetes-classification/) | Classification | SVM (linear kernel) | Accuracy 77.3% |
| [Sonar: rock vs mine](sonar-rock-vs-mine/) | Classification | Logistic Regression | Accuracy 76.2% |
| [Customer segmentation](customer-segmentation/) | Clustering | K-Means | Silhouette 0.55 |

## What I'd improve now

- **House price:** an R² of 0.58 from a handful of features is a baseline. Log-transforming the target, encoding categorical features and trying gradient boosting would likely lift it substantially.
- **Diabetes:** report precision and recall, not only accuracy. A missed diabetic patient costs far more than a false alarm, so recall matters most here.
- **Small datasets (Sonar, ~200 rows):** use cross-validation instead of a single train/test split, since one split can swing results by several points.

## Run locally

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook
```

The notebooks were first built in Google Colab and load their CSV from the same folder. The house-price notebook has a Colab upload cell; skip it when running locally.

## Author

**Anjali Sinkar** — [Portfolio](https://anjali-portfolio-six-beige.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/anjali-sinkar-97728925a) · [GitHub](https://github.com/Anjali-Sinkar)
