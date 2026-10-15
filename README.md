# 🛍️ Product Recommendation System Using Graphs

<p align="center">
  <strong>Discovering Product Relationships Through Graph Theory and Data Analysis</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/NetworkX-Graph%20Analysis-008B8B?style=for-the-badge" alt="NetworkX">
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge" alt="Matplotlib">
  <img src="https://img.shields.io/badge/Google%20Colab-Notebook-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Google Colab">
</p>

---

## 📌 About the Project

This project explores how **graph theory and network analysis** can be applied to e-commerce data to identify products frequently purchased together and generate product recommendations.

Using a synthetic dataset, I built a product co-purchase network, analyzed relationships between products, calculated association metrics, and developed a recommendation function based on purchasing patterns.

The project demonstrates how Python and data analysis can help businesses identify potential cross-selling opportunities and better understand product relationships.

## 🎯 Business Objectives

- Identify products frequently purchased together.
- Discover strong associations between product pairs.
- Analyze product connectivity within a network.
- Generate recommendations for complementary products.
- Demonstrate how purchasing data can support business decisions.

## 📊 Dataset Overview

| Metric | Description |
|:--|:--|
| 🧾 Orders | 1,000 |
| 📦 Products | 20 |
| 🗂️ Product categories | 5 |
| 🧪 Data source | Synthetic dataset |

> **Disclaimer:** The dataset was generated with Python for educational and portfolio purposes. It does not represent real transactions or actual customer behavior.

## 🛠️ Tech Stack

| Technology | Purpose |
|:--|:--|
| Python | Data processing and analysis |
| Pandas | Data manipulation and aggregation |
| NumPy | Synthetic data generation |
| NetworkX | Graph construction and network metrics |
| Matplotlib | Data visualization |
| Google Colab | Notebook development |
| GitHub | Documentation and version control |

## 🔍 Project Workflow

```text
Synthetic Data Generation
          ↓
Exploratory Data Analysis
          ↓
Product Co-Purchase Network
          ↓
Graph Metrics & Association Analysis
          ↓
Product Recommendation System
          ↓
Visualizations & Exported Results
```

## 🧠 Methodology

### 1. Data Preparation

Generated a synthetic product catalog and order-items dataset. Performed exploratory data analysis to inspect records, check missing values and duplicate product-order combinations, and summarize product sales.

### 2. Graph Construction

<img width="920" height="678" alt="image" src="https://github.com/user-attachments/assets/93119377-408d-44d7-81c1-e2ca6abdfa4b" />


Represented the purchasing relationships as an undirected graph:

- **Nodes:** Products in the catalog.
- **Edges:** Product pairs appearing in the same order.
- **Edge weights:** Number of orders containing both products.

### 3. Network Analysis

<img width="1091" height="591" alt="image" src="https://github.com/user-attachments/assets/2fe520d6-b322-4bfd-b328-f1f1b15b3a79" />


Calculated graph metrics to evaluate product relationships:

- **Degree:** Number of distinct products connected to a product.
- **Weighted Degree:** Total co-purchase frequency across a product's connections.

These metrics help identify products connected to a broad range of other products and products involved in frequent co-purchase relationships.

### 4. Association Metrics



Used three metrics to evaluate relationships between product pairs:

| Metric | What it measures |
|:--|:--|
| **Support** | How frequently two products occur together across all orders |
| **Confidence** | How often one product is purchased when the other is present |
| **Lift** | How strong an association is compared with the expected frequency under independence |

**Interpretation:** Lift greater than 1 indicates a positive association in the observed data. These metrics reveal patterns, not causation.

### 5. Recommendation Logic

Developed a Python function that recommends related products by ranking associations using **Lift** and **co-purchase frequency**.

A minimum co-purchase threshold helps filter out product

📈 Visualizations & Findings

1. Products Bought Together

This chart highlights the product pairs that most frequently appear in the same order, helping identify potential complementary products and cross-selling opportunities.

<img width="1092" height="592" alt="image" src="https://github.com/user-attachments/assets/889ce0f1-55ad-4ce9-9022-5f2b55b8179c" />


2. Product Associations by Lift

<img width="1087" height="590" alt="image" src="https://github.com/user-attachments/assets/e10ff04d-fe0b-4cb9-913f-39ba158fc084" />


This visualization ranks product pairs by Lift to identify stronger relative purchasing associations. Results should be interpreted alongside co-purchase frequency to avoid overvaluing rare combinations.

3. Top 10 Products by Number of Connections

<img width="990" height="589" alt="image" src="https://github.com/user-attachments/assets/b89073f4-853c-4131-99f3-ce4fc3313e0f" />


This chart compares products by the number of distinct connections in the network. Products with higher Degree values are associated with a broader variety of other products.

### This project demonstrates the practical application of:

- Data preparation and exploratory data analysis.

- Graph modeling and network analysis.

- Product association metrics.

- Python-based recommendation logic.

- Data visualization and analytical storytelling.

It connects technical analysis with a practical business use case: understanding which products may be relevant to recommend together.
