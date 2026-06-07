# Unsupervised Learning on Country Data
Celebal Technologies Internship Assignment

## What it does
Groups 162 countries into clusters based on income, health, and development indicators — without any labels. Uses K-Means and DBSCAN.

## Dataset
`country-data.csv` — 162 countries, 9 features (child mortality, GDP, income, life expectancy, etc.)

## Steps
1. Load & clean data
2. Scale features (StandardScaler)
3. Find best K using Elbow Method → **K=3**
4. Run K-Means + DBSCAN
5. Visualize with PCA

## Results
| Cluster | Label | Countries |
|---------|-------|-----------|
| 0 🔴 | Underdeveloped | 47 (Afghanistan, Niger, Somalia...) |
| 1 🟢 | Developed | 36 (USA, Germany, Japan...) |
| 2 🔵 | Developing | 79 (India, Brazil, China...) |

**Silhouette Score: 0.41**

## How to Run
1. Upload `country-data.csv` and the notebook to Colab or VS Code
2. Run Cell 1 (installs libraries)
3. Run All

## Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
