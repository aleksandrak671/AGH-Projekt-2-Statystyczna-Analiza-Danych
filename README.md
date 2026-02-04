# AGH Project 2: Statistical Data Analysis

Final project for the **Statistical Data Analysis** course (AGH University of Science and Technology).
Topic: **Multidimensional Scaling (MDS)** and **Principal Component Analysis (PCA)** on world country data.

---

## Objective

- Perform MDS using two methods:
  - Classical MDS – `cmdscale()`,
  - Sammon mapping – `MASS::sammon()`.
- Conduct PCA on the correlation matrix (`eigen()`, `prcomp()`).
- Compare MDS and PCA results and interpret the differences between countries.

---

## Data

File: **`countries of the world.csv`**
One observation = 1 country.

Variables used (development indicators):
- `GDP ($ per capita)`, `Infant mortality`, `Literacy`, `Phones`,
- `Birthrate`, `Deathrate`,
- `Agriculture`, `Industry`, `Service`.

The repository also contains **`countries_clean_scaled.csv`** – data after cleaning and standardization.

---

## Files

- `Projekt 2.Rmd` – Source code and description (R Markdown),
- `Projekt-2.html` – Rendered report,
- `countries of the world.csv` – Raw data,
- `countries_clean_scaled.csv` – Prepared data.

---

## Analysis Workflow

- **EDA**: Descriptive statistics, histograms, boxplots, correlations, Bartlett's test.
- **MDS**: 2D/3D cmdscale and 2D Sammon, STRESS calculation, quality comparison.
- **PCA**: Eigenvalues, scree plot, biplot, interpretation of PC1–PC3.
- **Comparison**: Correlation of coordinates, conclusions on which variables differentiate countries the most and how many components are sufficient (PC1–PC3 ≈ 85% variance).
