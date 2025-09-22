# 🏙 Airbnb NYC 2019 Data Analysis  

## 📌 Project Overview  
This project analyzes the **Airbnb NYC 2019 dataset** (~48,800 listings) to uncover insights about:  

- Price distributions  
- Listing concentrations by borough  
- Geographic patterns  
- Guest preferences  

The analysis includes **data cleaning, exploratory data analysis (EDA), visualization, and interactive mapping** with Plotly.  

👉 **Live Interactive Map:** [Click here to explore](https://traanvg.github.io/airbnb-nyc-analysis/interactive_map.html)  

---

## 📂 Dataset  
- **Source:** [Airbnb NYC 2019 on Kaggle](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)  
- **Original size:** 48,884 listings × 15 columns  
- **Cleaned dataset:** 48,868 listings × 13 columns  
- **Coverage:** All 5 NYC boroughs (Manhattan, Brooklyn, Queens, Bronx, Staten Island)  

---

## 🛠 Tools & Libraries  
- **Python:** Pandas, Matplotlib, Seaborn  
- **Visualization:** Plotly (interactive), Contextily (static maps)  
- **Notebook Environment:** Jupyter / VS Code  

---

## 🧹 Data Cleaning Steps  
- Removed duplicates and rows with missing `name`  
- Dropped unnecessary columns (`id`, `host_name`, `last_review`)  
- Filtered out invalid prices (≤ 0)  
- Filled missing values in `reviews_per_month` with 0  

✅ Final dataset ready for analysis with **13 useful columns**.  

---

## 📊 Exploratory Data Analysis  

### 1. Price Distribution  
- Most listings are priced under **$200/night**  
- Median ≈ **$100**  
- A few extreme outliers (> $500)  

### 2. Listings by Borough  
- **Manhattan and Brooklyn** account for ~80% of all listings  
- Queens, Bronx, and Staten Island together make up <20%  

### 3. Geographic Distribution by Borough  
- Dense clusters in **Manhattan and Brooklyn**  
- Sparse coverage in **Bronx and Staten Island**  

### 4. Geographic Distribution by Price  
- **Manhattan = premium cluster (luxury listings)**  
- **Bronx & Queens = budget-friendly areas**  
- **Brooklyn = mixed range**  

### 5. 🌍 Interactive Map (Plotly)  
👉 [Click here to explore the map](https://traanvg.github.io/airbnb-nyc-analysis/interactive_map.html)  

**Features:**  
- Zoom and pan across New York City  
- Hover tooltips show **neighborhood, room type, and price**  
- Continuous color scale for nightly price  

---

## 📌 Key Insights  
- **80% of listings** are in Manhattan & Brooklyn → highly concentrated market  
- **Manhattan’s average price** is ~3× higher than Queens → premium zone  
- **Entire homes/apartments (~60%)** dominate listings → guests prefer privacy  
- **Luxury clusters** are concentrated in Manhattan, while Bronx/Queens cater to budget travelers  

---

## 🚀 How to Run Locally  

Clone this repo:
```bash
git clone https://github.com/traanvg/airbnb-nyc-analysis.git
cd airbnb-nyc-analysis

## Install dependencies:
pip install -r requirements.txt

## Open the notebook in Jupyter or VS Code:
jupyter notebook Airbnb_NYC_Analysis.ipynb

## **Credits**

Dataset: Airbnb NYC 2019 on Kaggle

Author: Tran Vuong
