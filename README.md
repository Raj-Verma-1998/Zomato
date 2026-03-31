# 🍽️ Zomato Restaurant Clustering & Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikit-learn)
![NLTK](https://img.shields.io/badge/NLTK-NLP-green)
![VADER](https://img.shields.io/badge/VADER-Sentiment-purple)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

> A comprehensive machine learning project that performs **restaurant clustering** and **sentiment analysis** on Zomato restaurant data using KMeans and VADER NLP — across 10 structured experiments.

---

## 📦 Tech Stack & Libraries

| Category | Tools / Libraries |
|---|---|
| **Language** | Python 3.10 |
| **Data Manipulation** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-Learn (KMeans, PCA, StandardScaler) |
| **NLP / Sentiment** | NLTK, VADER (VaderSentiment) |
| **Dimensionality Reduction** | PCA (Principal Component Analysis) |
| **Clustering Evaluation** | Elbow Method, Silhouette Score |
| **Environment** | Jupyter Notebook |

---

## 📂 Dataset Description

This project uses two datasets sourced from Zomato:

### 1. `Zomato Restaurant names and Metadata.csv`
Contains structured metadata about restaurants listed on Zomato.

| Column | Description |
|---|---|
| `name` | Name of the restaurant |
| `online_order` | Whether online ordering is available |
| `book_table` | Whether table booking is available |
| `rate` | Customer rating (out of 5) |
| `votes` | Total number of votes |
| `location` | Area/locality of the restaurant |
| `rest_type` | Type of restaurant (e.g., Casual Dining) |
| `cuisines` | Cuisines served |
| `approx_cost(for two people)` | Approximate cost for two |
| `listed_in(type)` | Meal type listed |

### 2. `Zomato Restaurant reviews.csv`
Contains user-generated textual reviews for sentiment analysis.

| Column | Description |
|---|---|
| `restaurant` | Restaurant name |
| `reviewer` | Name of the reviewer |
| `review` | Full text of the review |
| `rating` | Rating given by reviewer |
| `time` | Timestamp of review |
| `pictures` | Number of pictures uploaded |

---

## ▶️ How to Run

### Prerequisites
Make sure you have Python 3.10+ installed.

```bash
# Clone the repository
git clone https://github.com/Raj-Verma-1998/Zomato.git
cd Zomato

# Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn nltk vaderSentiment jupyter

# Launch Jupyter Notebook
jupyter notebook
```

Then open the main notebook and run all cells sequentially.

> **Note:** Ensure both CSV files are in the same directory as the notebook before running.

---

## 🧪 Experiment Results

This project is structured around **10 experiments**, progressively building from data exploration to advanced clustering and sentiment analysis.

| # | Experiment | Description |
|---|---|---|
| 1 | Data Loading & EDA | Loaded datasets, explored shape, null values, data types |
| 2 | Data Cleaning | Handled missing values, formatted ratings, removed duplicates |
| 3 | Feature Engineering | Encoded categorical variables, scaled numerical features |
| 4 | Cost & Rating Analysis | Analyzed cost distribution vs. ratings across locations |
| 5 | Cuisine Analysis | Identified top cuisines and their rating patterns |
| 6 | Elbow Method | Determined optimal number of clusters (K) using inertia |
| 7 | KMeans Clustering | Grouped restaurants into clusters based on features |
| 8 | PCA Visualization | Reduced dimensions and visualized clusters in 2D |
| 9 | Sentiment Analysis | Applied VADER NLP on review text to classify sentiment |
| 10 | Cluster + Sentiment Fusion | Combined clustering results with sentiment scores for insights |

### Key Findings
- Optimal number of clusters identified: **k = 4**
- Majority of restaurants fall in the **mid-range cost** segment (₹200–₹600 for two)
- Sentiment analysis revealed **~65% positive**, **~20% neutral**, **~15% negative** reviews
- High-rated restaurants with positive sentiment clustered around specific localities

---

## 📊 Visualizations & Charts

The `output_artifacts/` folder contains all generated plots, including:

- 📈 **Rating Distribution** — Histogram of restaurant ratings
- 💰 **Cost vs. Rating Scatter Plot** — Relationship between price and quality
- 🗺️ **Location-wise Restaurant Count** — Bar chart of top localities
- 🍕 **Top Cuisines Bar Chart** — Most popular cuisines on Zomato
- 📉 **Elbow Curve** — Inertia vs. number of clusters (K)
- 🔵 **KMeans Cluster Plot** — PCA-reduced 2D cluster visualization
- 😊 **Sentiment Distribution Pie Chart** — Positive / Neutral / Negative split
- 🔥 **Sentiment by Cluster Heatmap** — Sentiment scores mapped across clusters

> All charts are saved as `.png` files inside the `output_artifacts/` directory.

---

## 📁 Repository Structure

```
Zomato/
│
├── output_artifacts/               # All generated visualizations
├── Zomato Restaurant names and Metadata.csv   # Restaurant metadata
├── Zomato Restaurant reviews.csv              # User reviews
├── Zomato_10_Experiments.pptx                 # Project presentation slides
├── README.md                                  # Project documentation
├── LICENSE                                    # MIT License
└── .gitignore
```

---

## 👤 Author

**Raj Verma**
- GitHub: [@Raj-Verma-1998](https://github.com/Raj-Verma-1998)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
