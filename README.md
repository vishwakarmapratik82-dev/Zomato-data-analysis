# Zomato Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue) ![EDA](https://img.shields.io/badge/EDA-Exploratory%20Analysis-green) ![Visualization](https://img.shields.io/badge/Visualization-Seaborn%20%7C%20Matplotlib-orange)

Exploratory data analysis on 148 Zomato restaurant records — uncovering trends in restaurant types, customer votes, ratings, pricing, and online ordering behavior.

---

## Dataset

- **148 restaurants** · 7 features · No missing values

| Column | Description |
|--------|-------------|
| `name` | Restaurant name |
| `online_order` | Accepts online orders (Yes/No) |
| `book_table` | Table booking available (Yes/No) |
| `rate` | Rating out of 5 (parsed from "X/5" format) |
| `votes` | Total customer votes |
| `approx_cost(for two people)` | Approximate cost in INR |
| `listed_in(type)` | Category: Buffet / Cafes / Dining / Other |

---

## Key Findings

- **Dining** is the most common restaurant type and receives the most votes
- Most restaurants are rated between **3.5 and 4.0**
- Couples most commonly prefer restaurants with an approximate cost of **₹300**
- **Online orders** receive higher ratings compared to offline orders
- The heatmap shows **77 dining restaurants** accept online orders vs 33 that do not

---

## Analysis Performed

| Analysis | Method |
|----------|--------|
| Type distribution | Count plot of restaurant categories |
| Votes by type | Line chart of total votes per category |
| Rating distribution | Histogram with 4 bins |
| Couple spending habits | Count plot of approx cost |
| Online vs Offline rating | Boxplot comparison |
| Order mode heatmap | Pivot table heatmap (restaurant type × online order) |

---

## Setup & Usage

### 1. Clone / download the project

```bash
git clone <your-repo-url>
cd zomato-data-analysis
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Add the dataset

Place `Zomato data .csv` in `/content/` (or update the path in the notebook).

### 4. Run the notebook

Open in **Google Colab** or **Jupyter Notebook** and run all cells.

---

## Dependencies

```
pandas==2.2.2
numpy==1.26.4
matplotlib==3.8.4
seaborn==0.13.2
```

---

## Project Structure

```
zomato-data-analysis/
│
├── Zomato_Data_Analysis_Project.ipynb   # Main analysis notebook
├── Zomato data .csv                     # Dataset
├── requirements.txt                     # Python dependencies
└── README.md                            # Project documentation
```
