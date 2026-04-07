# 📊 Matplotlib - Complete Data Visualisation Course

> A structured, beginner-to-advanced Matplotlib learning series built as an interactive Jupyter Notebook - pure `plt.` pyplot style, with a 9-chart student dashboard capstone.

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-11557c?style=for-the-badge)](https://matplotlib.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 🗂️ Repository Structure

```
Matplotlib/
│
├── 01 - Introduction of Matplotlib
├── 02 - Line Charts
├── 03 - Bar Charts
├── 04 - Scatter Plots
├── 05 - Histograms & Distributions
├── 06 - Pie & Donut Charts
├── 07 - Figure & Axes Customisation
├── 08 - Subplots & Layouts
├── 09 - Styles & Themes
├── 10 - Annotations & Text
├── 11 - Plotting with Pandas
├── 12 - Heatmaps & 2D Plots
├── 13 - Twin Axes & Dual Y-Axis
├── 14 - Saving & Exporting Figures
├── 15 - Student Data Dashboard
└── readme.md
```

---

## 📚 Course Contents

### `01` - Introduction to Matplotlib

What data visualisation is, why it matters, and how pyplot works.

```
Topics:
✅ What is Data Visualisation and why it matters
✅ Where charts fit in the Data Science pipeline
✅ What is Matplotlib and why use it
✅ pyplot - the simple drawing interface
✅ The 9-step pyplot workflow (used in every section)
✅ First chart - plt.plot(), plt.title(), plt.show()
```

---

### `02` - Line Charts

Best for showing trends over time or continuous relationships.

```
Topics:
✅ Basic single line - plt.plot()
✅ Multiple lines on one chart
✅ Line styles - solid, dashed, dotted, dash-dot
✅ Markers - o, s, ^, D, *
✅ fill_between - confidence bands and ranges
✅ plt.axhline() - reference lines
```

<!-- Add your line chart image below -->
<!-- ![Line Chart](images/line_chart.png) -->

---

### `03` - Bar Charts

Best for comparing discrete categories.

```
Topics:
✅ Vertical bar - plt.bar()
✅ Horizontal bar - plt.barh()
✅ Grouped bar charts
✅ Stacked bar charts
✅ Adding value labels on bars with plt.text()
```

<!-- Add your bar chart image below -->
<!-- ![Bar Chart](images/bar_chart.png) -->

---

### `04` - Scatter Plots

Best for exploring relationships between two numeric variables.

```
Topics:
✅ Basic scatter - plt.scatter()
✅ Color by category (gender groups)
✅ Colormap scatter - c= for third variable
✅ Bubble chart - s= encodes a third variable
✅ Pearson r - showing correlation on chart
```

<!-- Add your scatter plot image below -->
<!-- ![Scatter Plot](images/scatter_plot.png) -->

---

### `05` - Histograms & Distributions

Best for understanding how values are spread.

```
Topics:
✅ plt.hist() - bins, alpha, edgecolor
✅ Overlapping histograms for comparison
✅ plt.axvline() - mean and median lines
✅ plt.boxplot() - 5-number summary
✅ plt.violinplot() - full distribution shape
```

<!-- Add your histogram / distribution image below -->
<!-- ![Histograms](images/histograms.png) -->

---

### `06` - Pie & Donut Charts

Best for part-to-whole relationships (5 or fewer categories).

```
Topics:
✅ plt.pie() - labels, colors, startangle
✅ autopct - percentage labels on slices
✅ explode - pull out a slice
✅ Donut chart - wedgeprops=dict(width=0.5)
✅ Pie vs Bar - when to use which
```

<!-- Add your pie / donut chart image below -->
<!-- ![Pie Donut](images/pie_donut.png) -->

---

### `07` - Figure & Axes Customisation

Making charts look professional.

```
Topics:
✅ plt.figure() - figsize, dpi, facecolor
✅ Removing top and right spines
✅ plt.grid() - subtle grid lines
✅ Tick rotation and font size
✅ plt.legend() - position and styling
✅ Default vs fully customised - side by side
```

<!-- Add your customised chart image below -->
<!-- ![Customisation](images/customisation.png) -->

---

### `08` - Subplots & Layouts

Multiple charts in one figure.

```
Topics:
✅ plt.subplot(rows, cols, index)
✅ plt.subplot2grid() - custom proportions
✅ plt.suptitle() - overall figure title
✅ plt.tight_layout() - fix spacing
✅ 2×2 grid example
✅ Custom layout - wide top + smaller bottom charts
```

<!-- Add your subplot grid image below -->
<!-- ![Subplots](images/subplots.png) -->

---

### `09` - Styles & Themes

Change the entire look with one line.

```
Topics:
✅ plt.style.use() - apply a style globally
✅ with plt.style.context() - apply temporarily
✅ 6 popular styles compared side by side
✅ plt.rcParams - global default settings
✅ plt.rcdefaults() - reset to defaults
```

<!-- Add your styles comparison image below -->
<!-- ![Styles](images/styles.png) -->

---

### `10` - Annotations & Text

Guide the reader's eye to what matters.

```
Topics:
✅ plt.text() - add text anywhere on chart
✅ plt.annotate() - text with an arrow
✅ plt.axhline() / plt.axvline() - reference lines
✅ plt.axhspan() / plt.axvspan() - shaded zones
✅ Value labels and status labels on bars
```

<!-- Add your annotations image below -->
<!-- ![Annotations](images/annotations.png) -->

---

### `11` - Plotting with Pandas

Draw charts directly from a DataFrame.

```
Topics:
✅ df.plot(kind='bar') - bar from groupby
✅ df.plot(kind='hist') - histogram from DataFrame
✅ df.plot(kind='scatter', x=, y=) - scatter with colormap
✅ df.plot(kind='box') - box plot from DataFrame
✅ Combining df.plot() with plt.title() etc.
```

<!-- Add your Pandas plot image below -->
<!-- ![Pandas Plot](images/pandas_plot.png) -->

---

### `12` - Heatmaps & 2D Plots

Encode values as colours in a grid.

```
Topics:
✅ plt.imshow() - matrix as heatmap
✅ plt.colorbar() - colour scale
✅ Adding text labels inside each cell
✅ Correlation matrix heatmap
✅ City × Subject pivot heatmap
✅ plt.hexbin() - 2D histogram
```

<!-- Add your heatmap image below -->
<!-- ![Heatmap](images/heatmap.png) -->

---

### `13` - Twin Axes & Dual Y-Axis

Two different variables on the same chart.

```
Topics:
✅ plt.twinx() - second Y axis on right side
✅ Bar chart + line on same chart
✅ Colour-coded axis labels
✅ Combining legends from both axes
✅ Bar + two lines on dual Y axis
```

<!-- Add your dual Y-axis chart image below -->
<!-- ![Twin Axes](images/twin_axes.png) -->

---

### `14` - Saving & Exporting Figures

Save charts for reports, presentations, and web.

```
Topics:
✅ plt.savefig() - PNG, PDF, SVG, JPG
✅ dpi - resolution for screen vs print
✅ bbox_inches='tight' - remove white space
✅ transparent=True - transparent background
✅ File size comparison across formats and DPI
✅ Critical rule - savefig() BEFORE show()
```

---

### 🏆 Capstone Project - Student Data Dashboard

A complete 9-chart visual dashboard built using `plt.subplot()` - pure pyplot style.

**Dashboard layout - 3 rows × 3 columns:**

```
┌─────────────────┬─────────────────┬─────────────────┐
│  1. Histogram   │  2. Bar Chart   │  3. Scatter     │
│  Score dist.    │  Subject avgs   │  Study vs Score │
├─────────────────┼─────────────────┼─────────────────┤
│  4. Donut Chart │  5. Grouped Bar │  6. Heatmap     │
│  Grade split    │  City-subject   │  Correlation    │
├─────────────────┼─────────────────┼─────────────────┤
│  7. Horiz. Bar  │  8. Box Plot    │  9. Line Chart  │
│  Top 10 students│  Subject spread │  Attend vs Score│
└─────────────────┴─────────────────┴─────────────────┘
```

**What each chart reveals:**

| Chart | Insight |
|-------|---------|
| 1. Histogram | Is the overall score distribution normal or skewed? |
| 2. Bar | Which subject has the highest/lowest average? |
| 3. Scatter | Does more study lead to higher scores? |
| 4. Donut | What fraction of students got each grade? |
| 5. Grouped bar | Which city performs best in which subject? |
| 6. Heatmap | Are all subjects correlated with each other? |
| 7. Horizontal bar | Who are the top 10 performers? |
| 8. Box plot | Which subject has the most consistent scores? |
| 9. Line | Does higher attendance improve scores? |

<!-- Add your full dashboard image below -->
<!-- ![Student Dashboard](images/student_dashboard.png) -->

---

## 🚀 Getting Started

### Install dependencies

```bash
pip install matplotlib numpy pandas jupyter
```

### Clone and run

```bash
git clone https://github.com/Purvijain1234/Data-Analysis-with-Python.git
cd Data-Analysis-with-Python/Matplotlib

jupyter notebook
```

> 💡 The dataset is generated inside the notebook - just run the **setup cell at the top of Section 15** before building the dashboard.

---

### 💡 Chart selection guide

```
Trend over time           → plt.plot()
Compare categories        → plt.bar() / plt.barh()
Relationship (2 vars)     → plt.scatter()
Distribution of 1 var     → plt.hist() / plt.boxplot()
Part of a whole (≤6 cat)  → plt.pie()
Matrix / correlation      → plt.imshow()
Two different scales      → plt.twinx()
Multiple insights         → plt.subplot() dashboard
```

---

## 👩‍💻 Author

**Purvi Jain**

[![GitHub](https://img.shields.io/badge/GitHub-Purvijain1234-181717?style=flat-square&logo=github)](https://github.com/Purvijain1234)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Purvi_Jain-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/purvi-jain-315683326)

---

<div align="center">

⭐ **Star this repo if it helped you learn Matplotlib!** ⭐

*Part of the [Data Analysis with Python](https://github.com/Purvijain1234/Data-Analysis-with-Python) series*

</div>
