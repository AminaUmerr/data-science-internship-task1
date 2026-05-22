# Task 1 — Exploring and Visualizing the Iris Dataset

## Objective

Understand how to read, summarize, and visualize a dataset using Python.  
The Iris dataset is explored through data inspection and multiple visualizations to identify patterns and relationships among flower measurements.

---

## Dataset

**Name:** Iris Dataset  
**Source:** Loaded via `seaborn.load_dataset("iris")`  
**Shape:** 150 rows × 5 columns  
**Features:**
- `sepal_length` — Length of the sepal (cm)
- `sepal_width` — Width of the sepal (cm)
- `petal_length` — Length of the petal (cm)
- `petal_width` — Width of the petal (cm)
- `species` — Flower species: *setosa*, *versicolor*, or *virginica*

**Missing Values:** None

---

## Approach

1. **Loaded** the dataset using the `pandas` library (via seaborn's built-in loader).
2. **Inspected** the dataset structure using `.shape`, `.columns`, and `.head()`.
3. **Checked for missing values** using `.isnull().sum()` — no missing data found.
4. **Created visualizations** to explore relationships and distributions:
   - **Scatter plot** — Sepal length vs. petal length, colored by species.
   - **Histogram** — Distribution of sepal length values.
   - **Box plot** — Spread and outliers in sepal width across the dataset.

---

## Results and Insights

- **Scatter Plot:** Petal length and sepal length show a strong positive relationship. *Setosa* is clearly separated from *versicolor* and *virginica*, while the latter two overlap slightly. This suggests petal/sepal length can be useful features for classification.
- **Histogram:** Sepal length is roughly bell-shaped, ranging from ~4.3 cm to ~7.9 cm, with most values clustered between 5–6.5 cm.
- **Box Plot:** Sepal width has a relatively tight distribution with a few potential outliers on both ends. The median sepal width is around 3.0 cm.

---

## Libraries Used

- `pandas` — Data loading and inspection
- `matplotlib` — Base plotting
- `seaborn` — Statistical visualizations

---

## Files

| File | Description |
|------|-------------|
| `task1_iris.ipynb` | Jupyter Notebook with full code, visualizations, and conclusions |
| `README.md` | This file |
