<!-- Banner Typing Animation with Gradient Colors -->
<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&pause=800&color=FF5733,33FF57,3357FF&center=true&vCenter=true&width=900&lines=📊+Visualization;📈+Charts+%26+Plots;💻+Python+Matplotlib+Seaborn;📔+Jupyter+Notebooks" alt="Typing SVG" />
</p>

---

# 🚀 Visualization: Charts & Graphs

This module covers **data visualization using Python libraries** like Matplotlib, Seaborn, Lux, and more.  
Hands-on exercises are included in **Jupyter Notebooks**.

---

## 🧩 Module Structure

| Topic | Description |
|-------|------------|
| Introduction | Overview of data visualization concepts |
| Matplotlib | Getting started with Matplotlib |
| 📔 Jupyter Notebook – Matplotlib | Hands-on Matplotlib exercises |
| 🔗 Practice – Matplotlib | Practical exercises |
| Seaborn | Line plots using `sns.lineplot()` |
| 📔 Jupyter Notebook – Line Plot | Hands-on line plots |
| Bar Plots | Column charts using `sns.barplot()` |
| Heatmap | Heatmaps for correlation & patterns |
| 📔 Jupyter Notebook – Barplot & Heatmap | Practical exercises |
| 🔗 Practice – Line, Bar, Heatmap | Exercises |
| Scatter Plot | Scatter plots for data distribution |
| 📔 Jupyter Notebook – Scatterplot | Hands-on scatter plots |
| 🔗 Practice – Scatterplot | Exercises |
| Distribution | Histogram and KDE plots |
| KDE & CDE | Kernel Density & Cumulative Distribution plots |
| 📔 Jupyter Notebook – Distribution | Practical exercises |
| 🔗 Practice – Distribution | Exercises |
| Subplot | Multiple plots in one figure |
| 📔 Jupyter Notebook – Subplot | Practical exercises |
| 🔗 Practice – Subplot | Exercises |
| Bonus: Lux | Automatic visualization library |
| 📔 Jupyter Notebook – Lux | Hands-on Lux exercises |
| 🔗 Free Practice | Optional exercises |
| Choosing Plots | Guidelines for selecting the right chart |
| Final Practical Exercise | Module wrap-up project |

---

## 🛠 Technologies Used

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-1F77B4?style=for-the-badge&logo=seaborn&logoColor=white)
![Lux](https://img.shields.io/badge/Lux-FF6F61?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=BehruzMaxmudov1203&show_icons=true&theme=tokyonight" alt="GitHub Stats" /> 
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=BehruzMaxmudov1203&theme=tokyonight" alt="GitHub Streak" /> 
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=BehruzMaxmudov1203&theme=react-dark" alt="GitHub Activity Graph" /> 
</p>

---

## 📌 Example: Scatter Plot & Heatmap

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&pause=800&color=FF6F61,61FF6F,6161FF&center=true&vCenter=true&width=900&lines=Scatter+Plot;Heatmap;Bar+%26+Line+Plots;KDE+Distribution" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://media.giphy.com/media/xT0GqssRweIhlz209i/giphy.gif" width="450" alt="AI Neural Network Animation">
</p>


```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np

# Sample dataset
data = pd.DataFrame({
    'x': np.random.randn(100),
    'y': np.random.randn(100),
    'category': np.random.choice(['A','B','C'], size=100)
})

# Scatter Plot
plt.figure(figsize=(8,6))
sns.scatterplot(x='x', y='y', hue='category', data=data)
plt.title("Scatter Plot Example")
plt.show()

# Heatmap
corr = data[['x','y']].corr()
plt.figure(figsize=(6,4))
sns.heatmap(corr, annot=True, cmap='coolwarm')
plt.title("Heatmap Example")
plt.show()

# Bar Plot
sns.barplot(x='category', y='x', data=data)
plt.title("Bar Plot Example")
plt.show()
