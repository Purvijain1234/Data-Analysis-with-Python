# 📊 Seaborn - Complete Data Visualization Course

> A structured, beginner-to-advanced Seaborn learning series built as an interactive Jupyter Notebook - **pure seaborn only** (no matplotlib), with a comprehensive exploratory data analysis capstone project.

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-66A6FF?style=for-the-badge)](https://seaborn.pydata.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 🗂️ Repository Structure

```
Seaborn-Complete-Mastery/
│
├── 📓 Notebooks/
│   ├── 01-Introduction to Seaborn.ipynb
│   ├── 02-Themes, Styles & Color Palettes.ipynb
│   ├── 03-Relational Plots.ipynb
│   ├── 04-Categorical Plots.ipynb
│   ├── 05-Distribution Plots.ipynb
│   ├── 06-Regression Plots.ipynb
│   ├── 07-Multi-plot Grids.ipynb
│   ├── 08-Heatmaps & correlation.ipynb
│   ├── 09-Advanced Styling & Customization.ipynb
│   ├── 10-Capstone Penguin.ipynb
│   └── 11-Capstone Iris.ipynb
│
└── README.md 
```

---

## 📚 Course Contents

### `01` - Introduction & Dataset Loading

What is Seaborn and why use it over Matplotlib.

```
Topics:
✅ What is Seaborn and why it matters
✅ Beautiful by default - Seaborn's philosophy
✅ Figure-level vs Axes-level functions
✅ 7 Built-in Datasets (tips, iris, penguins, diamonds, flights, titanic, planets)
✅ Why only Seaborn? (no matplotlib complexity)
✅ The power of sns.load_dataset()
```

---

### `02` - Styling, Themes & Color Palettes

Change the entire look with one function.

```
Topics:
✅ sns.set_theme() - 5 built-in themes
  • darkgrid (default) - dark with grid
  • whitegrid - white with grid
  • dark - dark, no grid
  • white - minimal, clean
  • ticks - white with axis ticks
✅ sns.set_context() - 4 scaling contexts
  • paper - smallest (publications)
  • notebook - default (Jupyter)
  • talk - larger (presentations)
  • poster - largest (posters)
✅ Color Palettes (18 different palettes)
  • Categorical: deep, muted, pastel, bright, dark, colorblind
  • Sequential: Blues, Reds, Greens, YlOrRd, viridis, plasma
  • Diverging: coolwarm, RdBu, RdYlGn, icefire, vlag
✅ sns.color_palette() - create custom palettes
```

<p align="center">
  <img width="841" height="348" alt="Image" src="https://github.com/user-attachments/assets/87860970-867a-442e-99fb-90f552d62ac0" />
</p>

---

### `03` - Relational Plots (Scatter & Line)

Show relationships between continuous variables.

```
Topics:
✅ sns.relplot() - Figure-level (creates entire figure)
✅ Basic scatter: x, y variables
✅ Multi-dimensional scatter with:
  • hue - color by category
  • size - point size by numeric value
  • style - marker shape by category
✅ Line plots - kind='line'
✅ Subplots with col and row parameters
✅ Real example: Restaurant bill vs tip by gender & day
```

**Key Function:**
```python
sns.relplot(
    data=tips,
    x='total_bill',
    y='tip',
    hue='sex',           # Color by gender
    size='party_size',   # Size by party
    col='day',           # Separate by day
    height=5,
    aspect=1.3
)
```

<p align="center">
  <img width="1134" height="275" alt="Image" src="https://github.com/user-attachments/assets/2ca9b27d-60d7-4f88-90cd-4f37f4d6f991" />
</p>

---

### `04` - Categorical Plots - (Bar, Box, Violin, Point)

Compare values across categories using point-based plots.

```
Topics:
✅ sns.catplot() - Figure-level categorical plots
✅ Bar plot - kind='bar'
  • Shows mean with confidence interval
  • Best for comparing averages
✅ Count plot - kind='count'
  • Frequency of each category
  • See sample sizes
✅ Strip plot - kind='strip'
  • All individual points (with jitter)
  • See full distribution
✅ Box plot - kind='box'
  • Median, quartiles, outliers
  • 5-number summary
✅ Violin plot - kind='violin'
  • Full probability distribution
  • Beautiful and informative
✅ Real example: Tips by day, gender, meal type
```

<p align="center">
  <img width="1120" height="680" alt="Image" src="https://github.com/user-attachments/assets/5b2cc21e-e482-487b-998d-6e18f6b687d8" />
</p>

---

### `05` - Distribution Plots (Histogram, KDE, ECDF, Rug)

Understand how a single variable is distributed.

```
Topics:
✅ sns.displot() - Figure-level distribution plots
✅ Histogram - kind='hist'
  • Bars showing frequency in bins
  • kde=True adds smooth curve
✅ KDE (Kernel Density Estimation) - kind='kde'
  • Smooth probability density curve
  • Professional and elegant
✅ ECDF (Empirical Cumulative Distribution) - kind='ecdf'
  • Cumulative percentage
  • Great for comparing groups
✅ Rug plots - individual data points on axis
✅ Multi-group comparison with hue
✅ Create subplots with col and row
✅ Real example: Bill amount distribution by gender
```

<p align="center">
  <img width="1082" height="724" alt="Image" src="https://github.com/user-attachments/assets/20f52e4e-9bed-4760-ae50-ff93a8ee80ad" />
</p>

---

### `06` - Regression & Joint Plots

Show trends and relationships with fitting.

```
Topics:
✅ sns.lmplot() - Figure-level regression
  • Scatter with regression line
  • Confidence band (shaded area)
  • Separate lines by hue
✅ Polynomial regression - order parameter
  • order=1 (linear)
  • order=2 (quadratic)
  • order=3 (cubic)
✅ sns.jointplot() - Bivariate + marginals
  • Center: scatter/regression/KDE
  • Top: X distribution
  • Right: Y distribution
✅ Joint plot types:
  • scatter - points only
  • reg - with regression line
  • kde - smooth density
  • hex - heatmap for dense data
✅ Real example: Bill vs tip, diamonds carat vs price
```


<!-- <p align="center">
  <img width="587" height="384" alt="Image" src="https://github.com/user-attachments/assets/fc4c1d5a-17f7-4c2c-a004-5b3c90479a5e" />
</p>


<p align="center">
  <img width="460" height="458" alt="Image" src="https://github.com/user-attachments/assets/4b72d35d-65a5-4276-ad3c-ea1fbd0be29e" />
</p> -->


<table align="center">
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/fc4c1d5a-17f7-4c2c-a004-5b3c90479a5e" width="400">
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/4b72d35d-65a5-4276-ad3c-ea1fbd0be29e" width="400">
    </td>
  </tr>
</table>

---

### `07` - Multi-plot Grids (PairGrid & PairPlot)

See all relationships at once!

```
Topics:
✅ sns.pairplot() - Automatic scatter matrix
  • Diagonal: univariate distributions
  • Off-diagonal: bivariate relationships
  • Perfect for EDA!
✅ Color by hue parameter
✅ Different diagonal kinds:
  • hist - histogram
  • kde - smooth curve
  • auto - choose automatically
✅ sns.PairGrid() - Custom version
  • map_diag() - diagonal plots
  • map_upper() - upper triangle
  • map_lower() - lower triangle
✅ Real example: Iris flowers - all features vs all features
```

<p align="center">
<img width="716" height="645" alt="Image" src="https://github.com/user-attachments/assets/46b984d6-f1c3-4394-9aec-d5827f01be2b" />
</p>

---

### `08` - Heatmaps & Correlation Analysis

Encode 2D data as colors in a grid.

```
Topics:
✅ sns.heatmap() - 2D grid with colors
  • annot=True - show values
  • cmap - color palette
  • center - center value for diverging palettes
  • linewidths - cell borders
✅ Correlation matrices
  • Pearson correlation (r = -1 to +1)
  • Blue: negative, Red: positive
✅ Pivot tables as heatmaps
  • Aggregated data in grid
  • Day × Gender average tips
✅ sns.clustermap() - With hierarchical clustering
  • Reorders rows and columns by similarity
  • Shows dendrogram (clustering tree)
  • Reveals natural groupings
✅ Real example: Iris correlation, tips by day & gender
```

<p align="center">
<img width="564" height="547" alt="Image" src="https://github.com/user-attachments/assets/f1850c90-c638-4298-ac10-32bd15f8ae50" />
</p>

---

### `09` -Advanced Styling & Customization

Fine-tune your visualizations.

```
Topics:
✅ Global styling:
  • sns.set_theme()
  • sns.set_palette()
  • sns.set_context()
✅ Multiple encoding dimensions:
  • hue - color
  • size - point size
  • style - marker shape
  • col/row - subplots
✅ Alpha transparency
✅ Edge colors and line widths
✅ Custom legends and positioning
✅ Real example: Complex multi-dimensional scatter
```

---

### 🏆 Capstone Project - Complete EDA (Exploratory Data Analysis)

A comprehensive analysis of Antarctic Penguins dataset using **all Seaborn techniques**.

**Project Structure:**

```
Step 1: Dataset Exploration
├── Load penguins dataset (344 observations)
├── Examine shape, dtypes, missing values
└── Basic statistics

Step 2: Univariate Analysis (Individual Variables)
├── Bill length distribution
├── Flipper length distribution
├── Body mass distribution
└── By species (separate distributions)

Step 3: Bivariate Analysis (Pairs of Variables)
├── Bill length vs Flipper length (by species)
├── Bill depth vs Body mass (by species)
├── Mass distribution by species (violin plot)
└── Species separation analysis

Step 4: Multivariate Analysis (All Variables)
└── PairPlot - see all 6 relationships at once!

Step 5: Correlation Analysis
├── Correlation matrix heatmap
├── Identify strongest relationships
└── Understand variable interdependencies

Step 6: Insights & Conclusions
├── Three species are clearly distinct
├── Strong correlations within species
├── Flipper length & body mass highly correlated
└── Physical measurements can classify species
```

**Key Findings:**

| Finding | Insight |
|---------|---------|
| Species Separation | Adelie, Chinstrap, Gentoo occupy different measurement spaces |
| Strongest Correlation | Flipper length ↔ Body mass (r=0.87) |
| Negative Correlation | Bill length ↔ Bill depth (r=-0.24) - inverse relationship |
| Consistency | Each species shows consistent patterns within itself |
| Classification Potential | Physical measurements alone can reliably identify species |

<!-- <p align="center">
<img width="700" height="301" alt="Image" src="https://github.com/user-attachments/assets/2a0ccd61-074d-4660-8860-9e935065384d" />
</p>


<p align="center">
<img width="502" height="306" alt="Image" src="https://github.com/user-attachments/assets/ba8af4d2-e2d6-4e22-9c68-454691846d8a" />
</p>

<p align="center">
<img width="723" height="628" alt="Image" src="https://github.com/user-attachments/assets/368a9605-cfe0-4cac-bc5a-24a977dfda26" />
</p> -->


<table align="center">
<tr>
<td align="center">
<img src="https://github.com/user-attachments/assets/2a0ccd61-074d-4660-8860-9e935065384d" width="450">
</td>

<td align="center">
<img src="https://github.com/user-attachments/assets/ba8af4d2-e2d6-4e22-9c68-454691846d8a" width="450">
</td>
</tr>

<tr>
<td align="center">
<img src="https://github.com/user-attachments/assets/368a9605-cfe0-4cac-bc5a-24a977dfda26" width="450">
</td>

<td align="center">
<img src="https://github.com/user-attachments/assets/9c41e221-f9e4-4da1-b47d-763845808ac0" width="450">
</td>
</tr>
</table>

---

## 📊 Plot Selection Guide

```
Relationship between 2 continuous variables     → relplot(kind='scatter')
Trend over time / continuous relationship       → relplot(kind='line')
Compare values across categories                → catplot(kind='bar')
Show distribution within categories             → catplot(kind='box/violin')
Individual points in categories                 → catplot(kind='strip/swarm')
Distribution of single variable                 → displot(kind='hist/kde/ecdf')
Trend with fitting line                         → lmplot()
Bivariate + marginal distributions             → jointplot()
All variable relationships at once             → pairplot()
2D numerical data (correlation)                → heatmap()
Multi-panel complex analysis                   → catplot/relplot with col/row
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Basic pandas knowledge

### Installation

```bash
# Clone the repository
git clone https://github.com/YourUsername/Seaborn-Complete-Mastery.git
cd Seaborn-Complete-Mastery

# Install dependencies
pip install -r requirements.txt
```

### requirements.txt

```
jupyter>=1.0.0
seaborn>=0.12.0
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
```

### Running the Notebooks

```bash
# Start Jupyter
jupyter notebook

# Or use JupyterLab
jupyter lab
```

Then open any notebook (01 through 11) and run the cells sequentially.

> 💡 **Pro Tip:** All datasets are loaded from Seaborn's online repository - no local files needed. Just run `sns.load_dataset('name')` and it downloads automatically!

---

## 📊 Seaborn vs Matplotlib

| Feature | Seaborn | Matplotlib |
|---------|---------|-----------|
| **Learning Curve** | Gentle (high-level) | Steep (low-level) |
| **Code Length** | Brief (2-3 lines) | Verbose (10+ lines) |
| **Default Styling** | Beautiful | Plain |
| **Data Integration** | Direct (DataFrames) | Manual preprocessing |
| **Statistical Features** | Built-in (confidence intervals) | Manual calculation |
| **Best For** | Exploratory analysis & reports | Fine-grained customization |
| **Multi-panel Plots** | Automatic (relplot, catplot) | Manual (subplots) |

**Bottom Line:** Seaborn = Quick EDA | Matplotlib = Complete Control

---

## 💡 Key Concepts

### Figure-level Functions (What We Use!)
- `relplot()` - Relational plots with automatic subplots
- `catplot()` - Categorical plots with automatic subplots
- `displot()` - Distribution plots with automatic subplots
- `lmplot()` - Regression plots with automatic subplots
- `pairplot()` - Scatter matrix of all variables
- `jointplot()` - Bivariate + marginal distributions
- `clustermap()` - Heatmap with hierarchical clustering

### Encoding Dimensions
- **hue** - Color (categorical)
- **size** - Point size (numeric)
- **style** - Marker shape (categorical)
- **col/row** - Subplots (categorical)

### Why Only Seaborn?
- Simpler syntax
- Beautiful by default
- Perfect for exploratory analysis
- What professionals use for EDA
- Focus on data, not plotting mechanics

---


## 🤝 Contributing

Contributions welcome! Feel free to:
- Report bugs or issues
- Suggest improvements
- Add additional examples
- Improve documentation

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💼 Author

**Your Name / Organization**

- 📧 Email: your.email@example.com
- 💼 LinkedIn: [Your LinkedIn]
- 🐙 GitHub: [@YourGitHub]

---

## ⭐ Support This Project

If this course helped you learn Seaborn:

1. ⭐ **Star this repository** on GitHub
2. 🔖 **Bookmark** for future reference
3. 📤 **Share** with others learning data visualization
4. 💬 **Give feedback** - what could be better?

---

<div align="center">

⭐ **Star this repo if it helps you!** ⭐

*Part of the [Data Analysis with Python](https://github.com/user/data-analysis-python) series*

</div>
