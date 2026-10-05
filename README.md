# Week 6 Integrated Data Science Capstone
## Wine Cultivar Classification and Exploratory Analysis

This project demonstrates an end-to-end data science workflow using the public Wine dataset distributed with scikit-learn. The included CSV makes the project runnable without downloading data at execution time.

### Project contents
- `data/wine_dataset.csv` — 178 observations, 13 numeric input features, target class and class name
- `src/wine_capstone.py` — reproducible analysis and model training
- `outputs/figures/` — class distribution, correlation matrix, confusion matrix, feature signals, PCA projection
- `outputs/tables/` — model comparison, classification report, confusion matrix, K-Means assignments
- `Week_6_Integrated_Capstone_Report.docx` — formatted report

### Run
```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate
pip install -r requirements.txt
python src/wine_capstone.py
```

### Methods
- Stratified 80/20 train-test split (random state 42)
- Logistic Regression with StandardScaler
- Random Forest classifier
- Accuracy, weighted precision, weighted recall, weighted F1, and 5-fold cross-validation
- Exploratory plots, PCA visualization, and K-Means clustering

### Important interpretation note
The dataset is small and curated. A high score on this benchmark does not establish performance on unrelated real-world data. The class labels are dataset classes, not quality grades or consumer recommendations.
